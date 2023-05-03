# Comparing `tmp/abilian_devtools-0.5.1.tar.gz` & `tmp/abilian_devtools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abilian_devtools-0.5.1.tar", max compression
+gzip compressed data, was "abilian_devtools-0.5.2.tar", max compression
```

## Comparing `abilian_devtools-0.5.1.tar` & `abilian_devtools-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.5.1/LICENSES/
--rw-r--r--   0        0        0     3410 2023-03-30 06:46:33.989878 abilian_devtools-0.5.1/README.md
--rw-r--r--   0        0        0     3523 2023-04-25 11:54:35.057513 abilian_devtools-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.5.1/src/abilian_devtools/__init__.py
--rw-r--r--   0        0        0      824 2023-04-25 11:48:17.306722 abilian_devtools-0.5.1/src/abilian_devtools/cli.py
--rw-r--r--   0        0        0        0 2023-04-17 19:33:43.016062 abilian_devtools-0.5.1/src/abilian_devtools/commands/__init__.py
--rw-r--r--   0        0        0      321 2023-04-18 10:19:01.175151 abilian_devtools-0.5.1/src/abilian_devtools/commands/_util.py
--rw-r--r--   0        0        0      445 2023-04-18 10:21:00.387107 abilian_devtools-0.5.1/src/abilian_devtools/commands/all.py
--rw-r--r--   0        0        0      544 2023-04-18 10:21:00.406348 abilian_devtools-0.5.1/src/abilian_devtools/commands/audit.py
--rw-r--r--   0        0        0     1839 2023-04-25 11:24:43.696109 abilian_devtools-0.5.1/src/abilian_devtools/commands/bump.py
--rw-r--r--   0        0        0      956 2023-04-25 11:21:33.062708 abilian_devtools-0.5.1/src/abilian_devtools/commands/check.py
--rw-r--r--   0        0        0      794 2023-04-18 10:17:57.973688 abilian_devtools-0.5.1/src/abilian_devtools/commands/clean.py
--rw-r--r--   0        0        0      764 2023-04-25 11:21:33.063995 abilian_devtools-0.5.1/src/abilian_devtools/commands/format.py
--rw-r--r--   0        0        0     1424 2023-04-18 10:30:55.666246 abilian_devtools-0.5.1/src/abilian_devtools/commands/help.py
--rw-r--r--   0        0        0      687 2023-04-25 11:21:33.065600 abilian_devtools-0.5.1/src/abilian_devtools/commands/test.py
--rw-r--r--   0        0        0      718 2023-04-25 11:23:18.045129 abilian_devtools-0.5.1/src/abilian_devtools/invoke/__init__.py
--rw-r--r--   0        0        0      307 2023-04-18 10:31:18.457907 abilian_devtools-0.5.1/src/abilian_devtools/invoke/help.py
--rw-r--r--   0        0        0      470 2023-04-18 10:30:32.605718 abilian_devtools-0.5.1/src/abilian_devtools/invoke/subrepos.py
--rw-r--r--   0        0        0      795 2023-04-18 10:31:22.407446 abilian_devtools-0.5.1/src/abilian_devtools/invoke/versions.py
--rw-r--r--   0        0        0      479 2023-04-17 19:32:18.135821 abilian_devtools-0.5.1/src/abilian_devtools/shell.py
--rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 abilian_devtools-0.5.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.5.2/LICENSES/
+-rw-r--r--   0        0        0     5089 2023-05-03 06:06:57.428546 abilian_devtools-0.5.2/README.md
+-rw-r--r--   0        0        0     3536 2023-05-03 06:08:20.136207 abilian_devtools-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.5.2/src/abilian_devtools/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-25 11:48:17.306722 abilian_devtools-0.5.2/src/abilian_devtools/cli.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:33:43.016062 abilian_devtools-0.5.2/src/abilian_devtools/commands/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-18 10:19:01.175151 abilian_devtools-0.5.2/src/abilian_devtools/commands/_util.py
+-rw-r--r--   0        0        0      445 2023-04-18 10:21:00.387107 abilian_devtools-0.5.2/src/abilian_devtools/commands/all.py
+-rw-r--r--   0        0        0      544 2023-04-18 10:21:00.406348 abilian_devtools-0.5.2/src/abilian_devtools/commands/audit.py
+-rw-r--r--   0        0        0     1839 2023-04-25 11:24:43.696109 abilian_devtools-0.5.2/src/abilian_devtools/commands/bump.py
+-rw-r--r--   0        0        0     1139 2023-04-27 08:59:39.336786 abilian_devtools-0.5.2/src/abilian_devtools/commands/check.py
+-rw-r--r--   0        0        0      794 2023-04-18 10:17:57.973688 abilian_devtools-0.5.2/src/abilian_devtools/commands/clean.py
+-rw-r--r--   0        0        0      764 2023-04-25 11:21:33.063995 abilian_devtools-0.5.2/src/abilian_devtools/commands/format.py
+-rw-r--r--   0        0        0     1424 2023-04-18 10:30:55.666246 abilian_devtools-0.5.2/src/abilian_devtools/commands/help.py
+-rw-r--r--   0        0        0      687 2023-04-25 11:21:33.065600 abilian_devtools-0.5.2/src/abilian_devtools/commands/test.py
+-rw-r--r--   0        0        0      718 2023-04-25 11:23:18.045129 abilian_devtools-0.5.2/src/abilian_devtools/invoke/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-18 10:31:18.457907 abilian_devtools-0.5.2/src/abilian_devtools/invoke/help.py
+-rw-r--r--   0        0        0      470 2023-04-18 10:30:32.605718 abilian_devtools-0.5.2/src/abilian_devtools/invoke/subrepos.py
+-rw-r--r--   0        0        0      795 2023-04-18 10:31:22.407446 abilian_devtools-0.5.2/src/abilian_devtools/invoke/versions.py
+-rw-r--r--   0        0        0      479 2023-04-17 19:32:18.135821 abilian_devtools-0.5.2/src/abilian_devtools/shell.py
+-rw-r--r--   0        0        0     7074 1970-01-01 00:00:00.000000 abilian_devtools-0.5.2/PKG-INFO
```

### Comparing `abilian_devtools-0.5.1/pyproject.toml` & `abilian_devtools-0.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abilian-devtools"
-version = "0.5.1"
+version = "0.5.2"
 description = "A curated set of dependencies for quality software development"
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "abilian_devtools", from = "src" }]
 repository = "https://github.com/abilian/abilian-devtools"
 keywords = [
@@ -18,31 +18,31 @@
 
 [tool.poetry.scripts]
 adt = "abilian_devtools.cli:main"
 
 [tool.poetry.dependencies]
 # python = ">=3.8.1,<4.0"
 python = "^3.9"
-cleez = "^0.1.8"
+cleez = "^0.1.11"
 
 # Git integration
 pre-commit = "*"
 
 # Testing
-pytest = "^7"
-pytest-cov = "^4"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 profilehooks = "*"
 pytest-xdist = "*"
 pytest-random-order = "*"
 # pytest-testmon = "^1.2.0"
 nox = "*"
 
 # Linting
 ruff = "*"
-flake8 = "^6"
+flake8 = "^6.0.0"
 # + Plugins: see https://github.com/DmytroLitvinov/awesome-flake8-extensions
 flake8-bandit = "*"
 flake8-breakpoint = "*"
 flake8-cognitive-complexity = "*"
 flake8-datetimez = "*"
 flake8-functions = "*"
 flake8-if-expr = "*"
@@ -96,20 +96,20 @@
 pip = "*"
 pip-audit = "*"
 reuse = "*"
 safety = "*"
 vulture = "*"
 
 # Invoke
-invoke = "^2.0.0"
-tomlkit = "^0.11.6"
+invoke = "^2.1.1"
+tomlkit = "^0.11.8"
 
 [tool.poetry.group.dev.dependencies]
-scriv = "^1.2.0"
-types-invoke = "^2.0.0.1"
+scriv = "^1.3.1"
+types-invoke = "^2.0.0.6"
 snoop = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.deptry]
```

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/cli.py` & `abilian_devtools-0.5.2/src/abilian_devtools/cli.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/audit.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/audit.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/bump.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/bump.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/check.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 Abilian SAS <https://abilian.com/>
 #
 # SPDX-License-Identifier: MIT
-
+from pathlib import Path
 from typing import Optional
 
 from cleez.colors import bold
 from cleez.command import Argument, Command
 
 from ..shell import run
 from ._util import check_files_exist
@@ -25,14 +25,19 @@
         if not args:
             args = ["src", "tests"]
 
         check_files_exist(args)
 
         args_str = " ".join(args)
 
-        run(f"ruff {args_str}")
+        # Todo: more cases
+        if Path("etc").joinpath("ruff.toml").exists():
+            run(f"ruff lint -c etc/ruff.toml {args_str}")
+        else:
+            run(f"ruff {args_str}")
+
         run(f"flake8 {args_str}")
         run(f"mypy --show-error-codes {args_str}")
         run("pyright")
         run(f"vulture --min-confidence 80 {args_str}")
         # TODO: currently broken
         # run("deptry .")
```

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/clean.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/clean.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/format.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/format.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/help.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/help.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/commands/test.py` & `abilian_devtools-0.5.2/src/abilian_devtools/commands/test.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/invoke/__init__.py` & `abilian_devtools-0.5.2/src/abilian_devtools/invoke/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.1/src/abilian_devtools/invoke/versions.py` & `abilian_devtools-0.5.2/src/abilian_devtools/invoke/versions.py`

 * *Files identical despite different names*

