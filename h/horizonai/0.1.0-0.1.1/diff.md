# Comparing `tmp/horizonai-0.1.0.tar.gz` & `tmp/horizonai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizonai-0.1.0.tar", last modified: Wed May  3 18:06:32 2023, max compression
+gzip compressed data, was "horizonai-0.1.1.tar", last modified: Wed May  3 18:21:41 2023, max compression
```

## Comparing `horizonai-0.1.0.tar` & `horizonai-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:06:32.730380 horizonai-0.1.0/
--rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.0/LICENSE
--rw-r--r--   0 linatawfik   (501) staff       (20)      697 2023-05-03 18:06:32.730469 horizonai-0.1.0/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.0/README.md
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:06:32.729517 horizonai-0.1.0/horizonai/
--rw-r--r--   0 linatawfik   (501) staff       (20)       63 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/__init__.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1515 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/base.py
--rw-r--r--   0 linatawfik   (501) staff       (20)    14372 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/cli.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/project.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/task.py
--rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.0/horizonai/user.py
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:06:32.730261 horizonai-0.1.0/horizonai.egg-info/
--rw-r--r--   0 linatawfik   (501) staff       (20)      697 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/SOURCES.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/dependency_links.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/entry_points.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/requires.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 18:06:32.000000 horizonai-0.1.0/horizonai.egg-info/top_level.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 18:06:32.730714 horizonai-0.1.0/setup.cfg
--rw-r--r--   0 linatawfik   (501) staff       (20)      989 2023-05-03 18:04:56.000000 horizonai-0.1.0/setup.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.357352 horizonai-0.1.1/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.1/LICENSE
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 18:21:41.357432 horizonai-0.1.1/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.1/README.md
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.356530 horizonai-0.1.1/horizonai/
+-rw-r--r--   0 linatawfik   (501) staff       (20)       63 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/__init__.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1515 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/base.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)    14372 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/cli.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/project.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/task.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/user.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.357214 horizonai-0.1.1/horizonai.egg-info/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/SOURCES.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/dependency_links.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/entry_points.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/requires.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/top_level.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 18:21:41.357861 horizonai-0.1.1/setup.cfg
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 18:21:15.000000 horizonai-0.1.1/setup.py
```

### Comparing `horizonai-0.1.0/LICENSE` & `horizonai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/README.md` & `horizonai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/horizonai/base.py` & `horizonai-0.1.1/horizonai/base.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/horizonai/cli.py` & `horizonai-0.1.1/horizonai/cli.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/horizonai/project.py` & `horizonai-0.1.1/horizonai/project.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/horizonai/task.py` & `horizonai-0.1.1/horizonai/task.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.0/setup.py` & `horizonai-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-# setup.py
-
 from setuptools import setup, find_packages
+import os
+
+
+def read(file_name):
+    with open(os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8") as f:
+        return f.read()
+
 
 setup(
     name="horizonai",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     package_data={"": ["__init__.py"]},
     install_requires=[
         "requests",
         "click",
     ],
     entry_points={"console_scripts": ["horizon=horizonai.cli:cli"]},
     author="Horizon Team",
     author_email="team@gethorizon.ai",
     license="MIT",
     description="Python package and command line interface to access the Horizon AI API",
+    long_description=read("README.md"),  # Include README.md content
+    long_description_content_type="text/markdown",  # Specify content type as Markdown
     url="https://www.gethorizon.ai",
-    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.0-alpha.tar.gz",
+    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.1-alpha.tar.gz",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

