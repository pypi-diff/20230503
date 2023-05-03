# Comparing `tmp/visualblocks-0.0.3.tar.gz` & `tmp/visualblocks-0.0.4.tar.gz`

## Comparing `visualblocks-0.0.3.tar` & `visualblocks-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.3/.editorconfig
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visualblocks-0.0.3/src/visualblocks/__init__.py
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 visualblocks-0.0.3/src/visualblocks/server.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.3/.gitignore
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.3/README.pypi.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.4/.editorconfig
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visualblocks-0.0.4/src/visualblocks/__init__.py
+-rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 visualblocks-0.0.4/src/visualblocks/server.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.4/README.pypi.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.4/PKG-INFO
```

### Comparing `visualblocks-0.0.3/src/visualblocks/server.py` & `visualblocks-0.0.4/src/visualblocks/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import shutil
 import sys
 import threading
 import traceback
 import urllib.parse
 import zipfile
 
-_VISUAL_BLOCKS_BUNDLE_VERSION = '1683083994'
+_VISUAL_BLOCKS_BUNDLE_VERSION = '1683086528'
 
 # Disable logging from werkzeug.
 #
 # Without this, flask will show a warning about using dev server (which is OK
 # in our usecase).
 logging.getLogger('werkzeug').disabled = True
```

### Comparing `visualblocks-0.0.3/README.pypi.md` & `visualblocks-0.0.4/README.pypi.md`

 * *Files identical despite different names*

### Comparing `visualblocks-0.0.3/pyproject.toml` & `visualblocks-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visualblocks"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "Visual Blocks for Google Colaboratory"
 readme = "README.pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `visualblocks-0.0.3/PKG-INFO` & `visualblocks-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualblocks
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visual Blocks for Google Colaboratory
 Project-URL: Homepage, https://github.com/google/visualblocks
 Project-URL: Bug Tracker, https://github.com/google/visualblocks/issues
 Author-email: Google LLC <opensource@google.com>
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

