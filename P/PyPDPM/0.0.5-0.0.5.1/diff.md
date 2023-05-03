# Comparing `tmp/PyPDPM-0.0.5.tar.gz` & `tmp/PyPDPM-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDPM-0.0.5.tar", last modified: Wed May  3 02:59:55 2023, max compression
+gzip compressed data, was "PyPDPM-0.0.5.1.tar", last modified: Wed May  3 03:06:35 2023, max compression
```

## Comparing `PyPDPM-0.0.5.tar` & `PyPDPM-0.0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.880636 PyPDPM-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4931 2023-05-03 02:59:55.880636 PyPDPM-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.838678 PyPDPM-0.0.5/PyPDPM/
--rw-rw-rw-   0        0        0    26082 2023-05-03 02:59:47.000000 PyPDPM-0.0.5/PyPDPM/HIPPS.py
--rw-rw-rw-   0        0        0        0 2023-04-17 07:54:29.000000 PyPDPM-0.0.5/PyPDPM/__init__.py
--rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5/PyPDPM/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.879609 PyPDPM-0.0.5/PyPDPM.egg-info/
--rw-rw-rw-   0        0        0     4931 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4601 2023-05-03 02:51:00.000000 PyPDPM-0.0.5/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-03 02:59:55.882609 PyPDPM-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-05-03 02:58:30.000000 PyPDPM-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.486711 PyPDPM-0.0.5.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:06:35.487708 PyPDPM-0.0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.467710 PyPDPM-0.0.5.1/PyPDPM/
+-rw-rw-rw-   0        0        0    26082 2023-05-03 03:04:11.000000 PyPDPM-0.0.5.1/PyPDPM/HIPPS.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:54:29.000000 PyPDPM-0.0.5.1/PyPDPM/__init__.py
+-rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5.1/PyPDPM/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:06:35.485710 PyPDPM-0.0.5.1/PyPDPM.egg-info/
+-rw-rw-rw-   0        0        0     4928 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 03:06:35.000000 PyPDPM-0.0.5.1/PyPDPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4596 2023-05-03 03:05:29.000000 PyPDPM-0.0.5.1/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-03 03:06:35.488709 PyPDPM-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-03 03:06:10.000000 PyPDPM-0.0.5.1/setup.py
```

### Comparing `PyPDPM-0.0.5/LICENSE.txt` & `PyPDPM-0.0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5/PKG-INFO` & `PyPDPM-0.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 PyPDPM
-===
 
 .. image:: https://img.shields.io/pypi/v/icd.svg
     :target: https://pypi.python.org/pypi/icd
     :alt: Latest PyPI version
 
 
 Tools for working with the CMS case-mix classification model, payment driven payment model (PDPM). Deatils about PDPM can be found here: https://www.cms.gov/medicare/medicare-fee-for-service-payment/snfpps/pdpm.
```

### Comparing `PyPDPM-0.0.5/PyPDPM/HIPPS.py` & `PyPDPM-0.0.5.1/PyPDPM/HIPPS.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5/PyPDPM/mappings.py` & `PyPDPM-0.0.5.1/PyPDPM/mappings.py`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.5/PyPDPM.egg-info/PKG-INFO` & `PyPDPM-0.0.5.1/PyPDPM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 PyPDPM
-===
 
 .. image:: https://img.shields.io/pypi/v/icd.svg
     :target: https://pypi.python.org/pypi/icd
     :alt: Latest PyPI version
 
 
 Tools for working with the CMS case-mix classification model, payment driven payment model (PDPM). Deatils about PDPM can be found here: https://www.cms.gov/medicare/medicare-fee-for-service-payment/snfpps/pdpm.
```

### Comparing `PyPDPM-0.0.5/README.rst` & `PyPDPM-0.0.5.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 PyPDPM
-===
 
 .. image:: https://img.shields.io/pypi/v/icd.svg
     :target: https://pypi.python.org/pypi/icd
     :alt: Latest PyPI version
 
 
 Tools for working with the CMS case-mix classification model, payment driven payment model (PDPM). Deatils about PDPM can be found here: https://www.cms.gov/medicare/medicare-fee-for-service-payment/snfpps/pdpm.
```

### Comparing `PyPDPM-0.0.5/setup.py` & `PyPDPM-0.0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 setup(
     name='PyPDPM',
     packages=find_packages(include=['PyPDPM']),
-    version='0.0.5',
+    version='0.0.5.1',
     description='A Python library for dealing with PDPM HIPP codes',
     author='Caro Strickland',
     author_email='carostrickland321@gmail.com',
     url = 'https://github.com/Scorks/PyPDPM',
     long_description=readme,
     keywords = ['PDPM', 'HIPPS', 'ICD-10-CM Codes'],
     license='MIT',
```

