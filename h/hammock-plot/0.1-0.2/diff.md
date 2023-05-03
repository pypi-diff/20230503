# Comparing `tmp/hammock_plot-0.1.tar.gz` & `tmp/hammock_plot-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammock_plot-0.1.tar", last modified: Tue May  2 04:44:30 2023, max compression
+gzip compressed data, was "hammock_plot-0.2.tar", last modified: Wed May  3 15:37:33 2023, max compression
```

## Comparing `hammock_plot-0.1.tar` & `hammock_plot-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:44:30.441267 hammock_plot-0.1/
--rw-rw-rw-   0        0        0    10834 2023-05-02 04:44:30.441267 hammock_plot-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8765 2023-05-02 04:44:02.000000 hammock_plot-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 04:44:30.429259 hammock_plot-0.1/hammock_plot/
--rw-rw-rw-   0        0        0      107 2023-05-02 04:19:20.000000 hammock_plot-0.1/hammock_plot/__init__.py
--rw-rw-rw-   0        0        0    22194 2023-05-02 04:19:20.000000 hammock_plot-0.1/hammock_plot/hammock_plot.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:44:30.440260 hammock_plot-0.1/hammock_plot.egg-info/
--rw-rw-rw-   0        0        0    10834 2023-05-02 04:44:30.000000 hammock_plot-0.1/hammock_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-02 04:44:30.000000 hammock_plot-0.1/hammock_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:44:30.000000 hammock_plot-0.1/hammock_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-02 04:44:30.000000 hammock_plot-0.1/hammock_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 04:44:30.000000 hammock_plot-0.1/hammock_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 04:44:30.441267 hammock_plot-0.1/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-05-02 04:43:17.000000 hammock_plot-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:33.265576 hammock_plot-0.2/
+-rw-rw-rw-   0        0        0    10731 2023-05-03 15:37:33.265576 hammock_plot-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8698 2023-05-03 15:37:06.000000 hammock_plot-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:33.250575 hammock_plot-0.2/hammock_plot/
+-rw-rw-rw-   0        0        0      107 2023-05-02 04:19:20.000000 hammock_plot-0.2/hammock_plot/__init__.py
+-rw-rw-rw-   0        0        0    22194 2023-05-02 04:19:20.000000 hammock_plot-0.2/hammock_plot/hammock_plot.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:37:33.264575 hammock_plot-0.2/hammock_plot.egg-info/
+-rw-rw-rw-   0        0        0    10731 2023-05-03 15:37:33.000000 hammock_plot-0.2/hammock_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-03 15:37:33.000000 hammock_plot-0.2/hammock_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:37:33.000000 hammock_plot-0.2/hammock_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-03 15:37:33.000000 hammock_plot-0.2/hammock_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 15:37:33.000000 hammock_plot-0.2/hammock_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 15:37:33.265576 hammock_plot-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      883 2023-05-03 15:37:26.000000 hammock_plot-0.2/setup.py
```

### Comparing `hammock_plot-0.1/PKG-INFO` & `hammock_plot-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hammock_plot
-Version: 0.1
+Version: 0.2
 Summary: Hammock - visualization of categorical or mixed categorical/continuous data
 Home-page: https://github.com/TianchengY/hammock_plot
 Author: Tiancheng Yang
 Author-email: t77yang@uwaterloo.ca
 License: UNKNOWN
 Description: # Hammock plot
         
@@ -28,19 +28,15 @@
             destring.
         
         
         
         
         ## Getting started
         
-        You can install hammock from `conda` or `pip`:
-        
-        ```shell
-        conda install hammock_plot -c conda-forge
-        ```
+        You can install hammock from `pip`:
         
         ```shell
         pip install hammock_plot
         ```
         
         
         ### Example: Asthma data
```

### Comparing `hammock_plot-0.1/README.md` & `hammock_plot-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,15 @@
     destring.
 
 
 
 
 ## Getting started
 
-You can install hammock from `conda` or `pip`:
-
-```shell
-conda install hammock_plot -c conda-forge
-```
+You can install hammock from `pip`:
 
 ```shell
 pip install hammock_plot
 ```
 
 
 ### Example: Asthma data
```

### Comparing `hammock_plot-0.1/hammock_plot/hammock_plot.py` & `hammock_plot-0.2/hammock_plot/hammock_plot.py`

 * *Files identical despite different names*

### Comparing `hammock_plot-0.1/hammock_plot.egg-info/PKG-INFO` & `hammock_plot-0.2/hammock_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hammock-plot
-Version: 0.1
+Version: 0.2
 Summary: Hammock - visualization of categorical or mixed categorical/continuous data
 Home-page: https://github.com/TianchengY/hammock_plot
 Author: Tiancheng Yang
 Author-email: t77yang@uwaterloo.ca
 License: UNKNOWN
 Description: # Hammock plot
         
@@ -28,19 +28,15 @@
             destring.
         
         
         
         
         ## Getting started
         
-        You can install hammock from `conda` or `pip`:
-        
-        ```shell
-        conda install hammock_plot -c conda-forge
-        ```
+        You can install hammock from `pip`:
         
         ```shell
         pip install hammock_plot
         ```
         
         
         ### Example: Asthma data
```

### Comparing `hammock_plot-0.1/setup.py` & `hammock_plot-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # import versioneer
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hammock_plot",
-    version='0.1',
+    version='0.2',
     author="Tiancheng Yang",
     author_email="t77yang@uwaterloo.ca",
     description="Hammock - visualization of categorical or mixed categorical/continuous data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TianchengY/hammock_plot",
     packages=setuptools.find_packages(),
```

