# Comparing `tmp/ghanashops-scraper-1.0.0.tar.gz` & `tmp/ghanashops-scraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-1.0.0.tar", last modified: Tue May  2 23:48:58 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-1.0.1.tar", last modified: Wed May  3 00:02:35 2023, max compression
```

## Comparing `ghanashops-scraper-1.0.0.tar` & `ghanashops-scraper-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.0/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.0/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.0/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.0/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 23:48:55.000000 ghanashops-scraper-1.0.0/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:48:58.000000 ghanashops-scraper-1.0.0/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.0/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5727 2023-05-02 23:48:55.000000 ghanashops-scraper-1.0.0/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.0/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.1/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.1/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.1/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.1/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 00:02:30.000000 ghanashops-scraper-1.0.1/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.1/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5739 2023-05-03 00:02:30.000000 ghanashops-scraper-1.0.1/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.1/tonaton/utils.py
```

### Comparing `ghanashops-scraper-1.0.0/PKG-INFO` & `ghanashops-scraper-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.0 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.1 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.0/README.md` & `ghanashops-scraper-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.0/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.0 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.1 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.0/jumia/scraper.py` & `ghanashops-scraper-1.0.1/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.0/jumia/utils.py` & `ghanashops-scraper-1.0.1/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.0/setup.py` & `ghanashops-scraper-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-1.0.0/tonaton/scraper.py` & `ghanashops-scraper-1.0.1/tonaton/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         page_numbers = soup.find("section", class_="pagination")
         total_pages = int(page_numbers.text.strip().replace("\n", ",").split(",")[-2])
         self.limit_pages = limit_pages
         self.total_pages = total_pages
         if self.limit_pages is not None:
             self.total_pages = self.limit_pages
 
-    def download(self, output_dir=None):
+    async def download(self, output_dir=None):
         """scrape data"""
         try:
             print("saving results to csv...")
             if output_dir is None:
                 output_dir = os.getcwd()
                 SaveFile.mkdir(output_dir)
             if not os.path.isdir(output_dir):
@@ -82,29 +82,29 @@
             ) as csv_file:
                 fieldnames = ["product_description", "price", "location", "photo", "page_url"]
                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
                 writer.writeheader()
 
                 for page in range(1, self.total_pages + 1):
                     query_url = f"https://tonaton.com/search?query={self.query}&page={page}"
-                    with requests.Session() as session:
-                        results = session.get(query_url)
-                    time.sleep(2)
+                    # with requests.Session() as session:
+                    #     results = session.get(query_url)
+                    # time.sleep(2)
                     # tasks = []
-                    # task = asyncio.create_task(fetch_data(query_url))
+                    task = asyncio.create_task(fetch_data(query_url))
                     # tasks.append(task)
                     # responses = await asyncio.gather(*tasks)
                     # for results in responses:
 
-                    # results = await task
+                    results = await task
                     # results = await fetch_data(urls=pages)
                     # await asyncio.sleep(2)
                     # await asyncio.gather(*pages)
 
-                    html_soup = BeautifulSoup(results.text, 'html.parser')
+                    html_soup = BeautifulSoup(results, 'html.parser')
                     items = html_soup.find_all('a', class_='product__item')
 
                     for item in items:
                         product_description = item.find('p', class_='product__description').get_text(strip=True)
 
                         location = item.find('p', class_='product__location').get_text(strip=True)
 
@@ -136,10 +136,11 @@
         except Exception as err:
             print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Scrape complete!!!")
         print("Done!")
 
+#
 # if __name__ == '__main__':
 #     tonaton = Tonaton(query="laptop", starting_page=1)
-#     asyncio.run(tonaton.download())
+#     asyncio.run(tonaton.download(tonaton))
```

### Comparing `ghanashops-scraper-1.0.0/tonaton/utils.py` & `ghanashops-scraper-1.0.1/tonaton/utils.py`

 * *Files identical despite different names*

