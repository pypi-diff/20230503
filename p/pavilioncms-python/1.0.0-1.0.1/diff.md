# Comparing `tmp/pavilioncms-python-1.0.0.tar.gz` & `tmp/pavilioncms-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pavilioncms-python-1.0.0.tar", last modified: Thu Mar 16 11:15:58 2023, max compression
+gzip compressed data, was "pavilioncms-python-1.0.1.tar", last modified: Wed May  3 11:45:14 2023, max compression
```

## Comparing `pavilioncms-python-1.0.0.tar` & `pavilioncms-python-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      183 2023-02-19 18:16:48.000000 pavilioncms-python-1.0.0/HISTORY.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      262 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/MANIFEST.in
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     2973 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/PKG-INFO
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      909 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/README.rst
-drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-03-16 11:15:58.628790 pavilioncms-python-1.0.0/docs/
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      613 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/Makefile
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       28 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/authors.rst
--rwxrwxr-x   0 moluwole  (1000) moluwole  (1000)     4858 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/conf.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       33 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/contributing.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       28 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/history.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      309 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/index.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1154 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/installation.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      810 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/make.bat
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       27 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/readme.rst
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       79 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/docs/usage.rst
-drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/pavilion_cms/
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      484 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/__init__.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       22 2023-03-16 11:00:11.000000 pavilioncms-python-1.0.0/pavilion_cms/__version__.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      616 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/author.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      625 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/category.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1350 2023-03-16 06:22:08.000000 pavilioncms-python-1.0.0/pavilion_cms/client.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      840 2022-12-12 01:13:40.000000 pavilioncms-python-1.0.0/pavilion_cms/exceptions.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      662 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/posts.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      601 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/tag.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      525 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.0/pavilion_cms/utils.py
-drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     2973 2023-03-16 11:15:58.000000 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/PKG-INFO
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      717 2023-03-16 11:15:58.000000 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/SOURCES.txt
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)        1 2023-03-16 11:15:58.000000 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/dependency_links.txt
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       17 2023-03-16 11:15:58.000000 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/requires.txt
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       13 2023-03-16 11:15:58.000000 pavilioncms-python-1.0.0/pavilioncms_python.egg-info/top_level.txt
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      451 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/setup.cfg
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1709 2023-02-19 18:20:01.000000 pavilioncms-python-1.0.0/setup.py
-drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-03-16 11:15:58.632790 pavilioncms-python-1.0.0/tests/
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       42 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.0/tests/__init__.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)        0 2022-12-12 00:03:20.000000 pavilioncms-python-1.0.0/tests/conftest.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     3685 2022-12-12 01:17:20.000000 pavilioncms-python-1.0.0/tests/fixtures.py
--rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1695 2023-02-19 18:07:34.000000 pavilioncms-python-1.0.0/tests/test_client.py
+drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      183 2023-02-19 18:16:48.000000 pavilioncms-python-1.0.1/HISTORY.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      262 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/MANIFEST.in
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     2998 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/PKG-INFO
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      909 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/README.rst
+drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/docs/
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      613 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/Makefile
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       28 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/authors.rst
+-rwxrwxr-x   0 moluwole  (1000) moluwole  (1000)     4858 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/conf.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       33 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/contributing.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       28 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/history.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      309 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/index.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1154 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/installation.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      810 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/make.bat
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       27 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/readme.rst
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       79 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/docs/usage.rst
+drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/pavilion_cms/
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      484 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/__init__.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       22 2023-05-03 11:42:54.000000 pavilioncms-python-1.0.1/pavilion_cms/__version__.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      616 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/author.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      625 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/category.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1350 2023-05-03 11:43:07.000000 pavilioncms-python-1.0.1/pavilion_cms/client.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      840 2022-12-12 01:13:40.000000 pavilioncms-python-1.0.1/pavilion_cms/exceptions.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      662 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/posts.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      601 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/tag.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      525 2023-02-19 18:07:19.000000 pavilioncms-python-1.0.1/pavilion_cms/utils.py
+drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     2998 2023-05-03 11:45:14.000000 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/PKG-INFO
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      717 2023-05-03 11:45:14.000000 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)        1 2023-05-03 11:45:14.000000 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       17 2023-05-03 11:45:14.000000 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/requires.txt
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       13 2023-05-03 11:45:14.000000 pavilioncms-python-1.0.1/pavilioncms_python.egg-info/top_level.txt
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)      451 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/setup.cfg
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1709 2023-02-19 18:20:01.000000 pavilioncms-python-1.0.1/setup.py
+drwxrwxr-x   0 moluwole  (1000) moluwole  (1000)        0 2023-05-03 11:45:14.471146 pavilioncms-python-1.0.1/tests/
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)       42 2022-12-08 00:09:58.000000 pavilioncms-python-1.0.1/tests/__init__.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)        0 2022-12-12 00:03:20.000000 pavilioncms-python-1.0.1/tests/conftest.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     3685 2022-12-12 01:17:20.000000 pavilioncms-python-1.0.1/tests/fixtures.py
+-rw-rw-r--   0 moluwole  (1000) moluwole  (1000)     1695 2023-02-19 18:07:34.000000 pavilioncms-python-1.0.1/tests/test_client.py
```

### Comparing `pavilioncms-python-1.0.0/PKG-INFO` & `pavilioncms-python-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pavilioncms-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Package to make use of PavilionCMS
 Home-page: UNKNOWN
 Author: Oluwole Majiyagbe
 Author-email: info@firstpavitech.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -48,14 +48,18 @@
 client = PavilionCMS(read_token="your-read-token")
 ```
 
 #### Functions
 
 _*`tags`*_ => Get all your tags
 
+_*`category`*_ => Get all your categories
+
+_*`posts`*_ => Get all your published blog posts
+
 The client's tags function has the `all`, `get`, `next` and `previous` methods for making requests. 
 
 The `all` and `get` functions also accept an optional `params` argument to add additional data to the response. 
 
 The `next` and `previous` functions accept only a url which is gotten from the response of the `all` method. 
 
 > Reponses that request for a list are paginated. 
@@ -78,22 +82,23 @@
 
 print(tags[0])
  #{
  #   'id': '0b4cff81-c655-452a-881f-3a8eeab7ed09', 
  #   'name': 'top table', 
  #   'detail_url': '/api/v1/tag/0b4cff81-c655-452a-881f-3a8eeab7ed09/view/'
  # }
- ```
 
- _*`categories`*_ => Get all your categories
+ # To get the categories
 
- Same function call as tags. Has the `all`, `get`, `next` and `previous` calls. 
+ categories = client.category.all()
 
- Tags and Categories both share the same data structure
+ # To get the blog posts
 
+ posts = client.posts.all()
+ ```
 
 
  
 
  ..__history:
 
 # Release History
```

### Comparing `pavilioncms-python-1.0.0/README.rst` & `pavilioncms-python-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/docs/Makefile` & `pavilioncms-python-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/docs/conf.py` & `pavilioncms-python-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/docs/installation.rst` & `pavilioncms-python-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/docs/make.bat` & `pavilioncms-python-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/author.py` & `pavilioncms-python-1.0.1/pavilion_cms/author.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/category.py` & `pavilioncms-python-1.0.1/pavilion_cms/category.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/client.py` & `pavilioncms-python-1.0.1/pavilion_cms/client.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/exceptions.py` & `pavilioncms-python-1.0.1/pavilion_cms/exceptions.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/posts.py` & `pavilioncms-python-1.0.1/pavilion_cms/posts.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/tag.py` & `pavilioncms-python-1.0.1/pavilion_cms/tag.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilion_cms/utils.py` & `pavilioncms-python-1.0.1/pavilion_cms/utils.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/pavilioncms_python.egg-info/PKG-INFO` & `pavilioncms-python-1.0.1/pavilioncms_python.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pavilioncms-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Package to make use of PavilionCMS
 Home-page: UNKNOWN
 Author: Oluwole Majiyagbe
 Author-email: info@firstpavitech.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -48,14 +48,18 @@
 client = PavilionCMS(read_token="your-read-token")
 ```
 
 #### Functions
 
 _*`tags`*_ => Get all your tags
 
+_*`category`*_ => Get all your categories
+
+_*`posts`*_ => Get all your published blog posts
+
 The client's tags function has the `all`, `get`, `next` and `previous` methods for making requests. 
 
 The `all` and `get` functions also accept an optional `params` argument to add additional data to the response. 
 
 The `next` and `previous` functions accept only a url which is gotten from the response of the `all` method. 
 
 > Reponses that request for a list are paginated. 
@@ -78,22 +82,23 @@
 
 print(tags[0])
  #{
  #   'id': '0b4cff81-c655-452a-881f-3a8eeab7ed09', 
  #   'name': 'top table', 
  #   'detail_url': '/api/v1/tag/0b4cff81-c655-452a-881f-3a8eeab7ed09/view/'
  # }
- ```
 
- _*`categories`*_ => Get all your categories
+ # To get the categories
 
- Same function call as tags. Has the `all`, `get`, `next` and `previous` calls. 
+ categories = client.category.all()
 
- Tags and Categories both share the same data structure
+ # To get the blog posts
 
+ posts = client.posts.all()
+ ```
 
 
  
 
  ..__history:
 
 # Release History
```

### Comparing `pavilioncms-python-1.0.0/pavilioncms_python.egg-info/SOURCES.txt` & `pavilioncms-python-1.0.1/pavilioncms_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/setup.py` & `pavilioncms-python-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/tests/fixtures.py` & `pavilioncms-python-1.0.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `pavilioncms-python-1.0.0/tests/test_client.py` & `pavilioncms-python-1.0.1/tests/test_client.py`

 * *Files identical despite different names*

