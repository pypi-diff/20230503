# Comparing `tmp/pyella-1.3.0.tar.gz` & `tmp/pyella-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyella-1.3.0.tar", max compression
+gzip compressed data, was "pyella-1.4.0.tar", max compression
```

## Comparing `pyella-1.3.0.tar` & `pyella-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-30 13:31:56.361709 pyella-1.3.0/LICENSE
--rw-r--r--   0        0        0     1847 2023-04-30 13:31:56.361709 pyella-1.3.0/README.md
--rw-r--r--   0        0        0     2575 2023-04-30 13:32:25.834115 pyella-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      159 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/__init__.py
--rw-r--r--   0        0        0     4987 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/either.py
--rw-r--r--   0        0        0     3139 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/maybe.py
--rw-r--r--   0        0        0      265 2023-04-30 13:31:56.361709 pyella-1.3.0/src/pyella/shared.py
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 pyella-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-03 07:04:33.192094 pyella-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8651 2023-05-03 07:04:33.192094 pyella-1.4.0/README.md
+-rw-r--r--   0        0        0     2680 2023-05-03 07:05:08.344660 pyella-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      310 2023-05-03 07:04:33.192094 pyella-1.4.0/src/pyella/__init__.py
+-rw-r--r--   0        0        0    11112 2023-05-03 07:04:33.192094 pyella-1.4.0/src/pyella/either.py
+-rw-r--r--   0        0        0     7521 2023-05-03 07:04:33.192094 pyella-1.4.0/src/pyella/maybe.py
+-rw-r--r--   0        0        0      526 2023-05-03 07:04:33.192094 pyella-1.4.0/src/pyella/shared.py
+-rw-r--r--   0        0        0     9860 1970-01-01 00:00:00.000000 pyella-1.4.0/PKG-INFO
```

### Comparing `pyella-1.3.0/LICENSE` & `pyella-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyella-1.3.0/pyproject.toml` & `pyella-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,25 @@
 description = "This library brings common monads such `Maybe` and `Either` to your Python projects."
 documentation = "https://github.com/edeckers/pyella"
 homepage = ""
 include = [
     "LICENSE",
 ]
 keywords = [
+ "monad",
+ "fp",
+ "maybe",
+ "either",
 ]
 license = "MPL-2.0"
 maintainers = ["Ely Deckers"]
 name = "pyella"
 readme = "README.md"
 repository = "https://github.com/edeckers/pyella.git"
-version = "1.3.0"
+version = "1.4.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 bandit = "^1.7"
@@ -40,14 +44,17 @@
 nox = "^2022.1.7"
 pre-commit = "^2.17"
 pre-commit-hooks = "^4.1"
 pytest = "^7"
 pytest-cov = "^4"
 python-semantic-release = "^7.25.2"
 
+[tool.poetry.group.docs.dependencies]
+sphinx_mdinclude = "^0.5.3"
+
 #########################################################################################
 # Testing
 #########################################################################################
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
```

