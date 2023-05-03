# Comparing `tmp/PyPDPM-0.0.5.1.tar.gz` & `tmp/PyPDPM-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDPM-0.0.5.1.tar", last modified: Wed May  3 03:06:35 2023, max compression
+gzip compressed data, was "PyPDPM-0.0.5.2.tar", last modified: Wed May  3 03:13:49 2023, max compression
```

## Comparing `PyPDPM-0.0.5.1.tar` & `PyPDPM-0.0.5.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.486711 PyPDPM-0.0.5.1/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:06:35.487708 PyPDPM-0.0.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.467710 PyPDPM-0.0.5.1/PyPDPM/
--rw-rw-rw-   0        0        0    26082 2023-05-03 03:04:11.000000 PyPDPM-0.0.5.1/PyPDPM/HIPPS.py
--rw-rw-rw-   0        0        0        0 2023-04-17 07:54:29.000000 PyPDPM-0.0.5.1/PyPDPM/__init__.py
--rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5.1/PyPDPM/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.485710 PyPDPM-0.0.5.1/PyPDPM.egg-info/
--rw-rw-rw-   0        0        0     4928 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.1/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-03 03:06:35.488709 PyPDPM-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-03 03:06:10.000000 PyPDPM-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:13:49.722690 PyPDPM-0.0.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:13:49.722690 PyPDPM-0.0.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 03:13:49.702690 PyPDPM-0.0.5.2/PyPDPM/
+-rw-rw-rw-   0        0        0    26082 2023-05-03 03:11:58.000000 PyPDPM-0.0.5.2/PyPDPM/__init__.py
+-rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5.2/PyPDPM/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:13:49.720690 PyPDPM-0.0.5.2/PyPDPM.egg-info/
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:13:49.000000 PyPDPM-0.0.5.2/PyPDPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-03 03:13:49.000000 PyPDPM-0.0.5.2/PyPDPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:13:49.000000 PyPDPM-0.0.5.2/PyPDPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 03:13:49.000000 PyPDPM-0.0.5.2/PyPDPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.2/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-03 03:13:49.724690 PyPDPM-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-03 03:13:44.000000 PyPDPM-0.0.5.2/setup.py
```

### Comparing `PyPDPM-0.0.5.1/LICENSE.txt` & `PyPDPM-0.0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.1/PKG-INFO` & `PyPDPM-0.0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.1/PyPDPM/HIPPS.py` & `PyPDPM-0.0.5.2/PyPDPM/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.1/PyPDPM/mappings.py` & `PyPDPM-0.0.5.2/PyPDPM/mappings.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.1/PyPDPM.egg-info/PKG-INFO` & `PyPDPM-0.0.5.2/PyPDPM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.5.1/README.rst` & `PyPDPM-0.0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5.1/setup.py` & `PyPDPM-0.0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 setup(
     name='PyPDPM',
     packages=find_packages(include=['PyPDPM']),
-    version='0.0.5.1',
+    version='0.0.5.2',
     description='A Python library for dealing with PDPM HIPP codes',
     author='Caro Strickland',
     author_email='carostrickland321@gmail.com',
     url = 'https://github.com/Scorks/PyPDPM',
     long_description=readme,
     keywords = ['PDPM', 'HIPPS', 'ICD-10-CM Codes'],
     license='MIT',
```

