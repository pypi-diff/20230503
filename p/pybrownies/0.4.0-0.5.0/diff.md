# Comparing `tmp/pybrownies-0.4.0.tar.gz` & `tmp/pybrownies-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrownies-0.4.0.tar", last modified: Sun Apr 16 13:54:20 2023, max compression
+gzip compressed data, was "pybrownies-0.5.0.tar", last modified: Wed May  3 19:45:34 2023, max compression
```

## Comparing `pybrownies-0.4.0.tar` & `pybrownies-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      312 2023-03-09 14:00:58.650104 pybrownies-0.4.0/.flake8
--rw-r--r--   0        0        0      391 2023-03-09 13:46:50.824067 pybrownies-0.4.0/.gitignore
--rw-r--r--   0        0        0     1337 2023-04-16 13:39:07.302048 pybrownies-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-03-09 13:36:06.546449 pybrownies-0.4.0/LICENSE
--rw-r--r--   0        0        0     2096 2023-04-16 13:14:17.532084 pybrownies-0.4.0/README.md
--rw-r--r--   0        0        0     1223 2023-04-16 12:56:36.992967 pybrownies-0.4.0/TODO.md
--rw-r--r--   0        0        0       72 2023-04-16 13:22:08.727532 pybrownies-0.4.0/pybrownies/__init__.py
--rwxr-xr-x   0        0        0     2003 2023-04-14 08:34:55.833837 pybrownies-0.4.0/pybrownies/pprintenv.py
--rw-r--r--   0        0        0     4922 2023-04-16 13:14:01.674711 pybrownies-0.4.0/pybrownies/tasks/__init__.py
--rw-r--r--   0        0        0      538 2023-04-07 15:13:22.322754 pybrownies-0.4.0/pybrownies/tasks/__main__.py
--rw-r--r--   0        0        0     1536 2023-03-22 15:03:50.443936 pybrownies-0.4.0/pybrownies/testing.py
--rwxr-xr-x   0        0        0     2455 2023-03-13 15:59:23.508640 pybrownies-0.4.0/pybrownies/whichpy.py
--rw-r--r--   0        0        0     3572 2023-04-16 12:46:15.671197 pybrownies-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-03-16 13:12:34.051813 pybrownies-0.4.0/requirements/dev.txt
--rw-r--r--   0        0        0       54 2023-04-16 12:46:42.615666 pybrownies-0.4.0/requirements/prod.txt
--rw-r--r--   0        0        0       21 2023-03-16 13:23:23.748289 pybrownies-0.4.0/requirements/tox.txt
--rw-r--r--   0        0        0      587 2023-03-22 14:26:55.555464 pybrownies-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      504 2023-04-07 15:32:23.761986 pybrownies-0.4.0/tests/test_pprintenv.py
--rw-r--r--   0        0        0     2762 2023-04-07 15:13:22.324104 pybrownies-0.4.0/tests/test_tasks.py
--rw-r--r--   0        0        0     1689 2023-04-07 15:13:22.325316 pybrownies-0.4.0/tests/test_whichpy.py
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pybrownies-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      312 2023-03-09 14:00:58.650104 pybrownies-0.5.0/.flake8
+-rw-r--r--   0        0        0      391 2023-03-09 13:46:50.824067 pybrownies-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1517 2023-05-03 19:31:01.196701 pybrownies-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-03-09 13:36:06.546449 pybrownies-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2105 2023-05-03 19:38:56.184722 pybrownies-0.5.0/README.md
+-rw-r--r--   0        0        0     1223 2023-04-16 12:56:36.992967 pybrownies-0.5.0/TODO.md
+-rw-r--r--   0        0        0     3607 2023-05-03 19:33:10.857868 pybrownies-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-03-16 13:12:34.051813 pybrownies-0.5.0/requirements/dev.txt
+-rw-r--r--   0        0        0       54 2023-05-03 18:06:05.049080 pybrownies-0.5.0/requirements/prod.txt
+-rw-r--r--   0        0        0      141 2023-05-03 16:39:53.329428 pybrownies-0.5.0/src/pybrownies/__init__.py
+-rwxr-xr-x   0        0        0     2003 2023-04-14 08:34:55.833837 pybrownies-0.5.0/src/pybrownies/pprintenv.py
+-rw-r--r--   0        0        0     4922 2023-04-16 13:14:01.674711 pybrownies-0.5.0/src/pybrownies/tasks/__init__.py
+-rw-r--r--   0        0        0      538 2023-04-07 15:13:22.322754 pybrownies-0.5.0/src/pybrownies/tasks/__main__.py
+-rw-r--r--   0        0        0     1608 2023-05-03 19:28:44.045373 pybrownies-0.5.0/src/pybrownies/testing.py
+-rwxr-xr-x   0        0        0     2455 2023-03-13 15:59:23.508640 pybrownies-0.5.0/src/pybrownies/whichpy.py
+-rw-r--r--   0        0        0      587 2023-03-22 14:26:55.555464 pybrownies-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      504 2023-04-07 15:32:23.761986 pybrownies-0.5.0/tests/test_pprintenv.py
+-rw-r--r--   0        0        0     2766 2023-05-03 19:15:38.546518 pybrownies-0.5.0/tests/test_tasks.py
+-rw-r--r--   0        0        0     1689 2023-04-07 15:13:22.325316 pybrownies-0.5.0/tests/test_whichpy.py
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 pybrownies-0.5.0/PKG-INFO
```

### Comparing `pybrownies-0.4.0/CHANGELOG.md` & `pybrownies-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # CHANGELOG
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
 Version numbers follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.0] - 2023-05-03
+
+### Changed
+
+- pybrownies now work with [Rich](https://pypi.org/project/rich/) v12 as well. Previously, v13 was required.
+- Renamed `bro` to `brownie`.
+
 ## 0.4.0 - 2023-04-16
 
 ### Added
 
 - Linux and Windows are now supported. (Only MacOS was supported prior to this
   version.)
 - Added the `pybrownies.testing` module. It provides a @tmpdir decorator for
-  unit tests which is more usable than the pytest fixture.
+  unit tests which is easier to use than the pytest fixture.
 - `bro publish` has a new option `--show`. It publishes the project and
   displays the newly published project page in the web browser.
 
 ### Changed
 
 - Renamed `bld` to `bro`.
```

### Comparing `pybrownies-0.4.0/LICENSE` & `pybrownies-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/README.md` & `pybrownies-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Little helpers for developers
+# pybrownies
 
-This is a small library of utilities designed to assist in the creation and maintenance of Python projects. `bro` performs chores like testing, linting, building, publishing. `pprintenv` shows the shell environment like printenv, but prettier. `whichpy` locates Python packages and modules (like `which` locates program files).
+This is a small library of utilities designed to assist in the creation and maintenance of Python projects. `brownie` performs chores like testing, linting, building, publishing. `pprintenv` shows the shell environment like printenv, but prettier. `whichpy` locates Python packages and modules (like `which` locates program files).
 
 
 ## Installation
 
 A lean install installs just `pprintenv` and `whichpy`:
 
 ```sh
 % pip install pybrownies
 ```
 
-To also get the `bro` tool and its dependencies to help developing your project, enter
+To also get the `brownie` tool and its dependencies to help developing your project, enter
 
 ```sh
 % pip install pybrownies"[dev]"
 ```
 
 ## Usage
 
-*To see which `bro` tasks are available, enter*
+*To see which `brownie` tasks are available, enter*
 
 ```sh
-% bro --list
+% brownie --list
 Subcommands:
 
   clean       Remove non-code from the project.
   covreport   Show the coverage report in the default browser.
   dist        Create the sdist and wheel for the project.
   lint        Runs pylint and flake8 on every Python package within this
               project.
@@ -35,16 +35,16 @@
   test        Runs all unit tests, optionally with test coverage.
 %
 ```
 
 *To obtain more info on what a specific task does, enter e.g.*
 
 ```bash
-% bro publish -h
-Usage: bro [--core-opts] publish [--options] [other tasks here ...]
+% brownie publish -h
+Usage: brownie [--core-opts] publish [--options] [other tasks here ...]
 
 Docstring:
   Publishes the project on TestPyPI, or on PyPI with the --pypi option.
 
 Options:
   -p, --pypi   publish on pypi.org instead of test.pypi.org
   -s, --show   show the new page in the web browser
@@ -72,8 +72,8 @@
 ```bash
 % whichpy rich.console
 /home/you/dev/pybrownies/.venv3.10/lib/python3.10/site-packages/rich/console.py
 ```
 
 ## Credits
 
-`bro` is basically an [invoke](https://pypi.org/project/invoke/) task library. The colorful output is courtesy of [rich](https://pypi.org/project/rich/).
+`brownie` is basically an [invoke](https://pypi.org/project/invoke/) task library. The colorful output is courtesy of [Rich](https://pypi.org/project/rich/).
```

### Comparing `pybrownies-0.4.0/TODO.md` & `pybrownies-0.5.0/TODO.md`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/pybrownies/pprintenv.py` & `pybrownies-0.5.0/src/pybrownies/pprintenv.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/pybrownies/tasks/__init__.py` & `pybrownies-0.5.0/src/pybrownies/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/pybrownies/tasks/__main__.py` & `pybrownies-0.5.0/src/pybrownies/tasks/__main__.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/pybrownies/testing.py` & `pybrownies-0.5.0/src/pybrownies/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         chdir(tmpdir)
         cleanup = True
         try:
             decorated_function(*args, **kwargs)
         except AssertionError:
             cleanup = False
             raise
+        except Exception:
+            cleanup = False
+            raise
         finally:
             chdir(cwd)
             if cleanup:
                 rmtree(tmpdir)
     return decorator
 
 # I am aware of fixtures, including tmp_path. The problems arises when
```

### Comparing `pybrownies-0.4.0/pybrownies/whichpy.py` & `pybrownies-0.5.0/src/pybrownies/whichpy.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/pyproject.toml` & `pybrownies-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 # PROJECT METADATA
 # ======================================================================
 
 [project]
 name = "pybrownies"
+version = "0.5.0"
+description = "Little helpers for Python developers"
 authors = [
     { name = "Ralf Luetkemeier", email = "foss@rlue.de" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -31,18 +33,17 @@
     "Topic :: Software Development :: Build Tools",
     "Topic :: Utilities",
 ]
 keywords = ["helpers"]
 requires-python = ">=3.8,<3.12.0"
 # Invoke 2.0.0's loader module imports the deprecated "imp" module,
 # which is slated for removal in Python 3.12.
-dynamic = ["version", "description"]
 dependencies = [
-    "invoke >=2.0.0",
-    "rich >= 13.0.0",
+    "invoke >= 2.0.0",
+    "rich >= 12.0.0, < 14.0.0",
     "tomli >= 2.0.0; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 tox = [
     "pytest >=7.2.0",
 ]
@@ -53,15 +54,15 @@
     "pytest >=7.2.0",
     "pytest-cov >=4.0.0",
     "tox >= 4.4.0",
 ]
 # doc = ["sphinx"]
 
 [project.scripts]
-bro = "pybrownies.tasks.__main__:program.run"
+brownie = "pybrownies.tasks.__main__:program.run"
 dobby = "pybrownies.tasks.__main__:program.run"
 pprintenv = "pybrownies.pprintenv:main"
 whichpy = "pybrownies.whichpy:main"
 
 [project.urls]
 #changelog = "https://github.com/me/<repo>/CHANGELOG.md"
 #Documentation = "https://..."
@@ -92,23 +93,23 @@
 #ignore_errors = true
 
 [tool.coverage.run]
 # parallel = true
 # concurrency = ["multiprocessing"]
 # branch = true
 source = [
-    "pybrownies",
+    "src/pybrownies",
     "tests",
 ]
 
 ## Flit ----------------------------------------------------------------
 
 [tool.flit.sdist]
-include = ["docs/", "tests/",]
-# exclude = ["imgs/"]
+include = ["doc/", "tests/",]
+# exclude = ["img/"]
 
 ## Pylint --------------------------------------------------------------
 # Enter pylint --generate-toml-config for more info.
 
 [tool.pylint.main]
 # ignore = ["demo"]
 
@@ -138,11 +139,11 @@
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py{38,39,310,311}
 isolated_build = True
 
 [testenv]
-deps = -rrequirements/tox.txt
+deps = pytest
 commands = pytest
 """
 # platform = linux2|darwin
```

### Comparing `pybrownies-0.4.0/tests/__init__.py` & `pybrownies-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/tests/test_tasks.py` & `pybrownies-0.5.0/tests/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def test_clean():
     covfile = Path('.coverage')
     covfile.touch()
     dirlist = ['.coverage_report', '.mypy_cache', '.pytest_cache',
                '.tox', '.venv3.11', '__pycache__']
     for path in dirlist:
         Path(path).mkdir()
-    os.system('bld clean --pycaches --venvs')
+    os.system('brownie clean --pycaches --venvs')
     assert not covfile.exists()
     for path in dirlist:
         assert not Path(path).exists()
 
 
 @tmpdir
 def test_covreport(capsys):
```

### Comparing `pybrownies-0.4.0/tests/test_whichpy.py` & `pybrownies-0.5.0/tests/test_whichpy.py`

 * *Files identical despite different names*

### Comparing `pybrownies-0.4.0/PKG-INFO` & `pybrownies-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pybrownies
-Version: 0.4.0
-Summary: Little helpers for developing in Python
+Version: 0.5.0
+Summary: Little helpers for Python developers
 Keywords: helpers
 Author-email: Ralf Luetkemeier <foss@rlue.de>
 Requires-Python: >=3.8,<3.12.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -18,52 +18,52 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
-Requires-Dist: invoke >=2.0.0
-Requires-Dist: rich >= 13.0.0
+Requires-Dist: invoke >= 2.0.0
+Requires-Dist: rich >= 12.0.0, < 14.0.0
 Requires-Dist: tomli >= 2.0.0; python_version < '3.11'
 Requires-Dist: flake8 >=6.0.0 ; extra == "dev"
 Requires-Dist: flit >=3.8.0 ; extra == "dev"
 Requires-Dist: pylint >=2.16.0 ; extra == "dev"
 Requires-Dist: pytest >=7.2.0 ; extra == "dev"
 Requires-Dist: pytest-cov >=4.0.0 ; extra == "dev"
 Requires-Dist: tox >= 4.4.0 ; extra == "dev"
 Requires-Dist: pytest >=7.2.0 ; extra == "tox"
 Provides-Extra: dev
 Provides-Extra: tox
 
-# Little helpers for developers
+# pybrownies
 
-This is a small library of utilities designed to assist in the creation and maintenance of Python projects. `bro` performs chores like testing, linting, building, publishing. `pprintenv` shows the shell environment like printenv, but prettier. `whichpy` locates Python packages and modules (like `which` locates program files).
+This is a small library of utilities designed to assist in the creation and maintenance of Python projects. `brownie` performs chores like testing, linting, building, publishing. `pprintenv` shows the shell environment like printenv, but prettier. `whichpy` locates Python packages and modules (like `which` locates program files).
 
 
 ## Installation
 
 A lean install installs just `pprintenv` and `whichpy`:
 
 ```sh
 % pip install pybrownies
 ```
 
-To also get the `bro` tool and its dependencies to help developing your project, enter
+To also get the `brownie` tool and its dependencies to help developing your project, enter
 
 ```sh
 % pip install pybrownies"[dev]"
 ```
 
 ## Usage
 
-*To see which `bro` tasks are available, enter*
+*To see which `brownie` tasks are available, enter*
 
 ```sh
-% bro --list
+% brownie --list
 Subcommands:
 
   clean       Remove non-code from the project.
   covreport   Show the coverage report in the default browser.
   dist        Create the sdist and wheel for the project.
   lint        Runs pylint and flake8 on every Python package within this
               project.
@@ -72,16 +72,16 @@
   test        Runs all unit tests, optionally with test coverage.
 %
 ```
 
 *To obtain more info on what a specific task does, enter e.g.*
 
 ```bash
-% bro publish -h
-Usage: bro [--core-opts] publish [--options] [other tasks here ...]
+% brownie publish -h
+Usage: brownie [--core-opts] publish [--options] [other tasks here ...]
 
 Docstring:
   Publishes the project on TestPyPI, or on PyPI with the --pypi option.
 
 Options:
   -p, --pypi   publish on pypi.org instead of test.pypi.org
   -s, --show   show the new page in the web browser
@@ -109,9 +109,9 @@
 ```bash
 % whichpy rich.console
 /home/you/dev/pybrownies/.venv3.10/lib/python3.10/site-packages/rich/console.py
 ```
 
 ## Credits
 
-`bro` is basically an [invoke](https://pypi.org/project/invoke/) task library. The colorful output is courtesy of [rich](https://pypi.org/project/rich/).
+`brownie` is basically an [invoke](https://pypi.org/project/invoke/) task library. The colorful output is courtesy of [Rich](https://pypi.org/project/rich/).
```

