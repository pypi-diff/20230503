# Comparing `tmp/vector2dggs-0.3.0.tar.gz` & `tmp/vector2dggs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.3.0.tar", max compression
+gzip compressed data, was "vector2dggs-0.3.1.tar", max compression
```

## Comparing `vector2dggs-0.3.0.tar` & `vector2dggs-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7920 2023-05-02 23:30:42.832416 vector2dggs-0.3.0/README.md
--rw-r--r--   0        0        0     1092 2023-05-02 23:30:48.748444 vector2dggs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/cli.py
--rw-r--r--   0        0        0     9405 2023-04-28 03:53:55.148450 vector2dggs-0.3.0/vector2dggs/h3.py
--rw-r--r--   0        0        0     3074 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/katana.py
--rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7920 2023-05-03 01:16:48.563418 vector2dggs-0.3.1/README.md
+-rw-r--r--   0        0        0     1092 2023-05-03 01:16:53.215440 vector2dggs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/cli.py
+-rw-r--r--   0        0        0     9399 2023-05-03 01:16:28.111317 vector2dggs-0.3.1/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3074 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.3.1/PKG-INFO
```

### Comparing `vector2dggs-0.3.0/README.md` & `vector2dggs-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.0},
+  version={0.3.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.3.0/pyproject.toml` & `vector2dggs-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.3.0"
+version = "0.3.1"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.3.0/vector2dggs/cli.py` & `vector2dggs-0.3.1/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.0/vector2dggs/h3.py` & `vector2dggs-0.3.1/vector2dggs/h3.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     Ingest a vector dataset and index it to the H3 DGGS.
 
     VECTOR_INPUT is the path to input vector geospatial data.
     OUTPUT_DIRECTORY should be a directory, not a file or database table, as it willinstead be the write location for an Apache Parquet data store.
     """
     con: sqlalchemy.engine.Connection = None
     scheme: str = urlparse(vector_input).scheme
-    if scheme is not None and scheme != "file":
+    if bool(scheme) and scheme != "file":
         # Assume database connection
         con = sqlalchemy.create_engine(vector_input)
     elif not Path(vector_input).exists():
         if not scheme:
             LOGGER.warning(
                 f"Input vector {vector_input} does not exist, and is not recognised as a remote URI"
             )
```

### Comparing `vector2dggs-0.3.0/vector2dggs/katana.py` & `vector2dggs-0.3.1/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.0/PKG-INFO` & `vector2dggs-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -183,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.0},
+  version={0.3.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

