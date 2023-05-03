# Comparing `tmp/httpx-gssapi-0.1.7.tar.gz` & `tmp/httpx-gssapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx-gssapi-0.1.7.tar", last modified: Tue May 24 06:33:31 2022, max compression
+gzip compressed data, was "httpx-gssapi-0.2.tar", last modified: Wed May  3 04:27:50 2023, max compression
```

## Comparing `httpx-gssapi-0.1.7.tar` & `httpx-gssapi-0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12602 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8604 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/httpx_gssapi/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/httpx_gssapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/httpx_gssapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/httpx_gssapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11519 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/httpx_gssapi/gssapi_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12602 2022-05-24 06:33:30.000000 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-05-24 06:33:31.000000 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 06:33:31.000000 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-24 06:33:31.000000 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-24 06:33:31.000000 httpx-gssapi-0.1.7/httpx_gssapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-05-24 06:33:31.565090 httpx-gssapi-0.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      494 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-05-24 06:33:23.000000 httpx-gssapi-0.1.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/httpx_gssapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/httpx_gssapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/httpx_gssapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/httpx_gssapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/httpx_gssapi/gssapi_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/httpx_gssapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-03 04:27:50.000000 httpx-gssapi-0.2/httpx_gssapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-03 04:27:50.000000 httpx-gssapi-0.2/httpx_gssapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:27:50.000000 httpx-gssapi-0.2/httpx_gssapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 04:27:50.000000 httpx-gssapi-0.2/httpx_gssapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 04:27:50.000000 httpx-gssapi-0.2/httpx_gssapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:27:50.939134 httpx-gssapi-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/tests/test_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-03 04:27:45.000000 httpx-gssapi-0.2/versioneer.py
```

### Comparing `httpx-gssapi-0.1.7/HISTORY.rst` & `httpx-gssapi-0.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/LICENSE` & `httpx-gssapi-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/PKG-INFO` & `httpx-gssapi-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: httpx-gssapi
-Version: 0.1.7
+Version: 0.2
 Summary: A Python GSSAPI authentication handler for HTTPX
 Home-page: https://github.com/pythongssapi/httpx-gssapi
 Author: Ian Cordasco, Cory Benfield, Michael Komitee, Robbie Harwood, Roger Aiudi
 Author-email: aiudirog@gmail.com
 License: MIT
 Keywords: httpx,gssapi,kerberos
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 HTTPX GSSAPI authentication library
```

### Comparing `httpx-gssapi-0.1.7/README.rst` & `httpx-gssapi-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/httpx_gssapi/__init__.py` & `httpx-gssapi-0.2/httpx_gssapi/__init__.py`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/httpx_gssapi/exceptions.py` & `httpx-gssapi-0.2/httpx_gssapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/httpx_gssapi/gssapi_.py` & `httpx-gssapi-0.2/httpx_gssapi/gssapi_.py`

 * *Files identical despite different names*

### Comparing `httpx-gssapi-0.1.7/httpx_gssapi.egg-info/PKG-INFO` & `httpx-gssapi-0.2/httpx_gssapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: httpx-gssapi
-Version: 0.1.7
+Version: 0.2
 Summary: A Python GSSAPI authentication handler for HTTPX
 Home-page: https://github.com/pythongssapi/httpx-gssapi
 Author: Ian Cordasco, Cory Benfield, Michael Komitee, Robbie Harwood, Roger Aiudi
 Author-email: aiudirog@gmail.com
 License: MIT
 Keywords: httpx,gssapi,kerberos
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS
 
 HTTPX GSSAPI authentication library
```

### Comparing `httpx-gssapi-0.1.7/setup.cfg` & `httpx-gssapi-0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 author_email = aiudirog@gmail.com
 url = https://github.com/pythongssapi/httpx-gssapi
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: ISC License (ISCL)
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 keywords = 
 	httpx
 	gssapi
 	kerberos
 
 [options]
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
 packages = httpx_gssapi
 install_requires = 
-	httpx>=0.16,<0.24
+	httpx>=0.16,<0.25
 	gssapi
 
 [options.extras_require]
 test = 
 	pytest
 	k5test
 all =
```

### Comparing `httpx-gssapi-0.1.7/versioneer.py` & `httpx-gssapi-0.2/versioneer.py`

 * *Files identical despite different names*

