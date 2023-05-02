# Comparing `tmp/ghanashops-scraper-0.0.3.tar.gz` & `tmp/ghanashops-scraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-0.0.3.tar", last modified: Tue May  2 21:50:34 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-0.0.4.tar", last modified: Tue May  2 23:14:56 2023, max compression
```

## Comparing `ghanashops-scraper-0.0.3.tar` & `ghanashops-scraper-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2115 2023-05-02 21:46:49.000000 ghanashops-scraper-0.0.3/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.0.3/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.0.3/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.3/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 21:50:31.000000 ghanashops-scraper-0.0.3/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.0.3/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4762 2023-05-02 21:50:25.000000 ghanashops-scraper-0.0.3/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.3/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2115 2023-05-02 21:46:49.000000 ghanashops-scraper-0.0.4/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.0.4/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.0.4/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.4/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 23:14:47.000000 ghanashops-scraper-0.0.4/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:14:56.000000 ghanashops-scraper-0.0.4/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.0.4/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5596 2023-05-02 23:14:39.000000 ghanashops-scraper-0.0.4/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.4/tonaton/utils.py
```

### Comparing `ghanashops-scraper-0.0.3/PKG-INFO` & `ghanashops-scraper-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.3 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.4 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-0.0.3/README.md` & `ghanashops-scraper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-0.0.4/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.3 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.4 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-0.0.3/jumia/scraper.py` & `ghanashops-scraper-0.0.4/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.0.3/jumia/utils.py` & `ghanashops-scraper-0.0.4/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.0.3/setup.py` & `ghanashops-scraper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-0.0.3/tonaton/scraper.py` & `ghanashops-scraper-0.0.4/tonaton/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,31 @@
 BASE_URL = "https://tonaton.com"
 
 
 # query = https://tonaton.com/search?region=ashanti&query=houses&page=1
 # query = https://tonaton.com/c_vehicles?region=ashanti&page=1
 # query = https://tonaton.com/r_ashanti/c_real-estate?page=2
 
+# def get_tasks(urls, session):
+#     tasks = []
+#     for url in urls:
+#         tasks.append(asyncio.create_task(session.get(url)))
+#     return tasks
+#
+#
+# results = []
+#
+#
+# async def fetch_data(urls):
+#     async with aiohttp.ClientSession() as session:
+#         tasks = get_tasks(urls=urls, session=session)
+#         responses = await asyncio.gather(*tasks)
+#         for response in responses:
+#             results.append(await response.text())
+
 
 async def fetch_data(url):
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             return await response.text()
 
 
@@ -62,22 +79,30 @@
                     newline="",
                     encoding='utf-8'
             ) as csv_file:
                 fieldnames = ["product_description", "price", "location", "photo", "page_url"]
                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
                 writer.writeheader()
 
+                # pages = []
                 for page in range(1, self.total_pages + 1):
                     query_url = f"https://tonaton.com/search?query={self.query}&page={page}"
-
+                    tasks = []
                     task = asyncio.create_task(fetch_data(query_url))
-                    results = await task
+                    tasks.append(task)
+                    responses = await asyncio.gather(*tasks)
+                    for results in responses:
+
+                    #results = await task
+                    # results = await fetch_data(urls=pages)
+                    # await asyncio.sleep(2)
+                    # await asyncio.gather(*pages)
 
-                    html_soup = BeautifulSoup(results, 'html.parser')
-                    items = html_soup.find_all('a', class_='product__item')
+                        html_soup = BeautifulSoup(results, 'html.parser')
+                        items = html_soup.find_all('a', class_='product__item')
 
                     for item in items:
                         product_description = item.find('p', class_='product__description').get_text(strip=True)
 
                         location = item.find('p', class_='product__location').get_text(strip=True)
 
                         price = item.find('span', class_='product__title').get_text(strip=True)
@@ -109,10 +134,10 @@
             print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Scrape complete!!!")
         print("Done!")
 
 
-if __name__ == '__main__':
-    tonaton = Tonaton(query="laptop", starting_page=1)
-    asyncio.run(tonaton.download())
+# if __name__ == '__main__':
+#     tonaton = Tonaton(query="laptop", starting_page=1)
+#     asyncio.run(tonaton.download())
```

### Comparing `ghanashops-scraper-0.0.3/tonaton/utils.py` & `ghanashops-scraper-0.0.4/tonaton/utils.py`

 * *Files identical despite different names*

