# Comparing `tmp/otoole-1.0.2.tar.gz` & `tmp/otoole-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoole-1.0.2.tar", last modified: Thu Apr 20 02:05:42 2023, max compression
+gzip compressed data, was "otoole-1.0.3.tar", last modified: Wed May  3 20:29:19 2023, max compression
```

## Comparing `otoole-1.0.2.tar` & `otoole-1.0.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.266604 otoole-1.0.2/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      589 2023-02-26 01:13:12.000000 otoole-1.0.2/.coveragerc
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.166604 otoole-1.0.2/.github/
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.176604 otoole-1.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2384 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1277 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/ISSUE_TEMPLATE/docs.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      972 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/ISSUE_TEMPLATE/feature.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      261 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.176604 otoole-1.0.2/.github/workflows/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      410 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/workflows/citation.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      951 2023-04-20 01:42:03.000000 otoole-1.0.2/.github/workflows/python.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      700 2023-02-26 03:45:17.000000 otoole-1.0.2/.gitignore
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       54 2023-02-26 03:45:17.000000 otoole-1.0.2/.isort.cfg
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1519 2023-02-26 03:45:17.000000 otoole-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      490 2023-02-26 03:45:17.000000 otoole-1.0.2/.readthedocs.yml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      694 2023-02-26 03:45:17.000000 otoole-1.0.2/.zenodo.json
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      217 2023-02-26 03:45:17.000000 otoole-1.0.2/AUTHORS.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2862 2023-02-26 03:45:17.000000 otoole-1.0.2/CHANGELOG.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      599 2023-04-20 01:42:03.000000 otoole-1.0.2/CITATION.cff
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1077 2023-02-26 03:45:17.000000 otoole-1.0.2/LICENSE.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-04-20 02:05:42.266604 otoole-1.0.2/PKG-INFO
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1870 2023-04-20 01:42:03.000000 otoole-1.0.2/README.rst
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.186604 otoole-1.0.2/docs/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1154 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/Makefile
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.196604 otoole-1.0.2/docs/_static/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       18 2023-02-26 01:13:12.000000 otoole-1.0.2/docs/_static/.gitignore
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   135029 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/OSeMOSYS.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    61672 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/logo.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56337 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/osemosys_dataflow.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5597 2023-04-20 00:31:02.000000 otoole-1.0.2/docs/_static/otoole_figures.drawio
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   178856 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/overview.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   168226 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/overview_v2.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    95949 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/simplicity_res.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56119 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/validataion_model.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   217753 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/_static/workflow.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       41 2023-02-26 01:13:12.000000 otoole-1.0.2/docs/authors.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-02-26 01:13:12.000000 otoole-1.0.2/docs/changelog.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10307 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/conf.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12076 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/contributing.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11733 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/data.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8936 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/examples.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8264 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/functionality.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1334 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/index.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1116 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/install.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       67 2023-02-26 01:13:12.000000 otoole-1.0.2/docs/license.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      276 2023-02-26 03:45:17.000000 otoole-1.0.2/docs/requirements.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      355 2023-02-26 03:45:17.000000 otoole-1.0.2/pyproject.toml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      125 2023-04-20 01:42:03.000000 otoole-1.0.2/requirements.txt
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.206604 otoole-1.0.2/scripts/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      760 2023-02-26 01:13:12.000000 otoole-1.0.2/scripts/prepare_cbc.sh
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      824 2023-02-26 01:13:12.000000 otoole-1.0.2/scripts/prepare_cbc_short.sh
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1440 2023-04-20 02:05:42.266604 otoole-1.0.2/setup.cfg
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      703 2023-02-26 03:45:17.000000 otoole-1.0.2/setup.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.136604 otoole-1.0.2/src/
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.206604 otoole-1.0.2/src/otoole/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1059 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    15167 2023-03-31 16:26:19.000000 otoole-1.0.2/src/otoole/cli.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4184 2023-04-20 01:42:03.000000 otoole-1.0.2/src/otoole/exceptions.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18250 2023-04-20 01:42:03.000000 otoole-1.0.2/src/otoole/input.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.236604 otoole-1.0.2/src/otoole/preprocess/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.2/src/otoole/preprocess/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11432 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/preprocess/config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2303 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/preprocess/longify_data.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1183 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/preprocess/setup.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5680 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/preprocess/validate_config.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    13306 2023-04-20 01:42:03.000000 otoole-1.0.2/src/otoole/read_strategies.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.236604 otoole-1.0.2/src/otoole/results/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.2/src/otoole/results/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    32615 2023-04-20 01:42:03.000000 otoole-1.0.2/src/otoole/results/result_package.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11163 2023-04-20 01:42:03.000000 otoole-1.0.2/src/otoole/results/results.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8135 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/utils.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6344 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/validate.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4207 2023-02-26 01:13:12.000000 otoole-1.0.2/src/otoole/validate.yaml
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.236604 otoole-1.0.2/src/otoole/visualise/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      328 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/visualise/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     7101 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/visualise/res.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6685 2023-02-26 03:45:17.000000 otoole-1.0.2/src/otoole/write_strategies.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.216604 otoole-1.0.2/src/otoole.egg-info/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/PKG-INFO
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2330 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/SOURCES.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/dependency_links.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/entry_points.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-04-20 02:05:41.000000 otoole-1.0.2/src/otoole.egg-info/not-zip-safe
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      170 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/requires.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        7 2023-04-20 02:05:42.000000 otoole-1.0.2/src/otoole.egg-info/top_level.txt
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.246604 otoole-1.0.2/tests/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3649 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/conftest.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.256604 otoole-1.0.2/tests/fixtures/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   130205 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/fixtures/combined_inputs.xlsx
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11432 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/fixtures/config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4827 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/fixtures/config_r.yaml
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.256604 otoole-1.0.2/tests/fixtures/data/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      182 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/fixtures/data/AccumulatedAnnualDemand.csv
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       29 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/fixtures/data/AvailabilityFactor.csv
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    44422 2023-02-26 01:13:12.000000 otoole-1.0.2/tests/fixtures/simplicity-v0.2.1.zip
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    43735 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/fixtures/simplicity.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    75398 2023-02-26 01:13:12.000000 otoole-1.0.2/tests/fixtures/simplicity.xlsx
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 02:05:42.266604 otoole-1.0.2/tests/results/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    28520 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/results/test_results_package.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4802 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_cli.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2149 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_convert.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18062 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/test_input.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    41641 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/test_read_strategies.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1834 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_setup.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5060 2023-04-20 01:42:03.000000 otoole-1.0.2/tests/test_utils.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5223 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_validate.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11600 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_validate_config.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      377 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_visualise.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6654 2023-02-26 03:45:17.000000 otoole-1.0.2/tests/test_write_strategies.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2553 2023-03-30 17:38:39.000000 otoole-1.0.2/tox.ini
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.413532 otoole-1.0.3/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      589 2023-02-26 01:13:12.000000 otoole-1.0.3/.coveragerc
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.293532 otoole-1.0.3/.github/
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.303532 otoole-1.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2384 2023-04-20 01:42:03.000000 otoole-1.0.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1278 2023-05-03 17:17:12.000000 otoole-1.0.3/.github/ISSUE_TEMPLATE/docs.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      969 2023-05-03 17:17:12.000000 otoole-1.0.3/.github/ISSUE_TEMPLATE/feature.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      261 2023-04-20 01:42:03.000000 otoole-1.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.303532 otoole-1.0.3/.github/workflows/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      410 2023-04-20 01:42:03.000000 otoole-1.0.3/.github/workflows/citation.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      951 2023-04-20 01:42:03.000000 otoole-1.0.3/.github/workflows/python.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      700 2023-02-26 03:45:17.000000 otoole-1.0.3/.gitignore
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       54 2023-02-26 03:45:17.000000 otoole-1.0.3/.isort.cfg
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1519 2023-02-26 03:45:17.000000 otoole-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      490 2023-02-26 03:45:17.000000 otoole-1.0.3/.readthedocs.yml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      694 2023-02-26 03:45:17.000000 otoole-1.0.3/.zenodo.json
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      217 2023-02-26 03:45:17.000000 otoole-1.0.3/AUTHORS.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3643 2023-05-03 20:17:54.000000 otoole-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      599 2023-04-20 01:42:03.000000 otoole-1.0.3/CITATION.cff
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1125 2023-05-03 20:17:54.000000 otoole-1.0.3/LICENSE.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-05-03 20:29:19.413532 otoole-1.0.3/PKG-INFO
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1870 2023-05-03 17:17:12.000000 otoole-1.0.3/README.rst
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.313532 otoole-1.0.3/docs/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1154 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/Makefile
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.333532 otoole-1.0.3/docs/_static/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       18 2023-02-26 01:13:12.000000 otoole-1.0.3/docs/_static/.gitignore
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   135029 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/OSeMOSYS.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    61672 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/logo.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56337 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/osemosys_dataflow.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5597 2023-04-20 00:31:02.000000 otoole-1.0.3/docs/_static/otoole_figures.drawio
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   178856 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/overview.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   168226 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/overview_v2.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    95949 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/simplicity_res.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56119 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/validataion_model.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   217753 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/_static/workflow.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       41 2023-02-26 01:13:12.000000 otoole-1.0.3/docs/authors.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-02-26 01:13:12.000000 otoole-1.0.3/docs/changelog.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10329 2023-05-03 20:17:54.000000 otoole-1.0.3/docs/conf.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12051 2023-05-03 17:17:12.000000 otoole-1.0.3/docs/contributing.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12002 2023-05-03 20:17:54.000000 otoole-1.0.3/docs/data.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10846 2023-05-03 20:17:54.000000 otoole-1.0.3/docs/examples.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8270 2023-05-03 17:17:12.000000 otoole-1.0.3/docs/functionality.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1334 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/index.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1116 2023-02-26 03:45:17.000000 otoole-1.0.3/docs/install.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       67 2023-02-26 01:13:12.000000 otoole-1.0.3/docs/license.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      286 2023-05-03 20:17:54.000000 otoole-1.0.3/docs/requirements.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      355 2023-02-26 03:45:17.000000 otoole-1.0.3/pyproject.toml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      125 2023-04-20 01:42:03.000000 otoole-1.0.3/requirements.txt
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.333532 otoole-1.0.3/scripts/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      760 2023-02-26 01:13:12.000000 otoole-1.0.3/scripts/prepare_cbc.sh
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      824 2023-02-26 01:13:12.000000 otoole-1.0.3/scripts/prepare_cbc_short.sh
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1440 2023-05-03 20:29:19.433532 otoole-1.0.3/setup.cfg
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      703 2023-02-26 03:45:17.000000 otoole-1.0.3/setup.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.273532 otoole-1.0.3/src/
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.353532 otoole-1.0.3/src/otoole/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1059 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    15167 2023-03-31 16:26:19.000000 otoole-1.0.3/src/otoole/cli.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4546 2023-05-03 17:17:12.000000 otoole-1.0.3/src/otoole/exceptions.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18758 2023-05-03 20:17:54.000000 otoole-1.0.3/src/otoole/input.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.363532 otoole-1.0.3/src/otoole/preprocess/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.3/src/otoole/preprocess/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10703 2023-05-03 20:17:54.000000 otoole-1.0.3/src/otoole/preprocess/config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2303 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/preprocess/longify_data.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1183 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/preprocess/setup.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6026 2023-05-03 20:17:54.000000 otoole-1.0.3/src/otoole/preprocess/validate_config.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    13306 2023-04-20 01:42:03.000000 otoole-1.0.3/src/otoole/read_strategies.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.373532 otoole-1.0.3/src/otoole/results/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.3/src/otoole/results/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    32615 2023-04-20 01:42:03.000000 otoole-1.0.3/src/otoole/results/result_package.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11189 2023-05-03 20:17:54.000000 otoole-1.0.3/src/otoole/results/results.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8135 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/utils.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6344 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/validate.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4207 2023-02-26 01:13:12.000000 otoole-1.0.3/src/otoole/validate.yaml
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.383532 otoole-1.0.3/src/otoole/visualise/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      328 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/visualise/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     7101 2023-02-26 03:45:17.000000 otoole-1.0.3/src/otoole/visualise/res.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6749 2023-05-03 20:17:54.000000 otoole-1.0.3/src/otoole/write_strategies.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.363532 otoole-1.0.3/src/otoole.egg-info/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/PKG-INFO
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2330 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/SOURCES.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/dependency_links.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/entry_points.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-05-03 20:29:18.000000 otoole-1.0.3/src/otoole.egg-info/not-zip-safe
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      170 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/requires.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        7 2023-05-03 20:29:19.000000 otoole-1.0.3/src/otoole.egg-info/top_level.txt
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.403532 otoole-1.0.3/tests/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3649 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/conftest.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.413532 otoole-1.0.3/tests/fixtures/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   130205 2023-04-20 01:42:03.000000 otoole-1.0.3/tests/fixtures/combined_inputs.xlsx
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10703 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/fixtures/config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4098 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/fixtures/config_r.yaml
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.413532 otoole-1.0.3/tests/fixtures/data/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      182 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/fixtures/data/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       29 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/fixtures/data/AvailabilityFactor.csv
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    44422 2023-02-26 01:13:12.000000 otoole-1.0.3/tests/fixtures/simplicity-v0.2.1.zip
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    43735 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/fixtures/simplicity.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    75398 2023-02-26 01:13:12.000000 otoole-1.0.3/tests/fixtures/simplicity.xlsx
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-05-03 20:29:19.413532 otoole-1.0.3/tests/results/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    28520 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/results/test_results_package.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4802 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/test_cli.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2149 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/test_convert.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18088 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/test_input.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    41641 2023-04-20 01:42:03.000000 otoole-1.0.3/tests/test_read_strategies.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1802 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/test_setup.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5060 2023-04-20 01:42:03.000000 otoole-1.0.3/tests/test_utils.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5223 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/test_validate.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12004 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/test_validate_config.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      377 2023-02-26 03:45:17.000000 otoole-1.0.3/tests/test_visualise.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     7304 2023-05-03 20:17:54.000000 otoole-1.0.3/tests/test_write_strategies.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2553 2023-03-30 17:38:39.000000 otoole-1.0.3/tox.ini
```

### Comparing `otoole-1.0.2/.coveragerc` & `otoole-1.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `otoole-1.0.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/.github/ISSUE_TEMPLATE/docs.yaml` & `otoole-1.0.3/.github/ISSUE_TEMPLATE/docs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Documentation
 description: Issues relating to documentation
-title: "[DOCS] <Replace with short description of documentation issue>"
+title: "[DOCS]: <Replace with short description of documentation issue>"
 labels: ["documentation"]
 body:
 
 - type: dropdown
   id: issuetype
   attributes:
     label: Type of documentation issue.
```

### Comparing `otoole-1.0.2/.github/ISSUE_TEMPLATE/feature.yaml` & `otoole-1.0.3/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Feature request
-description: Ideas to improve the otoole
-title: "[FEATURE] <Replace with short description of feature request>"
+description: Ideas to improve otoole
+title: "[FEATURE]: <Replace with short description of feature request>"
 labels: ["enhancement"]
 body:
 
 - type: textarea
   id: request
   attributes:
     label: Feature Request
```

### Comparing `otoole-1.0.2/.github/workflows/python.yaml` & `otoole-1.0.3/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/.gitignore` & `otoole-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/.pre-commit-config.yaml` & `otoole-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/.zenodo.json` & `otoole-1.0.3/.zenodo.json`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/CHANGELOG.rst` & `otoole-1.0.3/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 =========
 Changelog
 =========
-Version 1.0
-===========
+
+Version 1.0.3
+=============
+- Improved error message for multiple names mismatches
+- Fix for excel pivoting bug (issue 171)
+- Fix data type casting issue for floats to ints (issue 167)
+- Deprecates calculated field for Result definitions in config file (issue 173)
+- Minor documentation updates
+
+Version 1.0.2
+=============
+- Fix of pandas version in setup.cfg
+
+Version 1.0.1
+=============
+- Updates to citation file
+- Relink to coveralls
+- Upgrade to pandas 2.0
+- Add issue and PR templates
+- Add reading checks between config file and input data
+
+Version 1.0.0
+=============
 - Requires explicit provision of a user-defined configuration file for otoole to workbook
 - Deprecates datapackage fuctionality
 - Adds setup command to generate template config.yaml and csv files
 - Documentation update
 - Bumped pyscaffold to 4.2
 - Otoole now requires Python 3.8 or later
 
+Version 0.11.0
+==============
+- Foundation for user defined configuration
+- Fix for issue #101
+- Better writing of floating point numbers as text
+
+Version 0.10.0
+==============
+- Adds support for OSeMOSYS v1.0, Gurobi and CBC
+
 Version 0.9
 ===========
 - Adds support for processing Gurobi solution files
 - Better handling of datatypes when converting datapackages
 - Fixing bugs on Windows where empty lines were written out during conversion to datapackage
 
 Version 0.8
```

### Comparing `otoole-1.0.2/CITATION.cff` & `otoole-1.0.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/LICENSE.txt` & `otoole-1.0.3/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Will Usher
+Copyright (c) 2023 Will Usher, Trevor Barnes, Hauke Henke, Christoph Muschner
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `otoole-1.0.2/PKG-INFO` & `otoole-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
```

### Comparing `otoole-1.0.2/README.rst` & `otoole-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/Makefile` & `otoole-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/OSeMOSYS.png` & `otoole-1.0.3/docs/_static/OSeMOSYS.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/logo.png` & `otoole-1.0.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/osemosys_dataflow.png` & `otoole-1.0.3/docs/_static/osemosys_dataflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/otoole_figures.drawio` & `otoole-1.0.3/docs/_static/otoole_figures.drawio`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/overview.png` & `otoole-1.0.3/docs/_static/overview.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/overview_v2.png` & `otoole-1.0.3/docs/_static/overview_v2.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/simplicity_res.png` & `otoole-1.0.3/docs/_static/simplicity_res.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/validataion_model.png` & `otoole-1.0.3/docs/_static/validataion_model.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/_static/workflow.png` & `otoole-1.0.3/docs/_static/workflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/conf.py` & `otoole-1.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     "use_repository_button": True,
     "use_edit_page_button": True,
     "extra_navbar":
         """
         <p>Theme by the <a href="https://executablebooks.org/en/latest/">Executable Book Project</a></p>
         <p>Logo by <a href="https://looka.com/">looka.com</a></p>
         """,
+    "icon_links": [],
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
```

### Comparing `otoole-1.0.2/docs/contributing.rst` & `otoole-1.0.3/docs/contributing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,27 +45,27 @@
 
 ``otoole`` documentation uses Sphinx_ as its main documentation compiler.
 This means that the docs are kept in the same repository as the project code, and
 that any documentation update is done in the same way was a code contribution.
 
 Our documentation is written in reStructuredText_.
 
-   .. tip::
-      Please notice that the `GitHub web interface`_ provides a quick way of
-      propose changes in ``otoole``'s files. While this mechanism can
-      be tricky for normal code contributions, it works perfectly fine for
-      contributing to the docs, and can be quite handy.
-
-      If you are interested in trying this method out, please navigate to
-      the ``docs`` folder in the source repository_, find which file you
-      would like to propose changes and click in the little pencil icon at the
-      top, to open `GitHub's code editor`_. Once you finish editing the file,
-      please write a message in the form at the bottom of the page describing
-      which changes have you made and what are the motivations behind them and
-      submit your proposal.
+.. tip::
+    Please notice that the `GitHub web interface`_ provides a quick way of
+    propose changes in ``otoole``'s files. While this mechanism can
+    be tricky for normal code contributions, it works perfectly fine for
+    contributing to the docs, and can be quite handy.
+
+    If you are interested in trying this method out, please navigate to
+    the ``docs`` folder in the source repository_, find which file you
+    would like to propose changes and click in the little pencil icon at the
+    top, to open `GitHub's code editor`_. Once you finish editing the file,
+    please write a message in the form at the bottom of the page describing
+    which changes have you made and what are the motivations behind them and
+    submit your proposal.
 
 When working on documentation changes in your local machine, you can
 compile them using |tox|_::
 
     tox -e docs
 
 and use Python's built-in web server for a preview in your web browser
```

### Comparing `otoole-1.0.2/docs/data.rst` & `otoole-1.0.3/docs/data.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 .. _dataformats:
 
 ============
 Data Formats
 ============
 
+This page explains the different data formatting options available in otoole. Firstly,
+the format of the user configuration file is explained. Following this, the different
+input data formats are explained.
+
+.. SEEALSO::
+   See the Simplicity_ repository for a full example of these formats
+
 User Configuration File
 -----------------------
 
 .. versionadded:: v1.0.0
-    The user configuration file
+    The user configuration file is now required for data conversion
 
 Overview
 ~~~~~~~~
 
 Most commands in ``otoole`` require the user to specify a configuration file that describes
 the ``parameters``, ``sets``, and ``results`` in the model. This configuration file is
 written in ``yaml`` and is typically saved as ``config.yaml``. This section will cover how to
@@ -35,16 +42,17 @@
 +-------------+------+------------+---------+
 | dtype       | X    | X          | X       |
 +-------------+------+------------+---------+
 | type        | X    | X          | X       |
 +-------------+------+------------+---------+
 | default     |      | X          | X       |
 +-------------+------+------------+---------+
-| calculated  |      |            | X       |
-+-------------+------+------------+---------+
+
+.. deprecated:: v1.0.3
+    The ``Calculated`` keyword is no longer needed for Result definitions
 
 .. WARNING::
    Names longer than 31 characters require a ``short_name`` field. This is due
    to character limits on excel sheet names. ``otoole`` will raise an error if a
    ``short_name`` is not provided in these instances.
 
 Sets Format
@@ -84,15 +92,14 @@
 
     AnnualEmissions:
         short_name: ParamName (Optional)
         indices: [SETNAME, SETNAME, ...]
         type: result
         dtype: "int" or "float"
         default: 0
-        calculated: "True" or "False"
 
 .. NOTE::
    It's convention in OSeMOSYS to use Pascal case for result names
 
 Examples
 ~~~~~~~~
 
@@ -117,31 +124,30 @@
 3. Result definition of ``AnnualEmissions``::
 
     AnnualEmissions:
         indices: [REGION,EMISSION,YEAR]
         type: result
         dtype: float
         default: 0
-        calculated: True
+
+.. TIP::
+   See the :ref:`examples` page to create a template configuration file
 
 Input Data
 ----------
 
+.. deprecated:: v1.0.0
+    The ``datapackage`` format is no longer supported
+
 Overview
 ~~~~~~~~
 
 This section will describe how to format data for ``excel``, ``csv``, and ``datafile``
 formats.
 
-.. deprecated:: v1.0.0
-    The ``datapackage`` format is no longer supported
-
-.. SEEALSO::
-   See the Simplicity_ repository for a full example of these formats
-
 Excel
 ~~~~~
 
 Interfacing with ``otoole`` through excel is a very user-friendly method to handle OSeMOSYS
 input data. In the excel workbook (an ``*.xlsx`` file), each sheet will correspond to a
 single parameter or set. Parameters that are indexed over years are pivoted on the ``YEAR``
 index. This creates a wide formatted dataset, where each year is the column header, with
```

### Comparing `otoole-1.0.2/docs/examples.rst` & `otoole-1.0.3/docs/examples.rst`

 * *Files 15% similar despite different names*

```diff
@@ -6,111 +6,135 @@
 
 This page will present examples to show the full functionality of ``otoole``. It will
 walk through the ``convert``, ``results``, ``setup``, ``viz`` and ``validate``
 functionality in seperate simple use cases.
 
 .. NOTE::
     To follow these examples, clone the Simplicity_ repository and run all commands
-    from the ``simplicity/`` directory.
+    from the ``simplicity/`` directory::
+
+        git clone https://github.com/OSeMOSYS/simplicity.git
+        cd simplicity
 
 .. CAUTION::
-    While ``otoole`` does not require any solver, these examples will use the
-    free and open-source tools GLPK_ and CBC_ to build and solve example
-    models.
+    While ``otoole`` does not require a solver, these examples
+    will use the free and open source solvers GLPK_ and CBC_.
+    Installation instructions are described in the `Solver Setup`_ section.
 
-Data Conversion
----------------
+Data Conversion with CSVs
+-------------------------
 
 Objective
 ~~~~~~~~~
 
-Use a folder of CSV data to build and solve an OSeMOSYS model with CBC. Generate
+Use a folder of CSV data to build and solve an OSeMOSYS model with CBC_. Generate
 the full suite of OSeMOSYS results.
 
 1. ``otoole`` Convert
 ~~~~~~~~~~~~~~~~~~~~~
-We first want to convert the folder of Simplicity_ CSVs (``data/``) into
-an OSeMOSYS datafile (``simplicity.txt``)::
+We first want to convert the folder of Simplicity_ CSVs into
+an OSeMOSYS datafile called ``simplicity.txt``::
 
     $ otoole convert csv datafile data simplicity.txt config.yaml
 
 2. Build the Model
 ~~~~~~~~~~~~~~~~~~~
 Use GLPK_ to build the model and save it as ``simplicity.lp``::
 
-    $ glpsol -m osemosys.txt -d simplicity.txt --wlp simplicity.lp --check
+    $ glpsol -m OSeMOSYS.txt -d simplicity.txt --wlp simplicity.lp --check
 
 .. TIP::
     See the `GLPK Wiki`_ for more information on the ``glpsol`` command
 
 3. Solve the Model
 ~~~~~~~~~~~~~~~~~~
 Use CBC_ to solve the model and save the solution file as ``simplicity.sol``::
 
     $ cbc simplicity.lp solve -solu simplicity.sol
 
 4. Generate the full set of results
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Create a folder to hold the results::
-
-    $ mkdir results
-
 Use ``otoole``'s ``result`` package to generate the results file::
 
     $ otoole results cbc csv simplicity.sol results config.yaml
 
-Result Processing
------------------
+5. View Results
+~~~~~~~~~~~~~~~
+Results are now viewable in the files ``results/*.csv``
+
+.. TIP::
+    Before moving onto the next section, remove all the generated files::
+
+        $ rm simplicity.lp simplicity.sol simplicity.txt results/*
+
+Data Conversion with Excel
+--------------------------
 
 Objective
 ~~~~~~~~~
 
-Use an excel worksheet to build and solve an OSeMOSYS model with CBC. Only
-generate the results for ``TotalDiscountedCost`` and ``TotalCapacityAnnual``.
+Use an excel worksheet to build and solve an OSeMOSYS model with CBC.
 
-1. ``otoole`` Convert
-~~~~~~~~~~~~~~~~~~~~~
-We first want to convert the excel workbook (``simplicity.xlsx``) into
-an OSeMOSYS datafile (``simplicity.txt```)::
+1. Create the Excel Workbook
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Use the example CSV data to create an Excel Workbook using ``otoole convert``::
 
-    $ otoole convert excel datafile data simplicity.xlsx config.yaml
+    $ otoole convert csv excel data simplicity.xlsx config.yaml
 
-2. Build the Model
+Excel workbooks are an easy way for humans to interface with OSeMOSYS data!
+
+2. Create the MathProg datafile
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Next, we want to convert the excel workbook (``simplicity.xlsx``) into
+an OSeMOSYS datafile (``simplicity.txt``)::
+
+    $ otoole convert excel datafile simplicity.xlsx simplicity.txt config.yaml
+
+3. Build the Model
 ~~~~~~~~~~~~~~~~~~
 Use GLPK_ to build the model and save it as ``simplicity.lp``::
 
-    $ glpsol -m osemosys.txt -d simplicity.txt --wlp simplicity.lp --check
+    $ glpsol -m OSeMOSYS.txt -d simplicity.txt --wlp simplicity.lp --check
 
-3. Solve the Model
+4. Solve the Model
 ~~~~~~~~~~~~~~~~~~
 Use CBC_ to solve the model and save the solution file as ``simplicity.sol``::
 
-    $ cbc simplicity.sol solve -solu simplicity.sol
+    $ cbc simplicity.lp solve -solu simplicity.sol
 
-4. Modify the Configuration File
+5. Generate the selected results
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Change the ``calculated`` fields for the ``TotalDiscountedCost`` and ``TotalCapacityAnnual``
-values to ``True``, and set all other ``calculated`` fields to ``False``::
+Use ``otoole``'s ``result`` package to generate the result CSVs::
 
-    TotalCapacityAnnual:
-        indices: [REGION, TECHNOLOGY, YEAR]
-        type: result
-        dtype: float
-        default: 0
-        calculated: True
+    $ otoole results cbc csv simplicity.sol results config.yaml
 
-5. Generate the selected results
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Create a folder to hold the results::
+Model Visualization
+-------------------
 
-    $ mkdir results
+Objective
+~~~~~~~~~
 
-Use ``otoole``'s ``result`` package to generate the result CSVs::
+Use ``otoole`` to visualize the reference energy system.
 
-    $ otoole results cbc csv simplicity.sol results config.yaml
+1. ``otoole`` Visualise
+~~~~~~~~~~~~~~~~~~~~~~~
+The visualization functionality of ``otoole`` will work with any supported
+input data format (``csv``, ``datafile``, or ``excel``). In this case, we will
+use the excel file, ``simplicity.xlsx``, to generate the RES.
+
+Run the following command, where the RES will be saved as the file ``res.png``::
+
+    $ otoole viz res excel simplicity.xlsx res.png config.yaml
+
+2. View the RES
+~~~~~~~~~~~~~~~
+Open the newly created file, ``res.png`` and the following image should be
+displayed
+
+.. image:: _static/simplicity_res.png
 
 Template Setup
 --------------
 
 Objective
 ~~~~~~~~~
 
@@ -118,29 +142,29 @@
 ``otoole convert`` commands
 
 1. Create the Configuration File
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Run the following command, to create a template configuration file
 called ``config.yaml``::
 
-    $ otoole setup config config.yaml
+    $ otoole setup config template_config.yaml
 
 2. Create the Template Data CSVs
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ``otoole`` will only generate template CSV data, however, we want to input
 data in Excel format. Therefore, we will first generate CSV data and convert
 it to Excel format::
 
-    $ otoole setup csv data
+    $ otoole setup csv template_data
 
 3. Add Year Definitions
 ~~~~~~~~~~~~~~~~~~~~~~~
-Open up the the file ``data/YEARS.csv`` and add all the years over the model
+Open up the the file ``template_data/YEARS.csv`` and add all the years over the model
 horizon. For example, if the model horizon is from 2020 to 2050, the
-``data/YEARS.csv`` file should be formatted as follows:
+``template_data/YEARS.csv`` file should be formatted as follows:
 
 +---------+
 | VALUE   |
 +=========+
 | 2020    |
 +---------+
 | 2021    |
@@ -158,45 +182,21 @@
    during the conversion process. This will save significant formatting time!
 
 4. Convert the CSV Template Data
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 To convert the template CSV data into Excel formatted data, run the following
 ``convert`` command::
 
-    $ otoole convert csv excel data data.xlsx config.yaml
+    $ otoole convert csv excel template_data template.xlsx template_config.yaml
 
 5. Add Model Data
 ~~~~~~~~~~~~~~~~~
-There should now be a file called ``data.xlsx`` that the user can open and
+There should now be a file called ``template.xlsx`` that the user can open and
 add data to.
 
-Model Visualization
--------------------
-
-Objective
-~~~~~~~~~
-
-Use ``otoole`` to visualize the reference energy system.
-
-1. ``otoole`` Visualise
-~~~~~~~~~~~~~~~~~~~~~~~
-The visualization functionality of ``otoole`` will work with any supported
-input data format (``csv``, ``datafile``, or ``excel``). In this case, we will
-use the excel file, ``simplicity.xlsx``, to generate the RES.
-
-Run the following command, where the RES will be saved as the file ``res.png``::
-
-    $ otoole viz res excel simplicity.xlsx res.png config.yaml
-
-2. View the RES
-~~~~~~~~~~~~~~~
-Open the newly created file, ``res.png`` and the following image should be
-displayed
-
-.. image:: _static/simplicity_res.png
 
 Model Validation
 ----------------
 
 .. NOTE::
     In this example, we will use a very simple model instead of the
     Simplicity_ demonstration model. This way the user does not need to be
@@ -281,16 +281,15 @@
     $ otoole validate datafile data.txt config.yaml --validate_config validate.yaml
 
 .. WARNING::
     Do not confuse the user configuation file (``config.yaml``) and the
     validation configuation file (``validate.yaml``). Both configuartion files
     are required for validation functionality.
 
-.. NOTE::
-   The final validation configuration file in this example will look like::
+The final validation configuration file in this example will look like::
 
     codes:
       fuels:
         'WND': Wind
         'COA': Coal
         'ELC': Electricity
       indetifiers:
@@ -318,13 +317,79 @@
           - name: techs
           valid: techs
           position: (1, 3)
           - name: fuels
           valid: fuels
           position: (4, 6)
 
+Solver Setup
+------------
+
+Objective
+~~~~~~~~~
+
+Install GLPK_ and CBC_ to use in the otoole examples.
+
+1. Install GLPK
+~~~~~~~~~~~~~~~~
+
+GLPK_ is a free and open-source linear program solver.
+
+To install it on **Linux**, run the command::
+
+    sudo apt-get update
+    sudo apt-get install glpk glpk-utils
+
+To install it on **Mac**, run the command::
+
+    brew install glpk
+
+.. To install it on **Windows**, follow the install instruction on the GLPK_
+.. website, and/or follow the instructions_ from the OSeMOSYS community
+
+2. Test the GLPK install
+~~~~~~~~~~~~~~~~~~~~~~~~
+Once installed, you should be able to call the ``glpsol`` command::
+
+    $ glpsol
+    GLPSOL: GLPK LP/MIP Solver, v4.65
+    No input problem file specified; try glpsol --help
+
+3. Install CBC
+~~~~~~~~~~~~~~
+
+CBC_ is a free and open-source mixed integer linear programming solver. Full
+install instructions can be found on the CBC_ website. However, the abbreviated
+instructions are shown below
+
+To install it on **Linux**, run the command::
+
+    sudo apt-get install coinor-cbc coinor-libcbc-dev
+
+To install it on **Mac**, run the command::
+
+    brew install coin-or-tools/coinor/cbc
+
+.. To install it on **Windows**, follow the install instruction on the CBC_
+.. website by downloading a binary
+
+4. Test the CBC install
+~~~~~~~~~~~~~~~~~~~~~~~
+Once installed, you should be able to directly call CBC::
+
+    $ cbc
+    Welcome to the CBC MILP Solver
+    Version: 2.10.3
+    Build Date: Mar 24 2020
+
+    CoinSolver takes input from arguments ( - switches to stdin)
+    Enter ? for list of commands or help
+    Coin:
+
+You can exit the solver by typing ``quit``
 
 .. _Simplicity: https://github.com/OSeMOSYS/simplicity
 .. _GLPK: https://www.gnu.org/software/glpk/
 .. _GLPK Wiki: https://en.wikibooks.org/wiki/GLPK/Using_GLPSOL
 .. _CBC: https://github.com/coin-or/Cbc
 .. _CPLEX: https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer
+.. _instructions: http://www.osemosys.org/uploads/1/8/5/0/18504136/glpk_installation_guide_for_windows10_-_201702.pdf
```

### Comparing `otoole-1.0.2/docs/functionality.rst` & `otoole-1.0.3/docs/functionality.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,23 @@
 
 Data Conversion
 ---------------
 
 Overview
 ~~~~~~~~
 
-``otoole`` supports many data pre-processing conversions so as to ease the tasks of
+``otoole`` supports different data pre-processing conversions so as to ease the tasks of
 the OSeMOSYS modeller. The modeller can generate data in any one of the formats and
 convert it to another format through a ``convert`` command. ``otoole`` currently supports
 conversion between the following formats:
 
 - Excel
 - A folder of CSV files
 - GNU MathProg datafile
 
-.. deprecated:: v1.0.0
-    The ``datapackage`` format is no longer supported
-
 ``otoole convert``
 ~~~~~~~~~~~~~~~~~~
 
 THe ``otoole convert``` command allows you to convert between various different
 input formats::
 
     $ otoole convert --help
@@ -55,14 +52,17 @@
     config                Path to config YAML file
 
     optional arguments:
     -h, --help            show this help message and exit
     --write_defaults      Writes default values
     --keep_whitespace     Keeps leading/trailing whitespace
 
+.. deprecated:: v1.0.0
+    The ``datapackage`` format is no longer supported
+
 .. versionadded:: v1.0.0
     The ``config`` positional argument is now required
 
 Result Processing
 -----------------
 
 Overview
@@ -125,15 +125,15 @@
 Setup
 -----
 The ``setup`` module in ``otoole`` allows you to generate template files to
 quickly get up and running.
 
 ``otoole setup``
 ~~~~~~~~~~~~~~~~
-The ``setup``command allows you to generate a template user configuration file,
+The ``setup`` command allows you to generate a template user configuration file,
 useful for ``conversion`` and ``result`` commands, and template input ``csv``
 data::
 
     $ otoole setup --help
 
     usage: otoole setup [-h] [--write_defaults] [--overwrite] {config,csv} data_path
```

### Comparing `otoole-1.0.2/docs/index.rst` & `otoole-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/docs/install.rst` & `otoole-1.0.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/scripts/prepare_cbc.sh` & `otoole-1.0.3/scripts/prepare_cbc.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/scripts/prepare_cbc_short.sh` & `otoole-1.0.3/scripts/prepare_cbc_short.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/setup.cfg` & `otoole-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/setup.py` & `otoole-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/__init__.py` & `otoole-1.0.3/src/otoole/__init__.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/cli.py` & `otoole-1.0.3/src/otoole/cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/exceptions.py` & `otoole-1.0.3/src/otoole/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import List, Union
+
+
 class OtooleException(Exception):
     """Base class for all otoole exceptions."""
 
     pass
 
 
 class OtooleValidationError(OtooleException):
@@ -73,23 +76,28 @@
 
 
 class OtooleNameMismatchError(OtooleException):
     """Names not consistent between read in data and config file"""
 
     def __init__(
         self,
-        name: str,
-        message: str = "Name not consistent between data and config file",
+        name: Union[List, str],
     ) -> None:
-        self.name = name
-        self.message = message
+        if isinstance(name, list):
+            self.message = "Names not consistent between data and config file"
+            self.name = ", ".join(sorted(name))
+        elif isinstance(name, str):
+            self.name = name
+            self.message = "Name not consistent between data and config file"
+        else:
+            raise TypeError("Incorrect type passed to OtooleNameMismatchError")
         super().__init__(self.message)
 
     def __str__(self):
-        return f"{self.name} -> {self.message}"
+        return f"{self.message}:\n\n{self.name}.\n\nUpdate config or data with matching names."
 
 
 class OtooleDeprecationError(OtooleException):
     """New version of otoole does drops this feature support
 
     Arguments
     ---------
```

### Comparing `otoole-1.0.2/src/otoole/input.py` & `otoole-1.0.3/src/otoole/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,23 +414,23 @@
         ------
         OtooleIndexError
             If actual indices do not match expected indices
         """
 
         actual_indices = df.index.names
         if actual_indices[0] is None:  # for ReadMemory
-            logger.debug(f"No mulit-index identified for {name}")
+            logger.debug(f"No multi-index identified for {name}")
             actual_indices = list(df)[:-1]  # Drop "VALUE"
 
         logger.debug(f"Actual indices for {name} are {actual_indices}")
         try:
             expected_indices = config["indices"]
             logger.debug(f"Expected indices for {name} are {expected_indices}")
         except KeyError:
-            logger.debug(f"No expected indices identifed for {name}")
+            logger.debug(f"No expected indices identified for {name}")
             return
 
         if actual_indices == expected_indices:
             return
         else:
             raise OtooleIndexError(
                 resource=name,
@@ -489,20 +489,30 @@
             except KeyError:
                 logger.debug("Unable to set index on {}".format(name))
                 pass
 
             logger.debug("Column dtypes identified: {}".format(config["index_dtypes"]))
             logger.debug(df.head())
             # Drop empty rows
-            df = (
-                df.dropna(axis=0, how="all")
-                .reset_index()
-                .astype(config["index_dtypes"])
-                .set_index(config["indices"])
-            )
+            try:
+                df = (
+                    df.dropna(axis=0, how="all")
+                    .reset_index()
+                    .astype(config["index_dtypes"])
+                    .set_index(config["indices"])
+                )
+            except ValueError:  # ValueError: invalid literal for int() with base 10:
+                df = df.dropna(axis=0, how="all").reset_index()
+                for index, dtype in config["index_dtypes"].items():
+                    if dtype == "int":
+                        df[index] = df[index].astype(float).astype(int)
+                    else:
+                        df[index] = df[index].astype(dtype)
+                df = df.set_index(config["indices"])
+
         else:
             logger.debug("Identified {} as a set".format(name))
             df = df.astype(config["dtype"])
 
         return df
 
     def _get_missing_input_dataframes(
@@ -572,14 +582,14 @@
                     expected.append(name)
         else:
             expected = [x for x in user_config]
 
         errors = list(set(expected).symmetric_difference(set(names)))
         if errors:
             logger.debug(f"data and config name errors are: {errors}")
-            raise OtooleNameMismatchError(name=errors[0])
+            raise OtooleNameMismatchError(name=errors)
 
     @abstractmethod
     def read(
         self, filepath: Union[str, TextIO], **kwargs
     ) -> Tuple[Dict[str, pd.DataFrame], Dict[str, Any]]:
         raise NotImplementedError()
```

### Comparing `otoole-1.0.2/src/otoole/preprocess/config.yaml` & `otoole-1.0.3/src/otoole/preprocess/config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -303,210 +303,176 @@
     dtype: float
     default: 0
 AnnualEmissions:
     indices: [REGION,EMISSION,YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AccumulatedNewCapacity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualFixedOperatingCost:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualTechnologyEmission:
     indices: [REGION, TECHNOLOGY, EMISSION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualTechnologyEmissionByMode:
     indices: [REGION, TECHNOLOGY, EMISSION, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualVariableOperatingCost:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 CapitalInvestment:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 Demand:
     indices: [REGION, TIMESLICE, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 DiscountedSalvageValue:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 DiscountedTechnologyEmissionsPenalty:
     short_name: DiscountedTechEmissionsPenalty
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NewCapacity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NewStorageCapacity:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NumberOfNewTechnologyUnits:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 ProductionByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 ProductionByTechnologyAnnual:
     indices: [REGION, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfActivity:
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 RateOfProductionByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfProductionByTechnologyByMode:
     short_name: RateOfProductionByTechByMode
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfUseByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfUseByTechnologyByMode:
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 SalvageValue:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 SalvageValueStorage:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelDayTypeFinish:
     indices: [REGION, STORAGE, SEASON, DAYTYPE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelDayTypeStart:
     indices: [REGION, STORAGE, SEASON, DAYTYPE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelSeasonStart:
     indices: [REGION, STORAGE, SEASON, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelYearStart:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelYearFinish:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 TotalAnnualTechnologyActivityByMode:
     short_name: TotalAnnualTechActivityByMode
     indices: [REGION, TECHNOLOGY, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalCapacityAnnual:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalDiscountedCost:
     indices: [REGION,YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalTechnologyAnnualActivity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalTechnologyModelPeriodActivity:
     short_name: TotalTechModelPeriodActivity
     indices: [REGION, TECHNOLOGY]
     type: result
     dtype: float
     default: 0
-    calculated: True
 Trade:
     indices: [REGION, REGION, TIMESLICE, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 UseByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
```

### Comparing `otoole-1.0.2/src/otoole/preprocess/longify_data.py` & `otoole-1.0.3/src/otoole/preprocess/longify_data.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/preprocess/setup.py` & `otoole-1.0.3/src/otoole/preprocess/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/preprocess/validate_config.py` & `otoole-1.0.3/src/otoole/preprocess/validate_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,26 +70,26 @@
         return values
 
     class Config:
         extra = "forbid"
 
 
 class UserDefinedSet(UserDefinedValue):
-    """Represents a parameter"""
+    """Represents a set"""
 
     @validator("dtype")
     @classmethod
     def check_dtype(cls, value, values):
         if value not in ["str", "int"]:
             raise ValueError(f"{values['name']} -> Value must be a 'str' or 'int'")
         return value
 
 
 class UserDefinedParameter(UserDefinedValue):
-    """Represents a user defined parameter"""
+    """Represents a parameter"""
 
     @validator("dtype")
     @classmethod
     def check_dtype(cls, value, values):
         if value not in ["float", "int"]:
             raise ValueError(f"{values['name']} -> Value must be an 'int' or 'float'")
         return value
@@ -122,35 +122,46 @@
                 raise ValueError(
                     f"{values['name']} -> User dtype is {dtype_input} while default value dtype is {dtype_default}"
                 )
         return values
 
 
 class UserDefinedResult(UserDefinedValue):
-    """Represents a parameter"""
+    """Represents a result"""
 
     @validator("dtype")
     @classmethod
     def check_dtype(cls, value, values):
         if value not in ["float", "int"]:
             raise ValueError(f"{values['name']} -> Value must be an 'int' or 'float'")
         return value
 
     @root_validator(pre=True)
     @classmethod
     def check_required_inputs(cls, values):
-        required = ["default", "defined_sets", "indices", "calculated"]
+        required = ["default", "defined_sets", "indices"]
         if not all(req in values for req in required):
             raise ValueError(
-                f"{values['name']} -> Missing one of required fields ('default', 'defined_sets', 'indices', calculated)"
+                f"{values['name']} -> Missing one of required fields ('default', 'defined_sets', 'indices')"
             )
         return values
 
     @root_validator(pre=True)
     @classmethod
+    def check_deprecated_values(cls, values):
+        deprecated = ["calculated", "Calculated"]
+        for v in values:
+            if v in deprecated:
+                logger.info(
+                    f"{values['name']} -> Config file field of '{v}' is deprecated. Remove '{v}' to suppress this warning."
+                )
+        return values
+
+    @root_validator(pre=True)
+    @classmethod
     def check_index_in_set(cls, values):
         if not all(i in values["defined_sets"] for i in values["indices"]):
             raise ValueError(f"{values['name']} -> Index not in user supplied sets")
         return values
 
     @root_validator(pre=True)
     @classmethod
```

### Comparing `otoole-1.0.2/src/otoole/read_strategies.py` & `otoole-1.0.3/src/otoole/read_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/results/result_package.py` & `otoole-1.0.3/src/otoole/results/result_package.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/results/results.py` & `otoole-1.0.3/src/otoole/results/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
             file_path,
             header=None,
             sep=" ",
             names=["Variable", "Value"],
             skiprows=2,
         )  # type: pd.DataFrame
         df[["Variable", "Index"]] = df["Variable"].str.split("(", expand=True)
-        df["Index"] = df["Index"].str.replace(")", "")
+        df["Index"] = df["Index"].str.replace(")", "", regex=False)
         LOGGER.debug(df)
         df = df[(df["Value"] != 0)].reset_index()
         return df[["Variable", "Index", "Value"]].astype({"Value": float})
 
 
 class ReadCbc(ReadResultsCBC):
     """Read a CBC solution file into memory
@@ -321,10 +321,10 @@
         df["Variable"] = (
             df["Variable"]
             .astype(str)
             .str.replace(r"^\*\*", "", regex=True)
             .str.split(expand=True)[1]
         )
         df[["Index", "Value"]] = df["indexvalue"].str.split(expand=True).loc[:, 0:1]
-        df["Index"] = df["Index"].str.replace(")", "")
+        df["Index"] = df["Index"].str.replace(")", "", regex=False)
         df = df.drop(columns=["indexvalue"])
         return df[["Variable", "Index", "Value"]].astype({"Value": float})
```

### Comparing `otoole-1.0.2/src/otoole/utils.py` & `otoole-1.0.3/src/otoole/utils.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/validate.py` & `otoole-1.0.3/src/otoole/validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/validate.yaml` & `otoole-1.0.3/src/otoole/validate.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/visualise/res.py` & `otoole-1.0.3/src/otoole/visualise/res.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/src/otoole/write_strategies.py` & `otoole-1.0.3/src/otoole/write_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
             names = index_names + column_names
         else:
             names = column_names
         logger.debug(f"Identified {len(names)} names: {names}")
 
         total_columns = len(names)
 
-        if total_columns > 3:
+        if "YEAR" not in names:
+            pivot = df.copy()
+        elif total_columns > 3:
             logger.debug("More than 3 columns for {}: {}".format(parameter_name, names))
             rows = names[0:-2]
             columns = names[-2]
             values = names[-1]
             logger.debug(f"Rows: {rows}; columns: {columns}; values: {values}")
             logger.debug("dtypes: {}".format(df.dtypes))
             pivot = df.reset_index().pivot(index=rows, columns=columns, values=values)
```

### Comparing `otoole-1.0.2/src/otoole.egg-info/PKG-INFO` & `otoole-1.0.3/src/otoole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
```

### Comparing `otoole-1.0.2/src/otoole.egg-info/SOURCES.txt` & `otoole-1.0.3/src/otoole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/conftest.py` & `otoole-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/fixtures/combined_inputs.xlsx` & `otoole-1.0.3/tests/fixtures/combined_inputs.xlsx`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/fixtures/config.yaml` & `otoole-1.0.3/tests/fixtures/config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -303,210 +303,176 @@
     dtype: float
     default: 0
 AnnualEmissions:
     indices: [REGION,EMISSION,YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AccumulatedNewCapacity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualFixedOperatingCost:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualTechnologyEmission:
     indices: [REGION, TECHNOLOGY, EMISSION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualTechnologyEmissionByMode:
     indices: [REGION, TECHNOLOGY, EMISSION, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 AnnualVariableOperatingCost:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 CapitalInvestment:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 Demand:
     indices: [REGION, TIMESLICE, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 DiscountedSalvageValue:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 DiscountedTechnologyEmissionsPenalty:
     short_name: DiscountedTechEmissionsPenalty
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NewCapacity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NewStorageCapacity:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 NumberOfNewTechnologyUnits:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 ProductionByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 ProductionByTechnologyAnnual:
     indices: [REGION, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfActivity:
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 RateOfProductionByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfProductionByTechnologyByMode:
     short_name: RateOfProductionByTechByMode
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfUseByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 RateOfUseByTechnologyByMode:
     indices: [REGION, TIMESLICE, TECHNOLOGY, MODE_OF_OPERATION, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 SalvageValue:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 SalvageValueStorage:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelDayTypeFinish:
     indices: [REGION, STORAGE, SEASON, DAYTYPE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelDayTypeStart:
     indices: [REGION, STORAGE, SEASON, DAYTYPE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelSeasonStart:
     indices: [REGION, STORAGE, SEASON, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelYearStart:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 StorageLevelYearFinish:
     indices: [REGION, STORAGE, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 TotalAnnualTechnologyActivityByMode:
     short_name: TotalAnnualTechActivityByMode
     indices: [REGION, TECHNOLOGY, MODE_OF_OPERATION, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalCapacityAnnual:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalDiscountedCost:
     indices: [REGION,YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalTechnologyAnnualActivity:
     indices: [REGION, TECHNOLOGY, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: True
 TotalTechnologyModelPeriodActivity:
     short_name: TotalTechModelPeriodActivity
     indices: [REGION, TECHNOLOGY]
     type: result
     dtype: float
     default: 0
-    calculated: True
 Trade:
     indices: [REGION, REGION, TIMESLICE, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
 UseByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
-    calculated: False
```

### Comparing `otoole-1.0.2/tests/fixtures/simplicity-v0.2.1.zip` & `otoole-1.0.3/tests/fixtures/simplicity-v0.2.1.zip`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/fixtures/simplicity.txt` & `otoole-1.0.3/tests/fixtures/simplicity.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/fixtures/simplicity.xlsx` & `otoole-1.0.3/tests/fixtures/simplicity.xlsx`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/results/test_results_package.py` & `otoole-1.0.3/tests/results/test_results_package.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_cli.py` & `otoole-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_convert.py` & `otoole-1.0.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_input.py` & `otoole-1.0.3/tests/test_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,17 +339,17 @@
             ["SIMPLICITY", "NGCC", 2016, 3.45],
         ],
         columns=["REGION", "TECHNOLOGY", "YEAR", "VALUE"],
     ).set_index(["REGION", "TECHNOLOGY", "YEAR"])
 
     capex_incorrect_dtype = pd.DataFrame(
         data=[
-            ["SIMPLICITY", "NGCC", "2014", 1.23],
-            ["SIMPLICITY", "NGCC", "2015", 2.34],
-            ["SIMPLICITY", "NGCC", "2016", 3.45],
+            ["SIMPLICITY", "NGCC", "2014", "1.23"],
+            ["SIMPLICITY", "NGCC", 2015.0, 2.34],
+            ["SIMPLICITY", "NGCC", "2016.0", 3.45],
         ],
         columns=["REGION", "TECHNOLOGY", "YEAR", "VALUE"],
     ).set_index(["REGION", "TECHNOLOGY", "YEAR"])
 
     capex_incorrect_header = pd.DataFrame(
         data=[
             ["SIMPLICITY", "NGCC", 2014, 1.23],
@@ -361,15 +361,17 @@
 
     year_correct = pd.DataFrame(data=[2014, 2015, 2016], columns=["VALUE"])
 
     year_incorrect_dtype = pd.DataFrame(
         data=["2014", "2015", "2016"], columns=["VALUE"]
     )
 
-    year_incorrect_header = pd.DataFrame(data=[2014, 2015, 2016], columns=["YEAR"])
+    year_incorrect_header = pd.DataFrame(
+        data=["2014", 2015.0, "2016.0"], columns=["YEAR"]
+    )
 
     input_data_correct = (
         ({"CapitalCost": capex_correct}, capex_correct),
         ({"YEAR": year_correct}, year_correct),
     )
 
     input_data_incorrect_dtype = (
```

### Comparing `otoole-1.0.2/tests/test_read_strategies.py` & `otoole-1.0.3/tests/test_read_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_setup.py` & `otoole-1.0.3/tests/test_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             "type": "set",
         },
         "Demand": {
             "indices": ["REGION", "TIMESLICE", "FUEL", "YEAR"],
             "type": "result",
             "dtype": "float",
             "default": 0,
-            "calculated": True,
         },
     }
 
     accumulated_annual_demand = pd.DataFrame(
         columns=["REGION", "FUEL", "YEAR", "VALUE"]
     ).astype(
         {
```

### Comparing `otoole-1.0.2/tests/test_utils.py` & `otoole-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_validate.py` & `otoole-1.0.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.2/tests/test_validate_config.py` & `otoole-1.0.3/tests/test_validate_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,76 @@
     valid_set = """
         SET_NAME:
           dtype: str
           type: set
           short_name: SET
     """
 
-    valid_parameter = """
+    valid_parameter_1 = """
+        Parameter_Name:
+          indices: [SET]
+          type: param
+          dtype: float
+          default: 0
+        SET:
+          dtype: str
+          type: set
+    """
+
+    valid_parameter_2 = """
         Parameter_Name:
           indices: [SET]
           type: param
           dtype: float
           default: 0
           short_name: Parameter
         SET:
           dtype: str
           type: set
     """
 
-    valid_result = """
+    valid_result_1 = """
+        Result_Name:
+          indices: [SET]
+          type: result
+          dtype: float
+          default: 0
+        SET:
+          dtype: str
+          type: set
+    """
+
+    valid_result_2 = """
         Result_Name:
           indices: [SET]
           type: result
           dtype: float
           default: 0
           calculated: True
           short_name: Result
         SET:
           dtype: str
           type: set
     """
 
-    config_data = [valid_set, valid_parameter, valid_result]
+    config_data = [
+        valid_set,
+        valid_parameter_1,
+        valid_parameter_2,
+        valid_result_1,
+        valid_result_2,
+    ]
 
-    config_data_ids = ["valid_set", "valid_parameter", "valid_result"]
+    config_data_ids = [
+        "valid_set",
+        "valid_parameter_1",
+        "valid_parameter_2",
+        "valid_result_1",
+        "valid_result_2",
+    ]
 
     @mark.parametrize("config_data", config_data, ids=config_data_ids)
     def test_valid_configs(self, config_data):
         config = load(config_data, Loader=SafeLoader)
         validate_config(config)
 
 
@@ -76,21 +110,19 @@
 
     invalid_duplicate_result_names = """
         Result:
           indices: [SET]
           type: result
           dtype: float
           default: 0
-          calculated: True
         Result:
           indices: [SET]
           type: result
           dtype: float
           default: 0
-          calculated: True
         SET:
           dtype: str
           type: set
     """
 
     invalid_duplicate_names_diff_types_1 = """
         Parameter:
@@ -158,15 +190,14 @@
 
     invalid_result_type = """
         Result:
           indices: [SET]
           type: not_valid_type
           dtype: float
           default: 0
-          calculated: True
         SET:
           dtype: str
           type: set
     """
 
     invalid_name_spaces = """
         Parameter With Spaces:
@@ -441,51 +472,47 @@
 
     invalid_unexpected_field = """
         Result:
           indices: [SET]
           type: result
           dtype: float
           default: 0
-          calculated: True
           fieldnotexpected: True
         SET:
           dtype: str
           type: set
     """
 
     invalid_missing_field = """
         Result:
           indices: [SET]
           type: result
           dtype: float
-          default: 0
         SET:
           dtype: str
           type: set
     """
 
     invalid_missing_index = """
         Result:
           indices: [SET, MISSING_SET]
           type: result
           dtype: float
           default: 0
-          calculated: True
         SET:
           dtype: str
           type: set
     """
 
     invalid_default = """
         Result:
           indices: [SET]
           type: result
           dtype: float
           default: s
-          calculated: True
         SET:
           dtype: str
           type: set
     """
 
     config_data = [
         invalid_dtype,
```

### Comparing `otoole-1.0.2/tests/test_write_strategies.py` & `otoole-1.0.3/tests/test_write_strategies.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,34 @@
             index=pd.MultiIndex.from_tuples(
                 [("SIMPLICITY", "COAL")], names=["REGION", "FUEL"]
             ),
         )
 
         pd.testing.assert_frame_equal(actual, expected)
 
+    def test_form_no_pivot(self, user_config):
+
+        convert = WriteExcel(user_config)  # typing: WriteExcel
+
+        # Technology to/from storage data
+        data = [
+            ["SIMPLICITY", "HYD2", "DAM", 1, 0],
+            ["SIMPLICITY", "HYD2", "DAM", 2, 1],
+        ]
+
+        df = pd.DataFrame(
+            data=data,
+            columns=["REGION", "TECHNOLOGY", "STORAGE", "MODE_OF_OPERATION", "VALUE"],
+        ).set_index(["REGION", "TECHNOLOGY", "STORAGE", "MODE_OF_OPERATION"])
+
+        actual = convert._form_parameter(df, "test_parameter", 0)
+        expected = df.copy()
+
+        pd.testing.assert_frame_equal(actual, expected)
+
     def test_write_out_empty_dataframe(self, user_config):
 
         temp_excel = NamedTemporaryFile(suffix=".xlsx")
         handle = pd.ExcelWriter(temp_excel.name)
         convert = WriteExcel(user_config)
 
         df = pd.DataFrame(
```

### Comparing `otoole-1.0.2/tox.ini` & `otoole-1.0.3/tox.ini`

 * *Files identical despite different names*

