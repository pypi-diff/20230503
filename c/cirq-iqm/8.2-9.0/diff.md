# Comparing `tmp/cirq-iqm-8.2.tar.gz` & `tmp/cirq-iqm-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirq-iqm-8.2.tar", last modified: Thu Dec 29 14:14:56 2022, max compression
+gzip compressed data, was "cirq-iqm-9.0.tar", last modified: Wed Jan 11 07:19:44 2023, max compression
```

## Comparing `cirq-iqm-8.2.tar` & `cirq-iqm-9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.652308 cirq-iqm-8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.628308 cirq-iqm-8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.636308 cirq-iqm-8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-29 14:13:38.000000 cirq-iqm-8.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-29 14:13:38.000000 cirq-iqm-8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2022-12-29 14:13:38.000000 cirq-iqm-8.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-29 14:13:38.000000 cirq-iqm-8.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2022-12-29 14:13:38.000000 cirq-iqm-8.2/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-29 14:13:38.000000 cirq-iqm-8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-29 14:14:56.652308 cirq-iqm-8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-29 14:13:38.000000 cirq-iqm-8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.640308 cirq-iqm-8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.628308 cirq-iqm-8.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.640308 cirq-iqm-8.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.640308 cirq-iqm-8.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2022-12-29 14:13:38.000000 cirq-iqm-8.2/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.640308 cirq-iqm-8.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/demo_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/demo_apollo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/demo_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/demo_iqm_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/demo_valkmusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2022-12-29 14:13:38.000000 cirq-iqm-8.2/examples/usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-29 14:13:38.000000 cirq-iqm-8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-29 14:14:56.652308 cirq-iqm-8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2022-12-29 14:13:38.000000 cirq-iqm-8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.632308 cirq-iqm-8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.644308 cirq-iqm-8.2/src/cirq_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.648308 cirq-iqm-8.2/src/cirq_iqm/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/apollo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/iqm_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/iqm_device_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/devices/valkmusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/extended_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/iqm_operation_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/iqm_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 14:13:38.000000 cirq-iqm-8.2/src/cirq_iqm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.644308 cirq-iqm-8.2/src/cirq_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-29 14:14:56.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2022-12-29 14:14:56.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 14:14:56.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 14:13:47.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-29 14:14:56.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-29 14:14:56.000000 cirq-iqm-8.2/src/cirq_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 14:14:56.652308 cirq-iqm-8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16275 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_apollo.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_iqm_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_iqm_device_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_iqm_operation_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_iqm_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_openqasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tests/test_valkmusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2022-12-29 14:13:38.000000 cirq-iqm-8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.109310 cirq-iqm-9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.101310 cirq-iqm-9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-11 07:18:23.000000 cirq-iqm-9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-11 07:18:23.000000 cirq-iqm-9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-01-11 07:18:23.000000 cirq-iqm-9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-11 07:18:23.000000 cirq-iqm-9.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-01-11 07:18:23.000000 cirq-iqm-9.0/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-11 07:18:23.000000 cirq-iqm-9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-11 07:19:44.109310 cirq-iqm-9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-01-11 07:18:23.000000 cirq-iqm-9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.101310 cirq-iqm-9.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-01-11 07:18:23.000000 cirq-iqm-9.0/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/demo_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/demo_apollo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/demo_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/demo_iqm_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/demo_valkmusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-01-11 07:18:23.000000 cirq-iqm-9.0/examples/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-11 07:18:23.000000 cirq-iqm-9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-11 07:19:44.109310 cirq-iqm-9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-11 07:18:23.000000 cirq-iqm-9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.101310 cirq-iqm-9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.105310 cirq-iqm-9.0/src/cirq_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.109310 cirq-iqm-9.0/src/cirq_iqm/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/apollo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/iqm_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/iqm_device_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/devices/valkmusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/extended_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/iqm_operation_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/iqm_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 07:18:23.000000 cirq-iqm-9.0/src/cirq_iqm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.109310 cirq-iqm-9.0/src/cirq_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-11 07:19:44.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-11 07:19:44.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 07:19:44.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 07:18:34.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-11 07:19:44.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-11 07:19:44.000000 cirq-iqm-9.0/src/cirq_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:19:44.109310 cirq-iqm-9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_apollo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_iqm_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_iqm_device_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_iqm_operation_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_iqm_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_openqasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tests/test_valkmusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-11 07:18:23.000000 cirq-iqm-9.0/tox.ini
```

### Comparing `cirq-iqm-8.2/.coveragerc` & `cirq-iqm-9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/.github/workflows/ci.yml` & `cirq-iqm-9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/.github/workflows/publish.yml` & `cirq-iqm-9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/.github/workflows/tag_and_release.yml` & `cirq-iqm-9.0/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/CHANGELOG.rst` & `cirq-iqm-9.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =========
 Changelog
 =========
 
+Version 9.0
+===========
+
+* User guide updated.
+
+Bugfixes
+--------
+
+* :meth:`.IQMDevice.route_circuit` bugfix: ``initial_mapping`` must be reversed to match the
+  :mod:`cirq.contrib.routing.greedy` convention.
+
 Version 8.2
 ===========
 
 * Upgrade to IQMClient version 10.0. `#95 <https://github.com/iqm-finland/cirq-on-iqm/pull/95>`_
 
 Version 8.1
 ===========
```

### Comparing `cirq-iqm-8.2/DEVELOPMENT.rst` & `cirq-iqm-9.0/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/LICENSE` & `cirq-iqm-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/PKG-INFO` & `cirq-iqm-9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-iqm
-Version: 8.2
+Version: 9.0
 Summary: Google Cirq adapter for IQM's quantum architectures
 Home-page: https://github.com/iqm-finland/cirq-on-iqm
 Author: Cirq on IQM developers
 Author-email: developers@meetiqm.com
 License: Apache 2.0
 Project-URL: Documentation, https://iqm-finland.github.io/cirq-on-iqm
 Platform: any
```

### Comparing `cirq-iqm-8.2/README.rst` & `cirq-iqm-9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/Makefile` & `cirq-iqm-9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/_static/images/favicon.ico` & `cirq-iqm-9.0/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/_static/images/logo.png` & `cirq-iqm-9.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/_templates/autosummary-class-template.rst` & `cirq-iqm-9.0/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/_templates/autosummary-module-template.rst` & `cirq-iqm-9.0/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/conf.py` & `cirq-iqm-9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/index.rst` & `cirq-iqm-9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/docs/user_guide.rst` & `cirq-iqm-9.0/docs/user_guide.rst`

 * *Files 7% similar despite different names*

```diff
@@ -55,152 +55,189 @@
 
     print(adonis.qubits)
 
 
 Constructing circuits
 ---------------------
 
-There are two main workflows of using :class:`cirq.Circuit` instances with IQM devices:
+There are two main ways of constructing :class:`cirq.Circuit` instances for IQM devices:
 
-1. Create a ``Circuit`` instance, use arbitrary qubit names and types. There is no
-   validation of the operations when appending. At any point the user can apply :meth:`.IQMDevice.decompose_circuit`
-   to decompose the circuit contents into the native operation set of the device, or :meth:`.IQMDevice.route_circuit`
-   to route the circuit to the device connectivity and device qubits.
+1. Create a ``Circuit`` instance using arbitrary qubit names and types.
 2. Create a ``Circuit`` from an OpenQASM 2.0 program. The qubit names are determined by the OpenQASM ``qreg`` names,
-   appended with zero-based indices. Proceed as in workflow 1.
+   appended with zero-based indices.
 
-Below we demonstrate examples of creating circuits in each of the two workflows.
+Below we give an example of each method.
 
-.. _workflow_1:
 
-Workflow 1
-^^^^^^^^^^
+Method 1
+^^^^^^^^
 
 Construct a circuit and use arbitrary qubits:
 
 .. code-block:: python
 
     import cirq
 
     q1, q2 = cirq.NamedQubit('Alice'), cirq.NamedQubit('Bob')
-    circuit_1 = cirq.Circuit()
-    circuit_1.append(cirq.X(q1))
-    circuit_1.append(cirq.H(q2))
-    circuit_1.append(cirq.CNOT(q1, q2))
-    circuit_1.append(cirq.measure(q1, q2, key='m'))
-    print(circuit_1)
+    circuit = cirq.Circuit()
+    circuit.append(cirq.X(q1))
+    circuit.append(cirq.H(q2))
+    circuit.append(cirq.CNOT(q1, q2))
+    circuit.append(cirq.measure(q1, q2, key='m'))
+    print(circuit)
 
 This will result in the circuit
 ::
 
    Alice: ───X───@───M('m')───
                  │   │
    Bob: ─────H───X───M────────
 
-After the circuit has been constructed, it can be decomposed and routed against a particular ``IQMDevice``.
+
+Method 2
+^^^^^^^^
+
+You can read an OpenQASM 2.0 program from a file (or a string), e.g.
+
+::
+
+   OPENQASM 2.0;
+   include "qelib1.inc";
+
+   qreg q[2];
+   creg m[2];
+
+   x q[0];
+   h q[1];
+   cx q[0], q[1];
+   measure q -> m;
+
+and convert it into a :class:`cirq.Circuit` object using :func:`.circuit_from_qasm`.
+
+.. code-block:: python
+
+    import cirq_iqm
+
+    with open('circuit.qasm', 'r') as f:
+        qasm_circuit = cirq_iqm.circuit_from_qasm(f.read())
+    print(qasm_circuit)
+
+::
+
+   q_0: ───X───@───M('m_0')───
+               │
+   q_1: ───H───X───M('m_1')───
+
+:func:`.circuit_from_qasm` uses the OpenQASM 2.0 parser in :mod:`cirq.contrib.qasm_import`.
+
+After a circuit has been constructed, it can be decomposed and routed against a particular ``IQMDevice``.
+
+
+Decomposition
+-------------
+
 The method :meth:`.IQMDevice.decompose_circuit` accepts a :class:`cirq.Circuit` object as an argument and
-returns the decomposed circuit containing only native gates for the corresponding device:
+returns the decomposed circuit containing only native operations for the corresponding device:
 
 .. code-block:: python
 
-    decomposed_circuit_1 = adonis.decompose_circuit(circuit_1)
+    decomposed_circuit = adonis.decompose_circuit(circuit)
+    print(decomposed_circuit)
+
+::
+
+    Alice: ───X────────────────────@───────────M('m')───
+                                   │           │
+    Bob: ─────Y^0.5───X───Y^-0.5───@───Y^0.5───M────────
+
+The Hadamard and CNOT gates are not native to Adonis, so they were decomposed to X, Y and CZ gates which are.
 
 
+.. _routing:
+
+Routing
+-------
+
+Routing means transforming a circuit such that it acts on the device qubits, and respects the
+device connectivity.
 The method :meth:`.IQMDevice.route_circuit` accepts a :class:`cirq.Circuit` object as an argument,
 and returns the circuit routed against the device, acting on the device qubits instead of the
 arbitrary qubits we had originally.
 
 .. code-block:: python
 
-    routed_circuit_1 = adonis.route_circuit(decomposed_circuit_1)
+    routed_circuit_1 = adonis.route_circuit(decomposed_circuit)
     print(routed_circuit_1)
 
-
 ::
 
     QB3: ───X────────────────────@───────────M('m')───
                                  │           │
     QB4: ───Y^0.5───X───Y^-0.5───@───Y^0.5───M────────
 
-By default :meth:`.route_circuit` returns only the routed circuit. However if you set its keyword
+By default :meth:`.route_circuit` returns only the routed circuit. However, if you set its keyword
 argument ``return_swap_network`` to ``True``, it will return the full
 :class:`cirq.contrib.routing.swap_network.SwapNetwork` object which contains the routed
 circuit itself and the mapping between the used device qubits and the original ones.
 
+You may also provide the initial mapping from the *logical* qubits in the circuit to the *physical*
+qubits on the device yourself, by using the keyword argument ``initial_mapping``.
+It serves as the starting point of the routing:
+
+.. code-block:: python
+
+    routed_circuit_2 = adonis.route_circuit(
+        decomposed_circuit,
+        initial_mapping={q1: adonis.qubits[2], q2: adonis.qubits[0]},
+    )
+    print(routed_circuit_2)
+
+::
+
+    QB1: ───Y^0.5───X───Y^-0.5───@───Y^0.5───────M────────
+                                 │               │
+    QB3: ───X────────────────────@───────────────M('m')───
+
 Under the hood, :meth:`.route_circuit` leverages the routing algorithm in :mod:`cirq.contrib.routing.router`.
 It works on single- and two-qubit gates, and measurement operations of arbitrary size.
 If you have gates involving more than two qubits you need to decompose them before routing.
 Since routing may add some SWAP gates to the circuit, you will need to decompose the circuit
 again after the routing, unless SWAP is a native gate for the target device.
 
+
+Optimization
+------------
+
 Yet another important topic is circuit optimization. In addition to the optimizers available in Cirq you can also
 benefit from Cirq on IQM's :mod:`.optimizers` module which contains some optimization tools geared towards IQM devices.
 The function :func:`.optimizers.simplify_circuit` is a convenience method encapsulating a particular sequence of
 optimizations. Let us try it out on our decomposed and routed circuit above:
 
 .. code-block:: python
 
     from cirq_iqm.optimizers import simplify_circuit
 
-    simplified_circuit_1 = simplify_circuit(routed_circuit_1)
-    print(simplified_circuit_1)
+    simplified_circuit = simplify_circuit(routed_circuit_1)
+    print(simplified_circuit)
 
 
 ::
 
     QB3: ───PhX(1)───@───────────────────M('m')───
                      │                   │
-    QB5: ────────────@───PhX(-0.5)^0.5───M────────
+    QB4: ────────────@───PhX(-0.5)^0.5───M────────
 
 
 .. note::
 
     The funtion :func:`.simplify_circuit` is not associated with any IQM device, so its result may contain non-native
     gates for a particular device. In the example above we don't have them, however it is generally a good idea to run
     decomposition once again after the simplification.
 
 
-Workflow 2
-^^^^^^^^^^
-
-You can read an OpenQASM 2.0 program from a file (or a string), e.g.
-
-::
-
-   OPENQASM 2.0;
-   include "qelib1.inc";
-
-   qreg q[2];
-   creg m[2];
-
-   x q[0];
-   h q[1];
-   cx q[0], q[1];
-   measure q -> m;
-
-and convert it into a :class:`cirq.Circuit` object using :func:`.circuit_from_qasm`.
-Once you have done this, you can perform the decomposition and routing steps as in
-the previous workflow to prepare the circuit for execution on an IQM device.
-
-.. code-block:: python
-
-    import cirq_iqm
-
-    with open('circuit.qasm', 'r') as f:
-        circuit_2 = cirq_iqm.circuit_from_qasm(f.read())
-    print(circuit_2)
-
-::
-
-   q_0: ───X───@───M('m_0')───
-               │
-   q_1: ───H───X───M('m_1')───
-
-:func:`.circuit_from_qasm` uses the OpenQASM 2.0 parser in :mod:`cirq.contrib.qasm_import`.
-
 
 Running on a real quantum computer
 ----------------------------------
 
 .. note::
 
    At the moment IQM does not provide a quantum computing service open to the general public.
@@ -214,49 +251,34 @@
 instance and use its :meth:`~.IQMSampler.run` method to send a circuit for execution and retrieve the results:
 
 .. code-block:: python
 
    from cirq_iqm.iqm_sampler import IQMSampler
 
    sampler = IQMSampler(iqm_server_url)
-   result = sampler.run(circuit_1, repetitions=10)
+   result = sampler.run(routed_circuit_1, repetitions=10)
    print(result.measurements['m'])
 
 
 Note that the code snippet above assumes that you have set the variable ``iqm_server_url`` to the URL
 of the IQM server. By default, the latest calibration set is used for running the circuit. If you want to use
 a particular calibration set, provide the ``calibration_set_id`` argument. The sampler will by default use an
 :class:`.IQMDevice` created based on architecture data obtained from the server, which is then available in the
 :attr:`.IQMSampler.device` property. Alternatively, the device can be specified directly with the ``device`` argument.
 
 If the IQM server you are connecting to requires authentication, you will also have to use
 `Cortex CLI <https://github.com/iqm-finland/cortex-cli>`_ to retrieve and automatically refresh access tokens,
 then set the ``IQM_TOKENS_FILE`` environment variable to use those tokens.
 See Cortex CLI's `documentation <https://iqm-finland.github.io/cortex-cli/readme.html>`_ for details.
-Alternatively, authorize with the IQM_AUTH_SERVER, IQM_AUTH_USERNAME and IQM_AUTH_PASSWORD environment variables
-or pass them as arguments to the constructor of :class:`.IQMProvider`, however this approach is less secure
-and considered deprecated.
-
-When executing a circuit that uses something other than the device qubits, you need to either route it first
-as explained in :ref:`workflow 1 <workflow_1>` above,
-or provide the mapping from the *logical* qubits in the circuit to the *physical* qubits on the device yourself.
-The initializer of :class:`.IQMSampler` accepts an optional argument called ``qubit_mapping`` which
-can be used to specify this correspondence.
-
-.. code-block:: python
-
-    import json
-
-
-    qubit_mapping = {'Alice': 'QB1', 'Bob': 'QB3'}
-
-    sampler = IQMSampler(iqm_server_url, qubit_mapping=qubit_mapping)
-    result = sampler.run(decomposed_circuit_1, repetitions=10)
-    print(result.measurements['m'])
+Alternatively, you can authenticate yourself using the ``IQM_AUTH_SERVER``, ``IQM_AUTH_USERNAME``
+and ``IQM_AUTH_PASSWORD`` environment variables, or pass them as arguments to the constructor of
+:class:`.IQMProvider`, but this approach is less secure and considered deprecated.
 
+When executing a circuit that uses something other than the device qubits, you need to route it first,
+as explained in the :ref:`routing` section above.
 
 
 More examples
 -------------
 
 More examples are available in the
 `examples directory <https://github.com/iqm-finland/cirq-on-iqm/tree/main/examples>`_
```

### Comparing `cirq-iqm-8.2/examples/demo_adonis.py` & `cirq-iqm-9.0/examples/demo_adonis.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/examples/demo_apollo.py` & `cirq-iqm-9.0/examples/demo_apollo.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/examples/demo_common.py` & `cirq-iqm-9.0/examples/demo_common.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/examples/demo_iqm_execution.py` & `cirq-iqm-9.0/examples/demo_iqm_execution.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/examples/demo_valkmusa.py` & `cirq-iqm-9.0/examples/demo_valkmusa.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/examples/usage.ipynb` & `cirq-iqm-9.0/examples/usage.ipynb`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/pyproject.toml` & `cirq-iqm-9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/setup.cfg` & `cirq-iqm-9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/setup.py` & `cirq-iqm-9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/__init__.py` & `cirq-iqm-9.0/src/cirq_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/__init__.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/adonis.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/adonis.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/apollo.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/apollo.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/iqm_device.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/iqm_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 to use with the architecture.
 """
 # pylint: disable=protected-access,no-self-use
 from __future__ import annotations
 
 import collections.abc as ca
 from math import pi as PI
-from typing import Dict, Optional, Union
+from typing import Optional, Union
 import uuid
 
 import cirq
 from cirq import InsertStrategy, MeasurementGate, devices, ops, protocols
 from cirq.contrib.routing.router import route_circuit
 
 from .iqm_device_metadata import IQMDeviceMetadata
@@ -174,26 +174,27 @@
         )
 
     def route_circuit(
         self,
         circuit: cirq.Circuit,
         *,
         return_swap_network: bool = False,
-        initial_mapping: Optional[Dict['cirq.Qid', 'cirq.Qid']] = None,
+        initial_mapping: Optional[dict['cirq.Qid', 'cirq.Qid']] = None,
     ) -> Union[cirq.Circuit, cirq.contrib.routing.SwapNetwork]:
-        """Routes the given circuit to the device connectivity.
+        """Routes the given circuit to the device connectivity and qubit names.
 
         The routed circuit uses the device qubits, and may have additional SWAP gates inserted to perform the qubit
-        routing. The function :func:`cirq.contrib.routing.router` is used for routing.
+        routing. The function :func:`cirq.contrib.routing.router.route_circuit` is used for routing.
         Note that only gates of one or two qubits, and measurement operations of arbitrary size are supported.
 
         Args:
             circuit: circuit to route
             return_swap_network: iff True, return the full swap network instead of the routed circuit
-            initial_mapping: mapping between logical and physical qubits
+            initial_mapping: Initial mapping from ``circuit`` qubits to device qubits, to serve as
+                the starting point of the routing. ``None`` means it will be generated automatically.
 
         Returns:
             routed circuit, or the swap network if requested
 
         Raises:
             ValueError: routing is impossible
         """
@@ -208,17 +209,24 @@
 
         modified_circuit = circuit.copy()
         modified_circuit.batch_remove([(ind, op) for ind, op, _ in measurement_ops])
         i_tag = uuid.uuid4()
         for q in measurement_qubits:
             modified_circuit.append(cirq.I(q).with_tags(i_tag))
 
+        if initial_mapping is not None:
+            # reverse the mapping to match the cirq.contrib.routing.greedy convention
+            initial_mapping = {v: k for k, v in initial_mapping.items()}
+
         # Route the modified circuit.
         swap_network = route_circuit(
-            modified_circuit, self._metadata.nx_graph, algo_name='greedy', initial_mapping=initial_mapping
+            modified_circuit,
+            self._metadata.nx_graph,
+            algo_name='greedy',
+            initial_mapping=initial_mapping,
         )
 
         # Return measurements to the circuit with potential qubit swaps.
         final_qubit_mapping = {v: k for k, v in swap_network.final_mapping().items()}
         new_measurements = []
         for _, op, gate in measurement_ops:
             new_qubits = [final_qubit_mapping[q] for q in op.qubits]
```

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/iqm_device_metadata.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/iqm_device_metadata.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/devices/valkmusa.py` & `cirq-iqm-9.0/src/cirq_iqm/devices/valkmusa.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/extended_qasm_parser.py` & `cirq-iqm-9.0/src/cirq_iqm/extended_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/iqm_operation_mapping.py` & `cirq-iqm-9.0/src/cirq_iqm/iqm_operation_mapping.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/iqm_sampler.py` & `cirq-iqm-9.0/src/cirq_iqm/iqm_sampler.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm/optimizers.py` & `cirq-iqm-9.0/src/cirq_iqm/optimizers.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/src/cirq_iqm.egg-info/PKG-INFO` & `cirq-iqm-9.0/src/cirq_iqm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-iqm
-Version: 8.2
+Version: 9.0
 Summary: Google Cirq adapter for IQM's quantum architectures
 Home-page: https://github.com/iqm-finland/cirq-on-iqm
 Author: Cirq on IQM developers
 Author-email: developers@meetiqm.com
 License: Apache 2.0
 Project-URL: Documentation, https://iqm-finland.github.io/cirq-on-iqm
 Platform: any
```

### Comparing `cirq-iqm-8.2/src/cirq_iqm.egg-info/SOURCES.txt` & `cirq-iqm-9.0/src/cirq_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tag-from-pipeline.sh` & `cirq-iqm-9.0/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/conftest.py` & `cirq-iqm-9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_adonis.py` & `cirq-iqm-9.0/tests/test_adonis.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     def test_routing_with_partial_initial_mapping(self, adonis, qubits):
         circuit = cirq.Circuit(
             cirq.CZ(qubits[0], qubits[1]),
             cirq.measure(qubits[0], key='mk0'),
             cirq.measure(qubits[1], key='mk1'),
         )
 
-        initial_mapping = dict(zip(adonis.metadata.nx_graph, qubits[0:2]))
+        initial_mapping = dict(zip(qubits[0:2], adonis.metadata.nx_graph))
         # route_circuit() checks mapping consistency when initial_mapping is provided
         new = adonis.route_circuit(circuit, initial_mapping=initial_mapping)
 
         adonis.validate_circuit(new)
 
     def test_routing_with_complete_initial_mapping(self, adonis, qubits):
         circuit = cirq.Circuit(
@@ -331,15 +331,15 @@
             cirq.measure(qubits[0], key='mk0'),
             cirq.measure(qubits[1], key='mk1'),
             cirq.measure(qubits[2], key='mk2'),
             cirq.measure(qubits[3], key='mk3'),
             cirq.measure(qubits[4], key='mk4'),
         )
 
-        initial_mapping = dict(zip(adonis.metadata.nx_graph, qubits[0:5]))
+        initial_mapping = dict(zip(qubits[0:5], adonis.metadata.nx_graph))
         # route_circuit() checks mapping consistency when initial_mapping is provided
         new = adonis.route_circuit(circuit, initial_mapping=initial_mapping)
 
         adonis.validate_circuit(new)
 
     def test_routing_circuit_too_large(self, adonis):
         """The circuit must fit on the device."""
```

### Comparing `cirq-iqm-8.2/tests/test_apollo.py` & `cirq-iqm-9.0/tests/test_apollo.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
     def test_routing_with_partial_initial_mapping(self, apollo, qubits):
         circuit = cirq.Circuit(
             cirq.CZ(qubits[0], qubits[1]),
             cirq.measure(qubits[0], key='mk0'),
             cirq.measure(qubits[1], key='mk1'),
         )
 
-        initial_mapping = dict(zip(apollo.metadata.nx_graph, qubits[0:2]))
+        initial_mapping = dict(zip(qubits[0:2], apollo.metadata.nx_graph))
         # route_circuit() checks mapping consistency when initial_mapping is provided
         new = apollo.route_circuit(circuit, initial_mapping=initial_mapping)
 
         apollo.validate_circuit(new)
 
     def test_routing_with_complete_initial_mapping(self, apollo, qubits):
         circuit = cirq.Circuit(
@@ -342,15 +342,15 @@
                 cirq.CZ(qubits[0], qubits[1]),
                 cirq.CZ(qubits[0], qubits[2]),
                 cirq.CZ(qubits[2], qubits[4]),
             ]
             + [cirq.measure([q]) for q in qubits]
         )
 
-        initial_mapping = dict(zip(apollo.metadata.nx_graph, qubits))
+        initial_mapping = dict(zip(qubits, apollo.metadata.nx_graph))
         # route_circuit() checks mapping consistency when initial_mapping is provided
         new = apollo.route_circuit(circuit, initial_mapping=initial_mapping)
 
         apollo.validate_circuit(new)
 
     def test_routing_circuit_too_large(self, apollo):
         """The circuit must fit on the device."""
```

### Comparing `cirq-iqm-8.2/tests/test_iqm_device.py` & `cirq-iqm-9.0/tests/test_iqm_device.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_iqm_device_metadata.py` & `cirq-iqm-9.0/tests/test_iqm_device_metadata.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_iqm_operation_mapping.py` & `cirq-iqm-9.0/tests/test_iqm_operation_mapping.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_iqm_sampler.py` & `cirq-iqm-9.0/tests/test_iqm_sampler.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_openqasm.py` & `cirq-iqm-9.0/tests/test_openqasm.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_optimization.py` & `cirq-iqm-9.0/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tests/test_valkmusa.py` & `cirq-iqm-9.0/tests/test_valkmusa.py`

 * *Files identical despite different names*

### Comparing `cirq-iqm-8.2/tox.ini` & `cirq-iqm-9.0/tox.ini`

 * *Files identical despite different names*

