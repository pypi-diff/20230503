# Comparing `tmp/pyubibot-0.0.3.tar.gz` & `tmp/pyubibot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyubibot-0.0.3.tar", last modified: Tue Jun 28 21:24:21 2022, max compression
+gzip compressed data, was "pyubibot-0.0.4.tar", last modified: Wed May  3 18:40:13 2023, max compression
```

## Comparing `pyubibot-0.0.3.tar` & `pyubibot-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2022-06-28 21:24:21.503844 pyubibot-0.0.3/
--rw-rw-r--   0 danny     (1000) danny     (1000)    11357 2022-06-18 11:51:50.000000 pyubibot-0.0.3/LICENSE
--rw-rw-r--   0 danny     (1000) danny     (1000)      825 2022-06-28 21:24:21.503844 pyubibot-0.0.3/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)      382 2022-06-18 20:06:04.000000 pyubibot-0.0.3/README.md
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2022-06-28 21:24:21.503844 pyubibot-0.0.3/pyubibot.egg-info/
--rw-rw-r--   0 danny     (1000) danny     (1000)      825 2022-06-28 21:24:21.000000 pyubibot-0.0.3/pyubibot.egg-info/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)      196 2022-06-28 21:24:21.000000 pyubibot-0.0.3/pyubibot.egg-info/SOURCES.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2022-06-28 21:24:21.000000 pyubibot-0.0.3/pyubibot.egg-info/dependency_links.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2022-06-28 21:24:21.000000 pyubibot-0.0.3/pyubibot.egg-info/top_level.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       38 2022-06-28 21:24:21.503844 pyubibot-0.0.3/setup.cfg
--rw-rw-r--   0 danny     (1000) danny     (1000)      690 2022-06-28 21:23:47.000000 pyubibot-0.0.3/setup.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2022-06-28 21:24:21.503844 pyubibot-0.0.3/test/
--rw-rw-r--   0 danny     (1000) danny     (1000)     1663 2022-06-19 11:55:46.000000 pyubibot-0.0.3/test/test_channels.py
--rw-rw-r--   0 danny     (1000) danny     (1000)      526 2022-06-28 21:07:24.000000 pyubibot-0.0.3/test/test_ubibot.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-05-03 18:40:13.880647 pyubibot-0.0.4/
+-rw-rw-r--   0 danny     (1000) danny     (1000)    11357 2023-04-30 09:13:11.000000 pyubibot-0.0.4/LICENSE
+-rw-rw-r--   0 danny     (1000) danny     (1000)      825 2023-05-03 18:40:13.880647 pyubibot-0.0.4/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)      382 2023-04-30 09:13:11.000000 pyubibot-0.0.4/README.md
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-05-03 18:40:13.880647 pyubibot-0.0.4/pyubibot/
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2533 2023-04-30 09:13:11.000000 pyubibot-0.0.4/pyubibot/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1943 2023-04-30 09:13:11.000000 pyubibot-0.0.4/pyubibot/channels.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      171 2023-04-30 09:13:11.000000 pyubibot-0.0.4/pyubibot/constants.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-05-03 18:40:13.880647 pyubibot-0.0.4/pyubibot.egg-info/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      825 2023-05-03 18:40:13.000000 pyubibot-0.0.4/pyubibot.egg-info/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)      277 2023-05-03 18:40:13.000000 pyubibot-0.0.4/pyubibot.egg-info/SOURCES.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-05-03 18:40:13.000000 pyubibot-0.0.4/pyubibot.egg-info/dependency_links.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       14 2023-05-03 18:40:13.000000 pyubibot-0.0.4/pyubibot.egg-info/top_level.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       38 2023-05-03 18:40:13.880647 pyubibot-0.0.4/setup.cfg
+-rw-rw-r--   0 danny     (1000) danny     (1000)      675 2023-05-03 18:40:03.000000 pyubibot-0.0.4/setup.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-05-03 18:40:13.880647 pyubibot-0.0.4/test/
+-rw-rw-r--   0 danny     (1000) danny     (1000)       36 2023-04-30 09:13:11.000000 pyubibot-0.0.4/test/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1663 2023-04-30 09:13:11.000000 pyubibot-0.0.4/test/test_channels.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      526 2023-04-30 09:13:11.000000 pyubibot-0.0.4/test/test_ubibot.py
```

### Comparing `pyubibot-0.0.3/LICENSE` & `pyubibot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyubibot-0.0.3/PKG-INFO` & `pyubibot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyubibot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation for Ubibot APIs.
 Home-page: https://github.com/dannytsang/pyubibot
 Author: Danny Tsang
 Author-email: danny@tsang.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyubibot-0.0.3/pyubibot.egg-info/PKG-INFO` & `pyubibot-0.0.4/pyubibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyubibot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation for Ubibot APIs.
 Home-page: https://github.com/dannytsang/pyubibot
 Author: Danny Tsang
 Author-email: danny@tsang.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyubibot-0.0.3/setup.py` & `pyubibot-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyubibot",
-    version="0.0.3",
+    version="0.0.4",
     author="Danny Tsang",
     author_email="danny@tsang.uk",
     description="Python implementation for Ubibot APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dannytsang/pyubibot",
-    packages=setuptools.find_packages(where="pyubibot"),
+    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent"
     ],
     python_requires=">=3.8"
-)
+)
```

### Comparing `pyubibot-0.0.3/test/test_channels.py` & `pyubibot-0.0.4/test/test_channels.py`

 * *Files identical despite different names*

### Comparing `pyubibot-0.0.3/test/test_ubibot.py` & `pyubibot-0.0.4/test/test_ubibot.py`

 * *Files identical despite different names*

