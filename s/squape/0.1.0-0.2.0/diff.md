# Comparing `tmp/squape-0.1.0.tar.gz` & `tmp/squape-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squape-0.1.0.tar", last modified: Mon Apr 17 17:37:53 2023, max compression
+gzip compressed data, was "squape-0.2.0.tar", last modified: Wed May  3 19:22:27 2023, max compression
```

## Comparing `squape-0.1.0.tar` & `squape-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 17:37:53.922061 squape-0.1.0/
--rw-rw-rw-   0        0        0      183 2023-03-26 19:20:26.000000 squape-0.1.0/.flake8
--rw-rw-rw-   0        0        0      227 2023-03-26 19:19:42.000000 squape-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1154 2023-04-17 13:36:44.000000 squape-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1541 2023-03-26 19:19:01.000000 squape-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1914 2023-04-17 17:37:53.921051 squape-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1377 2023-04-17 17:33:10.000000 squape-0.1.0/README.md
--rw-rw-rw-   0        0        0      757 2023-04-17 17:33:50.000000 squape-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       10 2023-03-26 19:20:26.000000 squape-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 17:37:53.922061 squape-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 17:37:53.916593 squape-0.1.0/squape/
--rw-rw-rw-   0        0        0      220 2023-04-17 17:33:50.000000 squape-0.1.0/squape/__init__.py
--rw-rw-rw-   0        0        0     7401 2023-04-17 17:33:50.000000 squape-0.1.0/squape/report.py
--rw-rw-rw-   0        0        0     1136 2023-04-17 17:33:50.000000 squape-0.1.0/squape/vps.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:37:53.919964 squape-0.1.0/squape.egg-info/
--rw-rw-rw-   0        0        0     1914 2023-04-17 17:37:53.000000 squape-0.1.0/squape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-17 17:37:53.000000 squape-0.1.0/squape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 17:37:53.000000 squape-0.1.0/squape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 17:37:53.000000 squape-0.1.0/squape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 19:22:27.488401 squape-0.2.0/
+-rw-rw-rw-   0        0        0      183 2023-03-26 19:20:26.000000 squape-0.2.0/.flake8
+-rw-rw-rw-   0        0        0      227 2023-03-26 19:19:42.000000 squape-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1214 2023-05-02 09:48:54.000000 squape-0.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      877 2023-05-03 19:16:58.000000 squape-0.2.0/HISTORY.md
+-rw-rw-rw-   0        0        0     1541 2023-03-26 19:19:01.000000 squape-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2185 2023-05-03 19:22:27.488401 squape-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-05-03 08:14:02.000000 squape-0.2.0/README.md
+-rw-rw-rw-   0        0        0      847 2023-05-03 08:14:02.000000 squape-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       10 2023-03-26 19:20:26.000000 squape-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 19:22:27.493415 squape-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 19:22:27.440265 squape-0.2.0/squape/
+-rw-rw-rw-   0        0        0      220 2023-04-17 17:33:50.000000 squape-0.2.0/squape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:22:27.481313 squape-0.2.0/squape/internal/
+-rw-rw-rw-   0        0        0      220 2023-05-02 09:42:03.000000 squape-0.2.0/squape/internal/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-02 09:42:03.000000 squape-0.2.0/squape/internal/exceptions.py
+-rw-rw-rw-   0        0        0     8426 2023-05-03 15:55:59.000000 squape-0.2.0/squape/report.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:22:27.487379 squape-0.2.0/squape/resources/
+-rw-rw-rw-   0        0        0    10904 2023-05-02 09:48:54.000000 squape-0.2.0/squape/resources/empty_video_with_message.mp4
+-rw-rw-rw-   0        0        0    10797 2023-05-02 09:48:54.000000 squape-0.2.0/squape/settings.py
+-rw-rw-rw-   0        0        0     3882 2023-05-02 09:48:54.000000 squape-0.2.0/squape/video.py
+-rw-rw-rw-   0        0        0     1179 2023-05-02 09:48:54.000000 squape-0.2.0/squape/vps.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:22:27.463564 squape-0.2.0/squape.egg-info/
+-rw-rw-rw-   0        0        0     2185 2023-05-03 19:22:26.000000 squape-0.2.0/squape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-03 19:22:27.000000 squape-0.2.0/squape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 19:22:26.000000 squape-0.2.0/squape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 19:22:26.000000 squape-0.2.0/squape.egg-info/top_level.txt
```

### Comparing `squape-0.1.0/.pre-commit-config.yaml` & `squape-0.2.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   - repo: https://github.com/asottile/reorder_python_imports
     rev: v3.9.0
     hooks:
       - id: reorder-python-imports
         args: [
           --unclassifiable-application-module, squish, 
           --unclassifiable-application-module, test,
+          --unclassifiable-application-module, squishinfo,
         ]
  
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
         language_version: python3.8
```

### Comparing `squape-0.1.0/LICENSE` & `squape-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squape-0.1.0/PKG-INFO` & `squape-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: squape
-Version: 0.1.0
-Summary: Reporting Utilities for the Squish GUI Tester
-Author-email: Cyber Alpaca <contact@cyberalpaca.com>
-Project-URL: Homepage, https://github.com/CyberAlpaca/squish-api-python-extension
-Project-URL: Cyber Alpaca, https://cyberalpaca.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Squish - version](https://img.shields.io/badge/Squish-v6.7.0+-brightgreen)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/squape)
-![PyPI - License](https://img.shields.io/pypi/l/squape)
+![PyPI - License](https://img.shields.io/pypi/l/SQUAPE)
 # SQUAPE - Squish API Python Extension
 Python package that extends Squish Python API. It provides tools for everyday automated test cases development.
 
 ### Requirements
 To enjoy all the features of the SQUAPE package, you have to use it with Squish version 6.7.0 or newer. 
 
 ### Installation
@@ -26,15 +12,18 @@
 You can install it via `pip` with the following commands:
 ```sh
 pip install squape
 ```
 
 ### Content
 The package consists of several modules:
-- report - adds features to enhance the reporting and verification capabilities of Squish.
+- report - adds features to enhance the reporting capabilities of Squish
+- settings - makes using various test settings easier and cleaner
+- video - adds features to enhance video capture capabilities of Squish
+- vps - extension of Squish verification points
 
 ## Contribution
 The package is created and maintained by [Cyber Alpaca](https://cyberalpaca.com/)  
 Pull requests for any issues are welcome.  
 In case where you would like to introduce a new feature or a major change, please open an issue first and discuss it with our team.
 
 ## License
```

### Comparing `squape-0.1.0/pyproject.toml` & `squape-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["squape"]
 namespaces = false
 
 [project]
 name = "squape"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Cyber Alpaca", email="contact@cyberalpaca.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-description = "Reporting Utilities for the Squish GUI Tester"
+description = "Python utilities for the Squish GUI Tester"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/CyberAlpaca/squish-api-python-extension"
 "Cyber Alpaca" = "https://cyberalpaca.com"
```

### Comparing `squape-0.1.0/squape/report.py` & `squape-0.2.0/squape/report.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,16 +13,56 @@
 class LogLevel:
     DEBUG = 10
     LOG = 20
     WARNING = 30
     FAIL = 40
     FATAL = 50
 
+    _nameToLevel = {
+        "FATAL": FATAL,
+        "FAIL": FAIL,
+        "WARN": WARNING,
+        "WARNING": WARNING,
+        "LOG": LOG,
+        "DEBUG": DEBUG,
+    }
 
-LOGLEVEL = LogLevel.LOG
+
+def set_level(level) -> None:
+    """Sets the Squish logging level, Level must be an int or a str.
+
+    Args:
+        level (int|str): log level to set
+
+    Examples:
+       set_level(report.LogLevel.WARNING)
+       set_level("FAIL")
+    """
+    global LOGLEVEL
+    LOGLEVEL = __translate_Level(level)
+
+
+LOGLEVEL = set_level(LogLevel.LOG)
+
+
+def __translate_Level(level) -> int:
+    """Translates the given log level to valid LogLevel
+
+    Args:
+        level (int|str): log level to translate
+    """
+    if isinstance(level, int):
+        rv = level
+    elif isinstance(level, str):
+        if level not in LogLevel._nameToLevel:
+            raise ValueError(f"Unknown LogLevel: {level}")
+        rv = LogLevel._nameToLevel[level]
+    else:
+        raise TypeError(f"LogLevel is not an integer or a valid string: {level}")
+    return rv
 
 
 def __is_level_enabled(level: LogLevel) -> bool:
     """Checks the given log level against the currently set LOGLEVEL
 
     Args:
         level (LogLevel): log level to check
```

### Comparing `squape-0.1.0/squape/vps.py` & `squape-0.2.0/squape/vps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (c) 2023, Cyber Alpaca
 # All rights reserved.
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
+import operator
+import time
+
 import squish
 import test
 
 
 def vph_property(
     object_name: any, property_name: str, expected_value: any, msg: str
 ) -> bool:
@@ -21,12 +24,12 @@
         expected_value (any): expected value of the verified property
         msg (str): verification message
     Returns:
         bool: True if verification is positive, False otherwise
     """
 
     obj = squish.waitForObjectExists(object_name)
-    property_value = getattr(obj, property_name)
+    property_value = operator.attrgetter(property_name)(obj)
     squish.highlightObject(obj, 200, False)
     result = test.compare(property_value, expected_value, msg)
-    squish.snooze(0.2)
+    time.sleep(0.200)
     return result
```

### Comparing `squape-0.1.0/squape.egg-info/PKG-INFO` & `squape-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: squape
-Version: 0.1.0
-Summary: Reporting Utilities for the Squish GUI Tester
+Version: 0.2.0
+Summary: Python utilities for the Squish GUI Tester
 Author-email: Cyber Alpaca <contact@cyberalpaca.com>
 Project-URL: Homepage, https://github.com/CyberAlpaca/squish-api-python-extension
 Project-URL: Cyber Alpaca, https://cyberalpaca.com
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Squish - version](https://img.shields.io/badge/Squish-v6.7.0+-brightgreen)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/squape)
-![PyPI - License](https://img.shields.io/pypi/l/squape)
+![PyPI - License](https://img.shields.io/pypi/l/SQUAPE)
 # SQUAPE - Squish API Python Extension
 Python package that extends Squish Python API. It provides tools for everyday automated test cases development.
 
 ### Requirements
 To enjoy all the features of the SQUAPE package, you have to use it with Squish version 6.7.0 or newer. 
 
 ### Installation
@@ -26,15 +28,18 @@
 You can install it via `pip` with the following commands:
 ```sh
 pip install squape
 ```
 
 ### Content
 The package consists of several modules:
-- report - adds features to enhance the reporting and verification capabilities of Squish.
+- report - adds features to enhance the reporting capabilities of Squish
+- settings - makes using various test settings easier and cleaner
+- video - adds features to enhance video capture capabilities of Squish
+- vps - extension of Squish verification points
 
 ## Contribution
 The package is created and maintained by [Cyber Alpaca](https://cyberalpaca.com/)  
 Pull requests for any issues are welcome.  
 In case where you would like to introduce a new feature or a major change, please open an issue first and discuss it with our team.
 
 ## License
```

