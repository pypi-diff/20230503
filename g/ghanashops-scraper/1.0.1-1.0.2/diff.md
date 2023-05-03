# Comparing `tmp/ghanashops-scraper-1.0.1.tar.gz` & `tmp/ghanashops-scraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-1.0.1.tar", last modified: Wed May  3 00:02:35 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-1.0.2.tar", last modified: Wed May  3 00:14:47 2023, max compression
```

## Comparing `ghanashops-scraper-1.0.1.tar` & `ghanashops-scraper-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.1/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.1/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.1/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.1/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 00:02:30.000000 ghanashops-scraper-1.0.1/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:02:35.000000 ghanashops-scraper-1.0.1/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.1/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5739 2023-05-03 00:02:30.000000 ghanashops-scraper-1.0.1/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.1/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.2/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.2/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.2/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.2/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 00:14:44.000000 ghanashops-scraper-1.0.2/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 00:14:47.000000 ghanashops-scraper-1.0.2/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.2/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5725 2023-05-03 00:12:45.000000 ghanashops-scraper-1.0.2/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.2/tonaton/utils.py
```

### Comparing `ghanashops-scraper-1.0.1/PKG-INFO` & `ghanashops-scraper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.1 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.2 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.1/README.md` & `ghanashops-scraper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.1/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-1.0.2/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.1 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.2 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.1/jumia/scraper.py` & `ghanashops-scraper-1.0.2/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.1/jumia/utils.py` & `ghanashops-scraper-1.0.2/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.1/setup.py` & `ghanashops-scraper-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-1.0.1/tonaton/scraper.py` & `ghanashops-scraper-1.0.2/tonaton/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,11 +136,11 @@
         except Exception as err:
             print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Scrape complete!!!")
         print("Done!")
 
-#
-# if __name__ == '__main__':
-#     tonaton = Tonaton(query="laptop", starting_page=1)
-#     asyncio.run(tonaton.download(tonaton))
+
+if __name__ == '__main__':
+    tonaton = Tonaton(query="laptop", starting_page=1)
+    asyncio.run(tonaton.download())
```

### Comparing `ghanashops-scraper-1.0.1/tonaton/utils.py` & `ghanashops-scraper-1.0.2/tonaton/utils.py`

 * *Files identical despite different names*

