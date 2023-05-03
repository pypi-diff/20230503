# Comparing `tmp/scrappier-1.5.0.tar.gz` & `tmp/scrappier-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappier-1.5.0.tar", last modified: Mon Jan  9 22:40:25 2023, max compression
+gzip compressed data, was "scrappier-1.6.0.tar", last modified: Wed May  3 18:41:19 2023, max compression
```

## Comparing `scrappier-1.5.0.tar` & `scrappier-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-01-09 22:40:25.490301 scrappier-1.5.0/
--rw-rw-r--   0 cris      (1000) cris      (1000)     1062 2022-12-24 00:23:27.000000 scrappier-1.5.0/LICENSE
--rw-rw-r--   0 cris      (1000) cris      (1000)     2396 2023-01-09 22:40:25.490301 scrappier-1.5.0/PKG-INFO
--rw-rw-r--   0 cris      (1000) cris      (1000)     2099 2023-01-09 22:40:18.000000 scrappier-1.5.0/README.md
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-01-09 22:40:25.486301 scrappier-1.5.0/scrappier/
--rw-rw-r--   0 cris      (1000) cris      (1000)       37 2022-12-24 01:55:03.000000 scrappier-1.5.0/scrappier/__init__.py
--rw-rw-r--   0 cris      (1000) cris      (1000)     3635 2023-01-09 21:50:55.000000 scrappier-1.5.0/scrappier/browser.py
--rw-rw-r--   0 cris      (1000) cris      (1000)     3318 2023-01-09 22:05:46.000000 scrappier-1.5.0/scrappier/element.py
--rw-rw-r--   0 cris      (1000) cris      (1000)      400 2022-12-24 00:13:12.000000 scrappier-1.5.0/scrappier/element_collection.py
--rw-rw-r--   0 cris      (1000) cris      (1000)     3381 2023-01-09 22:23:48.000000 scrappier-1.5.0/scrappier/element_finder.py
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-01-09 22:40:25.490301 scrappier-1.5.0/scrappier/exceptions/
--rw-rw-r--   0 cris      (1000) cris      (1000)        0 2022-12-24 21:35:08.000000 scrappier-1.5.0/scrappier/exceptions/__init__.py
--rw-rw-r--   0 cris      (1000) cris      (1000)       51 2022-12-24 21:32:10.000000 scrappier-1.5.0/scrappier/exceptions/element_not_found_exception.py
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-01-09 22:40:25.490301 scrappier-1.5.0/scrappier.egg-info/
--rw-rw-r--   0 cris      (1000) cris      (1000)     2396 2023-01-09 22:40:25.000000 scrappier-1.5.0/scrappier.egg-info/PKG-INFO
--rw-rw-r--   0 cris      (1000) cris      (1000)      399 2023-01-09 22:40:25.000000 scrappier-1.5.0/scrappier.egg-info/SOURCES.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)        1 2023-01-09 22:40:25.000000 scrappier-1.5.0/scrappier.egg-info/dependency_links.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)       29 2023-01-09 22:40:25.000000 scrappier-1.5.0/scrappier.egg-info/requires.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)       10 2023-01-09 22:40:25.000000 scrappier-1.5.0/scrappier.egg-info/top_level.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)       38 2023-01-09 22:40:25.490301 scrappier-1.5.0/setup.cfg
--rw-rw-r--   0 cris      (1000) cris      (1000)      761 2023-01-09 22:36:35.000000 scrappier-1.5.0/setup.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-03 18:41:19.805620 scrappier-1.6.0/
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1062 2023-05-03 17:29:47.000000 scrappier-1.6.0/LICENSE
+-rw-rw-r--   0 cris      (1000) cris      (1000)     2744 2023-05-03 18:41:19.793619 scrappier-1.6.0/PKG-INFO
+-rw-rw-r--   0 cris      (1000) cris      (1000)     2392 2023-05-03 18:41:08.000000 scrappier-1.6.0/README.md
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-03 18:41:19.769619 scrappier-1.6.0/scrappier/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       37 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     3376 2023-05-03 18:33:06.000000 scrappier-1.6.0/scrappier/browser.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     3318 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/element.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      400 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/element_collection.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     3381 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/element_finder.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-03 18:41:19.793619 scrappier-1.6.0/scrappier/exceptions/
+-rw-rw-r--   0 cris      (1000) cris      (1000)        0 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/exceptions/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)       51 2023-05-03 17:29:47.000000 scrappier-1.6.0/scrappier/exceptions/element_not_found_exception.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-03 18:41:19.785619 scrappier-1.6.0/scrappier.egg-info/
+-rw-rw-r--   0 cris      (1000) cris      (1000)     2744 2023-05-03 18:41:19.000000 scrappier-1.6.0/scrappier.egg-info/PKG-INFO
+-rw-rw-r--   0 cris      (1000) cris      (1000)      399 2023-05-03 18:41:19.000000 scrappier-1.6.0/scrappier.egg-info/SOURCES.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)        1 2023-05-03 18:41:19.000000 scrappier-1.6.0/scrappier.egg-info/dependency_links.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)       29 2023-05-03 18:41:19.000000 scrappier-1.6.0/scrappier.egg-info/requires.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)       10 2023-05-03 18:41:19.000000 scrappier-1.6.0/scrappier.egg-info/top_level.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)       38 2023-05-03 18:41:19.805620 scrappier-1.6.0/setup.cfg
+-rw-rw-r--   0 cris      (1000) cris      (1000)      761 2023-05-03 18:38:31.000000 scrappier-1.6.0/setup.py
```

### Comparing `scrappier-1.5.0/LICENSE` & `scrappier-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrappier-1.5.0/PKG-INFO` & `scrappier-1.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: scrappier
-Version: 1.5.0
-Summary: Scrapper for chrome
-Author: Cristian Guzmán
-Author-email: <cristian.guzman.contacto@gmail.com>
-Keywords: python,scrapper,web,scrapping,selenium,scrappier,browser,chrome
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Scrappier
 
 Scrappier is a web scrapper which uses chrome in a headless mode. This library provides an easy-to-read syntaxis to navigate through the different elements and perform actions.
 
 ## Requirements
 
 * python 3.8
@@ -129,8 +118,15 @@
 
 If you are a collaborator, please consider do the next:
 
 1. Create your new functionality
 2. Create a test of your new functionality
 3. change the version of the package in setup.py
 4. execute the next command: `python3 setup.py sdist bdist_wheel`
-5. 
+5. upload the package: `source venv/bin/active && twine upload dist/*<your-version>*`
+
+## for developers
+
+install twine: `python3 -m pip instal twine`
+install setuptools: `pip3 install setuptools`
+install setuptools: `python3 setup.py sdist bdist_wheel`
+upload your changes: `twine upload dist/*`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrappier-1.5.0/README.md` & `scrappier-1.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: scrappier
+Version: 1.6.0
+Summary: Scrapper for chrome
+Home-page: UNKNOWN
+Author: Cristian Guzmán
+Author-email: <cristian.guzman.contacto@gmail.com>
+License: UNKNOWN
+Keywords: python,scrapper,web,scrapping,selenium,scrappier,browser,chrome
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Scrappier
 
 Scrappier is a web scrapper which uses chrome in a headless mode. This library provides an easy-to-read syntaxis to navigate through the different elements and perform actions.
 
 ## Requirements
 
 * python 3.8
@@ -118,8 +132,16 @@
 
 If you are a collaborator, please consider do the next:
 
 1. Create your new functionality
 2. Create a test of your new functionality
 3. change the version of the package in setup.py
 4. execute the next command: `python3 setup.py sdist bdist_wheel`
-5. 
+5. upload the package: `source venv/bin/active && twine upload dist/*<your-version>*`
+
+## for developers
+
+install twine: `python3 -m pip instal twine`
+install setuptools: `pip3 install setuptools`
+install setuptools: `python3 setup.py sdist bdist_wheel`
+upload your changes: `twine upload dist/*`
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrappier-1.5.0/scrappier/browser.py` & `scrappier-1.6.0/scrappier/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-from .element import Element
-
 from datetime import datetime
 
-from scrappier.element_collection import ElementCollection
 from scrappier.element_finder import ElementFinder
 
 from selenium import webdriver
-from selenium.common.exceptions import TimeoutException
-from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 
 class Browser:
     
     options = [
         '--headless',
@@ -62,14 +55,17 @@
         path = f"{datetime.now().strftime('%d-%m-%Y-%H-%M-%S')}.png"
 
         self.screenshot(path)
 
     def html(self) -> str:
         return self.driver.page_source
 
+    def alert(self):
+        return self.driver.switch_to.alert
+
     def url(self) -> str:
         return self.driver.current_url
 
     def wait(self, seconds:int):
         self.driver.implicitly_wait(seconds)
 
     def select(input:str, value:str):
```

### Comparing `scrappier-1.5.0/scrappier/element.py` & `scrappier-1.6.0/scrappier/element.py`

 * *Files identical despite different names*

### Comparing `scrappier-1.5.0/scrappier/element_finder.py` & `scrappier-1.6.0/scrappier/element_finder.py`

 * *Files identical despite different names*

### Comparing `scrappier-1.5.0/scrappier.egg-info/PKG-INFO` & `scrappier-1.6.0/scrappier.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: scrappier
-Version: 1.5.0
+Version: 1.6.0
 Summary: Scrapper for chrome
+Home-page: UNKNOWN
 Author: Cristian Guzmán
 Author-email: <cristian.guzman.contacto@gmail.com>
+License: UNKNOWN
 Keywords: python,scrapper,web,scrapping,selenium,scrappier,browser,chrome
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Scrappier
 
 Scrappier is a web scrapper which uses chrome in a headless mode. This library provides an easy-to-read syntaxis to navigate through the different elements and perform actions.
@@ -129,8 +132,16 @@
 
 If you are a collaborator, please consider do the next:
 
 1. Create your new functionality
 2. Create a test of your new functionality
 3. change the version of the package in setup.py
 4. execute the next command: `python3 setup.py sdist bdist_wheel`
-5. 
+5. upload the package: `source venv/bin/active && twine upload dist/*<your-version>*`
+
+## for developers
+
+install twine: `python3 -m pip instal twine`
+install setuptools: `pip3 install setuptools`
+install setuptools: `python3 setup.py sdist bdist_wheel`
+upload your changes: `twine upload dist/*`
+
```

### Comparing `scrappier-1.5.0/setup.py` & `scrappier-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.5.0'
+VERSION = '1.6.0'
 DESCRIPTION = 'Scrapper for chrome'
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # Setting up
 setup(
```

