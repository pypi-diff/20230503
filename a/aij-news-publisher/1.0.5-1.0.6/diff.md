# Comparing `tmp/aij-news-publisher-1.0.5.tar.gz` & `tmp/aij-news-publisher-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-publisher-1.0.5.tar", last modified: Tue May  2 23:45:26 2023, max compression
+gzip compressed data, was "aij-news-publisher-1.0.6.tar", last modified: Tue May  2 23:49:02 2023, max compression
```

## Comparing `aij-news-publisher-1.0.5.tar` & `aij-news-publisher-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4314 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.5/README.md
--rw-rw-rw-   0        0        0     6331 2023-05-02 23:45:16.000000 aij-news-publisher-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/
--rw-rw-rw-   0        0        0     4314 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      147 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 23:45:28.000000 aij-news-publisher-1.0.5/src/news_publisher/
--rw-rw-rw-   0        0        0      583 2023-05-02 21:50:00.000000 aij-news-publisher-1.0.5/src/news_publisher/__init__.py
--rw-rw-rw-   0        0        0     3431 2023-05-02 22:53:06.000000 aij-news-publisher-1.0.5/src/news_publisher/api_server.py
--rw-rw-rw-   0        0        0     2942 2023-05-02 21:47:28.000000 aij-news-publisher-1.0.5/src/news_publisher/db_server.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     4314 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-publisher-1.0.6/README.md
+-rw-rw-rw-   0        0        0     6333 2023-05-02 23:48:52.000000 aij-news-publisher-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/
+-rw-rw-rw-   0        0        0     4314 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 23:49:04.000000 aij-news-publisher-1.0.6/src/news_publisher/
+-rw-rw-rw-   0        0        0      583 2023-05-02 21:50:00.000000 aij-news-publisher-1.0.6/src/news_publisher/__init__.py
+-rw-rw-rw-   0        0        0     3431 2023-05-02 22:53:06.000000 aij-news-publisher-1.0.6/src/news_publisher/api_server.py
+-rw-rw-rw-   0        0        0     2942 2023-05-02 21:47:28.000000 aij-news-publisher-1.0.6/src/news_publisher/db_server.py
```

### Comparing `aij-news-publisher-1.0.5/LICENSE.txt` & `aij-news-publisher-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.5/PKG-INFO` & `aij-news-publisher-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.5
+Version: 1.0.6
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.5/README.md` & `aij-news-publisher-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.5/pyproject.toml` & `aij-news-publisher-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-publisher"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.5"
+version = "1.0.6"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Publisher package"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -141,15 +141,15 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij-news-publisher"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-aijnp = "news_publisher:main"
+# aijnp = "news_publisher:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-news-publisher-1.0.5/src/aij_news_publisher.egg-info/PKG-INFO` & `aij-news-publisher-1.0.6/src/aij_news_publisher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-publisher
-Version: 1.0.5
+Version: 1.0.6
 Summary: AI Journalist News Publisher package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-publisher-1.0.5/src/news_publisher/__init__.py` & `aij-news-publisher-1.0.6/src/news_publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.5/src/news_publisher/api_server.py` & `aij-news-publisher-1.0.6/src/news_publisher/api_server.py`

 * *Files identical despite different names*

### Comparing `aij-news-publisher-1.0.5/src/news_publisher/db_server.py` & `aij-news-publisher-1.0.6/src/news_publisher/db_server.py`

 * *Files identical despite different names*

