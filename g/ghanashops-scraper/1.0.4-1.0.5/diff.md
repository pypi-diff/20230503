# Comparing `tmp/ghanashops-scraper-1.0.4.tar.gz` & `tmp/ghanashops-scraper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-1.0.4.tar", last modified: Wed May  3 00:28:35 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-1.0.5.tar", last modified: Wed May  3 01:41:20 2023, max compression
```

## Comparing `ghanashops-scraper-1.0.4.tar` & `ghanashops-scraper-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.4/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:28:34.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-03 00:28:34.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 00:28:34.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 00:28:34.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 00:28:34.000000 ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.4/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.4/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.4/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 00:28:32.000000 ghanashops-scraper-1.0.4/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:28:35.000000 ghanashops-scraper-1.0.4/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.4/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5728 2023-05-03 00:27:28.000000 ghanashops-scraper-1.0.4/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.4/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.5/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:41:19.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-05-03 01:41:19.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 01:41:19.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 01:41:19.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 01:41:19.000000 ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.5/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.5/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.5/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 01:41:11.000000 ghanashops-scraper-1.0.5/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:41:20.000000 ghanashops-scraper-1.0.5/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.5/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5804 2023-05-03 00:42:06.000000 ghanashops-scraper-1.0.5/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4874 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.5/tonaton/scrapy.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.5/tonaton/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5535 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.5/tonaton.py
```

### Comparing `ghanashops-scraper-1.0.4/PKG-INFO` & `ghanashops-scraper-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.4
+Version: 1.0.5
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.4 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.5 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.4/README.md` & `ghanashops-scraper-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.4/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-1.0.5/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.4
+Version: 1.0.5
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.4 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.5 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.4/jumia/scraper.py` & `ghanashops-scraper-1.0.5/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.4/jumia/utils.py` & `ghanashops-scraper-1.0.5/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.4/setup.py` & `ghanashops-scraper-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-1.0.4/tonaton/scraper.py` & `ghanashops-scraper-1.0.5/tonaton/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,21 +53,22 @@
             data.raise_for_status()
             sys.exit(1)
         soup = BeautifulSoup(data.content, 'html.parser')
         page_numbers = soup.find("section", class_="pagination")
         total_pages = int(page_numbers.text.strip().replace("\n", ",").split(",")[-2])
         self.limit_pages = limit_pages
         self.total_pages = total_pages
+        print(f"Scraping from: {self.total_pages} pages. Please wait...")
         if self.limit_pages is not None:
             self.total_pages = self.limit_pages
 
     def download(self, output_dir=None):
         """scrape data"""
         try:
-            print("saving results to csv...")
+            print("Saving results to csv...")
             if output_dir is None:
                 output_dir = os.getcwd()
                 SaveFile.mkdir(output_dir)
             if not os.path.isdir(output_dir):
                 raise ValueError(
                     f"Invalid output directory: {output_dir} is not a directory"
                 )
@@ -86,20 +87,20 @@
 
                 for page in range(1, self.total_pages + 1):
                     query_url = f"https://tonaton.com/search?query={self.query}&page={page}"
                     with requests.Session() as session:
                         results = session.get(query_url)
                     # time.sleep(2)
                     # tasks = []
-                    #task = asyncio.create_task(fetch_data(query_url))
+                    # task = asyncio.create_task(fetch_data(query_url))
                     # tasks.append(task)
                     # responses = await asyncio.gather(*tasks)
                     # for results in responses:
 
-                    #results = await task
+                    # results = await task
                     # results = await fetch_data(urls=pages)
                     # await asyncio.sleep(2)
                     # await asyncio.gather(*pages)
 
                     html_soup = BeautifulSoup(results.text, 'html.parser')
                     items = html_soup.find_all('a', class_='product__item')
```

### Comparing `ghanashops-scraper-1.0.4/tonaton/utils.py` & `ghanashops-scraper-1.0.5/tonaton/utils.py`

 * *Files identical despite different names*

