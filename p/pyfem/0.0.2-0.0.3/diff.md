# Comparing `tmp/pyfem-0.0.2.tar.gz` & `tmp/pyfem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.2.tar", last modified: Wed May  3 10:38:13 2023, max compression
+gzip compressed data, was "pyfem-0.0.3.tar", last modified: Wed May  3 10:50:29 2023, max compression
```

## Comparing `pyfem-0.0.2.tar` & `pyfem-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.860701 pyfem-0.0.2/
--rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      535 2023-05-03 10:38:13.860206 pyfem-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-05-03 09:58:16.000000 pyfem-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 10:38:13.860701 pyfem-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-05-03 10:37:50.000000 pyfem-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.821477 pyfem-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.836397 pyfem-0.0.2/src/pyfem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-03 10:34:48.000000 pyfem-0.0.2/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.846813 pyfem-0.0.2/src/pyfem/assembly/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.848301 pyfem-0.0.2/src/pyfem/elements/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.849789 pyfem-0.0.2/src/pyfem/fem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/fem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.851774 pyfem-0.0.2/src/pyfem/io/
--rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.2/src/pyfem/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.853263 pyfem-0.0.2/src/pyfem/materials/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/materials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.855247 pyfem-0.0.2/src/pyfem/mesh/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.856735 pyfem-0.0.2/src/pyfem/solvers/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/solvers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.858222 pyfem-0.0.2/src/pyfem/utils/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.845325 pyfem-0.0.2/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      535 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.265435 pyfem-0.0.3/
+-rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      535 2023-05-03 10:50:29.264940 pyfem-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-05-03 09:58:16.000000 pyfem-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:50:29.265932 pyfem-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-05-03 10:50:04.000000 pyfem-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.224120 pyfem-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.238652 pyfem-0.0.3/src/pyfem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-05-03 10:49:57.000000 pyfem-0.0.3/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.249068 pyfem-0.0.3/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.250556 pyfem-0.0.3/src/pyfem/elements/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.252540 pyfem-0.0.3/src/pyfem/fem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.255516 pyfem-0.0.3/src/pyfem/io/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.3/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-03 05:18:43.000000 pyfem-0.0.3/src/pyfem/io/arguments.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.257500 pyfem-0.0.3/src/pyfem/materials/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/materials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.258988 pyfem-0.0.3/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.261467 pyfem-0.0.3/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/solvers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.263452 pyfem-0.0.3/src/pyfem/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.3/src/pyfem/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:50:29.247580 pyfem-0.0.3/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-05-03 10:50:29.000000 pyfem-0.0.3/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-05-03 10:50:29.000000 pyfem-0.0.3/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:50:29.000000 pyfem-0.0.3/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 10:50:29.000000 pyfem-0.0.3/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 10:50:29.000000 pyfem-0.0.3/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.2/LICENSE` & `pyfem-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.2/PKG-INFO` & `pyfem-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.2
+Version: 0.0.3
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.2/setup.py` & `pyfem-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.2",
+    version="0.0.3",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.0.2/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.3/src/pyfem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.2
+Version: 0.0.3
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

