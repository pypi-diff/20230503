# Comparing `tmp/uw-saml-1.2.0.tar.gz` & `tmp/uw_saml-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw-saml-1.2.0.tar", max compression
+gzip compressed data, was "uw_saml-1.2.1.tar", max compression
```

## Comparing `uw-saml-1.2.0.tar` & `uw_saml-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      564 2022-05-19 15:35:03.434567 uw-saml-1.2.0/LICENSE
--rw-r--r--   0        0        0      606 2022-05-19 15:35:03.434567 uw-saml-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       53 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/VERSION
--rw-r--r--   0        0        0       70 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/__init__.py
--rw-r--r--   0        0        0     3221 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/auth.py
--rw-r--r--   0        0        0      389 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/idp/__init__.py
--rw-r--r--   0        0        0     1619 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/idp/attribute.py
--rw-r--r--   0        0        0     9896 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/idp/federated.py
--rw-r--r--   0        0        0     2589 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/idp/uw.py
--rw-r--r--   0        0        0     1538 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/mock.py
--rw-r--r--   0        0        0      279 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/python3_saml.py
--rw-r--r--   0        0        0     2302 2022-05-19 15:35:03.438567 uw-saml-1.2.0/uw_saml2/sp.py
--rw-r--r--   0        0        0      785 2022-05-19 15:36:19.040390 uw-saml-1.2.0/setup.py
--rw-r--r--   0        0        0      680 2022-05-19 15:36:19.040696 uw-saml-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      564 2023-05-03 21:52:56.227831 uw_saml-1.2.1/LICENSE
+-rw-r--r--   0        0        0      606 2023-05-03 21:52:56.227831 uw_saml-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/VERSION
+-rw-r--r--   0        0        0       70 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/__init__.py
+-rw-r--r--   0        0        0     3221 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/auth.py
+-rw-r--r--   0        0        0      389 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/attribute.py
+-rw-r--r--   0        0        0     9896 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/federated.py
+-rw-r--r--   0        0        0     2589 2023-05-03 21:52:56.227831 uw_saml-1.2.1/uw_saml2/idp/uw.py
+-rw-r--r--   0        0        0     1538 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/mock.py
+-rw-r--r--   0        0        0      279 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/python3_saml.py
+-rw-r--r--   0        0        0     2302 2023-05-03 21:52:56.231831 uw_saml-1.2.1/uw_saml2/sp.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.1/PKG-INFO
```

### Comparing `uw-saml-1.2.0/LICENSE` & `uw_saml-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/pyproject.toml` & `uw_saml-1.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uw-saml"
-version = "1.2.0"
+version = "1.2.1"
 description = "A UW-specific adapter to the python3-saml package."
 authors = []
 license = "Apache 2.0"
 packages = [
     { include = 'uw_saml2' }
 ]
```

### Comparing `uw-saml-1.2.0/uw_saml2/auth.py` & `uw_saml-1.2.1/uw_saml2/auth.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/uw_saml2/idp/attribute.py` & `uw_saml-1.2.1/uw_saml2/idp/attribute.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/uw_saml2/idp/federated.py` & `uw_saml-1.2.1/uw_saml2/idp/federated.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/uw_saml2/idp/uw.py` & `uw_saml-1.2.1/uw_saml2/idp/uw.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/uw_saml2/mock.py` & `uw_saml-1.2.1/uw_saml2/mock.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/uw_saml2/sp.py` & `uw_saml-1.2.1/uw_saml2/sp.py`

 * *Files identical despite different names*

### Comparing `uw-saml-1.2.0/PKG-INFO` & `uw_saml-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: uw-saml
-Version: 1.2.0
+Version: 1.2.1
 Summary: A UW-specific adapter to the python3-saml package.
 License: Apache 2.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: python3-saml
 Requires-Dist: Werkzeug (>=2.0.2,<3.0.0)
 Requires-Dist: cachelib (>=0.4.1,<0.5.0)
 Requires-Dist: onelogin (>=2.0.3,<3.0.0)
-Requires-Dist: python3-saml (>=1.14.0,<2.0.0); extra == "python3-saml"
+Requires-Dist: python3-saml (>=1.14.0,<2.0.0) ; extra == "python3-saml"
```

