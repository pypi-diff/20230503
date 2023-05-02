# Comparing `tmp/tap-rest-api-msdk-1.0.0.tar.gz` & `tmp/tap_rest_api_msdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-rest-api-msdk-1.0.0.tar", max compression
+gzip compressed data, was "tap_rest_api_msdk-1.1.1.tar", max compression
```

## Comparing `tap-rest-api-msdk-1.0.0.tar` & `tap_rest_api_msdk-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2021-10-20 17:57:42.088969 tap-rest-api-msdk-1.0.0/LICENSE
--rw-r--r--   0        0        0     1188 2022-02-18 22:57:36.287852 tap-rest-api-msdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       30 2022-02-18 17:35:28.062956 tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/__init__.py
--rw-r--r--   0        0        0      506 2022-02-18 17:35:28.063321 tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/client.py
--rw-r--r--   0        0        0     7676 2022-02-18 17:35:28.063704 tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/streams.py
--rw-r--r--   0        0        0    10590 2022-02-18 22:19:55.752464 tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/tap.py
--rw-r--r--   0        0        0     1969 2022-02-18 17:35:28.064447 tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/utils.py
--rw-r--r--   0        0        0      972 2022-02-18 23:01:48.963759 tap-rest-api-msdk-1.0.0/setup.py
--rw-r--r--   0        0        0      830 2022-02-18 23:01:48.964027 tap-rest-api-msdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 22:03:43.097034 tap_rest_api_msdk-1.1.1/LICENSE
+-rw-r--r--   0        0        0     8564 2023-05-02 22:03:43.097034 tap_rest_api_msdk-1.1.1/README.md
+-rw-r--r--   0        0        0     1209 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/__init__.py
+-rw-r--r--   0        0        0      506 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/client.py
+-rw-r--r--   0        0        0     7676 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/streams.py
+-rw-r--r--   0        0        0    10590 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/tap.py
+-rw-r--r--   0        0        0     1969 2023-05-02 22:03:43.101034 tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/utils.py
+-rw-r--r--   0        0        0     9760 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.1.1/setup.py
+-rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 tap_rest_api_msdk-1.1.1/PKG-INFO
```

### Comparing `tap-rest-api-msdk-1.0.0/LICENSE` & `tap_rest_api_msdk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-rest-api-msdk-1.0.0/pyproject.toml` & `tap_rest_api_msdk-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "tap-rest-api-msdk"
-version = "1.0.0"
+version = "1.1.1"
 description = "`tap-rest-api-msdk` is a Singer tap for REST APIs, built with the Meltano SDK for Singer Taps."
 authors = ["Josh Lloyd", "Fred Reimer"]
 keywords = [
     "ELT",
     "rest-api-msdk",
     "Meltano",
     "Singer",
     "REST",
     "API",
     "tap"
 ]
 license = "Apache 2.0"
 homepage = "https://github.com/Widen/tap-rest-api-msdk"
 repository = "https://github.com/Widen/tap-rest-api-msdk"
+readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "<3.10,>=3.6.2"
+python = "<3.10,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = "^0.3.11"
+singer-sdk = "^0.26.0"
 genson = "^1.2.2"
 atomicwrites = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 tox = "^3.24.4"
 flake8 = "^3.9.2"
```

### Comparing `tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/streams.py` & `tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/streams.py`

 * *Files identical despite different names*

### Comparing `tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/tap.py` & `tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/tap.py`

 * *Files identical despite different names*

### Comparing `tap-rest-api-msdk-1.0.0/tap_rest_api_msdk/utils.py` & `tap_rest_api_msdk-1.1.1/tap_rest_api_msdk/utils.py`

 * *Files identical despite different names*

