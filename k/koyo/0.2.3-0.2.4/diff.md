# Comparing `tmp/koyo-0.2.3.tar.gz` & `tmp/koyo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koyo-0.2.3.tar", last modified: Thu Apr 13 17:17:48 2023, max compression
+gzip compressed data, was "koyo-0.2.4.tar", last modified: Wed May  3 13:11:10 2023, max compression
```

## Comparing `koyo-0.2.3.tar` & `koyo-0.2.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.562429 koyo-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.566429 koyo-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-13 17:17:34.000000 koyo-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-13 17:17:34.000000 koyo-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 17:17:34.000000 koyo-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 17:17:48.570429 koyo-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 17:17:34.000000 koyo-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-13 17:17:34.000000 koyo-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:17:48.570429 koyo-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.562429 koyo-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.566429 koyo-0.2.3/src/koyo/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/src/koyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_koyo.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.129769 koyo-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.125769 koyo-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 13:10:51.000000 koyo-0.2.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 13:10:51.000000 koyo-0.2.4/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 13:10:51.000000 koyo-0.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.125769 koyo-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-03 13:10:51.000000 koyo-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-03 13:10:51.000000 koyo-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-03 13:10:51.000000 koyo-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 13:10:51.000000 koyo-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 13:11:10.129769 koyo-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 13:10:51.000000 koyo-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-03 13:10:51.000000 koyo-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:11:10.129769 koyo-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.125769 koyo-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.129769 koyo-0.2.4/src/koyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-03 13:10:51.000000 koyo-0.2.4/src/koyo/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.129769 koyo-0.2.4/src/koyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:11:10.000000 koyo-0.2.4/src/koyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:11:10.129769 koyo-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_koyo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-03 13:10:51.000000 koyo-0.2.4/tests/test_utilities.py
```

### Comparing `koyo-0.2.3/.github/workflows/ci.yml` & `koyo-0.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/.pre-commit-config.yaml` & `koyo-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/LICENSE` & `koyo-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/PKG-INFO` & `koyo-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -16,26 +16,32 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-# koyo
+# Kōyō
+
+A little library of utility functions that are used throughout various libraries of the Van de Plas lab.
 
 [![License](https://img.shields.io/pypi/l/koyo.svg?color=green)](https://github.com/vandeplaslab/koyo/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/koyo.svg?color=green)](https://pypi.org/project/koyo)
 [![Python Version](https://img.shields.io/pypi/pyversions/koyo.svg?color=green)](https://python.org)
 [![CI](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml/badge.svg)](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/vandeplaslab/koyo/branch/main/graph/badge.svg)](https://codecov.io/gh/vandeplaslab/koyo)
 
-Set of utility functions that are used throughout various libraries of the Van de Plas Lab.
-
 ## Installation
 
 ```bash
 pip install koyo
 ```
 
 ## Contributing
 
 Contributions are always welcome. Please feel free to submit PRs with new features, bug fixes, or documentation improvements.
+
+```bash
+git clone https://github.com/vandeplaslab/koyo.git
+
+pip install -e .[dev]
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `koyo-0.2.3/README.md` & `koyo-0.2.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-# koyo
+# Kōyō
+
+A little library of utility functions that are used throughout various libraries of the Van de Plas lab.
 
 [![License](https://img.shields.io/pypi/l/koyo.svg?color=green)](https://github.com/vandeplaslab/koyo/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/koyo.svg?color=green)](https://pypi.org/project/koyo)
 [![Python Version](https://img.shields.io/pypi/pyversions/koyo.svg?color=green)](https://python.org)
 [![CI](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml/badge.svg)](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/vandeplaslab/koyo/branch/main/graph/badge.svg)](https://codecov.io/gh/vandeplaslab/koyo)
 
-Set of utility functions that are used throughout various libraries of the Van de Plas Lab.
-
 ## Installation
 
 ```bash
 pip install koyo
 ```
 
 ## Contributing
 
-Contributions are always welcome. Please feel free to submit PRs with new features, bug fixes, or documentation improvements.
+Contributions are always welcome. Please feel free to submit PRs with new features, bug fixes, or documentation improvements.
+
+```bash
+git clone https://github.com/vandeplaslab/koyo.git
+
+pip install -e .[dev]
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `koyo-0.2.3/pyproject.toml` & `koyo-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,14 @@
   "setuptools >= 42",
   "wheel",
   "build",
   "setuptools_scm[toml]>=3.4"
 ]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-write_to = "src/koyo/_version.py"
-
 # https://peps.python.org/pep-0621/
 [project]
 name = "koyo"
 description = "Simple python ulitities for various projects."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "BSD 3-Clause License" }
@@ -31,15 +28,16 @@
     "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
     "numpy",
     "scipy",
     "numba",
-    "natsort"
+    "natsort",
+    "loguru"
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = [
     "pytest>=6.0",
@@ -65,14 +63,18 @@
 # spam-cli = "spam:main_cli"
 
 # Entry points
 # https://peps.python.org/pep-0621/#entry-points
 # [project.entry-points."spam.magical"]
 # tomatoes = "spam:main_tomatoes"
 
+
+[tool.setuptools_scm]
+write_to = "src/koyo/_version.py"
+
 # https://github.com/psf/black
 [tool.black]
 line-length = 120
 target-version = ['py37', 'py38', 'py39']
 include = '\.pyi?$'
 
 # https://github.com/charliermarsh/ruff
@@ -130,15 +132,14 @@
 pretty = true
 
 # # module specific overrides
 # [[tool.mypy.overrides]]
 # module = ["numpy.*",]
 # ignore_errors = true
 
-
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "except ImportError",
```

### Comparing `koyo-0.2.3/src/koyo/containers.py` & `koyo-0.2.4/src/koyo/containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/decorators.py` & `koyo-0.2.4/src/koyo/decorators.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/download.py` & `koyo-0.2.4/src/koyo/download.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/image.py` & `koyo-0.2.4/src/koyo/image.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/json.py` & `koyo-0.2.4/src/koyo/json.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/numpy.py` & `koyo-0.2.4/src/koyo/numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/secret.py` & `koyo-0.2.4/src/koyo/secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import hashlib
 import typing as ty
 import uuid
 
 from natsort import natsorted
 
-__all__ = ("get_short_hash", "hash_iterable", "hash_obj", "hash_parameters")
-
 
 def get_unique_str():
     """Gives random, unique name."""
     return str(uuid.uuid4().hex)
 
 
 def get_short_hash(n: int = 0) -> str:
```

### Comparing `koyo-0.2.3/src/koyo/spectrum.py` & `koyo-0.2.4/src/koyo/spectrum.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/timer.py` & `koyo-0.2.4/src/koyo/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,12 @@
 """Timer utilities."""
 import time
 import typing as ty
 from contextlib import contextmanager
 
-__all__ = [
-    "format_human_time",
-    "format_human_time_s",
-    "format_time",
-    "measure_time",
-    "MeasureTimer",
-    "report_measure_time",
-    "report_time",
-    "time_loop",
-    "time_average",
-    "Timer",
-]
-
-
 PERIODS = [
     ("year", 60 * 60 * 24 * 365 * 1e9),
     ("month", 60 * 60 * 24 * 30 * 1e9),
     ("day", 60 * 60 * 24 * 1e9),
     ("h", 60 * 60 * 1e9),
     ("min", 60 * 1e9),
     ("s", 1 * 1e9),
```

### Comparing `koyo-0.2.3/src/koyo/toml.py` & `koyo-0.2.4/src/koyo/toml.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/typing.py` & `koyo-0.2.4/src/koyo/typing.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/utilities.py` & `koyo-0.2.4/src/koyo/utilities.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo/visuals.py` & `koyo-0.2.4/src/koyo/visuals.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/src/koyo.egg-info/PKG-INFO` & `koyo-0.2.4/src/koyo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -16,26 +16,32 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-# koyo
+# Kōyō
+
+A little library of utility functions that are used throughout various libraries of the Van de Plas lab.
 
 [![License](https://img.shields.io/pypi/l/koyo.svg?color=green)](https://github.com/vandeplaslab/koyo/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/koyo.svg?color=green)](https://pypi.org/project/koyo)
 [![Python Version](https://img.shields.io/pypi/pyversions/koyo.svg?color=green)](https://python.org)
 [![CI](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml/badge.svg)](https://github.com/vandeplaslab/koyo/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/vandeplaslab/koyo/branch/main/graph/badge.svg)](https://codecov.io/gh/vandeplaslab/koyo)
 
-Set of utility functions that are used throughout various libraries of the Van de Plas Lab.
-
 ## Installation
 
 ```bash
 pip install koyo
 ```
 
 ## Contributing
 
 Contributions are always welcome. Please feel free to submit PRs with new features, bug fixes, or documentation improvements.
+
+```bash
+git clone https://github.com/vandeplaslab/koyo.git
+
+pip install -e .[dev]
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `koyo-0.2.3/src/koyo.egg-info/SOURCES.txt` & `koyo-0.2.4/src/koyo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/koyo/__init__.py
 src/koyo/_version.py
 src/koyo/containers.py
 src/koyo/decorators.py
 src/koyo/download.py
 src/koyo/image.py
 src/koyo/json.py
+src/koyo/logging.py
 src/koyo/numpy.py
 src/koyo/py.typed
 src/koyo/rand.py
 src/koyo/secret.py
 src/koyo/spectrum.py
 src/koyo/timer.py
 src/koyo/toml.py
```

### Comparing `koyo-0.2.3/tests/test_containers.py` & `koyo-0.2.4/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/tests/test_numpy.py` & `koyo-0.2.4/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/tests/test_secret.py` & `koyo-0.2.4/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/tests/test_timer.py` & `koyo-0.2.4/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.3/tests/test_utilities.py` & `koyo-0.2.4/tests/test_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import numpy as np
 import pytest
 from koyo.utilities import (
     check_image_orientation,
     check_value_order,
+    chunks,
     find_nearest_index,
     find_nearest_index_batch,
     find_nearest_index_single,
     find_nearest_value_single,
     format_size,
     get_kws,
     get_min_max,
     is_between,
     is_number,
     rescale,
 )
 
 
+def test_chunks():
+    values = [0, 1, 2, 3, 4, 5]
+    for chunk in chunks(values, 2):
+        assert len(chunk) == 2
+    assert len(list(chunks(values, n_tasks=2))) == 2
+
+
 def test_find_nearest_index_single():
     array = np.arange(10)
     assert find_nearest_index_single(array, 0) == 0
     assert find_nearest_index_single(array, 0.5) == 0
 
     assert find_nearest_index(array, 0) == 0
     assert find_nearest_index(array, 0.5) == 0
```

