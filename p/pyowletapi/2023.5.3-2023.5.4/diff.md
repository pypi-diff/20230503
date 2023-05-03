# Comparing `tmp/pyowletapi-2023.5.3.tar.gz` & `tmp/pyowletapi-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.5.3.tar", last modified: Wed May  3 13:39:16 2023, max compression
+gzip compressed data, was "pyowletapi-2023.5.4.tar", last modified: Wed May  3 14:50:57 2023, max compression
```

## Comparing `pyowletapi-2023.5.3.tar` & `pyowletapi-2023.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.975447 pyowletapi-2023.5.3/
--rw-rw-rw-   0        0        0     2175 2023-05-03 13:39:16.976446 pyowletapi-2023.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.930447 pyowletapi-2023.5.3/pyowletapi/
-drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.973447 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     2175 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-03 13:39:16.984449 pyowletapi-2023.5.3/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-05-03 13:39:12.000000 pyowletapi-2023.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.462345 pyowletapi-2023.5.4/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 14:50:57.463343 pyowletapi-2023.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.415345 pyowletapi-2023.5.4/pyowletapi/
+drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.460345 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-03 14:50:57.465343 pyowletapi-2023.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-05-03 14:50:49.000000 pyowletapi-2023.5.4/setup.py
```

### Comparing `pyowletapi-2023.5.3/PKG-INFO` & `pyowletapi-2023.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

### Comparing `pyowletapi-2023.5.3/README.md` & `pyowletapi-2023.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

### Comparing `pyowletapi-2023.5.3/setup.py` & `pyowletapi-2023.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    
     name="pyowletapi",
-    version="2023.05.3",
+    version="2023.05.4",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
     classifiers=[ 
         "License :: OSI Approved :: MIT License",
```

