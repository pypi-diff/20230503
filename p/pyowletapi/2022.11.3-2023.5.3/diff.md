# Comparing `tmp/pyowletapi-2022.11.3.tar.gz` & `tmp/pyowletapi-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2022.11.3.tar", last modified: Mon Nov 14 12:39:09 2022, max compression
+gzip compressed data, was "pyowletapi-2023.5.3.tar", last modified: Wed May  3 13:39:16 2023, max compression
```

## Comparing `pyowletapi-2022.11.3.tar` & `pyowletapi-2023.5.3.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 12:39:09.034123 pyowletapi-2022.11.3/
--rw-rw-rw-   0        0        0     1726 2022-11-14 12:39:09.034506 pyowletapi-2022.11.3/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2022-11-14 12:35:56.000000 pyowletapi-2022.11.3/README.md
--rw-rw-rw-   0        0        0       88 2022-11-12 00:42:12.000000 pyowletapi-2022.11.3/pyproject.toml
--rw-rw-rw-   0        0        0       85 2022-11-14 12:39:09.043506 pyowletapi-2022.11.3/setup.cfg
--rw-rw-rw-   0        0        0      846 2022-11-14 12:37:20.000000 pyowletapi-2022.11.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-14 12:39:08.968505 pyowletapi-2022.11.3/src/
-drwxrwxrwx   0        0        0        0 2022-11-14 12:39:09.002077 pyowletapi-2022.11.3/src/pyowletapi/
--rw-rw-rw-   0        0        0       17 2022-11-12 00:32:50.000000 pyowletapi-2022.11.3/src/pyowletapi/__init__.py
--rw-rw-rw-   0        0        0     9745 2022-11-14 12:35:47.000000 pyowletapi-2022.11.3/src/pyowletapi/api.py
--rw-rw-rw-   0        0        0      318 2022-11-12 00:01:08.000000 pyowletapi-2022.11.3/src/pyowletapi/exceptions.py
--rw-rw-rw-   0        0        0     3501 2022-11-14 12:33:31.000000 pyowletapi-2022.11.3/src/pyowletapi/owlet.py
--rw-rw-rw-   0        0        0     6935 2022-11-14 12:34:27.000000 pyowletapi-2022.11.3/src/pyowletapi/sock.py
-drwxrwxrwx   0        0        0        0 2022-11-14 12:39:09.031509 pyowletapi-2022.11.3/src/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     1726 2022-11-14 12:39:08.000000 pyowletapi-2022.11.3/src/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2022-11-14 12:39:08.000000 pyowletapi-2022.11.3/src/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 12:39:08.000000 pyowletapi-2022.11.3/src/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-11-14 12:39:08.000000 pyowletapi-2022.11.3/src/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-14 12:39:08.000000 pyowletapi-2022.11.3/src/pyowletapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.975447 pyowletapi-2023.5.3/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 13:39:16.976446 pyowletapi-2023.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.930447 pyowletapi-2023.5.3/pyowletapi/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:39:16.973447 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:39:16.000000 pyowletapi-2023.5.3/pyowletapi/pyowletapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-03 13:39:16.984449 pyowletapi-2023.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-05-03 13:39:12.000000 pyowletapi-2023.5.3/setup.py
```

### Comparing `pyowletapi-2022.11.3/PKG-INFO` & `pyowletapi-2023.5.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pyowletapi
-Version: 2022.11.3
-Summary: Owlet baby montior API wrapper
-Home-page: https://github.com/RyanClark123/pyowletapi
-Author: Ryan Clark
-Keywords: owlet,api,baby
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # Introduction
 
 First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
 
 inspiration and API reverse engineering taken from various projects:
 
 https://github.com/BastianPoe/owlet_api
```

### Comparing `pyowletapi-2022.11.3/setup.py` & `pyowletapi-2023.5.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    
     name="pyowletapi",
-    version="2022.11.3",
+    version="2023.05.3",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
     classifiers=[ 
         "License :: OSI Approved :: MIT License",        
         "Programming Language :: Python :: 3.9",
     ],
     
     keywords="owlet, api, baby",
-    package_dir={"": "src"}, 
-    packages=find_packages(where="src"), 
+    package_dir={"": "pyowletapi"}, 
+    packages=find_packages(where="pyowletapi"), 
     python_requires=">=3.9",
     
     install_requires=["aiohttp"], 
 )
```

