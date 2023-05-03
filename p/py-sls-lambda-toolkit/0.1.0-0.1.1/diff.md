# Comparing `tmp/py-sls-lambda-toolkit-0.1.0.tar.gz` & `tmp/py-sls-lambda-toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sls-lambda-toolkit-0.1.0.tar", last modified: Wed May  3 16:17:30 2023, max compression
+gzip compressed data, was "py-sls-lambda-toolkit-0.1.1.tar", last modified: Wed May  3 16:21:16 2023, max compression
```

## Comparing `py-sls-lambda-toolkit-0.1.0.tar` & `py-sls-lambda-toolkit-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:17:30.069655 py-sls-lambda-toolkit-0.1.0/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.1.0/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.1.0/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-03 16:17:30.069655 py-sls-lambda-toolkit-0.1.0/PKG-INFO
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:17:30.069655 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/
--rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      584 2023-05-03 16:03:44.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/crypto.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/http_event.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-28 14:57:53.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/http_response.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/logger.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/mappers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/parsers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/status_code.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/validators.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:17:30.069655 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-03 16:17:30.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      669 2023-05-03 16:17:30.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-05-03 16:17:30.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       58 2023-05-03 16:17:30.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-05-03 16:17:30.000000 py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.1.0/pyproject.toml
--rw-rw-r--   0 julio     (1000) julio     (1000)      952 2023-05-03 16:17:30.069655 py-sls-lambda-toolkit-0.1.0/setup.cfg
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:21:16.972370 py-sls-lambda-toolkit-0.1.1/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.1.1/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.1.1/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-03 16:21:16.972370 py-sls-lambda-toolkit-0.1.1/PKG-INFO
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:21:16.968370 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/http_event.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-28 14:57:53.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/http_response.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/logger.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/mappers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/parsers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      584 2023-05-03 16:03:44.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/password.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/status_code.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/validators.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-03 16:21:16.972370 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-03 16:21:16.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      671 2023-05-03 16:21:16.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-05-03 16:21:16.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       58 2023-05-03 16:21:16.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-05-03 16:21:16.000000 py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.1.1/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)      952 2023-05-03 16:21:16.972370 py-sls-lambda-toolkit-0.1.1/setup.cfg
```

### Comparing `py-sls-lambda-toolkit-0.1.0/LICENSE` & `py-sls-lambda-toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/PKG-INFO` & `py-sls-lambda-toolkit-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/crypto.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/password.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/http_event.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/http_response.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/mappers.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/parsers.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/status_code.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit/validators.py` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/PKG-INFO` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.1.0/py_sls_lambda_toolkit.egg-info/SOURCES.txt` & `py-sls-lambda-toolkit-0.1.1/py_sls_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
 setup.cfg
 py_sls_lambda_toolkit/__init__.py
-py_sls_lambda_toolkit/crypto.py
 py_sls_lambda_toolkit/dynamodb_shortcuts.py
 py_sls_lambda_toolkit/http_event.py
 py_sls_lambda_toolkit/http_response.py
 py_sls_lambda_toolkit/logger.py
 py_sls_lambda_toolkit/mappers.py
 py_sls_lambda_toolkit/parsers.py
+py_sls_lambda_toolkit/password.py
 py_sls_lambda_toolkit/scan_filter_builder.py
 py_sls_lambda_toolkit/status_code.py
 py_sls_lambda_toolkit/validators.py
 py_sls_lambda_toolkit.egg-info/PKG-INFO
 py_sls_lambda_toolkit.egg-info/SOURCES.txt
 py_sls_lambda_toolkit.egg-info/dependency_links.txt
 py_sls_lambda_toolkit.egg-info/requires.txt
```

### Comparing `py-sls-lambda-toolkit-0.1.0/setup.cfg` & `py-sls-lambda-toolkit-0.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-sls-lambda-toolkit
-version = 0.1.0
+version = 0.1.1
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
```

