# Comparing `tmp/vector2dggs-0.2.1.tar.gz` & `tmp/vector2dggs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.2.1.tar", max compression
+gzip compressed data, was "vector2dggs-0.3.0.tar", max compression
```

## Comparing `vector2dggs-0.2.1.tar` & `vector2dggs-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7920 2023-04-28 03:57:54.021647 vector2dggs-0.2.1/README.md
--rw-r--r--   0        0        0     1092 2023-04-28 03:58:19.141773 vector2dggs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-04-28 03:58:04.641700 vector2dggs-0.2.1/vector2dggs/__init__.py
--rw-r--r--   0        0        0      598 2023-04-28 03:53:40.792378 vector2dggs-0.2.1/vector2dggs/cli.py
--rw-r--r--   0        0        0     9405 2023-04-28 03:53:55.148450 vector2dggs-0.2.1/vector2dggs/h3.py
--rw-r--r--   0        0        0     2817 2023-04-26 00:14:53.266711 vector2dggs-0.2.1/vector2dggs/katana.py
--rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7920 2023-05-02 23:30:42.832416 vector2dggs-0.3.0/README.md
+-rw-r--r--   0        0        0     1092 2023-05-02 23:30:48.748444 vector2dggs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/cli.py
+-rw-r--r--   0        0        0     9405 2023-04-28 03:53:55.148450 vector2dggs-0.3.0/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3074 2023-05-02 23:30:16.752288 vector2dggs-0.3.0/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.3.0/PKG-INFO
```

### Comparing `vector2dggs-0.2.1/README.md` & `vector2dggs-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.2.1},
+  version={0.3.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.2.1/pyproject.toml` & `vector2dggs-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.2.1"
+version = "0.3.0"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.2.1/vector2dggs/cli.py` & `vector2dggs-0.3.0/vector2dggs/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # notice like this when it starts in an interactive mode:
 
 #     <program>  Copyright (C) <year>  <name of author>
 #     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
 #     This is free software, and you are welcome to redistribute it
 #     under certain conditions; type `show c' for details.
 
+
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     pass
 
 
 cli.add_command(h3)
```

### Comparing `vector2dggs-0.2.1/vector2dggs/h3.py` & `vector2dggs-0.3.0/vector2dggs/h3.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.2.1/vector2dggs/katana.py` & `vector2dggs-0.3.0/vector2dggs/katana.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,25 @@
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
 from shapely.geometry import box, Polygon, MultiPolygon, GeometryCollection
+from shapely.validation import explain_validity, make_valid
 
 
 def katana(geometry, threshold, count=0) -> GeometryCollection:
-    """Split a Polygon into two parts across it's shortest dimension"""
+    """
+    Split a polygon into two parts across it's shortest dimension.
+    Invalid input `geometry` will silently be made valid (if possible).
+    """
+    if not geometry.is_valid:
+        # print(explain_validity(geometry))
+        geometry = make_valid(geometry)
     bounds = geometry.bounds
     width = bounds[2] - bounds[0]
     height = bounds[3] - bounds[1]
     if max(width, height) <= threshold or count == 250:
         # either the polygon is smaller than the threshold, or the maximum
         # number of recursions has been reached
         return [geometry]
```

### Comparing `vector2dggs-0.2.1/PKG-INFO` & `vector2dggs-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.2.1
+Version: 0.3.0
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
-  version={0.2.1},
+  version={0.3.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

