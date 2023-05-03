# Comparing `tmp/pytest-dbt-core-0.2.0.tar.gz` & `tmp/pytest-dbt-core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-dbt-core-0.2.0.tar", last modified: Wed Mar  1 15:48:26 2023, max compression
+gzip compressed data, was "pytest-dbt-core-0.2.1.tar", last modified: Wed May  3 11:12:44 2023, max compression
```

## Comparing `pytest-dbt-core-0.2.0.tar` & `pytest-dbt-core-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/HOWTORELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/macros/normalize_column_names.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/tests/test_normalize_column_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/tests/test_spark_get_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/dbt_spark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/docs/source/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/src/pytest_dbt_core/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-01 15:48:26.000000 pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.515255 pytest-dbt-core-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/tests/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/tests/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/macros/fetch_single_statement.sql
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/macros/prices.sql
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:48:26.519255 pytest-dbt-core-0.2.0/tests/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/tests/test_fetch_single_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-01 15:48:13.000000 pytest-dbt-core-0.2.0/tests/dbt_project/tests/test_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/HOWTORELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:43.996846 pytest-dbt-core-0.2.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/macros/normalize_column_names.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/tests/test_normalize_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/tests/test_spark_get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/dbt_spark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/docs/source/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:43.996846 pytest-dbt-core-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/src/pytest_dbt_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.000846 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 11:12:43.000000 pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:43.996846 pytest-dbt-core-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/tests/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/tests/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/macros/fetch_single_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/macros/prices.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:12:44.004846 pytest-dbt-core-0.2.1/tests/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/tests/test_fetch_single_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-03 11:12:28.000000 pytest-dbt-core-0.2.1/tests/dbt_project/tests/test_prices.py
```

### Comparing `pytest-dbt-core-0.2.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `pytest-dbt-core-0.2.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `pytest-dbt-core-0.2.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/.github/pull_request_template.md` & `pytest-dbt-core-0.2.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/.github/workflows/workflow.yml` & `pytest-dbt-core-0.2.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/.gitignore` & `pytest-dbt-core-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/.pre-commit-config.yaml` & `pytest-dbt-core-0.2.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     language_version: python3.9
 - repo: https://github.com/humitos/mirrors-autoflake.git
   rev: v1.3
   hooks:
   - id: autoflake
     args: ['--in-place', '--remove-all-unused-imports']
 - repo: https://github.com/pycqa/flake8
-  rev: 3.9.2
+  rev: 5.0.4
   hooks:
   - id: flake8
     name: Run flake8 linter
     additional_dependencies: ["flake8-bugbear==20.11.1", "pep8-naming==0.11.1"]
 - repo: https://github.com/timothycrosley/isort
   rev: 5.11.5
   hooks:
```

### Comparing `pytest-dbt-core-0.2.0/CHANGELOG.md` & `pytest-dbt-core-0.2.1/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+## [0.2.1] - 2023-05-03
+
+- Support dbt v1.5 ([PR](https://github.com/godatadriven/pytest-dbt-core/pull/34))
+
 ## [0.2.0] - 2023-03-01
 
 - Add example with column rename macro ([PR](https://github.com/godatadriven/pytest-dbt-core/pull/19))
-- Add `--profiles-dir` as an option for setting the profiles directory
-- Extend tox matrix to test for dbt-spark minor versions ([PR](https://github.com/godatadriven/pytest-dbt-core/pull/29))
+- Add `--profiles-dir` as an option for setting the profiles directory ([PR](https://github.com/godatadriven/pytest-dbt-core/pull/25))
+- Extend tox matrix to test for dbt-spark minor versions ([issue](https://github.com/godatadriven/pytest-dbt-core/issues/28), [PR](https://github.com/godatadriven/pytest-dbt-core/pull/29))
 - Extend testing matrix to test for Python minor version 3.10 ([PR](https://github.com/godatadriven/pytest-dbt-core/pull/30))
 
-
 ## [0.1.0] - 2022-07-22
 
 - Run test examples from docs ([issue](https://github.com/godatadriven/pytest-dbt-core/issues/14), [PR](https://github.com/godatadriven/pytest-dbt-core/pull/17))
 - Add target flag ([issue](https://github.com/godatadriven/pytest-dbt-core/issues/11), [PR](https://github.com/godatadriven/pytest-dbt-core/pull/13))
 - Delete session module [is included in dbt-spark](https://github.com/dbt-labs/dbt-spark/issues/272)
 - Add Github templates
```

### Comparing `pytest-dbt-core-0.2.0/CONTRIBUTING.md` & `pytest-dbt-core-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/HOWTORELEASE.md` & `pytest-dbt-core-0.2.1/HOWTORELEASE.md`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/LICENSE` & `pytest-dbt-core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/PKG-INFO` & `pytest-dbt-core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dbt-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytest extension for dbt.
 Home-page: https://github.com/godatadriven/pytest-dbt-core
 Author: Cor Zuurmond
 Maintainer: Cor Zuurmond
 Maintainer-email: corzuurmond@godatadriven.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/godatadriven/pytest-dbt-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-dbt-core Version: 0.2.0 Summary: Pytest
+Metadata-Version: 2.1 Name: pytest-dbt-core Version: 0.2.1 Summary: Pytest
 extension for dbt. Home-page: https://github.com/godatadriven/pytest-dbt-core
 Author: Cor Zuurmond Maintainer: Cor Zuurmond Maintainer-email:
 corzuurmond@godatadriven.com License: Apache 2.0 Project-URL: Source, https://
 github.com/godatadriven/pytest-dbt-core Project-URL: Tracker, https://
 github.com/godatadriven/pytest-dbt-core/issues Keywords: dbt,SQL,data,data
 transformation,testing,pytest Platform: any Classifier: Framework :: Pytest
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `pytest-dbt-core-0.2.0/README.md` & `pytest-dbt-core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/Makefile` & `pytest-dbt-core-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/make.bat` & `pytest-dbt-core-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/macros/normalize_column_names.sql` & `pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/macros/normalize_column_names.sql`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/tests/test_normalize_column_names.py` & `pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/tests/test_normalize_column_names.py`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/_static/dbt_project/tests/test_spark_get_tables.py` & `pytest-dbt-core-0.2.1/docs/source/_static/dbt_project/tests/test_spark_get_tables.py`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/conf.py` & `pytest-dbt-core-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/configuration.rst` & `pytest-dbt-core-0.2.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/dbt_spark.rst` & `pytest-dbt-core-0.2.1/docs/source/dbt_spark.rst`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/docs/source/index.rst` & `pytest-dbt-core-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/scripts/release.py` & `pytest-dbt-core-0.2.1/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/setup.cfg` & `pytest-dbt-core-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 classifiers = 
 	Framework :: Pytest
 
 [options]
 packages = find:
 package_dir = =src
 install_requires = 
-	dbt-core>=1.0.0,<1.5.0
+	dbt-core>=1.0.0,<1.6.0
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
-	dbt-spark[ODBC]>=1.1.0,<1.5.0
+	dbt-spark[ODBC]>=1.1.0,<1.6.0
 	pyspark>=3.0.0,<4.0.0
 	pre-commit>=2.14.1
 	pytest>=6.2.5
 	pytest-spark>=0.6.0
 	pytest-cov>=2.12.1
 
 [options.entry_points]
@@ -66,15 +66,15 @@
 	--profiles-dir=./tests/dbt_project
 spark_options = 
 	spark.app.name: dbt-core
 	spark.executor.instances: 1
 	spark.sql.catalogImplementation: in-memory
 
 [tox:tox]
-envlist = py{3.7,3.8,3.9,3.10}-dbt-spark{11,12,13,14}
+envlist = py{3.7,3.8,3.9,3.10}-dbt-spark{11,12,13,14,15}
 isolated_build = true
 skip_missing_interpreters = true
 
 [testenv]
 description = run the tests with pytest under {basepython}
 setenv = 
 	PIP_DISABLE_PIP_VERSION_CHECK = 1
@@ -85,14 +85,15 @@
 	PYTEST_*
 	PIP_CACHE_DIR
 deps = 
 	dbt-spark11: dbt-spark[ODBC]~=1.1.0
 	dbt-spark12: dbt-spark[ODBC]~=1.2.0
 	dbt-spark13: dbt-spark[ODBC]~=1.3.0
 	dbt-spark14: dbt-spark[ODBC]~=1.4.0
+	dbt-spark15: dbt-spark[ODBC]~=1.5.0
 	pip >= 19.3.1
 extras = test
 commands = pytest {posargs:tests}
 
 [testenv:docs]
 description = run the tests in docs
 setenv = 
@@ -102,16 +103,17 @@
 	PYTEST_*
 	PIP_CACHE_DIR
 deps = 
 	dbt-spark11: dbt-spark[ODBC]~=1.1.0
 	dbt-spark12: dbt-spark[ODBC]~=1.2.0
 	dbt-spark13: dbt-spark[ODBC]~=1.3.0
 	dbt-spark14: dbt-spark[ODBC]~=1.4.0
+	dbt-spark15: dbt-spark[ODBC]~=1.5.0
 	pip >= 19.3.1
 extras = test
-commands_pre = dbt deps --project-dir {toxinidir}/docs/source/_static/dbt_project
+commands_pre = dbt deps --project-dir {toxinidir}/docs/source/_static/dbt_project --profiles-dir {toxinidir}/docs/source/_static/dbt_project
 commands = pytest {posargs:docs/source/_static/dbt_project/tests} --dbt-project-dir={toxinidir}/docs/source/_static/dbt_project --profiles-dir={toxinidir}/docs/source/_static/dbt_project
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pytest-dbt-core-0.2.0/src/pytest_dbt_core/fixtures.py` & `pytest-dbt-core-0.2.1/src/pytest_dbt_core/fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 
     Source
     ------
     See argparse `add_argument` statements in `dbt.main`.
     """
 
     project_dir: str
+    profiles_dir: str
     target: str | None
     profile: str | None
+    threads: int | None
 
 
 @pytest.fixture
 def config(request: SubRequest) -> RuntimeConfig:
     """
     Get the (runtime) config.
 
@@ -56,24 +58,25 @@
         The pytest request.
 
     Returns
     -------
     RuntimeConfig
         The runtime config.
     """
-
-    profiles_dir = request.config.getoption("--profiles-dir")
-    if profiles_dir:
-        flags.PROFILES_DIR = os.path.abspath(profiles_dir)
-
+    # For the  arguments that are hardcoded to `None`, dbt internals set the
+    # appropiate values
     args = Args(
         project_dir=request.config.getoption("--dbt-project-dir"),
+        profiles_dir=request.config.getoption("--profiles-dir"),
         target=request.config.getoption("--dbt-target"),
         profile=None,
+        threads=None,
     )
+    flags.set_from_args(args, user_config=None)
+
     config = RuntimeConfig.from_args(args)
     return config
 
 
 @pytest.fixture
 def adapter(config: RuntimeConfig) -> AdapterContainer:
     """
```

### Comparing `pytest-dbt-core-0.2.0/src/pytest_dbt_core/plugin.py` & `pytest-dbt-core-0.2.1/src/pytest_dbt_core/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/PKG-INFO` & `pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dbt-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pytest extension for dbt.
 Home-page: https://github.com/godatadriven/pytest-dbt-core
 Author: Cor Zuurmond
 Maintainer: Cor Zuurmond
 Maintainer-email: corzuurmond@godatadriven.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/godatadriven/pytest-dbt-core
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-dbt-core Version: 0.2.0 Summary: Pytest
+Metadata-Version: 2.1 Name: pytest-dbt-core Version: 0.2.1 Summary: Pytest
 extension for dbt. Home-page: https://github.com/godatadriven/pytest-dbt-core
 Author: Cor Zuurmond Maintainer: Cor Zuurmond Maintainer-email:
 corzuurmond@godatadriven.com License: Apache 2.0 Project-URL: Source, https://
 github.com/godatadriven/pytest-dbt-core Project-URL: Tracker, https://
 github.com/godatadriven/pytest-dbt-core/issues Keywords: dbt,SQL,data,data
 transformation,testing,pytest Platform: any Classifier: Framework :: Pytest
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `pytest-dbt-core-0.2.0/src/pytest_dbt_core.egg-info/SOURCES.txt` & `pytest-dbt-core-0.2.1/src/pytest_dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-dbt-core-0.2.0/tests/dbt_project/tests/test_prices.py` & `pytest-dbt-core-0.2.1/tests/dbt_project/tests/test_prices.py`

 * *Files identical despite different names*

