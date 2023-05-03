# Comparing `tmp/robolson-0.3.8.tar.gz` & `tmp/robolson-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robolson-0.3.8.tar", max compression
+gzip compressed data, was "robolson-0.3.9.tar", max compression
```

## Comparing `robolson-0.3.8.tar` & `robolson-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      800 2022-03-01 07:48:26.175730 robolson-0.3.8/config/clean.toml
--rw-r--r--   0        0        0      560 2022-03-03 22:25:37.859833 robolson-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1370 2022-03-03 22:20:19.066408 robolson-0.3.8/rob/__init__.py
--rw-r--r--   0        0        0     9461 2022-03-03 22:20:57.643345 robolson-0.3.8/rob/clean.py
--rw-r--r--   0        0        0     3371 2022-02-18 20:11:06.384003 robolson-0.3.8/rob/ffmpeg_concat.py
--rw-r--r--   0        0        0    19816 2021-10-05 21:28:44.953483 robolson-0.3.8/rob/hierarchy.py
--rw-r--r--   0        0        0     7590 2022-02-27 00:03:52.749759 robolson-0.3.8/rob/reddit_archive.py
--rw-r--r--   0        0        0     3922 2022-01-01 00:08:23.770615 robolson-0.3.8/rob/robai.py
--rw-r--r--   0        0        0      822 2022-03-03 22:25:40.996226 robolson-0.3.8/setup.py
--rw-r--r--   0        0        0      471 2022-03-03 22:25:40.996226 robolson-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      800 2022-03-01 07:48:26.175730 robolson-0.3.9/config/clean.toml
+-rw-r--r--   0        0        0      517 2022-03-03 22:36:47.590940 robolson-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1370 2022-03-03 22:20:19.066408 robolson-0.3.9/rob/__init__.py
+-rw-r--r--   0        0        0     9461 2022-03-03 22:20:57.643345 robolson-0.3.9/rob/clean.py
+-rw-r--r--   0        0        0     3371 2022-02-18 20:11:06.384003 robolson-0.3.9/rob/ffmpeg_concat.py
+-rw-r--r--   0        0        0    19816 2021-10-05 21:28:44.953483 robolson-0.3.9/rob/hierarchy.py
+-rw-r--r--   0        0        0     7590 2022-02-27 00:03:52.749759 robolson-0.3.9/rob/reddit_archive.py
+-rw-r--r--   0        0        0     3922 2022-01-01 00:08:23.770615 robolson-0.3.9/rob/robai.py
+-rw-r--r--   0        0        0      712 2022-03-03 22:37:01.742591 robolson-0.3.9/setup.py
+-rw-r--r--   0        0        0      471 2022-03-03 22:37:01.742591 robolson-0.3.9/PKG-INFO
```

### Comparing `robolson-0.3.8/config/clean.toml` & `robolson-0.3.9/config/clean.toml`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/pyproject.toml` & `robolson-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "robolson"
-version = "0.3.8"
+version = "0.3.9"
 description = "My collection of utilty scripts"
 authors = ["Rob L Olson <rob.louis@gmail.com>"]
 include = ["config/clean.toml", "rob/config/clean.toml"]
 packages = [
-    {include="*.py", from="rob"},{include="config/clean.toml"}
+    {include="rob"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^11.2.0"
 toml = "^0.10.2"
 praw = "^7.5.0"
```

### Comparing `robolson-0.3.8/rob/__init__.py` & `robolson-0.3.9/rob/__init__.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/rob/clean.py` & `robolson-0.3.9/rob/clean.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/rob/ffmpeg_concat.py` & `robolson-0.3.9/rob/ffmpeg_concat.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/rob/hierarchy.py` & `robolson-0.3.9/rob/hierarchy.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/rob/reddit_archive.py` & `robolson-0.3.9/rob/reddit_archive.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/rob/robai.py` & `robolson-0.3.9/rob/robai.py`

 * *Files identical despite different names*

### Comparing `robolson-0.3.8/setup.py` & `robolson-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
-package_dir = \
-{'': 'rob'}
-
 packages = \
 ['rob']
 
 package_data = \
 {'': ['*']}
 
-modules = \
-['clean']
 install_requires = \
 ['openai>=0.15.0,<0.16.0',
  'praw>=7.5.0,<8.0.0',
  'pydub>=0.25.1,<0.26.0',
  'rich>=11.2.0,<12.0.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'robolson',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'My collection of utilty scripts',
     'long_description': None,
     'author': 'Rob L Olson',
     'author_email': 'rob.louis@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
-    'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'py_modules': modules,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

