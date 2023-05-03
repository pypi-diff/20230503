# Comparing `tmp/wombato-0.0.5.tar.gz` & `tmp/wombato-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-rstfmkya\wombato-0.0.5.tar", last modified: Wed May  3 03:15:12 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-h3vbirma\wombato-0.0.6.tar", last modified: Wed May  3 03:30:58 2023, max compression
```

## Comparing `wombato-0.0.5.tar` & `wombato-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:15:12.000000 wombato-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0      529 2023-05-03 03:15:12.000000 wombato-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombato-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 03:15:12.000000 wombato-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-05-03 03:14:14.000000 wombato-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:15:12.000000 wombato-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombato-0.0.5/src/__init__.py
--rw-rw-rw-   0        0        0     9596 2023-05-01 13:07:41.000000 wombato-0.0.5/src/wombato.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/
--rw-rw-rw-   0        0        0      529 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-03 03:15:12.000000 wombato-0.0.5/wombato.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 03:30:58.000000 wombato-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      478 2023-05-03 03:30:58.000000 wombato-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombato-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:30:58.000000 wombato-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-05-03 03:30:37.000000 wombato-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:30:58.000000 wombato-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombato-0.0.6/src/__init__.py
+-rw-rw-rw-   0        0        0     9596 2023-05-01 13:07:41.000000 wombato-0.0.6/src/wombato.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-03 03:30:58.000000 wombato-0.0.6/wombato.egg-info/top_level.txt
```

### Comparing `wombato-0.0.5/LICENSE.md` & `wombato-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wombato-0.0.5/setup.py` & `wombato-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name="wombato",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(exclude=["tests", "examples", "docs"]),
     include_package_data=True,
     description="A Data-Ops tool for devs",
     long_description="Please refer to: README",
     long_description_content_type="text/markdown",
     url="https://github.com/prashdash112/wombat",
     author="Prashant Singh",
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9"
     ],
     license="Please refer to the readme",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=["numpy==1.23.5",
                       "pandas==1.5.2",
                       "pyhtml2pdf==0.0.6",
                       "ydata-profiling==4.1.1"]
                       )
```

### Comparing `wombato-0.0.5/src/wombato.py` & `wombato-0.0.6/src/wombato.py`

 * *Files identical despite different names*

