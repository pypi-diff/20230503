# Comparing `tmp/identify-2.5.8.tar.gz` & `tmp/identify-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "identify-2.5.8.tar", last modified: Thu Oct 27 19:59:06 2022, max compression
+gzip compressed data, was "identify-2.5.9.tar", last modified: Fri Nov 18 16:05:29 2022, max compression
```

## Comparing `identify-2.5.8.tar` & `identify-2.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:06.164093 identify-2.5.8/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1072 2022-10-27 19:59:02.000000 identify-2.5.8/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4704 2022-10-27 19:59:06.164093 identify-2.5.8/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4077 2022-10-27 19:59:02.000000 identify-2.5.8/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:06.164093 identify-2.5.8/identify/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:02.000000 identify-2.5.8/identify/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      730 2022-10-27 19:59:02.000000 identify-2.5.8/identify/cli.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11494 2022-10-27 19:59:02.000000 identify-2.5.8/identify/extensions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7932 2022-10-27 19:59:02.000000 identify-2.5.8/identify/identify.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      610 2022-10-27 19:59:02.000000 identify-2.5.8/identify/interpreters.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:02.000000 identify-2.5.8/identify/py.typed
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:06.164093 identify-2.5.8/identify/vendor/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:02.000000 identify-2.5.8/identify/vendor/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)   335105 2022-10-27 19:59:02.000000 identify-2.5.8/identify/vendor/licenses.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-27 19:59:06.164093 identify-2.5.8/identify.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4704 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      410 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2022-10-27 19:59:06.000000 identify-2.5.8/identify.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1258 2022-10-27 19:59:06.164093 identify-2.5.8/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-10-27 19:59:02.000000 identify-2.5.8/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:05:29.748150 identify-2.5.9/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1072 2022-11-18 16:02:25.000000 identify-2.5.9/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4704 2022-11-18 16:05:29.748150 identify-2.5.9/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4077 2022-11-18 16:02:25.000000 identify-2.5.9/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:05:29.748150 identify-2.5.9/identify/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:02:25.000000 identify-2.5.9/identify/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      730 2022-11-18 16:02:25.000000 identify-2.5.9/identify/cli.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11673 2022-11-18 16:05:29.000000 identify-2.5.9/identify/extensions.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7932 2022-11-18 16:02:25.000000 identify-2.5.9/identify/identify.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      610 2022-11-18 16:02:25.000000 identify-2.5.9/identify/interpreters.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:02:25.000000 identify-2.5.9/identify/py.typed
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:05:29.748150 identify-2.5.9/identify/vendor/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:02:25.000000 identify-2.5.9/identify/vendor/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)   335105 2022-11-18 16:02:25.000000 identify-2.5.9/identify/vendor/licenses.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-18 16:05:29.748150 identify-2.5.9/identify.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4704 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      410 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2022-11-18 16:05:29.000000 identify-2.5.9/identify.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1230 2022-11-18 16:05:29.748150 identify-2.5.9/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-11-18 16:02:25.000000 identify-2.5.9/setup.py
```

### Comparing `identify-2.5.8/LICENSE` & `identify-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/PKG-INFO` & `identify-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identify
-Version: 2.5.8
+Version: 2.5.9
 Summary: File identification library for Python
 Home-page: https://github.com/pre-commit/identify
 Author: Chris Kuehl
 Author-email: ckuehl@ocf.berkeley.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `identify-2.5.8/README.md` & `identify-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/identify/cli.py` & `identify-2.5.9/identify/cli.py`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/identify/extensions.py` & `identify-2.5.9/identify/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     'ear': {'binary', 'zip', 'jar'},
     'edn': {'text', 'clojure', 'edn'},
     'ejs': {'text', 'ejs'},
     'env': {'text', 'dotenv'},
     'eot': {'binary', 'eot'},
     'eps': {'binary', 'eps'},
     'erb': {'text', 'erb'},
+    'erl': {'text', 'erlang'},
     'exe': {'binary'},
     'eyaml': {'text', 'yaml'},
     'f03': {'text', 'fortran'},
     'f08': {'text', 'fortran'},
     'f90': {'text', 'fortran'},
     'f95': {'text', 'fortran'},
     'feature': {'text', 'gherkin'},
@@ -75,14 +76,15 @@
     'gypi': {'text', 'gyp', 'python'},
     'gz': {'binary', 'gzip'},
     'h': {'text', 'header', 'c', 'c++'},
     'hbs': {'text', 'handlebars'},
     'hcl': {'text', 'hcl'},
     'hh': {'text', 'header', 'c++'},
     'hpp': {'text', 'header', 'c++'},
+    'hrl': {'text', 'erlang'},
     'hs': {'text', 'haskell'},
     'htm': {'text', 'html'},
     'html': {'text', 'html'},
     'hxx': {'text', 'header', 'c++'},
     'icns': {'binary', 'icns'},
     'ico': {'binary', 'icon'},
     'ics': {'text', 'icalendar'},
@@ -329,11 +331,14 @@
     'Pipfile': EXTENSIONS['toml'],
     'Pipfile.lock': EXTENSIONS['json'],
     'PKGBUILD': {'text', 'bash', 'pkgbuild', 'alpm'},
     'poetry.lock': EXTENSIONS['toml'],
     'pylintrc': EXTENSIONS['ini'] | {'pylintrc'},
     'README': EXTENSIONS['txt'],
     'Rakefile': EXTENSIONS['rb'],
+    'rebar.config': EXTENSIONS['erl'],
     'setup.cfg': EXTENSIONS['ini'],
+    'sys.config': EXTENSIONS['erl'],
+    'sys.config.src': EXTENSIONS['erl'],
     'WORKSPACE': EXTENSIONS['bzl'],
     'wscript': EXTENSIONS['py'],
 }
```

### Comparing `identify-2.5.8/identify/identify.py` & `identify-2.5.9/identify/identify.py`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/identify/interpreters.py` & `identify-2.5.9/identify/interpreters.py`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/identify/vendor/licenses.py` & `identify-2.5.9/identify/vendor/licenses.py`

 * *Files identical despite different names*

### Comparing `identify-2.5.8/identify.egg-info/PKG-INFO` & `identify-2.5.9/identify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identify
-Version: 2.5.8
+Version: 2.5.9
 Summary: File identification library for Python
 Home-page: https://github.com/pre-commit/identify
 Author: Chris Kuehl
 Author-email: ckuehl@ocf.berkeley.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `identify-2.5.8/setup.cfg` & `identify-2.5.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = identify
-version = 2.5.8
+version = 2.5.9
 description = File identification library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/identify
 author = Chris Kuehl
 author_email = ckuehl@ocf.berkeley.edu
 license = MIT
@@ -44,15 +44,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

