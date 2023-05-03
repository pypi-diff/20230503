# Comparing `tmp/PyPDPM-0.0.4.tar.gz` & `tmp/PyPDPM-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDPM-0.0.4.tar", last modified: Wed May  3 02:51:15 2023, max compression
+gzip compressed data, was "PyPDPM-0.0.5.tar", last modified: Wed May  3 02:59:55 2023, max compression
```

## Comparing `PyPDPM-0.0.4.tar` & `PyPDPM-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:15.370392 PyPDPM-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4931 2023-05-03 02:51:15.371391 PyPDPM-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:15.358392 PyPDPM-0.0.4/PyPDPM/
--rw-rw-rw-   0        0        0    26135 2023-05-02 23:20:43.000000 PyPDPM-0.0.4/PyPDPM/HIPPS.py
--rw-rw-rw-   0        0        0        0 2023-04-17 07:54:29.000000 PyPDPM-0.0.4/PyPDPM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:15.369392 PyPDPM-0.0.4/PyPDPM.egg-info/
--rw-rw-rw-   0        0        0     4931 2023-05-03 02:51:15.000000 PyPDPM-0.0.4/PyPDPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-03 02:51:15.000000 PyPDPM-0.0.4/PyPDPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 02:51:15.000000 PyPDPM-0.0.4/PyPDPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 02:51:15.000000 PyPDPM-0.0.4/PyPDPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4601 2023-05-03 02:51:00.000000 PyPDPM-0.0.4/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-03 02:51:15.372390 PyPDPM-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-05-03 02:42:23.000000 PyPDPM-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.880636 PyPDPM-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:06:47.000000 PyPDPM-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4931 2023-05-03 02:59:55.880636 PyPDPM-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.838678 PyPDPM-0.0.5/PyPDPM/
+-rw-rw-rw-   0        0        0    26082 2023-05-03 02:59:47.000000 PyPDPM-0.0.5/PyPDPM/HIPPS.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:54:29.000000 PyPDPM-0.0.5/PyPDPM/__init__.py
+-rw-rw-rw-   0        0        0  3041219 2023-05-03 01:51:55.000000 PyPDPM-0.0.5/PyPDPM/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:59:55.879609 PyPDPM-0.0.5/PyPDPM.egg-info/
+-rw-rw-rw-   0        0        0     4931 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 02:59:55.000000 PyPDPM-0.0.5/PyPDPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4601 2023-05-03 02:51:00.000000 PyPDPM-0.0.5/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-03 02:59:55.882609 PyPDPM-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-05-03 02:58:30.000000 PyPDPM-0.0.5/setup.py
```

### Comparing `PyPDPM-0.0.4/LICENSE.txt` & `PyPDPM-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.4/PKG-INFO` & `PyPDPM-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.4/PyPDPM/HIPPS.py` & `PyPDPM-0.0.5/PyPDPM/HIPPS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-sys.path.append('..')
+# sys.path.append('..')
 
-from data import mappings
+import mappings
 
 PAYMENT_GROUP_TO_HIPPS_CODE_VALUE = {('TA', 'SA', 'ES3', 'NA'): 'A', ('TB', 'SB', 'ES2', 'NB'): 'B',
                                      ('TC', 'SC', 'ES1', 'NC'): 'C', ('TD', 'SD', 'HDE2', 'ND'): 'D',
                                      ('TE', 'SE', 'HDE1', 'NE'): 'E', ('TF', 'SF', 'HBC2', 'NF'): 'F',
                                      ('TG', 'SG', 'CBC2'): 'G', ('TH', 'SH', 'CA2'): 'H',
                                      ('TI', 'SI', 'CBC1'): 'I', ('TJ', 'SJ', 'CA1'): 'J',
                                      ('TK', 'SK', 'BAB2'): 'K', ('TL', 'SL', 'BAB1'): 'L',
@@ -595,9 +595,8 @@
 # print(_get_SLP_CaseMixClassificationGroup(True, True, False, True, ['I69991', 'C322', 'notACode']))
 
 code = get_PDPM_HIPPS_code('TC', 'SC', 'PA1', 'NA', 0)
 code = get_PDPM_HIPPS_code('TC', 'SC', 'PA1', 'NA')
 print(code)
 print(getReimbursementAmount(code, 4))
 print(calculateTotalReimbursement(code, 30))
-'''
-print(getReimbursementAmount('AAAA1', 2))
+'''
```

### Comparing `PyPDPM-0.0.4/PyPDPM.egg-info/PKG-INFO` & `PyPDPM-0.0.5/PyPDPM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDPM
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for dealing with PDPM HIPP codes
 Home-page: https://github.com/Scorks/PyPDPM
 Author: Caro Strickland
 Author-email: carostrickland321@gmail.com
 License: MIT
 Keywords: PDPM,HIPPS,ICD-10-CM Codes
 Platform: UNKNOWN
```

### Comparing `PyPDPM-0.0.4/README.rst` & `PyPDPM-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `PyPDPM-0.0.4/setup.py` & `PyPDPM-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 setup(
     name='PyPDPM',
     packages=find_packages(include=['PyPDPM']),
-    version='0.0.4',
+    version='0.0.5',
     description='A Python library for dealing with PDPM HIPP codes',
     author='Caro Strickland',
     author_email='carostrickland321@gmail.com',
     url = 'https://github.com/Scorks/PyPDPM',
     long_description=readme,
     keywords = ['PDPM', 'HIPPS', 'ICD-10-CM Codes'],
     license='MIT',
```

