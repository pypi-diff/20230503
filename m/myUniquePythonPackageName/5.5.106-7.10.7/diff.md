# Comparing `tmp/myUniquePythonPackageName-5.5.106.tar.gz` & `tmp/myUniquePythonPackageName-7.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myUniquePythonPackageName-5.5.106.tar", last modified: Thu Apr 20 10:39:49 2023, max compression
+gzip compressed data, was "myUniquePythonPackageName-7.10.7.tar", last modified: Fri Mar 31 12:05:44 2023, max compression
```

## Comparing `myUniquePythonPackageName-5.5.106.tar` & `myUniquePythonPackageName-7.10.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.127669 myUniquePythonPackageName-5.5.106/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-20 10:39:49.127669 myUniquePythonPackageName-5.5.106/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2858 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.107669 myUniquePythonPackageName-5.5.106/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.109669 myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.110669 myUniquePythonPackageName-5.5.106/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.118669 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.120669 myUniquePythonPackageName-5.5.106/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.123669 myUniquePythonPackageName-5.5.106/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/apimaticcalculator/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:39:49.127669 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-20 10:39:49.000000 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 10:39:49.000000 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:39:49.000000 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 10:39:49.000000 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-20 10:39:49.000000 myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-20 10:39:21.000000 myUniquePythonPackageName-5.5.106/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-20 10:39:49.128669 myUniquePythonPackageName-5.5.106/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.125621 myUniquePythonPackageName-7.10.7/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      244 2023-03-31 12:05:44.126621 myUniquePythonPackageName-7.10.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.102621 myUniquePythonPackageName-7.10.7/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.108621 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.111621 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.115621 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.117621 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.120621 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/apimaticcalculator/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:05:44.125621 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-03-31 12:05:44.000000 myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      592 2023-03-31 12:05:12.000000 myUniquePythonPackageName-7.10.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-03-31 12:05:44.127621 myUniquePythonPackageName-7.10.7/setup.cfg
```

### Comparing `myUniquePythonPackageName-5.5.106/LICENSE` & `myUniquePythonPackageName-7.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/api_helper.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/apimaticcalculator_client.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/configuration.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/base_controller.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/controllers/simple_calculator_controller.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/exceptions/api_exception.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_request.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/http/http_response.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/apimaticcalculator/models/operation_type_enum.py` & `myUniquePythonPackageName-7.10.7/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/myUniquePythonPackageName.egg-info/SOURCES.txt` & `myUniquePythonPackageName-7.10.7/myUniquePythonPackageName.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-5.5.106/pyproject.toml` & `myUniquePythonPackageName-7.10.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "myUniquePythonPackageName"
 description = "Simple calculator API hosted on APIMATIC"
-version = "5.5.106"
+version = "7.10.7"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "RandomPerson", email = "randomEmail@testing.com"}]
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
-testutils = ["pytest>=7.2.2"]
+testutils = ["pytest>=7.1.3"]
```

