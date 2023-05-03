# Comparing `tmp/toolium-3.0.0a4.tar.gz` & `tmp/toolium-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.0a4.tar", last modified: Mon Apr  3 07:17:26 2023, max compression
+gzip compressed data, was "toolium-3.0.0b1.tar", last modified: Tue Apr 25 13:22:15 2023, max compression
```

## Comparing `toolium-3.0.0a4.tar` & `toolium-3.0.0b1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:26.033852 toolium-3.0.0a4/
--rw-rw-rw-   0        0        0    28962 2023-04-03 07:16:13.000000 toolium-3.0.0a4/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.0a4/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     5523 2023-04-03 07:17:26.033852 toolium-3.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-03-28 11:00:00.000000 toolium-3.0.0a4/README.rst
--rw-rw-rw-   0        0        0        9 2023-04-03 07:16:49.000000 toolium-3.0.0a4/VERSION
--rw-rw-rw-   0        0        0      229 2023-03-28 11:00:00.000000 toolium-3.0.0a4/requirements.txt
--rw-rw-rw-   0        0        0      197 2023-03-28 11:00:00.000000 toolium-3.0.0a4/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-04-03 07:17:26.034854 toolium-3.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-03-28 11:00:00.000000 toolium-3.0.0a4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.880851 toolium-3.0.0a4/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0a4/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.904851 toolium-3.0.0a4/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0a4/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12432 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    11068 2023-03-28 11:00:00.000000 toolium-3.0.0a4/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    20883 2023-04-03 07:16:13.000000 toolium-3.0.0a4/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-03 07:16:13.000000 toolium-3.0.0a4/toolium/config_parser.py
--rw-rw-rw-   0        0        0    17134 2023-03-31 08:07:03.000000 toolium-3.0.0a4/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18420 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.964854 toolium-3.0.0a4/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.981855 toolium-3.0.0a4/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0a4/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.993852 toolium-3.0.0a4/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-03-31 13:44:01.000000 toolium-3.0.0a4/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8668 2023-03-28 11:00:00.000000 toolium-3.0.0a4/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:26.031851 toolium-3.0.0a4/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-03 07:16:35.000000 toolium-3.0.0a4/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31863 2023-04-03 07:16:35.000000 toolium-3.0.0a4/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18522 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-03-28 11:00:00.000000 toolium-3.0.0a4/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    14292 2023-03-27 14:34:03.000000 toolium-3.0.0a4/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-03-31 08:07:03.000000 toolium-3.0.0a4/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-04-03 07:17:25.889851 toolium-3.0.0a4/toolium.egg-info/
--rw-rw-rw-   0        0        0     5523 2023-04-03 07:17:25.000000 toolium-3.0.0a4/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-04-03 07:17:25.000000 toolium-3.0.0a4/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 07:17:25.000000 toolium-3.0.0a4/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-04-03 07:17:25.000000 toolium-3.0.0a4/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 07:17:25.000000 toolium-3.0.0a4/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.510889 toolium-3.0.0b1/
+-rw-rw-rw-   0        0        0    29325 2023-04-25 10:06:44.000000 toolium-3.0.0b1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5523 2023-04-25 13:22:15.511892 toolium-3.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-04 16:24:15.000000 toolium-3.0.0b1/README.rst
+-rw-rw-rw-   0        0        0        9 2023-04-15 11:17:06.000000 toolium-3.0.0b1/VERSION
+-rw-rw-rw-   0        0        0      225 2023-04-11 07:34:47.000000 toolium-3.0.0b1/requirements.txt
+-rw-rw-rw-   0        0        0      193 2023-04-11 07:34:47.000000 toolium-3.0.0b1/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-04-25 13:22:15.512892 toolium-3.0.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-04 16:24:15.000000 toolium-3.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.287892 toolium-3.0.0b1/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.319891 toolium-3.0.0b1/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12432 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    10586 2023-04-11 07:34:47.000000 toolium-3.0.0b1/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21012 2023-04-17 09:39:11.000000 toolium-3.0.0b1/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16655 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.398888 toolium-3.0.0b1/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.430889 toolium-3.0.0b1/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.449890 toolium-3.0.0b1/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8668 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.508891 toolium-3.0.0b1/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    31093 2023-04-25 10:44:38.000000 toolium-3.0.0b1/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-15 11:02:04.000000 toolium-3.0.0b1/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.299890 toolium-3.0.0b1/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5523 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.0a4/CHANGELOG.rst` & `toolium-3.0.0b1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 ------
 
 *Release date: In development*
 
 - Add support for Python 3.11
 - Add support for Selenium 4
 - Add support for Appium-Python-Client 2
-- Remove support for lettuce tests
 - Visual testing comparison has changed
 
    | It only needs PIL library to compare images and generate the differences images
    | Old PerceptualDiff and Magick engines have been removed
-   | Config property 'visualtests_engine' in [Server] section has been removed
+   | Config property `engine` in [VisualTests] section has been removed
    | Images distance calculation method has changed, it is recommended to review thresholds in tests
 
 - Now `gecko_driver_path`, `chrome_driver_path`, `explorer_driver_path` and `edge_driver_path` config properties
   in [Driver] section are optional, due to new SeleniumManager feature, that downloads drivers automatically
 - New optional config property `safari_driver_path` in [Driver] section to configure Safari driver
-- New optional config property `options` in [Chromer] section to configure Chrome options instead of using old
+- New optional config property `options` in [Chrome] section to configure Chrome options instead of using old
   property `goog:chromeOptions` in [Capabilities] section.
+- New optional config property `base_path` in [Server] section to allow using old Selenium 3 or Appium 1 remote servers
 - Update [RANDOM_PHONE_NUMBER] replacement using new `DataGenerator` class
+- Remove support for lettuce tests
+- Remove deprecated parameter `context` from `map_param` and POEditor methods
+- Remove deprecated config property `restart_driver_fail` in [Driver] section
+- Remove deprecated environment variables `Section_option`, `Config_environment` and `env`
 
 v2.7.0
 ------
 
 *Release date: 2023-02-24*
 
 - Fix drivers not being closed in `after_feature` when errors occur during `before_feature` steps execution
```

### Comparing `toolium-3.0.0a4/LICENSE` & `toolium-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/PKG-INFO` & `toolium-3.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.0a4
+Version: 3.0.0b1
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.0a4/README.rst` & `toolium-3.0.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/setup.py` & `toolium-3.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/behave/env_utils.py` & `toolium-3.0.0b1/toolium/behave/env_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/behave/environment.py` & `toolium-3.0.0b1/toolium/behave/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,30 @@
 limitations under the License.
 """
 
 import logging
 import os
 import re
 
-try:
-    from behave_pytest.hook import install_pytest_asserts
-except ImportError:
-    def install_pytest_asserts():
-        pass
-
 from toolium.utils import dataset
 from toolium.config_files import ConfigFiles
 from toolium.driver_wrapper import DriverWrappersPool
 from toolium.jira import add_jira_status, change_all_jira_status, save_jira_conf
 from toolium.visual_test import VisualTest
 from toolium.pageelements import PageElement
 from toolium.behave.env_utils import DynamicEnvironment
 
 
 def before_all(context):
     """Initialization method that will be executed before the test execution
 
     :param context: behave context
     """
-    # Use pytest asserts if behave_pytest is installed
-    install_pytest_asserts()
-
     # Get 'TOOLIUM_CONFIG_ENVIRONMENT' property from user input (e.g. -D TOOLIUM_CONFIG_ENVIRONMENT=ios)
     env = context.config.userdata.get('TOOLIUM_CONFIG_ENVIRONMENT')
-    # Deprecated: use TOOLIUM_CONFIG_ENVIRONMENT property
-    env = env if env else context.config.userdata.get('Config_environment')
-    # Deprecated: use TOOLIUM_CONFIG_ENVIRONMENT property
-    env = env if env else context.config.userdata.get('env')
     if env:
         os.environ['TOOLIUM_CONFIG_ENVIRONMENT'] = env
 
     if not hasattr(context, 'config_files'):
         context.config_files = ConfigFiles()
     context.config_files = DriverWrappersPool.initialize_config_files(context.config_files)
```

### Comparing `toolium-3.0.0a4/toolium/config_driver.py` & `toolium-3.0.0b1/toolium/config_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         :returns: a new remote selenium driver
         """
         # Get version and platform capabilities
         capabilities = self._get_capabilities_from_driver_type()
 
         # Get server url
-        server_url = f'{self.utils.get_server_url()}/wd/hub'
+        server_url = f"{self.utils.get_server_url()}{self.config.get_optional('Server', 'base_path', '')}"
 
         driver_name = self.utils.get_driver_name()
         if driver_name in ('android', 'ios', 'iphone'):
             # Get driver options
             options = AppiumOptions()
             self._add_capabilities_from_properties(capabilities, 'AppiumCapabilities')
             self._update_dict(options.capabilities, capabilities)
@@ -117,15 +117,15 @@
             # Get driver options
             if driver_name == 'firefox':
                 options = self._get_firefox_options(capabilities)
             elif driver_name == 'chrome':
                 options = self._get_chrome_options(capabilities)
             elif driver_name == 'safari':
                 options = self._get_safari_options(capabilities)
-            elif driver_name == 'explorer':
+            elif driver_name == 'iexplore':
                 options = self._get_explorer_options(capabilities)
             elif driver_name == 'edge':
                 options = self._get_edge_options(capabilities)
 
             # Create remote web driver
             driver = webdriver.Remote(command_executor=server_url, options=options)
 
@@ -188,14 +188,15 @@
 
         :param capabilities: capabilities object
         :param section: properties section
         """
         cap_type = {'Capabilities': 'server', 'AppiumCapabilities': 'Appium server'}
         try:
             for cap, cap_value in dict(self.config.items(section)).items():
+                cap = f'appium:{cap}' if section == 'AppiumCapabilities' else cap
                 self.logger.debug("Added %s capability: %s = %s", cap_type[section], cap, cap_value)
                 cap_value = cap_value if cap == 'browserVersion' else self._convert_property_type(cap_value)
                 self._update_dict(capabilities, {cap: cap_value}, initial_key=cap)
         except NoSectionError:
             pass
 
     def _setup_firefox(self):
```

### Comparing `toolium-3.0.0a4/toolium/config_files.py` & `toolium-3.0.0b1/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/config_parser.py` & `toolium-3.0.0b1/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/driver_wrapper.py` & `toolium-3.0.0b1/toolium/driver_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,22 @@
         """Configure selenium instance logger
 
         :param tc_config_log_filename: test case specific logging config file
         :param tc_output_log_filename: test case specific output logger file
         """
         # Get config logger filename
         config_log_filename = DriverWrappersPool.get_configured_value('TOOLIUM_CONFIG_LOG_FILENAME',
-                                                                      'Config_log_filename', tc_config_log_filename,
-                                                                      'logging.conf')
+                                                                      tc_config_log_filename, 'logging.conf')
         config_log_filename = os.path.join(DriverWrappersPool.config_directory, config_log_filename)
 
         # Configure logger only if logging filename has changed
         if self.config_log_filename != config_log_filename:
             # Get output logger filename
             output_log_filename = DriverWrappersPool.get_configured_value('TOOLIUM_OUTPUT_LOG_FILENAME',
-                                                                          'Output_log_filename', tc_output_log_filename,
-                                                                          'toolium.log')
+                                                                          tc_output_log_filename, 'toolium.log')
             output_log_filename = os.path.join(DriverWrappersPool.output_directory, output_log_filename)
             output_log_filename = output_log_filename.replace('\\', '\\\\')
 
             try:
                 logging.config.fileConfig(config_log_filename, {'logfilename': output_log_filename}, False)
             except Exception as exc:
                 print("[WARN] Error reading logging config file '{}': {}".format(config_log_filename, exc))
@@ -110,29 +108,26 @@
     def configure_properties(self, tc_config_prop_filenames=None, behave_properties=None):
         """Configure selenium instance properties
 
         :param tc_config_prop_filenames: test case specific properties filenames
         :param behave_properties: dict with behave user data properties
         """
         prop_filenames = DriverWrappersPool.get_configured_value('TOOLIUM_CONFIG_PROPERTIES_FILENAMES',
-                                                                 'Config_prop_filenames', tc_config_prop_filenames,
+                                                                 tc_config_prop_filenames,
                                                                  'properties.cfg;local-properties.cfg')
         prop_filenames = [os.path.join(DriverWrappersPool.config_directory, filename) for filename in
                           prop_filenames.split(';')]
         prop_filenames = ';'.join(prop_filenames)
 
         # Configure config only if properties filename has changed
         if self.config_properties_filenames != prop_filenames:
             # Initialize the config object
             self.config = ExtendedConfigParser.get_config_from_file(prop_filenames)
             self.config_properties_filenames = prop_filenames
 
-        # Override properties with system properties [Deprecated: use toolium system properties]
-        self.config.update_properties(os.environ)
-
         # Override properties with toolium system properties
         self.config.update_toolium_system_properties(os.environ)
 
         # Override properties with behave userdata properties
         if behave_properties:
             self.config.update_properties(behave_properties)
 
@@ -342,16 +337,15 @@
         :param scope: execution scope (function, module, class or session)
         :param test_passed: True if the test has passed
         :param context: behave context
         :returns: True if the driver should be reused
         """
         reuse_driver = self.config.getboolean_optional('Driver', 'reuse_driver')
         reuse_driver_session = self.config.getboolean_optional('Driver', 'reuse_driver_session')
-        restart_driver_after_failure = (self.config.getboolean_optional('Driver', 'restart_driver_after_failure') or
-                                        self.config.getboolean_optional('Driver', 'restart_driver_fail'))
+        restart_driver_after_failure = self.config.getboolean_optional('Driver', 'restart_driver_after_failure')
         if context and scope == 'function':
             reuse_driver = reuse_driver or (hasattr(context, 'reuse_driver_from_tags')
                                             and context.reuse_driver_from_tags)
         return (((reuse_driver and scope == 'function') or (reuse_driver_session and scope != 'session'))
                 and (test_passed or not restart_driver_after_failure))
 
     def get_driver_platform(self):
```

### Comparing `toolium-3.0.0a4/toolium/driver_wrappers_pool.py` & `toolium-3.0.0b1/toolium/driver_wrappers_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,57 +247,52 @@
                         driver_wrapper.utils.save_webdriver_logs(log_file_name)
                 except Exception as exc:
                     # Capture exceptions to avoid errors in teardown method due to session timeouts
                     driver_wrapper.logger.warning('Error downloading webdriver logs: %s' % exc)
             driver_index += 1
 
     @staticmethod
-    def get_configured_value(system_property_name, deprecated_system_property_name, specific_value, default_value):
+    def get_configured_value(system_property_name, specific_value, default_value):
         """Get configured value from system properties, method parameters or default value
 
         :param system_property_name: system property name
-        :param deprecated_system_property_name: deprecated system property name
         :param specific_value: test case specific value
         :param default_value: default value
         :returns: configured value
         """
         try:
             return os.environ[system_property_name]
         except KeyError:
-            try:
-                return os.environ[deprecated_system_property_name]
-            except KeyError:
-                return specific_value if specific_value else default_value
+            return specific_value if specific_value else default_value
 
     @classmethod
     def configure_common_directories(cls, tc_config_files):
         """Configure common config and output folders for all tests
 
         :param tc_config_files: test case specific config files
         """
         if cls.config_directory is None:
             # Get config directory from properties
-            config_directory = cls.get_configured_value('TOOLIUM_CONFIG_DIRECTORY', 'Config_directory',
+            config_directory = cls.get_configured_value('TOOLIUM_CONFIG_DIRECTORY',
                                                         tc_config_files.config_directory, 'conf')
-            prop_filenames = cls.get_configured_value('TOOLIUM_CONFIG_PROPERTIES_FILENAMES', 'Config_prop_filenames',
+            prop_filenames = cls.get_configured_value('TOOLIUM_CONFIG_PROPERTIES_FILENAMES',
                                                       tc_config_files.config_properties_filenames, 'properties.cfg')
             cls.config_directory = cls._find_parent_directory(config_directory, prop_filenames.split(';')[0])
 
             # Get output directory from properties and create it
-            cls.output_directory = cls.get_configured_value('TOOLIUM_OUTPUT_DIRECTORY', 'Output_directory',
+            cls.output_directory = cls.get_configured_value('TOOLIUM_OUTPUT_DIRECTORY',
                                                             tc_config_files.output_directory, 'output')
             if not os.path.isabs(cls.output_directory):
                 # If output directory is relative, we use the same path as config directory
                 cls.output_directory = os.path.join(os.path.dirname(cls.config_directory), cls.output_directory)
             makedirs_safe(cls.output_directory)
 
             # Get visual baseline directory from properties
             default_baseline = os.path.join(cls.output_directory, 'visualtests', 'baseline')
             cls.visual_baseline_directory = cls.get_configured_value('TOOLIUM_VISUAL_BASELINE_DIRECTORY',
-                                                                     'Visual_baseline_directory',
                                                                      tc_config_files.visual_baseline_directory,
                                                                      default_baseline)
             if not os.path.isabs(cls.visual_baseline_directory):
                 # If baseline directory is relative, we use the same path as config directory
                 cls.visual_baseline_directory = os.path.join(os.path.dirname(cls.config_directory),
                                                              cls.visual_baseline_directory)
 
@@ -360,15 +355,15 @@
         :returns: initialized config files object
         """
         # Initialize config files
         if tc_config_files is None:
             tc_config_files = ConfigFiles()
 
         # Update properties and log file names if an environment is configured
-        env = DriverWrappersPool.get_configured_value('TOOLIUM_CONFIG_ENVIRONMENT', 'Config_environment', None, None)
+        env = DriverWrappersPool.get_configured_value('TOOLIUM_CONFIG_ENVIRONMENT', None, None)
         if env:
             # Update config properties filenames
             prop_filenames = tc_config_files.config_properties_filenames
             new_prop_filenames_list = prop_filenames.split(';') if prop_filenames else ['properties.cfg']
             base, ext = os.path.splitext(new_prop_filenames_list[0])
             new_prop_filenames_list.append('{}-{}{}'.format(env, base, ext))
             new_prop_filenames_list.append('local-{}-{}{}'.format(env, base, ext))
```

### Comparing `toolium-3.0.0a4/toolium/jira.py` & `toolium-3.0.0b1/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/__init__.py` & `toolium-3.0.0b1/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/button_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/checkbox_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/group_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/input_radio_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/input_text_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/link_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/page_element.py` & `toolium-3.0.0b1/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/page_elements.py` & `toolium-3.0.0b1/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/select_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageelements/text_page_element.py` & `toolium-3.0.0b1/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageobjects/common_object.py` & `toolium-3.0.0b1/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageobjects/mobile_page_object.py` & `toolium-3.0.0b1/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pageobjects/page_object.py` & `toolium-3.0.0b1/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/pytest_fixtures.py` & `toolium-3.0.0b1/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/resources/VisualTests.css` & `toolium-3.0.0b1/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/resources/VisualTests.js` & `toolium-3.0.0b1/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/resources/VisualTestsTemplate.html` & `toolium-3.0.0b1/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/selenoid.py` & `toolium-3.0.0b1/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/test_cases.py` & `toolium-3.0.0b1/toolium/test_cases.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/utils/data_generator.py` & `toolium-3.0.0b1/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/utils/dataset.py` & `toolium-3.0.0b1/toolium/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 import datetime
 import json
 import logging
 import os
 import random as r
 import re
 import string
+import uuid
+
 from ast import literal_eval
 from copy import deepcopy
-import uuid
+from inspect import isfunction
 from toolium.utils.data_generator import DataGenerator
 
 logger = logging.getLogger(__name__)
 
 # Base path for BASE64 and FILE conversions
 base_base64_path = ''
 base_file_path = ''
@@ -62,19 +64,21 @@
         [NULL] Generates a None object
         [TRUE] Generates a boolean True
         [FALSE] Generates a boolean False
         [EMPTY] Generates an empty string
         [B] Generates a blank space
         [UUID] Generates a v4 UUID
         [RANDOM] Generates a random value
-        [RANDOM_PHONE_NUMBER] Generates a random phone number following the pattern +34654XXXXXX, using the language and country specified in dataset.language and dataset.country
+        [RANDOM_PHONE_NUMBER] Generates a random phone number for language and country configured in dataset.language
+            and dataset.country
         [TIMESTAMP] Generates a timestamp from the current time
         [DATETIME] Generates a datetime from the current time
         [NOW] Similar to DATETIME without milliseconds; the format depends on the language
-        [NOW(%Y-%m-%dT%H:%M:%SZ)] Same as NOW but using an specific format by the python strftime function of the datetime module
+        [NOW(%Y-%m-%dT%H:%M:%SZ)] Same as NOW but using an specific format by the python strftime function of the
+            datetime module
         [NOW + 2 DAYS] Similar to NOW but two days later
         [NOW - 1 MINUTES] Similar to NOW but one minute earlier
         [NOW(%Y-%m-%dT%H:%M:%SZ) - 7 DAYS] Similar to NOW but seven days before and with the indicated format
         [TODAY] Similar to NOW without time; the format depends on the language
         [TODAY + 2 DAYS] Similar to NOW, but two days later
         [STR:xxxx] Cast xxxx to a string
         [INT:xxxx] Cast xxxx to an int
@@ -142,25 +146,25 @@
             param_replaced = True
             break
     return new_param, param_replaced
 
 
 def _find_param_date_expressions(param):
     """
-    Finds in a param one or several date expressions. 
+    Finds in a param one or several date expressions.
     For example, for a param like "it happened on [NOW - 1 MONTH] of the last year and will happen [TODAY('%d/%m')]",
     this method returns an array with two string elements: "[NOW - 1 MONTH]" and [TODAY('%d/%m')]"
     The kind of expressions to search are based on these rules:
     - expression is sorrounded by [ and ]
     - first word of the expression is either NOW or TODAY
-    - when first word is NOW, it can have an addtional format for the date between parenthesis, 
+    - when first word is NOW, it can have an addtional format for the date between parenthesis,
         like NOW(%Y-%m-%dT%H:%M:%SZ). The definition of the format is the same as considered by the
         python strftime function of the datetime module
-    - and optional offset can be given by indicating how many days, hours, etc.. to add or remove to the current datetime.
-        This part of the expression includes a +/- symbol plus a number and a unit
+    - and optional offset can be given by indicating how many days, hours, etc.. to add or remove to the current
+        datetime. This part of the expression includes a +/- symbol plus a number and a unit
 
     Some valid expressions are:
         [NOW]
         [TODAY]
         [NOW(%Y-%m-%dT%H:%M:%SZ)]
         [NOW(%Y-%m-%dT%H:%M:%SZ) - 180 DAYS]
         [NOW(%H:%M:%S) + 4 MINUTES]
@@ -187,35 +191,41 @@
     alphanums = ''.join([string.ascii_lowercase, string.digits])  # abcdefghijklmnopqrstuvwxyz0123456789
     replacements = {
         '[EMPTY]': '',
         '[B]': ' ',
         '[UUID]': str(uuid.uuid4()),
         # make sure random is not made up of digits only, by forcing the first char to be a letter
         '[RANDOM]': ''.join([r.choice(string.ascii_lowercase), *(r.choice(alphanums) for i in range(7))]),
-        '[RANDOM_PHONE_NUMBER]': DataGenerator().phone_number,
+        '[RANDOM_PHONE_NUMBER]': _get_random_phone_number,
         '[TIMESTAMP]': str(int(datetime.datetime.timestamp(datetime.datetime.utcnow()))),
         '[DATETIME]': str(datetime.datetime.utcnow()),
         '[NOW]': str(datetime.datetime.utcnow().strftime(date_format)),
         '[TODAY]': str(datetime.datetime.utcnow().strftime(date_day_format))
     }
-    
-    # append date expressions found in param to the replacement dict 
+
+    # append date expressions found in param to the replacement dict
     date_expressions = _find_param_date_expressions(param)
     for date_expr in date_expressions:
         replacements[date_expr] = _replace_param_date(date_expr, language)[0]
 
     new_param = param
     param_replaced = False
     for key in replacements.keys():
         if key in new_param:
-            new_param = new_param.replace(key, replacements[key])
+            new_value = replacements[key]() if isfunction(replacements[key]) else replacements[key]
+            new_param = new_param.replace(key, new_value)
             param_replaced = True
     return new_param, param_replaced
 
 
+def _get_random_phone_number():
+    # Method to avoid executing data generator when it is not needed
+    return DataGenerator().phone_number
+
+
 def _replace_param_transform_string(param):
     """
     Transform param value according to the specified prefix.
     Available transformations: DICT, LIST, INT, FLOAT, STR, UPPER, LOWER
 
     :param param: parameter value
     :return: tuple with replaced value and boolean to know if replacement has been done
@@ -241,29 +251,29 @@
 
 
 def _replace_param_date(param, language):
     """
     Transform param value in a date after applying the specified delta.
     E.g. [TODAY - 2 DAYS], [NOW - 10 MINUTES]
     An specific format could be defined in the case of NOW this way: NOW('THEFORMAT')
-    where THEFORMAT is any valid format accepted by the python 
-    [datetime.strftime](https://docs.python.org/3/library/datetime.html#datetime.date.strftime) function 
+    where THEFORMAT is any valid format accepted by the python
+    [datetime.strftime](https://docs.python.org/3/library/datetime.html#datetime.date.strftime) function
 
     :param param: parameter value
     :param language: language to configure date format for NOW and TODAY
     :return: tuple with replaced value and boolean to know if replacement has been done
     """
     def _date_matcher():
         return re.match(r'\[(NOW(?:\((?:.*)\)|)|TODAY)(?:\s*([\+|-]\s*\d+)\s*(\w+)\s*)?\]', param)
 
     def _offset_datetime(amount, units):
         now = datetime.datetime.utcnow()
         if not amount or not units:
             return now
-        the_amount = int(amount.replace(' ',''))
+        the_amount = int(amount.replace(' ', ''))
         the_units = units.lower()
         return now + datetime.timedelta(**dict([(the_units, the_amount)]))
 
     def _is_only_date(base):
         return 'TODAY' in base
 
     def _default_format(base):
@@ -345,42 +355,23 @@
             if param.startswith('{') or param.startswith('['):
                 new_param = json.loads(param)
         except Exception:
             pass
     return new_param
 
 
-# Ignore flake8 warning until deprecated context parameter is removed
-# flake8: noqa: C901
-def map_param(param, context=None):
+def map_param(param):
     """
     Transform the given string by replacing specific patterns containing keys with their values,
     which can be obtained from the Behave context or from environment files or variables.
     See map_one_param function for a description of the available tags and replacement logic.
 
     :param param: string parameter
-    :param context: Behave context object (deprecated parameter)
     :return: string with the applied replacements
     """
-    if context:
-        logger.warning('Deprecated context parameter has been sent to map_param method. Please, configure dataset'
-                       ' global variables instead of passing context to map_param.')
-        global language, language_terms, project_config, toolium_config, poeditor_terms, behave_context
-        if hasattr(context, 'language'):
-            language = context.language
-        if hasattr(context, 'language_dict'):
-            language_terms = context.language_dict
-        if hasattr(context, 'project_config'):
-            project_config = context.project_config
-        if hasattr(context, 'toolium_config'):
-            toolium_config = context.toolium_config
-        if hasattr(context, 'poeditor_export'):
-            poeditor_terms = context.poeditor_export
-        behave_context = context
-
     if not isinstance(param, str):
         return param
 
     map_regex = r"[\[CONF:|\[LANG:|\[POE:|\[ENV:|\[BASE64:|\[TOOLIUM:|\[CONTEXT:|\[FILE:][a-zA-Z\.\:\/\_\-\ 0-9]*\]"
     map_expressions = re.compile(map_regex)
 
     mapped_param = param
@@ -390,15 +381,15 @@
     else:
         # The parameter is a combination of text and configuration parameters.
         for match in map_expressions.findall(param):
             mapped_param = mapped_param.replace(match, str(map_one_param(match)))
 
     if mapped_param != param:
         # Calling to map_param recursively to replace parameters that include another parameters
-        mapped_param = map_param(mapped_param, context)
+        mapped_param = map_param(mapped_param)
 
     return mapped_param
 
 
 def map_one_param(param):
     """
     Analyze the pattern in the given string and find out its transformed value.
@@ -562,15 +553,15 @@
     :param config: toolium config object
     :return: mapped value
     """
     try:
         section = param.split("_", 1)[0]
         property_name = param.split("_", 1)[1]
     except IndexError:
-        msg = f"Invalid format in Toolium config param '{param}'. Valid format: 'Section_property'."
+        msg = f"Invalid format in Toolium config param '{param}'. Valid format: 'Section_option'."
         logger.error(msg)
         raise IndexError(msg)
 
     try:
         mapped_value = config.get(section, property_name)
         logger.debug(f"Mapping Toolium config param 'param' to its configured value '{mapped_value}'")
     except Exception:
@@ -585,15 +576,15 @@
     Find the value of the given param using it as a key in the context storage dictionary (context.storage) or in the
     context object itself. The key might be comprised of dotted tokens. In such case, the searched key is the first
     token. The rest of the tokens are considered nested properties/objects.
     So, for example, in the basic case, "last_request_result" could be used as key that would be searched into context
     storage or the context object itself. In a dotted case, "last_request.result" is searched as a "last_request" key
     in the context storage or as a property of the context object whose name is last_request. In both cases, when found,
     "result" is considered (and resolved) as a property into the returned value.
-    
+
     There is not limit in the nested levels of dotted tokens, so a key like a.b.c.d will be tried to be resolved as:
 
     context.storage['a'].b.c.d
         or
     context.a.b.c.d
 
     :param param: key to be searched (e.g. "last_request_result" / "last_request.result")
@@ -621,15 +612,14 @@
             msg = f"'{part}' is not an attribute of {value}"
             logger.error(msg)
             raise AttributeError(msg)
 
     return value
 
 
-
 def get_message_property(param, language_terms, language_key):
     """
     Return the message for the given param, using it as a key in the list of language properties.
     Dot notation is used (e.g. "home.button.send").
 
     :param param: message key
     :param language_terms: dict with language terms
@@ -654,15 +644,15 @@
     """
     Return the translation(s) for the given POEditor reference from the given terms in poeditor_terms.
 
     :param reference: POEditor reference
     :param poeditor_terms: poeditor terms
     :return: list of strings with the translations from POEditor or string with the translation if only one was found
     """
-    poeditor_config = project_config['poeditor'] if 'poeditor' in project_config else {}
+    poeditor_config = project_config['poeditor'] if project_config and 'poeditor' in project_config else {}
     key = poeditor_config['key_field'] if 'key_field' in poeditor_config else 'reference'
     search_type = poeditor_config['search_type'] if 'search_type' in poeditor_config else 'contains'
     # Get POEditor prefixes and add no prefix option
     poeditor_prefixes = poeditor_config['prefixes'] if 'prefixes' in poeditor_config else []
     poeditor_prefixes.append('')
     translation = []
     for prefix in poeditor_prefixes:
```

### Comparing `toolium-3.0.0a4/toolium/utils/download_files.py` & `toolium-3.0.0b1/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/utils/driver_utils.py` & `toolium-3.0.0b1/toolium/utils/driver_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         server_type = 'local'
         if self.driver_wrapper.config.getboolean_optional('Server', 'enabled'):
             # Request session info from grid hub
             session_id = self.driver_wrapper.driver.session_id
             self.logger.debug("Trying to identify remote node")
             try:
                 # Request session info from grid hub and extract remote node
-                url = '{}/grid/api/testsession?session={}'.format(self.get_server_url(),
-                                                                  session_id)
+                url = '{}/grid/api/testsession?session={}'.format(self.get_server_url(), session_id)
                 proxy_id = requests.get(url).json()['proxyId']
                 remote_node = urlparse(proxy_id).hostname if urlparse(proxy_id).hostname else proxy_id
                 server_type = 'grid'
                 self.logger.debug("Test running in remote node %s", remote_node)
             except (ValueError, KeyError):
                 try:
                     # Request session info from GGR and extract remote node
```

### Comparing `toolium-3.0.0a4/toolium/utils/driver_wait_utils.py` & `toolium-3.0.0b1/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/utils/path_utils.py` & `toolium-3.0.0b1/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium/utils/poeditor.py` & `toolium-3.0.0b1/toolium/utils/poeditor.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,35 +69,28 @@
 ENDPOINT_POEDITOR_EXPORT_PROJECT = "v2/projects/export"
 ENDPOINT_POEDITOR_DOWNLOAD_FILE = "v2/download/file"
 
 # Configure logger
 logger = logging.getLogger(__name__)
 
 
-def download_poeditor_texts(context=None, file_type='json'):
+def download_poeditor_texts(file_type='json'):
     """
     Executes all steps to download texts from POEditor and saves them to a file in output dir
 
-    :param context: behave context (deprecated)
     :param file_type: file type (only json supported)
     :return: N/A
     """
-    if context:
-        logger.warning('Deprecated context parameter has been sent to download_poeditor_texts method. Please, configure'
-                       ' dataset global variables instead of passing context to download_poeditor_texts.')
     project_info = get_poeditor_project_info_by_name()
     language_codes = get_poeditor_language_codes(project_info)
     language = get_valid_lang(language_codes)
     poeditor_terms = export_poeditor_project(project_info, language, file_type)
     save_downloaded_file(poeditor_terms)
     # Save terms in dataset to be used in [POE:] map_param replacements
     dataset.poeditor_terms = poeditor_terms
-    if context:
-        # Save terms in context for backwards compatibility
-        context.poeditor_export = dataset.poeditor_terms
 
 
 def get_poeditor_project_info_by_name(project_name=None):
     """
     Get POEditor project info from project name from config or parameter
 
     :param project_name: POEditor project name
@@ -134,32 +127,25 @@
     language_codes = [lang['code'] for lang in response_data['result']['languages']]
     assert not len(language_codes) == 0, "ERROR: Not languages found in POEditor"
     logger.info('POEditor languages in "%s" project: %s %s' % (project_info['name'], len(language_codes),
                                                                language_codes))
     return language_codes
 
 
-def search_terms_with_string(context=None, lang=None):
+def search_terms_with_string(lang=None):
     """
     Saves POEditor terms for a given existing language in that project
 
-    :param context: behave context (deprecated)
     :param lang: a valid language existing in that POEditor project
     :return: N/A (saves it to context.poeditor_terms)
     """
-    if context:
-        logger.warning('Deprecated context parameter has been sent to search_terms_with_string method. Please, '
-                       'configure dataset global variables instead of passing context to search_terms_with_string.')
     project_info = get_poeditor_project_info_by_name()
     language_codes = get_poeditor_language_codes(project_info)
     language = get_valid_lang(language_codes, lang)
     dataset.poeditor_terms = get_all_terms(project_info, language)
-    if context:
-        # Save terms in context for backwards compatibility
-        context.poeditor_terms = dataset.poeditor_terms
 
 
 def export_poeditor_project(project_info, lang, file_type):
     """
     Export all texts in project to a given file type
 
     :param project_info: project info
@@ -294,24 +280,18 @@
     response_data = r.json()
     assert_poeditor_response_code(response_data, "200")
     terms = response_data['result']['terms']
     logger.info('POEditor terms in "%s" project with "%s" language: %s' % (project_info['name'], lang, len(terms)))
     return terms
 
 
-def load_poeditor_texts(context=None):
+def load_poeditor_texts():
     """
     Download POEditor texts and save in output folder if the config exists or use previously downloaded texts
-
-    :param context: behave context (deprecated parameter)
     """
-    if context:
-        logger.warning('Deprecated context parameter has been sent to load_poeditor_texts method. Please, '
-                       'configure POEditor global variables instead of passing context to load_poeditor_texts.')
-
     if get_poeditor_api_token():
         # Try to get poeditor mode param from toolium config first
         poeditor_mode = dataset.toolium_config.get_optional('TestExecution', 'poeditor_mode')
         if poeditor_mode:
             dataset.project_config['poeditor']['mode'] = poeditor_mode
         if 'mode' in dataset.project_config['poeditor'] and map_param('[CONF:poeditor.mode]') == 'offline':
             file_path = get_poeditor_file_path()
@@ -321,21 +301,18 @@
                 error_message = 'You are using offline POEditor mode but poeditor file has not been found in %s' % \
                                 file_path
                 logger.error(error_message)
                 assert False, error_message
 
             with open(file_path, 'r') as f:
                 dataset.poeditor_terms = json.load(f)
-                if context:
-                    # Workaround for backwards compatibility
-                    context.poeditor_export = dataset.poeditor_terms
                 last_mod_time = time.strftime('%d/%m/%Y %H:%M:%S', time.localtime(os.path.getmtime(file_path)))
                 logger.info('Using local POEditor file "%s" with date: %s' % (file_path, last_mod_time))
         else:  # without mode configured or mode = 'online'
-            download_poeditor_texts(context)
+            download_poeditor_texts()
     else:
         logger.info("POEditor is not configured")
 
 
 def get_poeditor_file_path():
     """
     Get configured POEditor file path or default file path
```

### Comparing `toolium-3.0.0a4/toolium/visual_test.py` & `toolium-3.0.0b1/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0a4/toolium.egg-info/PKG-INFO` & `toolium-3.0.0b1/toolium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.0a4
+Version: 3.0.0b1
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.0a4/toolium.egg-info/SOURCES.txt` & `toolium-3.0.0b1/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

