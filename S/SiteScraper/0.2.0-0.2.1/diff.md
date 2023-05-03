# Comparing `tmp/SiteScraper-0.2.0.tar.gz` & `tmp/SiteScraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-0.2.0.tar", last modified: Mon May  1 18:02:04 2023, max compression
+gzip compressed data, was "SiteScraper-0.2.1.tar", last modified: Wed May  3 17:18:41 2023, max compression
```

## Comparing `SiteScraper-0.2.0.tar` & `SiteScraper-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.676737 SiteScraper-0.2.0/
--rw-rw-rw-   0        0        0      159 2023-05-01 18:02:04.675739 SiteScraper-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.667762 SiteScraper-0.2.0/SiteScraper/
--rw-rw-rw-   0        0        0     7864 2023-05-01 15:59:21.000000 SiteScraper-0.2.0/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       33 2023-04-30 14:41:47.000000 SiteScraper-0.2.0/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.674743 SiteScraper-0.2.0/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 18:02:04.676737 SiteScraper-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-05-01 17:58:01.000000 SiteScraper-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.739139 SiteScraper-0.2.1/
+-rw-rw-rw-   0        0        0      159 2023-05-03 17:18:41.738141 SiteScraper-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.730465 SiteScraper-0.2.1/SiteScraper/
+-rw-rw-rw-   0        0        0     8875 2023-05-03 17:15:01.000000 SiteScraper-0.2.1/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       35 2023-05-01 18:12:54.000000 SiteScraper-0.2.1/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.737144 SiteScraper-0.2.1/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:18:41.739139 SiteScraper-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      341 2023-05-03 17:17:45.000000 SiteScraper-0.2.1/setup.py
```

### Comparing `SiteScraper-0.2.0/SiteScraper/SiteScraper.py` & `SiteScraper-0.2.1/SiteScraper/SiteScraper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 import time
 import logging
 class yt_vedio():
-       
+    def web_driver_chrome(self):
+            options = webdriver.ChromeOptions()
+            options.add_argument("--verbose")
+            options.add_argument('--no-sandbox')
+            options.add_argument('--headless')
+            options.add_argument('--disable-gpu')
+            options.add_argument("--window-size=1920, 1200")
+            options.add_argument('--disable-dev-shm-usage')
+            driver = webdriver.Chrome(options=options)
+            return driver 
+    def web_driver_firefox(self):
+            options = webdriver.FirefoxOptions()
+            options.add_argument("--verbose")
+            options.add_argument('--no-sandbox')
+            options.add_argument('--headless')
+            options.add_argument('--disable-gpu')
+            options.add_argument("--window-size=1920, 1200")
+            options.add_argument('--disable-dev-shm-usage')
+            driver = webdriver.Firefox(options=options)
+            return driver
     def yt_vedios_data(self, url,browser='Chrome'):
         if browser=='Chrome' or browser=='chrome':
-            driver = webdriver.Chrome()
+            driver = self.web_driver_chrome()
+           
             self.url = url
             try:
                 driver.get(self.url)
                 
                 prev_h = 0
                 while True:
                     height = driver.execute_script('''
                         return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );''')
-                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+500})")
+                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
 
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 title = list()
@@ -42,28 +62,28 @@
                 driver.quit()
                 return list_of_dic
             except:
                 driver.quit()
                 logging.error("Invalid url")
             
         else:
-            driver = webdriver.Firefox()
+            driver =self.web_driver_firefox()
             self.url = url
             try:
                 driver.get(self.url)
                 
                 prev_h = 0
                 while True:
                     height = driver.execute_script('''
                         return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );''')
-                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+500})")
+                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
 
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 title = list()
@@ -82,30 +102,30 @@
                 driver.quit()
                 return list_of_dic
             except:
                 driver.quit()
                 logging.error("Invalid url")
     def yt_vedio_comment(self,url,browser='Chrome'):
         if browser=='Chrome' or browser=='chrome':
-            driver = webdriver.Chrome()
-            self.url = url
             try:
+                driver =self.web_driver_chrome()
+                self.url = url
                 driver.get(url)
                 time.sleep(5)
                 prev_h = 0
                 while True:
                     #Returns the page length dynamically
                     height = driver.execute_script('''
                             return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );
                         ''')
-                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+600})")
+                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
                 comments_text = driver.find_elements(By.XPATH, '//*[@id="content-text"]')
                 # print(elements)
                 txt=list()
@@ -124,30 +144,30 @@
                 driver.quit()
                 return dic
 
             except:
                 driver.quit()
                 logging.error('Invalid url')
         else: 
-            driver = webdriver.Firefox()
+            driver =self.web_driver_firefox()
             self.url = url
             try:
                 driver.get(url)
                 time.sleep(5)
                 prev_h = 0
                 while True:
                     #Returns the page lenght dynamically
                     height = driver.execute_script('''
                             return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );
                         ''')
-                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+500})")
+                    driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
                 comments_text = driver.find_elements(By.XPATH, '//*[@id="content-text"]')
                 # print(elements)
                 txt=list()
```

