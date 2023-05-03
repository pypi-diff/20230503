# Comparing `tmp/okta_jwt_verifier-0.2.3.tar.gz` & `tmp/okta_jwt_verifier-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/okta_jwt_verifier-0.2.3.tar", last modified: Tue Nov 16 15:55:54 2021, max compression
+gzip compressed data, was "okta_jwt_verifier-0.2.4.tar", last modified: Wed May  3 14:05:02 2023, max compression
```

## Comparing `okta_jwt_verifier-0.2.3.tar` & `okta_jwt_verifier-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.716843 okta_jwt_verifier-0.2.3/
--rw-r--r--   0 bretterer   (501) staff       (20)     9810 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/LICENSE.md
--rw-r--r--   0 bretterer   (501) staff       (20)     1292 2021-11-16 15:55:54.717017 okta_jwt_verifier-0.2.3/PKG-INFO
--rw-r--r--   0 bretterer   (501) staff       (20)     8471 2021-11-03 14:32:54.000000 okta_jwt_verifier-0.2.3/README.md
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.696766 okta_jwt_verifier-0.2.3/okta_jwt_verifier/
--rw-r--r--   0 bretterer   (501) staff       (20)      227 2021-11-16 15:55:03.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/__init__.py
--rw-r--r--   0 bretterer   (501) staff       (20)     3550 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/config_validator.py
--rw-r--r--   0 bretterer   (501) staff       (20)      788 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/constants.py
--rw-r--r--   0 bretterer   (501) staff       (20)     1698 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/error_messages.py
--rw-r--r--   0 bretterer   (501) staff       (20)      230 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/exceptions.py
--rw-r--r--   0 bretterer   (501) staff       (20)     2874 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/jwt_utils.py
--rw-r--r--   0 bretterer   (501) staff       (20)    15102 2021-11-16 15:55:03.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/jwt_verifier.py
--rw-r--r--   0 bretterer   (501) staff       (20)     2002 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier/request_executor.py
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.698867 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/
--rw-r--r--   0 bretterer   (501) staff       (20)     1292 2021-11-16 15:55:54.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/PKG-INFO
--rw-r--r--   0 bretterer   (501) staff       (20)      738 2021-11-16 15:55:54.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/SOURCES.txt
--rw-r--r--   0 bretterer   (501) staff       (20)        1 2021-11-16 15:55:54.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/dependency_links.txt
--rw-r--r--   0 bretterer   (501) staff       (20)       40 2021-11-16 15:55:54.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/requires.txt
--rw-r--r--   0 bretterer   (501) staff       (20)       24 2021-11-16 15:55:54.000000 okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/top_level.txt
--rw-r--r--   0 bretterer   (501) staff       (20)      105 2021-11-16 15:55:54.717630 okta_jwt_verifier-0.2.3/setup.cfg
--rw-r--r--   0 bretterer   (501) staff       (20)     1458 2021-11-16 15:55:03.000000 okta_jwt_verifier-0.2.3/setup.py
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.685626 okta_jwt_verifier-0.2.3/tests/
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.705659 okta_jwt_verifier-0.2.3/tests/integration/
--rw-r--r--   0 bretterer   (501) staff       (20)        0 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/tests/integration/__init__.py
--rw-r--r--   0 bretterer   (501) staff       (20)     1867 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/tests/integration/test_jwt_verifier.py
-drwxr-xr-x   0 bretterer   (501) staff       (20)        0 2021-11-16 15:55:54.716144 okta_jwt_verifier-0.2.3/tests/unit/
--rw-r--r--   0 bretterer   (501) staff       (20)        0 2021-05-07 13:59:51.000000 okta_jwt_verifier-0.2.3/tests/unit/__init__.py
--rw-r--r--   0 bretterer   (501) staff       (20)     5558 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/tests/unit/test_config_validator.py
--rw-r--r--   0 bretterer   (501) staff       (20)     1273 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/tests/unit/test_jwt_utils.py
--rw-r--r--   0 bretterer   (501) staff       (20)    12278 2021-11-16 15:55:03.000000 okta_jwt_verifier-0.2.3/tests/unit/test_jwt_verifier.py
--rw-r--r--   0 bretterer   (501) staff       (20)     1583 2021-10-04 15:13:48.000000 okta_jwt_verifier-0.2.3/tests/unit/test_request_executor.py
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.648673 okta_jwt_verifier-0.2.4/
+-rw-r--r--   0 bretterer   (502) staff       (20)     9810 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/LICENSE.md
+-rw-r--r--   0 bretterer   (502) staff       (20)     1158 2023-05-03 14:05:02.648811 okta_jwt_verifier-0.2.4/PKG-INFO
+-rw-r--r--   0 bretterer   (502) staff       (20)     8471 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/README.md
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.642426 okta_jwt_verifier-0.2.4/okta_jwt_verifier/
+-rw-r--r--   0 bretterer   (502) staff       (20)      227 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/__init__.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     3550 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/config_validator.py
+-rw-r--r--   0 bretterer   (502) staff       (20)      788 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/constants.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     1698 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/error_messages.py
+-rw-r--r--   0 bretterer   (502) staff       (20)      230 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/exceptions.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     2874 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/jwt_utils.py
+-rw-r--r--   0 bretterer   (502) staff       (20)    15102 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/jwt_verifier.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     2002 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier/request_executor.py
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.644902 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/
+-rw-r--r--   0 bretterer   (502) staff       (20)     1158 2023-05-03 14:05:02.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/PKG-INFO
+-rw-r--r--   0 bretterer   (502) staff       (20)      738 2023-05-03 14:05:02.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/SOURCES.txt
+-rw-r--r--   0 bretterer   (502) staff       (20)        1 2023-05-03 14:05:02.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/dependency_links.txt
+-rw-r--r--   0 bretterer   (502) staff       (20)       41 2023-05-03 14:05:02.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/requires.txt
+-rw-r--r--   0 bretterer   (502) staff       (20)       24 2023-05-03 14:05:02.000000 okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/top_level.txt
+-rw-r--r--   0 bretterer   (502) staff       (20)      105 2023-05-03 14:05:02.649360 okta_jwt_verifier-0.2.4/setup.cfg
+-rw-r--r--   0 bretterer   (502) staff       (20)     1459 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/setup.py
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.636522 okta_jwt_verifier-0.2.4/tests/
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.645837 okta_jwt_verifier-0.2.4/tests/integration/
+-rw-r--r--   0 bretterer   (502) staff       (20)        0 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/integration/__init__.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     1867 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/integration/test_jwt_verifier.py
+drwxr-xr-x   0 bretterer   (502) staff       (20)        0 2023-05-03 14:05:02.648283 okta_jwt_verifier-0.2.4/tests/unit/
+-rw-r--r--   0 bretterer   (502) staff       (20)        0 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/unit/__init__.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     5558 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/unit/test_config_validator.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     1273 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/unit/test_jwt_utils.py
+-rw-r--r--   0 bretterer   (502) staff       (20)    12278 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/unit/test_jwt_verifier.py
+-rw-r--r--   0 bretterer   (502) staff       (20)     1583 2023-05-03 14:04:43.000000 okta_jwt_verifier-0.2.4/tests/unit/test_request_executor.py
```

### Comparing `okta_jwt_verifier-0.2.3/LICENSE.md` & `okta_jwt_verifier-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/PKG-INFO` & `okta_jwt_verifier-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: okta_jwt_verifier
-Version: 0.2.3
+Version: 0.2.4
 Summary: Okta JWT Verifier
 Home-page: https://github.com/okta/okta-jwt-verifier-python
 Author: Okta, Inc.
 Author-email: devex@okta.com
 License: Apache License 2.0
-Description: Okta JWT Verifier
-        =================
-        
-        A Python library for OKTA JWT tokens validation
-        
-        Getting Started
-        ---------------
-        ``` $ pip install okta-jwt-verifier ```
-        
-        Look for our quickstart guide here!
-        - https://github.com/okta/okta-jwt-verifier-python
-        
-        Okta Developer Forum
-        --------------------
-        
-        Find out more and look for help here: https://devforum.okta.com/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE.md
+
+Okta JWT Verifier
+=================
+
+A Python library for OKTA JWT tokens validation
+
+Getting Started
+---------------
+``` $ pip install okta-jwt-verifier ```
+
+Look for our quickstart guide here!
+- https://github.com/okta/okta-jwt-verifier-python
+
+Okta Developer Forum
+--------------------
+
+Find out more and look for help here: https://devforum.okta.com/
```

### Comparing `okta_jwt_verifier-0.2.3/README.md` & `okta_jwt_verifier-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/config_validator.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/config_validator.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/constants.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/constants.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/error_messages.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/error_messages.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/jwt_utils.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/jwt_verifier.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/jwt_verifier.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier/request_executor.py` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier/request_executor.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/PKG-INFO` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: okta-jwt-verifier
-Version: 0.2.3
+Version: 0.2.4
 Summary: Okta JWT Verifier
 Home-page: https://github.com/okta/okta-jwt-verifier-python
 Author: Okta, Inc.
 Author-email: devex@okta.com
 License: Apache License 2.0
-Description: Okta JWT Verifier
-        =================
-        
-        A Python library for OKTA JWT tokens validation
-        
-        Getting Started
-        ---------------
-        ``` $ pip install okta-jwt-verifier ```
-        
-        Look for our quickstart guide here!
-        - https://github.com/okta/okta-jwt-verifier-python
-        
-        Okta Developer Forum
-        --------------------
-        
-        Find out more and look for help here: https://devforum.okta.com/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE.md
+
+Okta JWT Verifier
+=================
+
+A Python library for OKTA JWT tokens validation
+
+Getting Started
+---------------
+``` $ pip install okta-jwt-verifier ```
+
+Look for our quickstart guide here!
+- https://github.com/okta/okta-jwt-verifier-python
+
+Okta Developer Forum
+--------------------
+
+Find out more and look for help here: https://devforum.okta.com/
```

### Comparing `okta_jwt_verifier-0.2.3/okta_jwt_verifier.egg-info/SOURCES.txt` & `okta_jwt_verifier-0.2.4/okta_jwt_verifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/setup.py` & `okta_jwt_verifier-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=[
         "acachecontrol",
         "aiohttp",
         "python-jose",
-        "retry"
+        "retry2"
     ]
 )
```

### Comparing `okta_jwt_verifier-0.2.3/tests/integration/test_jwt_verifier.py` & `okta_jwt_verifier-0.2.4/tests/integration/test_jwt_verifier.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/tests/unit/test_config_validator.py` & `okta_jwt_verifier-0.2.4/tests/unit/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/tests/unit/test_jwt_utils.py` & `okta_jwt_verifier-0.2.4/tests/unit/test_jwt_utils.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/tests/unit/test_jwt_verifier.py` & `okta_jwt_verifier-0.2.4/tests/unit/test_jwt_verifier.py`

 * *Files identical despite different names*

### Comparing `okta_jwt_verifier-0.2.3/tests/unit/test_request_executor.py` & `okta_jwt_verifier-0.2.4/tests/unit/test_request_executor.py`

 * *Files identical despite different names*

