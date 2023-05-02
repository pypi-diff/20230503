# Comparing `tmp/aij-news-client-1.0.4.tar.gz` & `tmp/aij-news-client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-client-1.0.4.tar", last modified: Tue May  2 23:37:10 2023, max compression
+gzip compressed data, was "aij-news-client-1.0.5.tar", last modified: Tue May  2 23:44:09 2023, max compression
```

## Comparing `aij-news-client-1.0.4.tar` & `aij-news-client-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4302 2023-05-02 23:37:12.000000 aij-news-client-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.4/README.md
--rw-rw-rw-   0        0        0     6292 2023-05-02 23:36:58.000000 aij-news-client-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 23:37:12.000000 aij-news-client-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/
--rw-rw-rw-   0        0        0     4302 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/aij_news_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 23:37:10.000000 aij-news-client-1.0.4/src/news_client/
--rw-rw-rw-   0        0        0     6360 2023-05-02 23:36:46.000000 aij-news-client-1.0.4/src/news_client/__init__.py
--rw-rw-rw-   0        0        0      832 2023-05-02 22:32:04.000000 aij-news-client-1.0.4/src/news_client/news_consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.5/README.md
+-rw-rw-rw-   0        0        0     6292 2023-05-02 23:43:58.000000 aij-news-client-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/
+-rw-rw-rw-   0        0        0     4302 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/aij_news_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 23:44:10.000000 aij-news-client-1.0.5/src/news_client/
+-rw-rw-rw-   0        0        0     6362 2023-05-02 23:42:04.000000 aij-news-client-1.0.5/src/news_client/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-05-02 22:32:04.000000 aij-news-client-1.0.5/src/news_client/news_consumer.py
```

### Comparing `aij-news-client-1.0.4/LICENSE.txt` & `aij-news-client-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.4/PKG-INFO` & `aij-news-client-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.4/README.md` & `aij-news-client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.4/pyproject.toml` & `aij-news-client-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-client"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.4"
+version = "1.0.5"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Client package"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-news-client-1.0.4/src/aij_news_client.egg-info/PKG-INFO` & `aij-news-client-1.0.5/src/aij_news_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.4/src/news_client/__init__.py` & `aij-news-client-1.0.5/src/news_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import threading
 import cv2
 import mediapipe as mp
 import screeninfo
 import time
 
-from news_client import NewsConsumer
+from news_consumer import NewsConsumer
 
 articles = []
 headings = None
 
 def callback(self, ch, method, properties, body):
     """
     This method prints the articles.
```

### Comparing `aij-news-client-1.0.4/src/news_client/news_consumer.py` & `aij-news-client-1.0.5/src/news_client/news_consumer.py`

 * *Files identical despite different names*

