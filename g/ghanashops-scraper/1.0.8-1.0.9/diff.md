# Comparing `tmp/ghanashops-scraper-1.0.8.tar.gz` & `tmp/ghanashops-scraper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-1.0.8.tar", last modified: Wed May  3 02:05:44 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-1.0.9.tar", last modified: Wed May  3 02:13:41 2023, max compression
```

## Comparing `ghanashops-scraper-1.0.8.tar` & `ghanashops-scraper-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.8/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.8/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.8/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.8/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 02:05:42.000000 ghanashops-scraper-1.0.8/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:05:44.000000 ghanashops-scraper-1.0.8/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.8/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5804 2023-05-03 00:42:06.000000 ghanashops-scraper-1.0.8/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4899 2023-05-03 02:05:30.000000 ghanashops-scraper-1.0.8/tonaton/scrapy.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.8/tonaton/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5535 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.8/tonaton.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.9/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.9/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.9/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.9/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 02:13:39.000000 ghanashops-scraper-1.0.9/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 02:13:41.000000 ghanashops-scraper-1.0.9/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.9/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5804 2023-05-03 00:42:06.000000 ghanashops-scraper-1.0.9/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4914 2023-05-03 02:13:17.000000 ghanashops-scraper-1.0.9/tonaton/scrapy.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.9/tonaton/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5535 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.9/tonaton.py
```

### Comparing `ghanashops-scraper-1.0.8/PKG-INFO` & `ghanashops-scraper-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.8 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.9 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.8/README.md` & `ghanashops-scraper-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.8/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-1.0.9/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.8 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.9 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.8/jumia/scraper.py` & `ghanashops-scraper-1.0.9/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.8/jumia/utils.py` & `ghanashops-scraper-1.0.9/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.8/setup.py` & `ghanashops-scraper-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-1.0.8/tonaton/scraper.py` & `ghanashops-scraper-1.0.9/tonaton/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.8/tonaton/scrapy.py` & `ghanashops-scraper-1.0.9/tonaton/scrapy.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         except Exception as err:
             print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Scrape complete!!!")
         print("Done!")
 
-
-def main():
-    tonaton = Tonaton(query="TV")
-    asyncio.run(tonaton.get_data())
-    tonaton.download()
-
-
-if __name__ == '__main__':
-    main()
+#
+# def main():
+#     tonaton = Tonaton(query="TV")
+#     asyncio.run(tonaton.get_data())
+#     tonaton.download()
+#
+#
+# if __name__ == '__main__':
+#     main()
```

### Comparing `ghanashops-scraper-1.0.8/tonaton/utils.py` & `ghanashops-scraper-1.0.9/tonaton/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.8/tonaton.py` & `ghanashops-scraper-1.0.9/tonaton.py`

 * *Files identical despite different names*

