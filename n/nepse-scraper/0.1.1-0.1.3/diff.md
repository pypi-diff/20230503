# Comparing `tmp/nepse_scraper-0.1.1.tar.gz` & `tmp/nepse_scraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepse_scraper-0.1.1.tar", last modified: Wed May  3 06:59:12 2023, max compression
+gzip compressed data, was "nepse_scraper-0.1.3.tar", last modified: Wed May  3 07:29:32 2023, max compression
```

## Comparing `nepse_scraper-0.1.1.tar` & `nepse_scraper-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.395278 nepse_scraper-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-05-03 03:10:57.000000 nepse_scraper-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3155 2023-05-03 06:59:12.395278 nepse_scraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2479 2023-05-03 06:49:00.000000 nepse_scraper-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.377401 nepse_scraper-0.1.1/nepse_scraper/
--rw-rw-rw-   0        0        0    23784 2023-05-03 06:45:39.000000 nepse_scraper-0.1.1/nepse_scraper/Scraper.py
--rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.1/nepse_scraper/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-05-03 06:36:54.000000 nepse_scraper-0.1.1/nepse_scraper/apis.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.394274 nepse_scraper-0.1.1/nepse_scraper.egg-info/
--rw-rw-rw-   0        0        0     3155 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-03 06:59:12.396280 nepse_scraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1133 2023-05-03 06:57:40.000000 nepse_scraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:29:32.181038 nepse_scraper-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-05-03 03:10:57.000000 nepse_scraper-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3155 2023-05-03 07:29:32.181038 nepse_scraper-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2479 2023-05-03 06:49:00.000000 nepse_scraper-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:29:32.159562 nepse_scraper-0.1.3/nepse_scraper/
+-rw-rw-rw-   0        0        0    23862 2023-05-03 07:14:45.000000 nepse_scraper-0.1.3/nepse_scraper/Scraper.py
+-rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.3/nepse_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-05-03 06:36:54.000000 nepse_scraper-0.1.3/nepse_scraper/apis.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:29:32.167738 nepse_scraper-0.1.3/nepse_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3155 2023-05-03 07:29:32.000000 nepse_scraper-0.1.3/nepse_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-03 07:29:32.000000 nepse_scraper-0.1.3/nepse_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:29:32.000000 nepse_scraper-0.1.3/nepse_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-03 07:29:32.000000 nepse_scraper-0.1.3/nepse_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 07:29:32.000000 nepse_scraper-0.1.3/nepse_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-03 07:29:32.182042 nepse_scraper-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1133 2023-05-03 07:29:23.000000 nepse_scraper-0.1.3/setup.py
```

### Comparing `nepse_scraper-0.1.1/LICENSE.txt` & `nepse_scraper-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.1/PKG-INFO` & `nepse_scraper-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nepse_scraper
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.3.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nepse_scraper-0.1.1/README.md` & `nepse_scraper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.1/nepse_scraper/Scraper.py` & `nepse_scraper-0.1.3/nepse_scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from urllib3.exceptions import InsecureRequestWarning
 from urllib3 import disable_warnings
 import time
 from wasmtime import Store,Module,Instance
 import json
 import os
 
-WASM_FILE = r'nepse_scraper\nepse.wasm'
+import pkg_resources
+WASM_FILE = pkg_resources.resource_filename(__name__, 'nepse.wasm')
 
+
+# WASM_FILE = r'nepse.wasm'
 from .apis import api_dict
 
 ROOT_URL = 'https://www.nepalstock.com.np'
 
 class TokenParser():
     def __init__(self):
         self.store = Store()
```

### Comparing `nepse_scraper-0.1.1/nepse_scraper/apis.py` & `nepse_scraper-0.1.3/nepse_scraper/apis.py`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.1/nepse_scraper.egg-info/PKG-INFO` & `nepse_scraper-0.1.3/nepse_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nepse-scraper
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.3.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nepse_scraper-0.1.1/setup.py` & `nepse_scraper-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path
 
 current_dir = path.abspath(path.dirname(__file__))
 
-VERSION = '0.1.1'
+VERSION = '0.1.3'
 DESCRIPTION = 'Python Scraper for Nepse'
 
 with open(path.join(current_dir, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
@@ -18,15 +18,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url='https://github.com/polymorphisma/nepse_scraper/',  
     install_requires=['requests','urllib3','wasmtime', 'retrying'],
     keywords=['python', 'nepse data', 'nepse scraper'],
-    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz",
+    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.3.tar.gz",
     classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```

