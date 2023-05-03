# Comparing `tmp/vin_decoder_nhtsa-0.0.1.tar.gz` & `tmp/vin_decoder_nhtsa-0.0.2.tar.gz`

## Comparing `vin_decoder_nhtsa-0.0.1.tar` & `vin_decoder_nhtsa-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/setup.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/src/vin_decoder_nhtsa/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/src/vin_decoder_nhtsa/decoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/tests/test_decoder.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/LICENSE
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/setup.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/src/vin_decoder_nhtsa/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/src/vin_decoder_nhtsa/decoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/tests/test_decoder.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/LICENSE
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 vin_decoder_nhtsa-0.0.2/PKG-INFO
```

### Comparing `vin_decoder_nhtsa-0.0.1/.github/workflows/publish-pypi.yml` & `vin_decoder_nhtsa-0.0.2/.github/workflows/publish-pypi.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 name: Publish to PyPi
 
-on:
-  pull_request:
+on:  
+  push:
+    tags:
+      - '*'
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
@@ -17,11 +19,10 @@
       - name: Build package
         run: |
           python3 -m build
       
       - name: Upload package
         env:
           TWINE_USERNAME: __token__
-          # TWINE_PASSWORD: ${{ secrets.TEST_PYPI_TOKEN }}
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
           python3 -m twine upload --repository pypi dist/*
```

### Comparing `vin_decoder_nhtsa-0.0.1/src/vin_decoder_nhtsa/decoder.py` & `vin_decoder_nhtsa-0.0.2/src/vin_decoder_nhtsa/decoder.py`

 * *Files identical despite different names*

### Comparing `vin_decoder_nhtsa-0.0.1/LICENSE` & `vin_decoder_nhtsa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vin_decoder_nhtsa-0.0.1/pyproject.toml` & `vin_decoder_nhtsa-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vin_decoder_nhtsa"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alex Conrey", email="alex@conrey.engineering" },
 ]
 description = "Python module for decoding VIN metadata from NHTSA API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vin_decoder_nhtsa-0.0.1/PKG-INFO` & `vin_decoder_nhtsa-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vin_decoder_nhtsa
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python module for decoding VIN metadata from NHTSA API
 Project-URL: Homepage, https://github.com/conrey-engineering/python_vin_decoder_nhtsa
 Project-URL: Bug Tracker, https://github.com/conrey-engineering/python_vin_decoder_nhtsa/issues
 Author-email: Alex Conrey <alex@conrey.engineering>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

