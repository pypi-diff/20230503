# Comparing `tmp/pyopp-0.0.6.tar.gz` & `tmp/pyopp-0.0.7.tar.gz`

## Comparing `pyopp-0.0.6.tar` & `pyopp-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyopp-0.0.6/src/pyopp/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pyopp-0.0.6/src/pyopp/cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyopp-0.0.6/src/pyopp/enums.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pyopp-0.0.6/src/pyopp/main.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyopp-0.0.6/src/pyopp/utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyopp-0.0.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyopp-0.0.6/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyopp-0.0.6/README.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 pyopp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyopp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/enums.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/main.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyopp-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyopp-0.0.7/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyopp-0.0.7/README.md
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pyopp-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyopp-0.0.7/PKG-INFO
```

### Comparing `pyopp-0.0.6/src/pyopp/main.py` & `pyopp-0.0.7/src/pyopp/main.py`

 * *Files identical despite different names*

### Comparing `pyopp-0.0.6/src/pyopp/utils.py` & `pyopp-0.0.7/src/pyopp/utils.py`

 * *Files identical despite different names*

### Comparing `pyopp-0.0.6/LICENSE` & `pyopp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopp-0.0.6/pyproject.toml` & `pyopp-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyopp"
-version = "0.0.6"
+version = "0.0.7"
 description = "Over-powered print(er) for Python."
 readme = "README.md"
 requires-python = ">=3.10.4"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "console", "pprint"]
 classifiers = [
@@ -24,15 +24,15 @@
   "Operating System :: MacOS",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet",
 ]
-dependencies = ["pygments~=2.13.0"]
+dependencies = ["pygments~=2.0.0"]
 
 [project.urls]
 Homepage = "https://github.com/waydegg/pyopp"
 Source = "https://github.com/waydegg/pyopp"
 
 [project.scripts]
 pyopp = "pyopp.cli:main"
```

### Comparing `pyopp-0.0.6/PKG-INFO` & `pyopp-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Over-powered print(er) for Python.
 Project-URL: Homepage, https://github.com/waydegg/pyopp
 Project-URL: Source, https://github.com/waydegg/pyopp
 Author-email: Wayde Gilliam <waydegilliam@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: console,pprint,python
@@ -20,11 +20,11 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.4
-Requires-Dist: pygments~=2.13.0
+Requires-Dist: pygments~=2.0.0
 Description-Content-Type: text/markdown
 
 # pyopp
```

