# Comparing `tmp/aij-news-publisher-1.0.3.tar.gz` & `tmp/aij-news-publisher-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-publisher-1.0.3.tar", last modified: Tue May  2 21:50:28 2023, max compression
+gzip compressed data, was "aij-news-publisher-1.0.4.tar", last modified: Tue May  2 22:57:07 2023, max compression
```

## Comparing `aij-news-publisher-1.0.3.tar` & `aij-news-publisher-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4314 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.3/README.md
--rw-rw-rw-   0        0        0     6331 2023-05-02 21:50:16.000000 aij-news-publisher-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/
--rw-rw-rw-   0        0        0     4314 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      147 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 21:50:30.000000 aij-news-publisher-1.0.3/src/news_publisher/
--rw-rw-rw-   0        0        0      583 2023-05-02 21:50:00.000000 aij-news-publisher-1.0.3/src/news_publisher/__init__.py
--rw-rw-rw-   0        0        0     3255 2023-05-02 21:48:22.000000 aij-news-publisher-1.0.3/src/news_publisher/api_server.py
--rw-rw-rw-   0        0        0     2942 2023-05-02 21:47:28.000000 aij-news-publisher-1.0.3/src/news_publisher/db_server.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4314 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.4/README.md
+-rw-rw-rw-   0        0        0     6331 2023-05-02 22:56:50.000000 aij-news-publisher-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/
+-rw-rw-rw-   0        0        0     4314 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      147 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 22:57:08.000000 aij-news-publisher-1.0.4/src/news_publisher/
+-rw-rw-rw-   0        0        0      583 2023-05-02 21:50:00.000000 aij-news-publisher-1.0.4/src/news_publisher/__init__.py
+-rw-rw-rw-   0        0        0     3431 2023-05-02 22:53:06.000000 aij-news-publisher-1.0.4/src/news_publisher/api_server.py
+-rw-rw-rw-   0        0        0     2942 2023-05-02 21:47:28.000000 aij-news-publisher-1.0.4/src/news_publisher/db_server.py
```

### Comparing `aij-news-publisher-1.0.3/LICENSE.txt` & `aij-news-publisher-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.3/PKG-INFO` & `aij-news-publisher-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.3
+Version: 1.0.4
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.3/README.md` & `aij-news-publisher-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.3/pyproject.toml` & `aij-news-publisher-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-publisher"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.3"
+version = "1.0.4"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Publisher package"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-news-publisher-1.0.3/src/aij_news_publisher.egg-info/PKG-INFO` & `aij-news-publisher-1.0.4/src/aij_news_publisher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.3
+Version: 1.0.4
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.3/src/news_publisher/__init__.py` & `aij-news-publisher-1.0.4/src/news_publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.3/src/news_publisher/api_server.py` & `aij-news-publisher-1.0.4/src/news_publisher/api_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,10 +59,16 @@
             print("Loading the news from the database...")
             
 
         # do not close the connection until the message is delivered
         if self.connection.is_open:
             self.connection.close()
 
-        # call the function again after 60 seconds
-        Timer(60, self.publish_news_data).start()
+        # call the function again after 100 seconds because there are max. 100 results per page
+        Timer(100, self.publish).start()
 
+
+    def destroy(self):
+        """
+        Destroy the connection to the RabbitMQ server
+        """
+        self.connection.close()
```

### Comparing `aij-news-publisher-1.0.3/src/news_publisher/db_server.py` & `aij-news-publisher-1.0.4/src/news_publisher/db_server.py`

 * *Files identical despite different names*

