# Comparing `tmp/horizonai-0.1.4.tar.gz` & `tmp/horizonai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizonai-0.1.4.tar", last modified: Wed May  3 20:12:22 2023, max compression
+gzip compressed data, was "horizonai-0.1.5.tar", last modified: Wed May  3 20:18:49 2023, max compression
```

## Comparing `horizonai-0.1.4.tar` & `horizonai-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:12:22.891780 horizonai-0.1.4/
--rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.4/LICENSE
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:12:22.891878 horizonai-0.1.4/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.4/README.md
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:12:22.890808 horizonai-0.1.4/horizonai/
--rw-r--r--   0 linatawfik   (501) staff       (20)       63 2023-05-03 16:55:57.000000 horizonai-0.1.4/horizonai/__init__.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1542 2023-05-03 20:09:16.000000 horizonai-0.1.4/horizonai/base.py
--rw-r--r--   0 linatawfik   (501) staff       (20)    14474 2023-05-03 18:31:03.000000 horizonai-0.1.4/horizonai/cli.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.4/horizonai/project.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.4/horizonai/task.py
--rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.4/horizonai/user.py
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:12:22.891658 horizonai-0.1.4/horizonai.egg-info/
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/SOURCES.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/dependency_links.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/entry_points.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/requires.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 20:12:22.000000 horizonai-0.1.4/horizonai.egg-info/top_level.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 20:12:22.892130 horizonai-0.1.4/setup.cfg
--rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 20:12:08.000000 horizonai-0.1.4/setup.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.967282 horizonai-0.1.5/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.5/LICENSE
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:18:49.967351 horizonai-0.1.5/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.5/README.md
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.966407 horizonai-0.1.5/horizonai/
+-rw-r--r--   0 linatawfik   (501) staff       (20)       83 2023-05-03 20:15:40.000000 horizonai-0.1.5/horizonai/__init__.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1542 2023-05-03 20:09:16.000000 horizonai-0.1.5/horizonai/base.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)    14474 2023-05-03 18:31:03.000000 horizonai-0.1.5/horizonai/cli.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/project.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/task.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/user.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.967181 horizonai-0.1.5/horizonai.egg-info/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/SOURCES.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/dependency_links.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/entry_points.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/requires.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/top_level.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 20:18:49.967566 horizonai-0.1.5/setup.cfg
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 20:18:13.000000 horizonai-0.1.5/setup.py
```

### Comparing `horizonai-0.1.4/LICENSE` & `horizonai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/PKG-INFO` & `horizonai-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.4-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.4/README.md` & `horizonai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/horizonai/base.py` & `horizonai-0.1.5/horizonai/base.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/horizonai/cli.py` & `horizonai-0.1.5/horizonai/cli.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/horizonai/project.py` & `horizonai-0.1.5/horizonai/project.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/horizonai/task.py` & `horizonai-0.1.5/horizonai/task.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.4/horizonai.egg-info/PKG-INFO` & `horizonai-0.1.5/horizonai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.4-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.4/setup.py` & `horizonai-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 def read(file_name):
     with open(os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="horizonai",
-    version="0.1.4",
+    version="0.1.5",
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
     long_description=read("README.md"),  # Include README.md content
     long_description_content_type="text/markdown",  # Specify content type as Markdown
     url="https://www.gethorizon.ai",
-    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.4-alpha.tar.gz",
+    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

