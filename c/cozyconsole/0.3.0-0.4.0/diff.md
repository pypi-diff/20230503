# Comparing `tmp/cozyconsole-0.3.0.tar.gz` & `tmp/cozyconsole-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozyconsole-0.3.0.tar", last modified: Sun Apr 16 17:58:11 2023, max compression
+gzip compressed data, was "cozyconsole-0.4.0.tar", last modified: Wed May  3 20:12:46 2023, max compression
```

## Comparing `cozyconsole-0.3.0.tar` & `cozyconsole-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      322 2023-03-06 18:51:00.597302 cozyconsole-0.3.0/.flake8
--rw-r--r--   0        0        0      380 2022-04-11 00:36:10.335950 cozyconsole-0.3.0/.gitignore
--rw-r--r--   0        0        0     1540 2023-04-16 17:53:22.224944 cozyconsole-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-03-02 17:27:37.362021 cozyconsole-0.3.0/LICENSE
--rw-r--r--   0        0        0     1477 2023-04-16 17:51:10.546564 cozyconsole-0.3.0/README.md
--rw-r--r--   0        0        0     1309 2023-04-16 14:18:38.958582 cozyconsole-0.3.0/TODO.md
--rw-r--r--   0        0        0      246 2023-04-16 17:52:41.079983 cozyconsole-0.3.0/cozyconsole/__init__.py
--rw-r--r--   0        0        0     2720 2023-03-15 10:52:03.514104 cozyconsole-0.3.0/cozyconsole/activity.py
--rw-r--r--   0        0        0     2333 2023-03-14 13:49:26.424895 cozyconsole-0.3.0/cozyconsole/consolex.py
--rw-r--r--   0        0        0        0 2023-03-05 18:11:42.368586 cozyconsole-0.3.0/cozyconsole/demo/__init__.py
--rw-r--r--   0        0        0      137 2023-03-05 21:52:01.395177 cozyconsole-0.3.0/cozyconsole/demo/__main__.py
--rw-r--r--   0        0        0     8406 2023-03-10 18:33:17.330338 cozyconsole-0.3.0/cozyconsole/demo/activity.py
--rw-r--r--   0        0        0     6281 2023-03-11 13:22:03.043447 cozyconsole-0.3.0/cozyconsole/markdownpatcher.py
--rw-r--r--   0        0        0     3028 2023-04-16 15:45:28.531104 cozyconsole-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        8 2023-03-08 02:01:55.943174 cozyconsole-0.3.0/requirements/.gitignore
--rw-r--r--   0        0        0       60 2023-03-22 16:00:00.774320 cozyconsole-0.3.0/requirements/dev.txt
--rw-r--r--   0        0        0        6 2023-02-27 17:36:33.136881 cozyconsole-0.3.0/requirements/prod.txt
--rw-r--r--   0        0        0       21 2023-03-16 17:17:16.490172 cozyconsole-0.3.0/requirements/tox.txt
--rw-r--r--   0        0        0        0 2022-04-03 15:18:52.166048 cozyconsole-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3676 2023-04-07 18:45:40.542701 cozyconsole-0.3.0/tests/test_activity.py
--rw-r--r--   0        0        0     1295 2023-04-07 18:47:03.366275 cozyconsole-0.3.0/tests/test_console.py
--rw-r--r--   0        0        0     2289 2023-03-22 15:58:16.034562 cozyconsole-0.3.0/tests/test_markdownpatcher.py
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 cozyconsole-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      322 2023-03-06 18:51:00.597302 cozyconsole-0.4.0/.flake8
+-rw-r--r--   0        0        0      380 2022-04-11 00:36:10.335950 cozyconsole-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1725 2023-05-03 20:11:01.479134 cozyconsole-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-03-02 17:27:37.362021 cozyconsole-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1477 2023-04-16 17:51:10.546564 cozyconsole-0.4.0/README.md
+-rw-r--r--   0        0        0     1309 2023-04-16 14:18:38.958582 cozyconsole-0.4.0/TODO.md
+-rw-r--r--   0        0        0     3028 2023-05-03 19:47:33.330665 cozyconsole-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        8 2023-03-08 02:01:55.943174 cozyconsole-0.4.0/requirements/.gitignore
+-rw-r--r--   0        0        0       60 2023-03-22 16:00:00.774320 cozyconsole-0.4.0/requirements/dev.txt
+-rw-r--r--   0        0        0        6 2023-02-27 17:36:33.136881 cozyconsole-0.4.0/requirements/prod.txt
+-rw-r--r--   0        0        0      246 2023-05-03 19:50:49.438248 cozyconsole-0.4.0/src/cozyconsole/__init__.py
+-rw-r--r--   0        0        0     2720 2023-03-15 10:52:03.514104 cozyconsole-0.4.0/src/cozyconsole/activity.py
+-rw-r--r--   0        0        0     2333 2023-03-14 13:49:26.424895 cozyconsole-0.4.0/src/cozyconsole/consolex.py
+-rw-r--r--   0        0        0        0 2023-03-05 18:11:42.368586 cozyconsole-0.4.0/src/cozyconsole/demo/__init__.py
+-rw-r--r--   0        0        0      137 2023-03-05 21:52:01.395177 cozyconsole-0.4.0/src/cozyconsole/demo/__main__.py
+-rw-r--r--   0        0        0     8406 2023-03-10 18:33:17.330338 cozyconsole-0.4.0/src/cozyconsole/demo/activity.py
+-rw-r--r--   0        0        0     6281 2023-03-11 13:22:03.043447 cozyconsole-0.4.0/src/cozyconsole/markdownpatcher.py
+-rw-r--r--   0        0        0        0 2022-04-03 15:18:52.166048 cozyconsole-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3676 2023-04-07 18:45:40.542701 cozyconsole-0.4.0/tests/test_activity.py
+-rw-r--r--   0        0        0     1295 2023-04-07 18:47:03.366275 cozyconsole-0.4.0/tests/test_console.py
+-rw-r--r--   0        0        0     2373 2023-05-03 19:53:05.800489 cozyconsole-0.4.0/tests/test_markdownpatcher.py
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 cozyconsole-0.4.0/PKG-INFO
```

### Comparing `cozyconsole-0.3.0/CHANGELOG.md` & `cozyconsole-0.4.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # CHANGELOG
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Version numbers follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## 0.4.0 - 2023-05-03
+
+### Added
+
+- Experimental support for Python 3.12 (3.12.0a7).
+
+### Changed
+
+- Tested chlog against Rich v12.0.0. Previously, Rich v13.0.0 or later was required.
+
 ## 0.3.0 - 2023-04-16
 
 ### Added
 
 - Ubuntu and Windows (Git Bash) are now supported. (Only MacOS was supported
   prior to this version.)
```

### Comparing `cozyconsole-0.3.0/LICENSE` & `cozyconsole-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/README.md` & `cozyconsole-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/TODO.md` & `cozyconsole-0.4.0/TODO.md`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/cozyconsole/activity.py` & `cozyconsole-0.4.0/src/cozyconsole/activity.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/cozyconsole/consolex.py` & `cozyconsole-0.4.0/src/cozyconsole/consolex.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/cozyconsole/demo/activity.py` & `cozyconsole-0.4.0/src/cozyconsole/demo/activity.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/cozyconsole/markdownpatcher.py` & `cozyconsole-0.4.0/src/cozyconsole/markdownpatcher.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/pyproject.toml` & `cozyconsole-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
 ]
 keywords = ["cli", "console", "rich"]
 requires-python = ">=3.8,<4"
 dynamic = ["version", "description"]
 dependencies = [
-    "rich >=13.0.0",
+    "rich >=12.0.0, <14.0.0",
 ]
 
 [project.optional-dependencies]
 test = [
-    "pytest >=7.2.1",
+    "pytest >=7.2.0",
 ]
 # doc = ["sphinx"]
 
 [project.scripts]
 # script = "cozyconsole.script:main"
 
 [project.urls]
@@ -73,22 +73,22 @@
 ]
 #ignore_errors = true
 
 [tool.coverage.run]
 # parallel = true
 # concurrency = ["multiprocessing"]
 # branch = true
-source = ["cozyconsole"]
+source = ["src/cozyconsole"]
 omit = ["cozyconsole/demo/activity.py"]
 
 ## Flit ----------------------------------------------------------------
 
 [tool.flit.sdist]
 include = ["doc/", "tests/",]
-exclude = ["imgs/"]
+exclude = ["img/"]
 
 ## Pylint --------------------------------------------------------------
 # Enter pylint --generate-toml-config for more info.
 
 [tool.pylint.main]
 # ignore = ["demo"]
 
@@ -113,15 +113,15 @@
 ]
 
 ## Tox -----------------------------------------------------------------
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,39,310,311}
+envlist = py{38,39,310,311,312}
 isolated_build = True
 
 [testenv]
-deps = -rrequirements/dev.txt
+deps = pytest
 commands = pytest
 """
 # platform = linux2|darwin
```

### Comparing `cozyconsole-0.3.0/tests/test_activity.py` & `cozyconsole-0.4.0/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/tests/test_console.py` & `cozyconsole-0.4.0/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `cozyconsole-0.3.0/tests/test_markdownpatcher.py` & `cozyconsole-0.4.0/tests/test_markdownpatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # pylint: disable = missing-function-docstring, missing-module-docstring
 
 import os
 from pathlib import Path
 import shutil
 import sys
 
+import pytest
+
 from cozyconsole.markdownpatcher import console, main, MarkdownPatcher
 import cozyconsole.markdownpatcher
 
+
+@pytest.mark.skip(reason='Run this only if Rich v13 is installed.')
 def test_patch():
     # pylint: disable=protected-access, import-outside-toplevel
     curr_path = Path().cwd().resolve()
     test_path = Path(__file__).parent.resolve()
     try:
         from rich.markdown import __file__ as md_module
         os.chdir(test_path)
```

### Comparing `cozyconsole-0.3.0/PKG-INFO` & `cozyconsole-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cozyconsole
-Version: 0.3.0
+Version: 0.4.0
 Summary: Making development of console-based apps a little more convenient
 Keywords: cli,console,rich
 Author-email: Ralf Luetkemeier <foss@rlue.de>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
-Requires-Dist: rich >=13.0.0
-Requires-Dist: pytest >=7.2.1 ; extra == "test"
+Requires-Dist: rich >=12.0.0, <14.0.0
+Requires-Dist: pytest >=7.2.0 ; extra == "test"
 Provides-Extra: test
 
 # cozyconsole
 
 ## Caveat
 
 This package exists to support my other projects. Those may require breaking changes in here. Consequently, cozyconsole may never become "stable", never reach v1.0.0. Considering how little is in here at the moment, it is probably not worth your time.
```

