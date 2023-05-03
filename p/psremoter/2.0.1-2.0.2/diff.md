# Comparing `tmp/psremoter-2.0.1.tar.gz` & `tmp/psremoter-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psremoter-2.0.1.tar", last modified: Wed May  3 13:49:15 2023, max compression
+gzip compressed data, was "psremoter-2.0.2.tar", last modified: Wed May  3 13:52:13 2023, max compression
```

## Comparing `psremoter-2.0.1.tar` & `psremoter-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:49:15.909006 psremoter-2.0.1/
--rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1364 2023-05-03 13:49:15.908041 psremoter-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 13:49:15.909006 psremoter-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-05-03 13:49:10.000000 psremoter-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:49:15.881022 psremoter-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 13:49:15.886020 psremoter-2.0.1/src/psremoter/
--rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-2.0.1/src/psremoter/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-2.0.1/src/psremoter/connector.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:49:15.907041 psremoter-2.0.1/src/psremoter.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-05-03 13:49:15.000000 psremoter-2.0.1/src/psremoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-03 13:49:15.000000 psremoter-2.0.1/src/psremoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:49:15.000000 psremoter-2.0.1/src/psremoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 13:49:15.000000 psremoter-2.0.1/src/psremoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.226792 psremoter-2.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-2.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1364 2023-05-03 13:52:13.225793 psremoter-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:52:13.226792 psremoter-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-05-03 13:52:04.000000 psremoter-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.198809 psremoter-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.204805 psremoter-2.0.2/src/psremoter/
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-2.0.2/src/psremoter/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-2.0.2/src/psremoter/connector.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.223794 psremoter-2.0.2/src/psremoter.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/top_level.txt
```

### Comparing `psremoter-2.0.1/LICENSE.txt` & `psremoter-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psremoter-2.0.1/PKG-INFO` & `psremoter-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 2.0.1
+Version: 2.0.2
 Summary: Powershell remote client tool for Python
 Home-page: https://github.com/danielMandelblat/psremoter
 Author: Daniel Mandelblat
 Author-email: danielmande@gmail.com
 Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psremoter-2.0.1/setup.py` & `psremoter-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "psremoter",
-    version = "2.0.1",
+    version = "2.0.2",
     author = "Daniel Mandelblat",
     author_email = "danielmande@gmail.com",
     description = "Powershell remote client tool for Python",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/danielMandelblat/psremoter",
     project_urls = {
```

### Comparing `psremoter-2.0.1/src/psremoter/connector.py` & `psremoter-2.0.2/src/psremoter/connector.py`

 * *Files identical despite different names*

### Comparing `psremoter-2.0.1/src/psremoter.egg-info/PKG-INFO` & `psremoter-2.0.2/src/psremoter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 2.0.1
+Version: 2.0.2
 Summary: Powershell remote client tool for Python
 Home-page: https://github.com/danielMandelblat/psremoter
 Author: Daniel Mandelblat
 Author-email: danielmande@gmail.com
 Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

