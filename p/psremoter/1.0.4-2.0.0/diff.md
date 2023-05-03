# Comparing `tmp/psremoter-1.0.4.tar.gz` & `tmp/psremoter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psremoter-1.0.4.tar", last modified: Mon May  1 11:18:06 2023, max compression
+gzip compressed data, was "psremoter-2.0.0.tar", last modified: Wed May  3 13:45:03 2023, max compression
```

## Comparing `psremoter-1.0.4.tar` & `psremoter-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 11:18:06.174005 psremoter-1.0.4/
--rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1363 2023-05-01 11:18:06.172006 psremoter-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-05-01 11:14:35.000000 psremoter-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 11:18:06.174005 psremoter-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-05-01 11:17:41.000000 psremoter-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:18:06.129031 psremoter-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 11:18:06.137027 psremoter-1.0.4/src/psremoter/
--rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-1.0.4/src/psremoter/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-1.0.4/src/psremoter/connector.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:18:06.167013 psremoter-1.0.4/src/psremoter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-05-01 11:18:06.000000 psremoter-1.0.4/src/psremoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-01 11:18:06.000000 psremoter-1.0.4/src/psremoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 11:18:06.000000 psremoter-1.0.4/src/psremoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 11:18:06.000000 psremoter-1.0.4/src/psremoter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 11:18:06.170009 psremoter-1.0.4/tests/
--rw-rw-rw-   0        0        0      545 2023-05-01 10:47:51.000000 psremoter-1.0.4/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:45:03.333264 psremoter-2.0.0/
+-rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1364 2023-05-03 13:45:03.332264 psremoter-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:45:03.333264 psremoter-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-05-03 13:43:10.000000 psremoter-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:45:03.318274 psremoter-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:45:03.323267 psremoter-2.0.0/src/psremoter/
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-2.0.0/src/psremoter/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-2.0.0/src/psremoter/connector.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:45:03.331263 psremoter-2.0.0/src/psremoter.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-05-03 13:45:03.000000 psremoter-2.0.0/src/psremoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-03 13:45:03.000000 psremoter-2.0.0/src/psremoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:45:03.000000 psremoter-2.0.0/src/psremoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 13:45:03.000000 psremoter-2.0.0/src/psremoter.egg-info/top_level.txt
```

### Comparing `psremoter-1.0.4/LICENSE.txt` & `psremoter-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psremoter-1.0.4/PKG-INFO` & `psremoter-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.4
+Version: 2.0.0
 Summary: Powershell remote client tool for Python
 Home-page: https://github.com/danielMandelblat/psremoter
 Author: Daniel Mandelblat
-Author-email: danielmande@gmail.cm
+Author-email: danielmande@gmail.com
 Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `psremoter-1.0.4/setup.py` & `psremoter-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "psremoter",
-    version = "1.0.4",
+    version = "2.0.0",
     author = "Daniel Mandelblat",
-    author_email = "danielmande@gmail.cm",
+    author_email = "danielmande@gmail.com",
     description = "Powershell remote client tool for Python",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/danielMandelblat/psremoter",
     project_urls = {
         "Bug Tracker": "https://github.com/danielMandelblat/psremoter",
     },
```

### Comparing `psremoter-1.0.4/src/psremoter/connector.py` & `psremoter-2.0.0/src/psremoter/connector.py`

 * *Files identical despite different names*

### Comparing `psremoter-1.0.4/src/psremoter.egg-info/PKG-INFO` & `psremoter-2.0.0/src/psremoter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.4
+Version: 2.0.0
 Summary: Powershell remote client tool for Python
 Home-page: https://github.com/danielMandelblat/psremoter
 Author: Daniel Mandelblat
-Author-email: danielmande@gmail.cm
+Author-email: danielmande@gmail.com
 Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

