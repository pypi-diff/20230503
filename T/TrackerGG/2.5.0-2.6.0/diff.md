# Comparing `tmp/TrackerGG-2.5.0.tar.gz` & `tmp/TrackerGG-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackerGG-2.5.0.tar", last modified: Tue May  2 07:14:56 2023, max compression
+gzip compressed data, was "TrackerGG-2.6.0.tar", last modified: Wed May  3 07:33:30 2023, max compression
```

## Comparing `TrackerGG-2.5.0.tar` & `TrackerGG-2.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.570174 TrackerGG-2.5.0/
--rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-05-02 07:14:56.568163 TrackerGG-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.512987 TrackerGG-2.5.0/TrackerGG/
-drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.566166 TrackerGG-2.5.0/TrackerGG/Models/
--rw-rw-rw-   0        0        0      821 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/__init__.py
--rw-rw-rw-   0        0        0     3416 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/apex.py
--rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.5.0/TrackerGG/Models/csgo.py
--rw-rw-rw-   0        0        0     1506 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/platform.py
--rw-rw-rw-   0        0        0     1445 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/segment.py
--rw-rw-rw-   0        0        0     2073 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/user.py
--rw-rw-rw-   0        0        0      972 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/__init__.py
--rw-rw-rw-   0        0        0     7666 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/client.py
--rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/TrackerGG/httpclient.py
--rw-rw-rw-   0        0        0     1703 2023-05-01 23:37:40.000000 TrackerGG-2.5.0/TrackerGG/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.531482 TrackerGG-2.5.0/TrackerGG.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 07:14:56.571174 TrackerGG-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-02 07:14:44.000000 TrackerGG-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:30.013049 TrackerGG-2.6.0/
+-rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1425 2023-05-03 07:33:30.011052 TrackerGG-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:29.978896 TrackerGG-2.6.0/TrackerGG/
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:30.010046 TrackerGG-2.6.0/TrackerGG/Models/
+-rw-rw-rw-   0        0        0      821 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/Models/__init__.py
+-rw-rw-rw-   0        0        0     3416 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/Models/apex.py
+-rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.6.0/TrackerGG/Models/csgo.py
+-rw-rw-rw-   0        0        0     1506 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/Models/platform.py
+-rw-rw-rw-   0        0        0     1445 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/Models/segment.py
+-rw-rw-rw-   0        0        0     2073 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/Models/user.py
+-rw-rw-rw-   0        0        0      972 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/__init__.py
+-rw-rw-rw-   0        0        0     7666 2023-05-02 07:13:38.000000 TrackerGG-2.6.0/TrackerGG/client.py
+-rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.6.0/TrackerGG/httpclient.py
+-rw-rw-rw-   0        0        0     1703 2023-05-01 23:37:40.000000 TrackerGG-2.6.0/TrackerGG/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:33:29.996336 TrackerGG-2.6.0/TrackerGG.egg-info/
+-rw-rw-rw-   0        0        0     1425 2023-05-03 07:33:29.000000 TrackerGG-2.6.0/TrackerGG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-05-03 07:33:29.000000 TrackerGG-2.6.0/TrackerGG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:33:29.000000 TrackerGG-2.6.0/TrackerGG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 07:33:29.000000 TrackerGG-2.6.0/TrackerGG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 07:33:29.000000 TrackerGG-2.6.0/TrackerGG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:33:30.013049 TrackerGG-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-03 07:33:21.000000 TrackerGG-2.6.0/setup.py
```

### Comparing `TrackerGG-2.5.0/LICENSE` & `TrackerGG-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/PKG-INFO` & `TrackerGG-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.5.0
+Version: 2.6.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.5.0/README.md` & `TrackerGG-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/__init__.py` & `TrackerGG-2.6.0/TrackerGG/Models/__init__.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/apex.py` & `TrackerGG-2.6.0/TrackerGG/Models/apex.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/csgo.py` & `TrackerGG-2.6.0/TrackerGG/Models/csgo.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/platform.py` & `TrackerGG-2.6.0/TrackerGG/Models/platform.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/segment.py` & `TrackerGG-2.6.0/TrackerGG/Models/segment.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/Models/user.py` & `TrackerGG-2.6.0/TrackerGG/Models/user.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/__init__.py` & `TrackerGG-2.6.0/TrackerGG/__init__.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/client.py` & `TrackerGG-2.6.0/TrackerGG/client.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/httpclient.py` & `TrackerGG-2.6.0/TrackerGG/httpclient.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG/utils.py` & `TrackerGG-2.6.0/TrackerGG/utils.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.5.0/TrackerGG.egg-info/PKG-INFO` & `TrackerGG-2.6.0/TrackerGG.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.5.0
+Version: 2.6.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.5.0/setup.py` & `TrackerGG-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setuptools.setup(
     name="TrackerGG",
-    version="2.5.0",
+    version="2.6.0",
     author="DevRuby",
     author_email="hiveruby@gmail.com",
     description="TrackerGG API Wrapper Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dev-ruby/TrackerGG",
     packages=setuptools.find_packages(),
```

