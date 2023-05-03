# Comparing `tmp/amps-py-0.1.3.tar.gz` & `tmp/amps-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amps-py-0.1.3.tar", last modified: Tue Apr 18 03:12:22 2023, max compression
+gzip compressed data, was "amps-py-0.1.4.tar", last modified: Wed May  3 19:41:11 2023, max compression
```

## Comparing `amps-py-0.1.3.tar` & `amps-py-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.435683 amps-py-0.1.3/
--rw-r--r--   0 abhayram   (501) staff       (20)     1074 2023-04-13 22:49:51.000000 amps-py-0.1.3/LICENSE
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-04-18 03:12:22.435774 amps-py-0.1.3/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      314 2023-04-13 22:49:51.000000 amps-py-0.1.3/README.md
--rw-r--r--   0 abhayram   (501) staff       (20)       84 2023-04-13 22:49:51.000000 amps-py-0.1.3/pyproject.toml
--rw-r--r--   0 abhayram   (501) staff       (20)      638 2023-04-18 03:12:22.436124 amps-py-0.1.3/setup.cfg
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.433386 amps-py-0.1.3/src/
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.434273 amps-py-0.1.3/src/amps/
--rw-r--r--   0 abhayram   (501) staff       (20)    35433 2023-04-17 04:58:50.000000 amps-py-0.1.3/src/amps/__init__.py
-drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-04-18 03:12:22.435512 amps-py-0.1.3/src/amps_py.egg-info/
--rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/PKG-INFO
--rw-r--r--   0 abhayram   (501) staff       (20)      203 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/SOURCES.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        1 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/dependency_links.txt
--rw-r--r--   0 abhayram   (501) staff       (20)        5 2023-04-18 03:12:22.000000 amps-py-0.1.3/src/amps_py.egg-info/top_level.txt
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 19:41:11.300265 amps-py-0.1.4/
+-rw-r--r--   0 abhayram   (501) staff       (20)     1074 2023-04-13 22:49:51.000000 amps-py-0.1.4/LICENSE
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-03 19:41:11.300414 amps-py-0.1.4/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      314 2023-04-13 22:49:51.000000 amps-py-0.1.4/README.md
+-rw-r--r--   0 abhayram   (501) staff       (20)       84 2023-04-13 22:49:51.000000 amps-py-0.1.4/pyproject.toml
+-rw-r--r--   0 abhayram   (501) staff       (20)      638 2023-05-03 19:41:11.302563 amps-py-0.1.4/setup.cfg
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 19:41:11.297096 amps-py-0.1.4/src/
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 19:41:11.298527 amps-py-0.1.4/src/amps/
+-rw-r--r--   0 abhayram   (501) staff       (20)    35476 2023-05-03 19:19:25.000000 amps-py-0.1.4/src/amps/__init__.py
+drwxr-xr-x   0 abhayram   (501) staff       (20)        0 2023-05-03 19:41:11.300102 amps-py-0.1.4/src/amps_py.egg-info/
+-rw-r--r--   0 abhayram   (501) staff       (20)      828 2023-05-03 19:41:11.000000 amps-py-0.1.4/src/amps_py.egg-info/PKG-INFO
+-rw-r--r--   0 abhayram   (501) staff       (20)      203 2023-05-03 19:41:11.000000 amps-py-0.1.4/src/amps_py.egg-info/SOURCES.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        1 2023-05-03 19:41:11.000000 amps-py-0.1.4/src/amps_py.egg-info/dependency_links.txt
+-rw-r--r--   0 abhayram   (501) staff       (20)        5 2023-05-03 19:41:11.000000 amps-py-0.1.4/src/amps_py.egg-info/top_level.txt
```

### Comparing `amps-py-0.1.3/LICENSE` & `amps-py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amps-py-0.1.3/PKG-INFO` & `amps-py-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amps-py-0.1.3/setup.cfg` & `amps-py-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amps-py
-version = 0.1.3
+version = 0.1.4
 author = Abhay Ram
 author_email = abhayram@hub4edi.com
 description = Package for Interfacing with AMPS from Agile Data Inc.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mftlabs.github.io/amps-py
 project_urls =
```

### Comparing `amps-py-0.1.3/src/amps/__init__.py` & `amps-py-0.1.4/src/amps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,21 +139,22 @@
         self.log("error", message)
 
 
 class DB:
     def __init__(self, env):
         self.env = env
 
-    def find(self, collection, clauses):
+    def find(self, collection, clauses={}, opts={}):
         coll = bytes(collection, "utf-8")
         collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
             b'index'), [bytes(self.env, "utf-8"), coll])
         clauses = Map(clauses)
+        opts = Map(opts)
         result = call(Atom(b'Elixir.Amps.PyService'),
-                      Atom(b'find'), [collection, clauses])
+                      Atom(b'find'), [collection, clauses, opts])
         return Util.unravel_erlport_object(result)
 
     def find_one(self, collection, clauses):
         coll = bytes(collection, "utf-8")
         collection = call(Atom(b'Elixir.AmpsUtil'), Atom(
             b'index'), [bytes(self.env, "utf-8"), coll])
         clauses = Map(clauses)
```

### Comparing `amps-py-0.1.3/src/amps_py.egg-info/PKG-INFO` & `amps-py-0.1.4/src/amps_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amps-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for Interfacing with AMPS from Agile Data Inc.
 Home-page: https://mftlabs.github.io/amps-py
 Author: Abhay Ram
 Author-email: abhayram@hub4edi.com
 Project-URL: Bug Tracker, https://github.com/mftlabs/amps-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

