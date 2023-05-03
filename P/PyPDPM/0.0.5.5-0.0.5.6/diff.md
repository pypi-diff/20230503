# Comparing `tmp/PyPDPM-0.0.5.5.tar.gz` & `tmp/PyPDPM-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDPM-0.0.5.5.tar", last modified: Wed May  3 03:39:02 2023, max compression
+gzip compressed data, was "PyPDPM-0.0.5.6.tar", last modified: Wed May  3 03:43:09 2023, max compression
```

## Comparing `PyPDPM-0.0.5.5.tar` & `PyPDPM-0.0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:39:02.933317 PyPDPM-0.0.5.5/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:39:02.933317 PyPDPM-0.0.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 03:39:02.895318 PyPDPM-0.0.5.5/PyPDPM/
--rw-rw-rw-   0        0        0    26082 2023-05-03 03:36:15.000000 PyPDPM-0.0.5.5/PyPDPM/HIPPS.py
--rw-rw-rw-   0        0        0       43 2023-05-03 03:38:10.000000 PyPDPM-0.0.5.5/PyPDPM/__init__.py
--rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5.5/PyPDPM/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:39:02.931317 PyPDPM-0.0.5.5/PyPDPM.egg-info/
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:39:02.000000 PyPDPM-0.0.5.5/PyPDPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-03 03:39:02.000000 PyPDPM-0.0.5.5/PyPDPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:39:02.000000 PyPDPM-0.0.5.5/PyPDPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 03:39:02.000000 PyPDPM-0.0.5.5/PyPDPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.5/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-03 03:39:02.935315 PyPDPM-0.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      660 2023-05-03 03:38:36.000000 PyPDPM-0.0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:43:09.013710 PyPDPM-0.0.5.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:43:09.013710 PyPDPM-0.0.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 03:43:08.992706 PyPDPM-0.0.5.6/PyPDPM/
+-rw-rw-rw-   0        0        0    26082 2023-05-03 03:36:15.000000 PyPDPM-0.0.5.6/PyPDPM/HIPPS.py
+-rw-rw-rw-   0        0        0       43 2023-05-03 03:40:37.000000 PyPDPM-0.0.5.6/PyPDPM/__init__.py
+-rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5.6/PyPDPM/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:43:09.010707 PyPDPM-0.0.5.6/PyPDPM.egg-info/
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:43:08.000000 PyPDPM-0.0.5.6/PyPDPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-03 03:43:08.000000 PyPDPM-0.0.5.6/PyPDPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:43:08.000000 PyPDPM-0.0.5.6/PyPDPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 03:43:08.000000 PyPDPM-0.0.5.6/PyPDPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.6/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-03 03:43:09.015706 PyPDPM-0.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-03 03:43:07.000000 PyPDPM-0.0.5.6/setup.py
```

### Comparing `PyPDPM-0.0.5.5/LICENSE.txt` & `PyPDPM-0.0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.5/PKG-INFO` & `PyPDPM-0.0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.5/PyPDPM/HIPPS.py` & `PyPDPM-0.0.5.6/PyPDPM/HIPPS.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.5/PyPDPM/mappings.py` & `PyPDPM-0.0.5.6/PyPDPM/mappings.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.5/PyPDPM.egg-info/PKG-INFO` & `PyPDPM-0.0.5.6/PyPDPM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.5/README.rst` & `PyPDPM-0.0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.5/setup.py` & `PyPDPM-0.0.5.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 setup(
     name='PyPDPM',
-    packages=find_packages(include=['PyPDPM', 'PyPDPM.mappings']),
-    version='0.0.5.5',
+    packages=find_packages(include=['PyPDPM', 'PyPDPM.mappings', 'PyPDPM.HIPPS']),
+    version='0.0.5.6',
     description='A Python library for dealing with PDPM HIPP codes',
     author='Caro Strickland',
     author_email='carostrickland321@gmail.com',
     url = 'https://github.com/Scorks/PyPDPM',
     long_description=readme,
     keywords = ['PDPM', 'HIPPS', 'ICD-10-CM Codes'],
     license='MIT',
```

