# Comparing `tmp/crawler_commons-0.0.1.tar.gz` & `tmp/crawler_commons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crawler_commons-0.0.1.tar", last modified: Tue Apr 11 09:33:57 2023, max compression
+gzip compressed data, was "dist/crawler_commons-0.0.2.tar", last modified: Wed May  3 17:15:53 2023, max compression
```

## Comparing `crawler_commons-0.0.1.tar` & `crawler_commons-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     1487 2023-04-11 09:33:14.000000 crawler_commons-0.0.1/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.1/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.1/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      552 2023-04-11 09:33:54.000000 crawler_commons-0.0.1/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      205 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       11 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawler_commons.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-11 09:33:57.000000 crawler_commons-0.0.1/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.2/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.2/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.2/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      552 2023-05-03 17:15:51.000000 crawler_commons-0.0.2/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      205 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       11 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/setup.cfg
```

### Comparing `crawler_commons-0.0.1/LICENSE` & `crawler_commons-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.1/setup.py` & `crawler_commons-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.1",
+    version="0.0.2",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(),
```

