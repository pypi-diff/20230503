# Comparing `tmp/selenium-recaptcha-solver-1.7.0.tar.gz` & `tmp/selenium-recaptcha-solver-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-recaptcha-solver-1.7.0.tar", last modified: Wed Apr  5 10:14:07 2023, max compression
+gzip compressed data, was "selenium-recaptcha-solver-1.8.0.tar", last modified: Wed May  3 07:26:43 2023, max compression
```

## Comparing `selenium-recaptcha-solver-1.7.0.tar` & `selenium-recaptcha-solver-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/
--rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     3501 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-03-25 19:51:06.000000 selenium-recaptcha-solver-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.235616 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/
--rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/__init__.py
--rw-rw-rw-   0        0        0     1702 2023-03-25 19:51:06.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/delay_config.py
--rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/exceptions.py
--rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/services.py
--rw-rw-rw-   0        0        0     9587 2023-04-05 09:59:38.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/solver.py
-drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.241617 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/
--rw-rw-rw-   0        0        0     3501 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-05 10:13:09.000000 selenium-recaptcha-solver-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.464227 selenium-recaptcha-solver-1.8.0/
+-rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3280 2023-05-03 07:26:43.463225 selenium-recaptcha-solver-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2023-05-03 07:15:11.000000 selenium-recaptcha-solver-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.457989 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/
+-rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/delay_config.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/exceptions.py
+-rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/services.py
+-rw-rw-rw-   0        0        0     8881 2023-05-03 07:23:51.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/solver.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.462226 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/
+-rw-rw-rw-   0        0        0     3280 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:26:43.464227 selenium-recaptcha-solver-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-05-03 07:26:38.000000 selenium-recaptcha-solver-1.8.0/setup.py
```

### Comparing `selenium-recaptcha-solver-1.7.0/LICENSE` & `selenium-recaptcha-solver-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.7.0/PKG-INFO` & `selenium-recaptcha-solver-1.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.7.0
+Version: 1.8.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
@@ -39,29 +39,28 @@
 ```bash
 python -m pip install selenium-recaptcha-solver
 ```
 
 ## Usage example with ReCAPTCHA demo site
 
 ```python
-from selenium_recaptcha_solver import RecaptchaSolver, StandardDelayConfig
+from selenium_recaptcha_solver import RecaptchaSolver
 from selenium.webdriver.common.by import By
-import undetected_chromedriver as webdriver  # Using an undetected webdriver is recommended, but you can still use a vanilla selenium webdriver.
-import pytest
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
-options = webdriver.ChromeOptions()
+options = Options()
 
 options.add_argument("--headless")
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
-options.add_argument('--incognito')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
 
 test_driver = webdriver.Chrome(options=options)
 
 solver = RecaptchaSolver(driver=test_driver)
@@ -78,18 +77,18 @@
 ## Demonstration
 [![Image from Gyazo](https://i.gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1.gif)](https://gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1)
 
 ## Avoiding detection
 
 To decrease your chances of ReCAPTCHA detecting automated queries, try the following:
 - Use a custom user-agent header (Make sure it's not a headless user-agent!)
-- Use a hard-to-detect web driver (Good example: https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+- Use a hard-to-detect web driver 
 - Use proxies to avoid IP blacklisting
 
 An example of a good user-agent: Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36
 
-An example of a bad user-agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
+An example of a bad user-agent: are Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
 
 Note the last part of the user-agent; the headless specification is usually there.
 
 ## Questions
 If the documentation hasn't covered something, or you have questions about how to use the package or how it works, please reach out.
```

### Comparing `selenium-recaptcha-solver-1.7.0/README.md` & `selenium-recaptcha-solver-1.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,29 +27,28 @@
 ```bash
 python -m pip install selenium-recaptcha-solver
 ```
 
 ## Usage example with ReCAPTCHA demo site
 
 ```python
-from selenium_recaptcha_solver import RecaptchaSolver, StandardDelayConfig
+from selenium_recaptcha_solver import RecaptchaSolver
 from selenium.webdriver.common.by import By
-import undetected_chromedriver as webdriver  # Using an undetected webdriver is recommended, but you can still use a vanilla selenium webdriver.
-import pytest
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
-options = webdriver.ChromeOptions()
+options = Options()
 
 options.add_argument("--headless")
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
-options.add_argument('--incognito')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
 
 test_driver = webdriver.Chrome(options=options)
 
 solver = RecaptchaSolver(driver=test_driver)
@@ -66,18 +65,18 @@
 ## Demonstration
 [![Image from Gyazo](https://i.gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1.gif)](https://gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1)
 
 ## Avoiding detection
 
 To decrease your chances of ReCAPTCHA detecting automated queries, try the following:
 - Use a custom user-agent header (Make sure it's not a headless user-agent!)
-- Use a hard-to-detect web driver (Good example: https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+- Use a hard-to-detect web driver 
 - Use proxies to avoid IP blacklisting
 
 An example of a good user-agent: Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36
 
-An example of a bad user-agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
+An example of a bad user-agent: are Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
 
 Note the last part of the user-agent; the headless specification is usually there.
 
 ## Questions
 If the documentation hasn't covered something, or you have questions about how to use the package or how it works, please reach out.
```

### Comparing `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/services.py` & `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/services.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/solver.py` & `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.common.exceptions import TimeoutException
 from pydub import AudioSegment
-from typing import Optional
+from typing import Union, Optional
 import speech_recognition as sr
 import tempfile
 import requests
 import random
 import uuid
 import time
 import os
@@ -40,34 +40,38 @@
         self._driver = driver
         self._service = service
         self._delay_config = delay_config
 
         # Initialise speech recognition API object
         self._recognizer = sr.Recognizer()
 
-    def click_recaptcha_v2(self, iframe: WebElement) -> None:
+    def click_recaptcha_v2(self, iframe: WebElement, by_selector: Optional[str] = None) -> None:
         """
         Click the "I'm not a robot" checkbox and then solve a reCAPTCHA v2 challenge.
 
         Call this method directly on web pages with an "I'm not a robot" checkbox. See <https://developers.google.com/recaptcha/docs/versions> for details of how this works.
 
         :param iframe: web element for inline frame of reCAPTCHA to solve
+        :param by_selector: By selector to use to find the iframe, if ``iframe`` is a string
         :raises selenium.common.exceptions.TimeoutException: if a timeout occurred while waiting
         """
 
-        self._driver.switch_to.frame(iframe)
+        if isinstance(iframe, str):
+            WebDriverWait(self._driver, 150).until(
+                ec.frame_to_be_available_and_switch_to_it((by_selector, iframe)))
+
+        else:
+            self._driver.switch_to.frame(iframe)
 
-        checkbox = self._driver.find_element(
+        checkbox = self._wait_for_element(
             by='id',
-            value='recaptcha-anchor',
+            locator='recaptcha-anchor',
+            timeout=150,
         )
 
-        if self._delay_config:
-            self._delay_config.delay_before_click_checkbox()
-
         self._js_click(checkbox)
 
         if self._delay_config:
             self._delay_config.delay_after_click_checkbox()
 
         if checkbox.get_attribute('aria-checked') == 'true':
             return
@@ -95,48 +99,30 @@
         self._driver.switch_to.frame(iframe)
 
         # If the captcha image audio is available, locate it. Otherwise, skip to the next line of code.
 
         try:
             self._wait_for_element(
                 by=By.XPATH,
-                locator='//*[@id="recaptcha-image-button"]',
+                locator='//*[@id="recaptcha-audio-button"]',
                 timeout=1,
             ).click()
 
         except TimeoutException:
             pass
 
-        # Locate captcha audio button and click it via JavaScript
-        audio_button = self._wait_for_element(
-            by=By.ID,
-            locator='recaptcha-audio-button',
-            timeout=10,
-        )
-
-        if self._delay_config:
-            self._delay_config.delay_before_click_audio_button()
-
-        self._js_click(audio_button)
-
-        if self._delay_config:
-            self._delay_config.delay_after_click_audio_button()
-
         self._solve_audio_challenge()
 
         # Locate verify button and click it via JavaScript
         verify_button = self._wait_for_element(
             by=By.ID,
             locator='recaptcha-verify-button',
             timeout=5,
         )
 
-        if self._delay_config:
-            self._delay_config.delay_before_click_verify_button()
-
         self._js_click(verify_button)
 
         if self._delay_config:
             self._delay_config.delay_after_click_verify_button()
 
         try:
             self._wait_for_element(
@@ -150,22 +136,16 @@
             # Locate verify button again to avoid stale element reference and click it via JavaScript
             second_verify_button = self._wait_for_element(
                 by=By.ID,
                 locator='recaptcha-verify-button',
                 timeout=5,
             )
 
-            if self._delay_config:
-                self._delay_config.delay_before_click_verify_button()
-
             self._js_click(second_verify_button)
 
-            if self._delay_config:
-                self._delay_config.delay_after_click_verify_button()
-
         except TimeoutException:
             pass
 
         self._driver.switch_to.parent_frame()
 
     def _solve_audio_challenge(self) -> None:
         try:
@@ -216,22 +196,16 @@
         for path in tmp_files:
             if os.path.exists(path):
                 os.remove(path)
 
         # Write transcribed text to iframe's input box
         response_textbox = self._driver.find_element(By.ID, 'audio-response')
 
-        if self._delay_config:
-            self._delay_config.delay_before_type_answer()
-
         self._human_type(element=response_textbox, text=recognized_text)
 
-        if self._delay_config:
-            self._delay_config.delay_after_type_answer()
-
     def _js_click(self, element: WebElement) -> None:
         """
         Perform click on given web element using JavaScript.
 
         :param element: web element to click
         """
```

### Comparing `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/PKG-INFO` & `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.7.0
+Version: 1.8.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
@@ -39,29 +39,28 @@
 ```bash
 python -m pip install selenium-recaptcha-solver
 ```
 
 ## Usage example with ReCAPTCHA demo site
 
 ```python
-from selenium_recaptcha_solver import RecaptchaSolver, StandardDelayConfig
+from selenium_recaptcha_solver import RecaptchaSolver
 from selenium.webdriver.common.by import By
-import undetected_chromedriver as webdriver  # Using an undetected webdriver is recommended, but you can still use a vanilla selenium webdriver.
-import pytest
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
-options = webdriver.ChromeOptions()
+options = Options()
 
 options.add_argument("--headless")
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
-options.add_argument('--incognito')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
 
 test_driver = webdriver.Chrome(options=options)
 
 solver = RecaptchaSolver(driver=test_driver)
@@ -78,18 +77,18 @@
 ## Demonstration
 [![Image from Gyazo](https://i.gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1.gif)](https://gyazo.com/858ceb5df9f43f6aafadf69e233cd2d1)
 
 ## Avoiding detection
 
 To decrease your chances of ReCAPTCHA detecting automated queries, try the following:
 - Use a custom user-agent header (Make sure it's not a headless user-agent!)
-- Use a hard-to-detect web driver (Good example: https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+- Use a hard-to-detect web driver 
 - Use proxies to avoid IP blacklisting
 
 An example of a good user-agent: Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36
 
-An example of a bad user-agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
+An example of a bad user-agent: are Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/92.0.4512.0 Safari/537.36
 
 Note the last part of the user-agent; the headless specification is usually there.
 
 ## Questions
 If the documentation hasn't covered something, or you have questions about how to use the package or how it works, please reach out.
```

### Comparing `selenium-recaptcha-solver-1.7.0/setup.py` & `selenium-recaptcha-solver-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='selenium-recaptcha-solver',
-    version='1.7.0',
+    version='1.8.0',
     license='MIT',
     author='Tomás Perestrelo',
     author_email='tomasperestrelo21@gmail.com',
     packages=find_packages(exclude=('tests*', 'testing*')),
     url='https://github.com/thicccat688/selenium-recaptcha-solver',
     download_url='https://pypi.org/project/selenium-recaptcha-solver',
     keywords='python, captcha, speech recognition, selenium, web automation',
```

