# Comparing `tmp/iqm-cortex-cli-4.0.tar.gz` & `tmp/iqm-cortex-cli-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-4.0.tar", last modified: Thu Apr 20 09:51:12 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-4.1.tar", last modified: Wed May  3 14:16:58 2023, max compression
```

## Comparing `iqm-cortex-cli-4.0.tar` & `iqm-cortex-cli-4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.586837 iqm-cortex-cli-4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.578837 iqm-cortex-cli-4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.578837 iqm-cortex-cli-4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-04-20 09:51:12.586837 iqm-cortex-cli-4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.578837 iqm-cortex-cli-4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.578837 iqm-cortex-cli-4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.582837 iqm-cortex-cli-4.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.582837 iqm-cortex-cli-4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:51:12.586837 iqm-cortex-cli-4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.578837 iqm-cortex-cli-4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.582837 iqm-cortex-cli-4.0/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26350 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/src/cortex_cli/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.582837 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 09:51:12.000000 iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.586837 iqm-cortex-cli-4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/cortex_cli_auth_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/cortex_cli_auth_logout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/cortex_cli_auth_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/cortex_cli_init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:12.586837 iqm-cortex-cli-4.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-20 09:50:32.000000 iqm-cortex-cli-4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.440132 iqm-cortex-cli-4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26350 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tox.ini
```

### Comparing `iqm-cortex-cli-4.0/.github/workflows/ci.yml` & `iqm-cortex-cli-4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-4.1/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/CHANGELOG.rst` & `iqm-cortex-cli-4.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 4.1
+===========
+
+* Generate license information for dependencies on every release `#44 <https://github.com/iqm-finland/cortex-cli/pull/44>`_
+
 Version 4.0
 ===========
 
 * Remove circuit execution command `#43 <https://github.com/iqm-finland/cortex-cli/pull/43>`_
 
 
 Version 3.6
```

### Comparing `iqm-cortex-cli-4.0/DEVELOPMENT.rst` & `iqm-cortex-cli-4.1/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/LICENSE.rst` & `iqm-cortex-cli-4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/PKG-INFO` & `iqm-cortex-cli-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.0
+Version: 4.1
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.0/README.rst` & `iqm-cortex-cli-4.1/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/Makefile` & `iqm-cortex-cli-4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_static/images/favicon.ico` & `iqm-cortex-cli-4.1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_static/images/logo.png` & `iqm-cortex-cli-4.1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-4.1/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-4.1/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_templates/page.html` & `iqm-cortex-cli-4.1/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/_templates/versioning.html` & `iqm-cortex-cli-4.1/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/docs/conf.py` & `iqm-cortex-cli-4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/pyproject.toml` & `iqm-cortex-cli-4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/cortex_cli/__init__.py` & `iqm-cortex-cli-4.1/src/cortex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/cortex_cli/auth.py` & `iqm-cortex-cli-4.1/src/cortex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-4.1/src/cortex_cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/cortex_cli/models.py` & `iqm-cortex-cli-4.1/src/cortex_cli/models.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-4.1/src/cortex_cli/token_manager.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.0
+Version: 4.1
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.0/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tag-from-pipeline.sh` & `iqm-cortex-cli-4.1/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/auth_test.py` & `iqm-cortex-cli-4.1/tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/conftest.py` & `iqm-cortex-cli-4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/cortex_cli_auth_login_test.py` & `iqm-cortex-cli-4.1/tests/cortex_cli_auth_login_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/cortex_cli_auth_logout_test.py` & `iqm-cortex-cli-4.1/tests/cortex_cli_auth_logout_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/cortex_cli_auth_status_test.py` & `iqm-cortex-cli-4.1/tests/cortex_cli_auth_status_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/cortex_cli_init_test.py` & `iqm-cortex-cli-4.1/tests/cortex_cli_init_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/cortex_cli_test.py` & `iqm-cortex-cli-4.1/tests/cortex_cli_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/resources/tokens.json` & `iqm-cortex-cli-4.1/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tests/token_manager_test.py` & `iqm-cortex-cli-4.1/tests/token_manager_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.0/tox.ini` & `iqm-cortex-cli-4.1/tox.ini`

 * *Files identical despite different names*

