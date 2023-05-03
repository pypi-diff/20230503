# Comparing `tmp/numbers-c2pa-0.0.3.tar.gz` & `tmp/numbers-c2pa-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-5xsw33ey/numbers-c2pa-0.0.3.tar", last modified: Sun Apr 23 18:23:09 2023, max compression
+gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-7x0w56jv/numbers-c2pa-0.0.4.tar", last modified: Wed May  3 06:40:59 2023, max compression
```

## Comparing `numbers-c2pa-0.0.3.tar` & `numbers-c2pa-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/src/numbers_c2pa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:23:08.000000 numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:23:09.000000 numbers-c2pa-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 18:22:57.000000 numbers-c2pa-0.0.3/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/src/numbers_c2pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/src/numbers_c2pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/src/numbers_c2pa/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/src/numbers_c2pa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:59.000000 numbers-c2pa-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 06:40:41.000000 numbers-c2pa-0.0.4/tests/test_core.py
```

### Comparing `numbers-c2pa-0.0.3/LICENSE` & `numbers-c2pa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.3/PKG-INFO` & `numbers-c2pa-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numbers-c2pa-0.0.3/README.md` & `numbers-c2pa-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.3/setup.cfg` & `numbers-c2pa-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = numbers-c2pa
-version = 0.0.3
+version = 0.0.4
 author = Numbers Co., Inc
 author_email = dev@numbersprotocol.io
 description = Numbers C2PA tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = authenticity
 url = https://github.com/numbersprotocol/numbers-c2pa
```

### Comparing `numbers-c2pa-0.0.3/src/numbers_c2pa/core.py` & `numbers-c2pa-0.0.4/src/numbers_c2pa/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import mimetypes
 import os
 import subprocess
 from datetime import datetime
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from typing import Any, Dict, Optional
 
+from .exceptions import NoClaimFound, UnknownError
+
 
 def _mimetype_to_ext(asset_mime_type: str):
     ext = mimetypes.guess_extension(asset_mime_type)
     if not ext:
         raise ValueError(f'Could not find a file extension for MIME type: {asset_mime_type}')
     return ext
 
@@ -87,20 +89,24 @@
         if private_key:
             env_vars['C2PA_PRIVATE_KEY'] = private_key
         if sign_cert:
             env_vars['C2PA_SIGN_CERT'] = sign_cert
         command = f'c2patool {asset_file} -m {manifest_file} -o {asset_c2pa_file}'
         if force_overwrite:
             command += ' -f'
-        subprocess.run(
-            command,
-            shell=True,
-            env=env_vars,
-            check=True,
-        )
+        try:
+            subprocess.run(
+                command,
+                shell=True,
+                env=env_vars,
+                check=True,
+                stderr=subprocess.PIPE,
+            )
+        except subprocess.CalledProcessError as e:
+            raise UnknownError(e.stderr)
 
         with open(asset_c2pa_file, 'rb') as f:
             asset_c2pa_bytes = f.read()
         return asset_c2pa_bytes
 
 
 def inject_file(
@@ -121,33 +127,49 @@
         if private_key:
             env_vars['C2PA_PRIVATE_KEY'] = private_key
         if sign_cert:
             env_vars['C2PA_SIGN_CERT'] = sign_cert
         command = f'c2patool {asset_file} -m {manifest_temp_file.name} -o {c2pa_output_file}'
         if force_overwrite:
             command += ' -f'
-        subprocess.run(
-            command,
-            shell=True,
-            env=env_vars,
-            check=True,
-        )
+        try:
+            subprocess.run(
+                command,
+                shell=True,
+                env=env_vars,
+                check=True,
+                stderr=subprocess.PIPE,
+            )
+        except subprocess.CalledProcessError as e:
+            raise UnknownError(e.stderr)
 
 
 def read_c2pa(asset_c2pa_bytes: bytes, asset_mime_type: str):
     file_ext = _mimetype_to_ext(asset_mime_type)
     with TemporaryDirectory(prefix='temp_dir') as temp_dir:
         asset_c2pa_file = os.path.join(temp_dir, f'asset-c2pa.{file_ext}')
         with open(asset_c2pa_file, 'wb') as f:
             f.write(asset_c2pa_bytes)
 
-        command = ['c2patool', asset_c2pa_file]
-        output = subprocess.check_output(command, text=True)
-        json_output = json.loads(output)
-        return json_output
+        try:
+            command = ['c2patool', asset_c2pa_file]
+            output = subprocess.check_output(command, text=True, stderr=subprocess.PIPE)
+            json_output = json.loads(output)
+            return json_output
+        except subprocess.CalledProcessError as e:
+            if 'No claim found' in e.stderr:
+                raise NoClaimFound
+            else:
+                raise UnknownError(e.stderr)
 
 
 def read_c2pa_file(c2pa_file: str):
     command = ['c2patool', c2pa_file]
-    output = subprocess.check_output(command, text=True)
-    json_output = json.loads(output)
-    return json_output
+    try:
+        output = subprocess.check_output(command, text=True, stderr=subprocess.PIPE)
+        json_output = json.loads(output)
+        return json_output
+    except subprocess.CalledProcessError as e:
+        if 'No claim found' in e.stderr:
+            raise NoClaimFound
+        else:
+            raise UnknownError(e.stderr)
```

### Comparing `numbers-c2pa-0.0.3/src/numbers_c2pa/utils.py` & `numbers-c2pa-0.0.4/src/numbers_c2pa/utils.py`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.3/src/numbers_c2pa.egg-info/PKG-INFO` & `numbers-c2pa-0.0.4/src/numbers_c2pa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

