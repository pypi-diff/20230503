# Comparing `tmp/demesdraw-0.3.1.tar.gz` & `tmp/demesdraw-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demesdraw-0.3.1.tar", last modified: Mon Sep 19 11:24:36 2022, max compression
+gzip compressed data, was "demesdraw-0.4.0.tar", last modified: Wed May  3 19:02:35 2023, max compression
```

## Comparing `demesdraw-0.3.1.tar` & `demesdraw-0.4.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.713802 demesdraw-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.701802 demesdraw-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.701802 demesdraw-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.github/workflows/wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-19 11:24:20.000000 demesdraw-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-09-19 11:24:20.000000 demesdraw-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-09-19 11:24:20.000000 demesdraw-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-19 11:24:36.713802 demesdraw-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-09-19 11:24:20.000000 demesdraw-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.701802 demesdraw-0.3.1/demesdraw/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10034 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/size_history.py
--rw-r--r--   0 runner    (1001) docker     (121)    26284 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/tubes.py
--rw-r--r--   0 runner    (1001) docker     (121)    17612 2022-09-19 11:24:20.000000 demesdraw-0.3.1/demesdraw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.705802 demesdraw-0.3.1/demesdraw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-19 11:24:36.000000 demesdraw-0.3.1/demesdraw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.705802 demesdraw-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.705802 demesdraw-0.3.1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_ext/inject_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.705802 demesdraw-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    56402 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_size_history.svg
--rw-r--r--   0 runner    (1001) docker     (121)   428886 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_tubes.svg
--rw-r--r--   0 runner    (1001) docker     (121)   475270 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_tubes_custom.svg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/api.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      586 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/is_new_stable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-09-19 11:24:20.000000 demesdraw-0.3.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-19 11:24:20.000000 demesdraw-0.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.709802 demesdraw-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/bottleneck.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/cloning_example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_asymmetric_migration_changing_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_deme_ancestors.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_deme_many_epochs_global.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_deme_many_epochs_local.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_deme_many_epochs_overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_migration_properties.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_pulse_properties.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/defaults_symmetric_migration_changing_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/line_topology.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/linear_size_function_example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/lots_of_ancestors.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/minimal.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/offshoots.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/one-deme-constant-N.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/one-deme-three-epoch-with-exp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/one-deme-two-epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/reticulate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.713802 demesdraw-0.3.1/examples/stdpopsim/
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/AraTha__African2Epoch_1H18.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/AraTha__African3Epoch_1H18.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/AraTha__SouthMiddleAtlas_1D17.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/DroMel__African3Epoch_1S16.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/DroMel__OutOfAfrica_2L06.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__Africa_1T12.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__AmericanAdmixture_4B11.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__AncientEurasia_9K19.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__AshkSub_7G19.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfricaArchaicAdmixture_5R19.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfrica_2T12.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfrica_3G09.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__PapuansOutOfAfrica_10J19.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/HomSap__Zigzag_1S14.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stdpopsim/PonAbe__TwoSpecies_2L11.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/stepping_stone_model.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/two-epoch-1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/two-epoch-2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-19 11:24:20.000000 demesdraw-0.3.1/examples/utility_graph.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-19 11:24:20.000000 demesdraw-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.713802 demesdraw-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-19 11:24:20.000000 demesdraw-0.3.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-19 11:24:20.000000 demesdraw-0.3.1/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-19 11:24:20.000000 demesdraw-0.3.1/requirements/minimal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-19 11:24:20.000000 demesdraw-0.3.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-19 11:24:20.000000 demesdraw-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-09-19 11:24:36.713802 demesdraw-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 11:24:36.713802 demesdraw-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/plot_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9598 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/test_demesdraw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/test_import_visibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    21090 2022-09-19 11:24:20.000000 demesdraw-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.560152 demesdraw-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.548152 demesdraw-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.548152 demesdraw-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.github/workflows/wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-03 19:02:21.000000 demesdraw-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-03 19:02:21.000000 demesdraw-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-03 19:02:21.000000 demesdraw-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-05-03 19:02:35.560152 demesdraw-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-05-03 19:02:21.000000 demesdraw-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.548152 demesdraw-0.4.0/demesdraw/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10091 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/size_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27477 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/tubes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20740 2023-05-03 19:02:21.000000 demesdraw-0.4.0/demesdraw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.548152 demesdraw-0.4.0/demesdraw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2831 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-03 19:02:35.000000 demesdraw-0.4.0/demesdraw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.552152 demesdraw-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1431 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.552152 demesdraw-0.4.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_ext/inject_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.552152 demesdraw-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)    56402 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_size_history.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   428886 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_tubes.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   475270 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_tubes_custom.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/api.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)      586 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/is_new_stable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9418 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/layout.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-05-03 19:02:21.000000 demesdraw-0.4.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-03 19:02:21.000000 demesdraw-0.4.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.556152 demesdraw-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/bottleneck.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/cloning_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_asymmetric_migration_changing_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_deme_ancestors.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_deme_many_epochs_global.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_deme_many_epochs_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_deme_many_epochs_overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_migration_properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_pulse_properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/defaults_symmetric_migration_changing_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/line_topology.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/linear_size_function_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/lots_of_ancestors.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/minimal.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/offshoots.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/one-deme-constant-N.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/one-deme-three-epoch-with-exp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/one-deme-two-epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/reticulate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.560152 demesdraw-0.4.0/examples/stdpopsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/AraTha__African2Epoch_1H18.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/AraTha__African3Epoch_1H18.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/AraTha__SouthMiddleAtlas_1D17.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/DroMel__African3Epoch_1S16.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/DroMel__OutOfAfrica_2L06.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__Africa_1T12.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__AmericanAdmixture_4B11.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__AncientEurasia_9K19.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__AshkSub_7G19.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfricaArchaicAdmixture_5R19.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfrica_2T12.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfrica_3G09.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__PapuansOutOfAfrica_10J19.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/HomSap__Zigzag_1S14.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stdpopsim/PonAbe__TwoSpecies_2L11.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/stepping_stone_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/two-epoch-1.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/two-epoch-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-03 19:02:21.000000 demesdraw-0.4.0/examples/utility_graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-03 19:02:21.000000 demesdraw-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.560152 demesdraw-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-03 19:02:21.000000 demesdraw-0.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-03 19:02:21.000000 demesdraw-0.4.0/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-03 19:02:21.000000 demesdraw-0.4.0/requirements/minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-03 19:02:21.000000 demesdraw-0.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-03 19:02:21.000000 demesdraw-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-05-03 19:02:35.564152 demesdraw-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 19:02:35.560152 demesdraw-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/plot_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9819 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/test_demesdraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/test_import_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37932 2023-05-03 19:02:21.000000 demesdraw-0.4.0/tests/test_utils.py
```

### Comparing `demesdraw-0.3.1/.github/mergify.yml` & `demesdraw-0.4.0/.github/mergify.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 queue_rules:
   - name: default
     conditions:
       - base=main
       - check-success=build-docs
       - check-success=lint
       - check-success=tests (macos-11, 3.7)
-      - check-success=tests (macos-11, 3.10)
+      - check-success=tests (macos-11, 3.11)
       - check-success=tests (ubuntu-20.04, 3.7)
-      - check-success=tests (ubuntu-20.04, 3.10)
+      - check-success=tests (ubuntu-20.04, 3.11)
       - check-success=tests (windows-2022, 3.7)
-      - check-success=tests (windows-2022, 3.10)
+      - check-success=tests (windows-2022, 3.11)
 
 pull_request_rules:
   - name: automatic merge for Dependabot pull requests
     conditions:
       - base=main
       - author~=^dependabot(|-preview)\[bot\]$
       - check-success=build-docs
       - check-success=lint
       - check-success=tests (macos-11, 3.7)
-      - check-success=tests (macos-11, 3.10)
+      - check-success=tests (macos-11, 3.11)
       - check-success=tests (ubuntu-20.04, 3.7)
-      - check-success=tests (ubuntu-20.04, 3.10)
+      - check-success=tests (ubuntu-20.04, 3.11)
       - check-success=tests (windows-2022, 3.7)
-      - check-success=tests (windows-2022, 3.10)
+      - check-success=tests (windows-2022, 3.11)
     actions:
       queue:
         name: default
   - name: automatic merge for main when CI passes and reviewed
     conditions:
       - "#approved-reviews-by>=1"
       - base=main
       - check-success=build-docs
       - check-success=lint
       - check-success=tests (macos-11, 3.7)
-      - check-success=tests (macos-11, 3.10)
+      - check-success=tests (macos-11, 3.11)
       - check-success=tests (ubuntu-20.04, 3.7)
-      - check-success=tests (ubuntu-20.04, 3.10)
+      - check-success=tests (ubuntu-20.04, 3.11)
       - check-success=tests (windows-2022, 3.7)
-      - check-success=tests (windows-2022, 3.10)
+      - check-success=tests (windows-2022, 3.11)
     actions:
       queue:
         name: default
```

### Comparing `demesdraw-0.3.1/.github/workflows/docs.yaml` & `demesdraw-0.4.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/.github/workflows/lint.yaml` & `demesdraw-0.4.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/.github/workflows/tests.yaml` & `demesdraw-0.4.0/.github/workflows/tests.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,28 @@
     branches: [ main ]
 
 jobs:
   canceller:
     runs-on: ubuntu-20.04
     steps:
       - name: cancel previous runs
-        uses: styfle/cancel-workflow-action@0.10.0
+        uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
   tests:
     defaults:
       run:
         shell: bash
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-2022, macos-11]
-        python-version: [3.7, "3.10"]
+        python-version: [3.7, "3.11"]
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
 
     steps:
       - name: checkout
         uses: actions/checkout@v3
@@ -55,11 +55,14 @@
             -n auto \
             --cov=demesdraw \
             --cov-report=term-missing \
             --cov-report=xml \
             tests
 
       - name: upload coverage report to codecov
-        uses: codecov/codecov-action@v3.1.0
+        uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
           env_vars: OS,PYTHON
+          # Use upload token to avoid upload failures.
+          # https://github.com/codecov/codecov-action/issues/837
+          token: 64ca2265-7e09-4e46-a3b9-85ed23998c7e
```

### Comparing `demesdraw-0.3.1/.github/workflows/wheel.yaml` & `demesdraw-0.4.0/.github/workflows/wheel.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
 
     steps:
       - name: download wheel
         uses: actions/download-artifact@v3
         with:
           name: wheel-and-sdist
           path: dist/
```

### Comparing `demesdraw-0.3.1/CHANGELOG.md` & `demesdraw-0.4.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [0.4.0] - 2023-05-03
+
+* Documented the layout algorithm used in tubes plots.
+* Added `scale_bar` option to `demesdraw.tubes()`, and `--scale-bar` option
+  to the `demesdraw tubes` CLI, to draw a scale bar that indicates the
+  population size.
+* Removed dependency on `cvxpy` by going back to `scipy`
+  for optimisation of the deme positions. The trust-constr
+  method with linear constraints seems to work well.
+
 ## [0.3.1] - 2022-09-19
 
 * Added mouseover annotation popups for interactive tubes plots.
 * Dropped support for Python 3.6.
 * Performance improvement when calculating tube positions.
 * Fix incompatibility with "legend" labels and matplotlib 3.6.0.
```

### Comparing `demesdraw-0.3.1/LICENSE` & `demesdraw-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/PKG-INFO` & `demesdraw-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demesdraw
-Version: 0.3.1
+Version: 0.4.0
 Summary: drawing tools for Demes demographic models
 Home-page: https://github.com/grahamgower/demesdraw
 Author: Graham Gower
 License: ISC
 Project-URL: Documentation, https://grahamgower.github.io/demesdraw/
 Project-URL: Source Code, https://github.com/grahamgower/demesdraw
 Project-URL: Bug Tracker, https://github.com/grahamgower/demesdraw/issues
```

### Comparing `demesdraw-0.3.1/README.md` & `demesdraw-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/demesdraw/__main__.py` & `demesdraw-0.4.0/demesdraw/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,18 +62,31 @@
     """
     Plot a demes-as-tubes schematic of the model and the demes' relationships.
     """
 
     def __init__(self, subparsers):
         super().__init__(subparsers, "tubes")
 
+        self.parser.add_argument(
+            "--scale-bar",
+            action="store_true",
+            default=False,
+            help="Draw a scale bar that indicates population size.",
+        )
+
     def __call__(self, args):
         graph = demes.load(args.input_file)
         fig, ax = demesdraw.utils.get_fig_axes(aspect=args.aspect, scale=args.scale)
-        demesdraw.tubes(graph, ax=ax, log_time=args.log_time, title=args.title)
+        demesdraw.tubes(
+            graph,
+            ax=ax,
+            log_time=args.log_time,
+            title=args.title,
+            scale_bar=args.scale_bar,
+        )
         if args.output_file is not None:
             fig.savefig(args.output_file)
         else:
             # interactive plot
             plt.show()
```

### Comparing `demesdraw-0.3.1/demesdraw/size_history.py` & `demesdraw-0.4.0/demesdraw/size_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 import demes
 import numpy as np
 import matplotlib
 
 from demesdraw import utils
 
 
 def size_history(
     graph: demes.Graph,
-    ax: matplotlib.axes.Axes = None,
-    colours: utils.ColourOrColourMapping = None,
+    ax: matplotlib.axes.Axes | None = None,
+    colours: utils.ColourOrColourMapping | None = None,
     log_time: bool = False,
     log_size: bool = False,
-    title: str = None,
+    title: str | None = None,
     inf_ratio: float = 0.1,
     inf_label: bool = False,
     invert_x: bool = False,
     annotate_epochs: bool = False,
     num_points: int = 100,
 ) -> matplotlib.axes.Axes:
     """
```

### Comparing `demesdraw-0.3.1/demesdraw/tubes.py` & `demesdraw-0.4.0/demesdraw/tubes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Dict, Mapping, List, Tuple
 
 import demes
 import numpy as np
 import matplotlib
 import matplotlib.patheffects
 
@@ -145,30 +146,33 @@
     :return:
         A dictionary mapping deme names to positions.
     """
     sep = utils.separation_heuristic(graph)
     positions = utils.minimal_crossing_positions(
         graph, sep=sep, unique_interactions=False
     )
-    return utils.cvxpy_optimise(graph, positions, sep=sep, unique_interactions=False)
+    return utils.optimise_positions(
+        graph, positions=positions, sep=sep, unique_interactions=False
+    )
 
 
 def tubes(
     graph: demes.Graph,
-    ax: matplotlib.axes.Axes = None,
-    colours: utils.ColourOrColourMapping = None,
+    ax: matplotlib.axes.Axes | None = None,
+    colours: utils.ColourOrColourMapping | None = None,
     log_time: bool = False,
-    title: str = None,
+    title: str | None = None,
     inf_ratio: float = 0.2,
-    positions: Mapping[str, float] = None,
+    positions: Mapping[str, float] | None = None,
     num_lines_per_migration: int = 10,
-    seed: int = None,
-    max_time: float = None,
+    seed: int | None = None,
+    max_time: float | None = None,
     labels: str = "xticks-mid",
     fill: bool = True,
+    scale_bar: bool = False,
 ) -> matplotlib.axes.Axes:
     """
     Plot a demes-as-tubes schematic of the graph and the demes' relationships.
 
     Each deme is depicted as a tube, where the tube’s width is
     proportional to the deme’s size at any given time.
     Horizontal lines with arrows indicate either:
@@ -240,14 +244,17 @@
            labels are written in the middle of each deme's tube.
          * ``None``: no labels are written.
 
     :type labels: str or None
     :param fill:
         If True, the inside of the tubes will be painted.
         If False, only the outline of the tubes will be drawn.
+    :param scale_bar:
+        If True, draw a scale bar that indicates population size.
+        If False (*default*), no scale bar will be shown.
     :return:
         The matplotlib axes onto which the figure was drawn.
     """
     if labels not in ("xticks", "legend", "mid", "xticks-legend", "xticks-mid", None):
         raise ValueError(f"Unexpected value for labels: '{labels}'")
 
     if ax is None:
@@ -510,23 +517,42 @@
             )
 
     if title is not None:
         ax.set_title(title)
 
     ax.set_xticks(xticks)
     ax.set_xticklabels(xticklabels)
-    ax.tick_params("x", length=0)
-    ax.spines["top"].set_visible(False)
-    ax.spines["right"].set_visible(False)
-    ax.spines["bottom"].set_visible(False)
+    ax.tick_params(axis="x", length=0)
+    ax.tick_params(axis="x", which="minor", bottom=False)
+    ax.spines[["top", "right", "bottom"]].set_visible(False)
 
     ax.set_ylabel(f"time ago ({graph.time_units})")
 
     ax.set_ylim(1 if log_time else 0, inf_start_time)
 
+    if scale_bar:
+        # Plot a scale bar that indicates the population size.
+        width = utils.size_max(graph)
+        transform = matplotlib.transforms.blended_transform_factory(
+            ax.transData, ax.transAxes
+        )
+        x_offset = min(min(t.size1) for t in tubes.values())
+        ax_sb = ax.inset_axes([x_offset, -0.16, width, 1e-6], transform=transform)
+
+        ax_sb.yaxis.set_major_locator(matplotlib.ticker.NullLocator())
+        ax_sb.spines[["left", "right", "top"]].set_visible(False)
+        ax_sb.xaxis.set_ticks_position("top")
+        locator = matplotlib.ticker.AutoLocator()
+        locator.set_params(integer=True)
+        ax_sb.xaxis.set_major_locator(locator)
+        ax_sb.xaxis.set_minor_locator(matplotlib.ticker.AutoMinorLocator())
+        ax_sb.set_xlim(0, width)
+        ax_sb.set_xlabel("deme size (individuals)")
+        ax_sb.xaxis.set_label_position("bottom")
+
     # Status bar text when in interactive mode.
     def format_coord(x, y):
         return f"time={y:.1f}"
 
     ax.format_coord = format_coord
 
     # Note: we must hold a reference to the motion_notify_event callback,
```

### Comparing `demesdraw-0.3.1/demesdraw/utils.py` & `demesdraw-0.4.0/demesdraw/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from __future__ import annotations
 import itertools
 import math
 from typing import Dict, List, Mapping, Set, Tuple, Union
 import warnings
 
-import cvxpy as cp
 import demes
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+import scipy.optimize
 
 __all__ = [
     "get_fig_axes",
     "size_max",
     "size_min",
     "log_size_heuristic",
     "log_time_heuristic",
     "separation_heuristic",
+    "minimal_crossing_positions",
+    "optimise_positions",
 ]
 
 
 # Override the symbols that are returned when calling dir(<module-name>).
 def __dir__():
     return sorted(__all__)
 
@@ -86,15 +89,15 @@
         else:
             inf_start_time = oldest_noninf_time / (1 - inf_ratio)
     return inf_start_time
 
 
 def _get_colours(
     graph: demes.Graph,
-    colours: ColourOrColourMapping = None,
+    colours: ColourOrColourMapping | None = None,
     default_colour: Colour = "gray",
 ) -> Mapping[str, Colour]:
     """
     Convert the polymorphic ``colours`` into a dictionary of colours,
     keyed by deme name.
 
     :param demes.Graph graph: The graph to which colours will apply.
@@ -104,17 +107,17 @@
           All demes not in the dict will be drawn with ``default_colour``.
         * Otherwise, if ``colours`` can be interpreted as a matplotlib
           colour, all demes will be drawn with this colour.
     :type: dict or str
     """
     if colours is None:
         if len(graph.demes) <= 10:
-            cmap = matplotlib.cm.get_cmap("tab10")
+            cmap = plt.get_cmap("tab10")
         elif len(graph.demes) <= 20:
-            cmap = matplotlib.cm.get_cmap("tab20")
+            cmap = plt.get_cmap("tab20")
         else:
             raise ValueError(
                 "Graph has more than 20 demes, so colours must be specified."
             )
         new_colours = {deme.name: cmap(j) for j, deme in enumerate(graph.demes)}
     elif isinstance(colours, Mapping):
         bad_names = list(colours.keys() - set([deme.name for deme in graph.demes]))
@@ -134,15 +137,15 @@
                 f"Colour '{colours}' not interpretable as a matplotlib colour"
             ) from e
         new_colours = {deme.name: colour for deme in graph.demes}
     return new_colours
 
 
 def get_fig_axes(
-    aspect: float = None, scale: float = None, **kwargs
+    aspect: float | None = None, scale: float | None = None, **kwargs
 ) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
     """
     Get a matplotlib figure and axes.
 
     The default width and height of a matplotlib figure is 6.4 x 4.8 inches.
     To create axes on a figure with other sizes, the ``figsize`` argument
     can be passed to :func:`matplotlib.pyplot.subplots`.
@@ -169,15 +172,19 @@
     """
     if aspect is None:
         aspect = 9.0 / 16.0
     if scale is None:
         scale = 1.0
     fig, ax = plt.subplots(figsize=scale * plt.figaspect(aspect), **kwargs)
     if not fig.get_constrained_layout():
-        fig.set_tight_layout(True)
+        if hasattr(fig, "set_layout_engine"):
+            fig.set_layout_engine("tight")
+        else:
+            # matplotlib < 3.6 compat
+            fig.set_tight_layout(True)
     return fig, ax
 
 
 def size_max(graph: demes.Graph) -> float:
     """
     Get the maximum deme size in the graph.
 
@@ -272,35 +279,35 @@
     dm_j: Union[demes.Deme, demes.AsymmetricMigration],
     dm_k: Union[demes.Deme, demes.AsymmetricMigration],
 ) -> bool:
     """Returns true if dm_j and dm_k intersect in time."""
     return not (dm_j.end_time >= dm_k.start_time or dm_k.end_time >= dm_j.start_time)
 
 
-def coexistence_indices(graph: demes.Graph) -> List[Tuple[int, int]]:
+def _coexistence_indices(graph: demes.Graph) -> List[Tuple[int, int]]:
     """Pairs of indices of demes that exist simultaneously."""
     contemporaries = []
     for j, deme_j in enumerate(graph.demes):
         for k, deme_k in enumerate(graph.demes[j + 1 :], j + 1):
             if _intersect(deme_j, deme_k):
                 contemporaries.append((j, k))
     return contemporaries
 
 
-def successors_indices(graph: demes.Graph) -> Dict[int, List[int]]:
+def _successors_indices(graph: demes.Graph) -> Dict[int, List[int]]:
     """Graph successors, but use indices rather than deme names"""
     idx = {deme.name: j for j, deme in enumerate(graph.demes)}
     successors = dict()
     for deme, children in graph.successors().items():
         if len(children) > 0:
             successors[idx[deme]] = [idx[child] for child in children]
     return successors
 
 
-def interactions_indices(graph: demes.Graph, *, unique: bool) -> List[Tuple[int, int]]:
+def _interactions_indices(graph: demes.Graph, *, unique: bool) -> List[Tuple[int, int]]:
     """Pairs of indices of demes that exchange migrants (migrations or pulses)."""
     idx = {deme.name: j for j, deme in enumerate(graph.demes)}
     interactions = []
     for migration in graph.migrations:
         interactions.append((idx[migration.source], idx[migration.dest]))
     for pulse in graph.pulses:
         for source in pulse.sources:
@@ -315,14 +322,26 @@
             i2.add((a, b))
         interactions = list(i2)
 
     return interactions
 
 
 def _get_line_candidates(graph: demes.Graph, unique: bool):
+    """
+    Construct candidate orderings that, if present, would cause lines to cross.
+
+    Each candidate is a triplet of demes, [A, B, C], which says that when the
+    demes A,B,C are ordered with B between A and C, then there will be a line
+    drawn between A and C that will cross deme B.
+
+    :return:
+        A 2d numpy array of candidate indices, where each row is a candidate
+        triplet, and the array entries are the deme indexes (which correspond
+        to the ordering of the demes in the graph).
+    """
     candidates = []
     # Ancestry lines.
     for child in graph.demes:
         for parent_name in child.ancestors:
             for deme in graph.demes:
                 if deme is child or deme.name == parent_name:
                     continue
@@ -363,15 +382,15 @@
 
     :param xx:
         The positions of the demes in the graph. This is a 2d array,
         where each row in xx is a distinct vector of proposed positions.
         Specifically, xx[j, k] is the position of deme k in the j'th
         proposed positions vector.
     :param candidates:
-        A 2d array of candidate indices.
+        A 2d array of candidate indices. See _get_line_candidates().
     :return:
         The number of lines crossing demes. This is a 1d array
         of counts, one for each vector of proposed positions.
     """
     if candidates.size == 0:
         return np.array(0)
     a = xx[..., candidates[:, 0]]
@@ -383,39 +402,47 @@
 
 
 def minimal_crossing_positions(
     graph: demes.Graph,
     *,
     sep: float,
     unique_interactions: bool,
-    maxiter: int = 1000000,
+    maxiter: int = 1_000_000,
     seed: int = 1234,
 ) -> Dict[str, float]:
     """
-    Find an ordering of demes that minimises line crossings.
+    Find an ordering of demes that minimises lines crossing demes.
 
-    Lines may be for ancestry, pulses, or migrations. A naive algorithm is
-    used to search for the optimal ordering: if :math:`n!` <= ``maxiter``,
-    where ``n`` is the number of demes in the graph, then all possible
-    orderings may be evaluated; otherwise up to ``maxiter`` random
-    permutations are evaluated. If a proposed ordering produces zero line
-    crossings, the algorithm terminates early.
+    Lines may be for ancestry, pulses, or migrations. Finding the optimal
+    ordering is hard, but counting how many lines cross for any given ordering
+    is simple, and can be calculated for multiple candidate orderings using
+    vectorised numpy operations. So a naive algorithm is used to search for
+    a good ordering:
+
+      - if :math:`n!` <= ``maxiter``, where ``n`` is the number of demes in the
+        graph, then all possible orderings may be evaluated,
+      - otherwise up to ``maxiter`` random orderings are evaluated.
+
+    If a proposed ordering produces zero line crossings, the algorithm
+    terminates early. Furthermore, if no ordering is superior to the order
+    that demes were specified in the model (i.e. the order in ``graph.demes``),
+    then the model's order will be used.
 
     :param graph:
         Graph for which positions should be obtained.
     :param sep:
         The separation distance between demes.
     :param maxiter:
         Maximum number of orderings to search through.
     :param seed:
         Seed for the random number generator.
     :return:
         A dictionary mapping deme names to positions.
     """
-    # Initial ordering.
+    # Initial ordering according to the model.
     x0 = np.arange(0, sep * len(graph.demes), sep)
 
     def propose_positions_batches(num_proposals: int, batch_size=200):
         n = len(graph.demes)
         if math.factorial(n) <= num_proposals:
             # Generate all permutations.
             iperms = itertools.permutations(x0, n)
@@ -447,70 +474,118 @@
                 x_best = x_proposal_batch[best]
                 if crosses == 0:
                     break
 
     return {deme.name: float(pos) for deme, pos in zip(graph.demes, x_best)}
 
 
-def cvxpy_optimise(
+def _optimise_positions_objective(x, successors, interactions):
+    """
+    Objective to be minimised by optimise_positions().
+
+    :return:
+        A 2-tuple of (f(x), g(x)), where f is the objective function
+        and g is the Jacobian (a vector of partial derivatives of f).
+    """
+    f = 0
+    g = np.zeros_like(x)
+    for parent, children in successors.items():
+        a = x[parent]
+        b = np.mean([x[child] for child in children])
+        f += (a - b) ** 2
+        g[parent] += 2 * (a - b)
+        for child in children:
+            g[child] += 2 * (b - a) / len(children)
+    for j, k in interactions:
+        f += (x[j] - x[k]) ** 2
+        g[j] += 2 * (x[j] - x[k])
+        g[k] += 2 * (x[k] - x[j])
+    return f, g
+
+
+def optimise_positions(
     graph: demes.Graph,
-    positions: Mapping[str, float],
     *,
+    positions: Mapping[str, float],
     sep: float,
     unique_interactions: bool,
 ) -> Dict[str, float]:
     """
     Optimise the given positions into a tree-like layout.
 
-    Convex optimisation is used to minimise the distances:
-
+    The objective is to minimise the distances:
       - from each parent deme to the mean position of its children,
       - and between interacting demes (where interactions are either
         migrations or pulses).
 
-    Subject to the constraints that:
-
-      - demes are ordered like in the input ``positions``,
-      - and demes have a minimum separation distance ``sep``.
+    Subject to the constraints that contemporaneous demes:
+      - are ordered like in the input ``positions``,
+      - and have a minimum separation distance ``sep``.
 
     :param graph:
         Graph for which positions should be optimised.
     :param positions:
         A dictionary mapping deme names to positions.
     :param sep:
         The minimum separation distance between contemporary demes.
     :return:
         A dictionary mapping deme names to positions.
     """
-    contemporaries = coexistence_indices(graph)
+    contemporaries = _coexistence_indices(graph)
+    successors = _successors_indices(graph)
+    interactions = _interactions_indices(graph, unique=unique_interactions)
     if len(contemporaries) == 0:
         # There are no constraints, so stack demes on top of each other.
         return {deme.name: 0 for deme in graph.demes}
-    successors = successors_indices(graph)
-    interactions = interactions_indices(graph, unique=unique_interactions)
-
-    vs = [cp.Variable() for _ in graph.demes]
-    # Place the root at position 0.
-    vs[0].value = 0
-
-    z = 0
-    for parent, children in successors.items():
-        a = vs[parent]
-        b = sum(vs[child] for child in children) / len(children)
-        z += (a - b) ** 2
-    if len(interactions) > 0:
-        z += cp.sum_squares(cp.hstack([vs[j] - vs[k] for j, k in interactions]))
-    objective = cp.Minimize(z)
-
-    constraints = []
-    x = np.array([positions[deme.name] for deme in graph.demes])
+    if len(successors) == 0 and len(interactions) == 0:
+        # Nothing to optimise. Use the positions provided to us.
+        return dict(positions)
+
+    x0 = np.array([positions[deme.name] for deme in graph.demes])
+    # Place the first deme at position 0.
+    x0 -= x0[0]
+
+    # Build matrix of linear constraints to ensure that contemporaries
+    # are ordered and separated by sep.
+    C = []
     for j, k in contemporaries:
-        if x[j] < x[k]:
+        if x0[j] < x0[k]:
             j, k = k, j
-        constraints.append(vs[j] - vs[k] >= sep)
+        c = [0] * len(x0)
+        c[j] = 1
+        c[k] = -1
+        C.append(c)
+    constraints = [scipy.optimize.LinearConstraint(C, lb=sep, ub=np.inf)]
+
+    res = scipy.optimize.minimize(
+        _optimise_positions_objective,
+        x0,
+        args=(successors, interactions),
+        # The objective function returns a 2-tuple of (f_x, g_x), where f_x
+        # is the objective evalutated at x, and g_x is the Jacobian of f
+        # evaluated at x.
+        jac=True,
+        # Don't use the quasi-Newton Hessian approximation (the default for
+        # method="trust-constr" if nothing is specified). This performs
+        # poorly, and produces warnings, for some of the test cases.
+        # Writing the Hessian function manually would be tedious,
+        # and I'd certainly get it wrong. But since I did manually
+        # implement the Jacobian, scipy can use a finite-difference
+        # approximation for the Hessian, by specifying either "2-point",
+        # "3-point", or "cs". The "2-point" option seems to work fine.
+        hess="2-point",
+        method="trust-constr",
+        constraints=constraints,
+        bounds=scipy.optimize.Bounds(lb=np.min(x0) - sep, ub=np.max(x0) + sep),
+    )
+
+    if not res.success:
+        warnings.warn(
+            f"Failed to optimise: {res}\n\n"
+            "Please report this in the issue tracker at "
+            "https://github.com/grahamgower/demesdraw/issues"
+        )
+        return dict(positions)
 
-    prob = cp.Problem(objective, constraints)
-    prob.solve("OSQP")
-    if prob.status != cp.OPTIMAL:
-        raise RuntimeError(f"Failed to optimise: {prob}")
+    x = res.x
 
-    return {graph.demes[j].name: float(v.value) for j, v in enumerate(vs)}
+    return {graph.demes[j].name: float(xj) for j, xj in enumerate(x)}
```

### Comparing `demesdraw-0.3.1/demesdraw.egg-info/PKG-INFO` & `demesdraw-0.4.0/demesdraw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demesdraw
-Version: 0.3.1
+Version: 0.4.0
 Summary: drawing tools for Demes demographic models
 Home-page: https://github.com/grahamgower/demesdraw
 Author: Graham Gower
 License: ISC
 Project-URL: Documentation, https://grahamgower.github.io/demesdraw/
 Project-URL: Source Code, https://github.com/grahamgower/demesdraw
 Project-URL: Bug Tracker, https://github.com/grahamgower/demesdraw/issues
```

### Comparing `demesdraw-0.3.1/demesdraw.egg-info/SOURCES.txt` & `demesdraw-0.4.0/demesdraw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 docs/_config.yml
 docs/_toc.yml
 docs/api.md
 docs/build.sh
 docs/cli.md
 docs/examples.ipynb
 docs/is_new_stable.py
+docs/layout.md
 docs/quickstart.md
 docs/_ext/inject_version.py
 docs/_static/AmericanAdmixture_4B11_size_history.svg
 docs/_static/AmericanAdmixture_4B11_tubes.svg
 docs/_static/AmericanAdmixture_4B11_tubes_custom.svg
+docs/_static/custom.css
 examples/bottleneck.yaml
 examples/cloning_example.yaml
 examples/defaults_asymmetric_migration_changing_rate.yaml
 examples/defaults_deme_ancestors.yaml
 examples/defaults_deme_many_epochs_global.yaml
 examples/defaults_deme_many_epochs_local.yaml
 examples/defaults_deme_many_epochs_overrides.yaml
```

### Comparing `demesdraw-0.3.1/docs/CHANGELOG.md` & `demesdraw-0.4.0/docs/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [0.4.0] - 2023-05-03
+
+* Documented the layout algorithm used in tubes plots.
+* Added `scale_bar` option to `demesdraw.tubes()`, and `--scale-bar` option
+  to the `demesdraw tubes` CLI, to draw a scale bar that indicates the
+  population size.
+* Removed dependency on `cvxpy` by going back to `scipy`
+  for optimisation of the deme positions. The trust-constr
+  method with linear constraints seems to work well.
+
 ## [0.3.1] - 2022-09-19
 
 * Added mouseover annotation popups for interactive tubes plots.
 * Dropped support for Python 3.6.
 * Performance improvement when calculating tube positions.
 * Fix incompatibility with "legend" labels and matplotlib 3.6.0.
```

### Comparing `demesdraw-0.3.1/docs/_config.yml` & `demesdraw-0.4.0/docs/_config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 # Book settings
 # Learn more at https://jupyterbook.org/customize/config.html
 
 title: DemesDraw
 author: Graham Gower
-copyright: "2021"
+copyright: "2021-2023"
 only_build_toc_files: true
 
 execute:
   execute_notebooks: cache
   timeout: 100
 
 repository:
   url: https://github.com/grahamgower/demesdraw
   path_to_book: docs
   branch: main
 
-html:
-  use_issues_button: true
-  use_repository_button: true
-  use_edit_page_button: true
-
 sphinx:
   extra_extensions:
   - sphinx.ext.autodoc
   - sphinx.ext.viewcode
   - sphinx.ext.intersphinx
   - sphinxcontrib.programoutput
   - sphinx_issues
 
   local_extensions:
     # Add version string to the navbar and footer.
-    inject_version: _ext
+    # Works with sphinx-book-theme, but not with piccolo_theme.
+    #inject_version: _ext
 
   config:
     autodoc_typehints: description
     intersphinx_mapping:
       python: ["https://docs.python.org/3/", null]
       demes: ["https://popsim-consortium.github.io/demes-docs/stable/", null]
       matplotlib: ["https://matplotlib.org/stable/", null]
     issues_github_path: grahamgower/demesdraw
+
+    html_show_sphinx: false
+    # https://piccolo-theme.readthedocs.io/
+    html_theme: "piccolo_theme"
+    # some custom css to fix piccolo/notebook in dark modes
+    html_static_path: ["_static"]
+    html_css_files: ["custom.css"]
+
+    html_theme_options:
+        globaltoc_collapse: false
+        globaltoc_maxdepth: -1
+        globaltoc_includehidden: true
+
+        ## piccolo_theme options
+        #dark_mode_code_blocks: false
+        source_url: https://github.com/grahamgower/demesdraw
```

### Comparing `demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_size_history.svg` & `demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_size_history.svg`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_tubes.svg` & `demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_tubes.svg`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/_static/AmericanAdmixture_4B11_tubes_custom.svg` & `demesdraw-0.4.0/docs/_static/AmericanAdmixture_4B11_tubes_custom.svg`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/build.sh` & `demesdraw-0.4.0/docs/build.sh`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/examples.ipynb` & `demesdraw-0.4.0/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/is_new_stable.py` & `demesdraw-0.4.0/docs/is_new_stable.py`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/docs/quickstart.md` & `demesdraw-0.4.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/cloning_example.yaml` & `demesdraw-0.4.0/examples/cloning_example.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/defaults_deme_ancestors.yaml` & `demesdraw-0.4.0/examples/defaults_deme_ancestors.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/defaults_deme_many_epochs_overrides.yaml` & `demesdraw-0.4.0/examples/defaults_deme_many_epochs_overrides.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/linear_size_function_example.yaml` & `demesdraw-0.4.0/examples/linear_size_function_example.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/lots_of_ancestors.yaml` & `demesdraw-0.4.0/examples/lots_of_ancestors.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/offshoots.yaml` & `demesdraw-0.4.0/examples/offshoots.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/reticulate.yaml` & `demesdraw-0.4.0/examples/reticulate.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/AraTha__African3Epoch_1H18.yaml` & `demesdraw-0.4.0/examples/stdpopsim/AraTha__African3Epoch_1H18.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/AraTha__SouthMiddleAtlas_1D17.yaml` & `demesdraw-0.4.0/examples/stdpopsim/AraTha__SouthMiddleAtlas_1D17.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/DroMel__African3Epoch_1S16.yaml` & `demesdraw-0.4.0/examples/stdpopsim/DroMel__African3Epoch_1S16.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/DroMel__OutOfAfrica_2L06.yaml` & `demesdraw-0.4.0/examples/stdpopsim/DroMel__OutOfAfrica_2L06.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__AmericanAdmixture_4B11.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__AmericanAdmixture_4B11.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__AncientEurasia_9K19.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__AncientEurasia_9K19.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__AshkSub_7G19.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__AshkSub_7G19.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfricaArchaicAdmixture_5R19.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfricaArchaicAdmixture_5R19.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfrica_2T12.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfrica_2T12.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__OutOfAfrica_3G09.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__OutOfAfrica_3G09.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/HomSap__PapuansOutOfAfrica_10J19.yaml` & `demesdraw-0.4.0/examples/stdpopsim/HomSap__PapuansOutOfAfrica_10J19.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/stdpopsim/PonAbe__TwoSpecies_2L11.yaml` & `demesdraw-0.4.0/examples/stdpopsim/PonAbe__TwoSpecies_2L11.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/examples/utility_graph.yaml` & `demesdraw-0.4.0/examples/utility_graph.yaml`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/setup.cfg` & `demesdraw-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 	Bug Tracker = https://github.com/grahamgower/demesdraw/issues
 
 [options]
 packages = demesdraw
 include_package_data = True
 python_requires = >= 3.7
 install_requires = 
-	cvxpy
 	demes >= 0.2.0
 	matplotlib >= 3.3.1
 	numpy >= 1.20.0
+	scipy
 setup_requires = 
 	setuptools
 	setuptools_scm
 
 [options.entry_points]
 console_scripts = 
 	demesdraw = demesdraw.__main__:cli
@@ -57,14 +57,20 @@
 
 [mypy-ruamel.*]
 ignore_missing_imports = True
 
 [mypy-matplotlib.*]
 ignore_missing_imports = True
 
+[mypy-mpmath.*]
+ignore_missing_imports = True
+
+[mypy-scipy.*]
+ignore_missing_imports = True
+
 [tool:pytest]
 addopts = -n auto
 testpaths = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `demesdraw-0.3.1/tests/__init__.py` & `demesdraw-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `demesdraw-0.3.1/tests/plot_examples.py` & `demesdraw-0.4.0/tests/plot_examples.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from demesdraw import utils
 from tests import example_files
 
 
 with PdfPages("spacing.pdf") as pdf:
     for _n in range(30):
         n = _n + 1
+        print(n)
         b = demes.Builder(defaults=dict(epoch=dict(start_size=100)))
         for j in range(n):
             b.add_deme(f"d{j}")
             if j > 0:
                 b.add_migration(demes=[f"d{j - 1}", f"d{j}"], rate=1e-5)
         graph = b.resolve()
 
@@ -23,17 +24,17 @@
         if n > 20:
             colours = "black"
         ax = demesdraw.tubes(graph, colours=colours)
         pdf.savefig(ax.figure)
         plt.close(ax.figure)
 
 with PdfPages("examples.pdf") as pdf:
-
     for filename in sorted(example_files()):
         title = filename.name
+        print(title)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", "Multiple pulses", UserWarning, "demes")
             graph = demes.load(filename)
 
         fig, (ax1, ax2) = utils.get_fig_axes(
             scale=1.5, nrows=2, constrained_layout=True
         )
@@ -50,11 +51,12 @@
         )
         demesdraw.tubes(
             graph,
             ax=ax2,
             log_time=log_time,
             # fill=False,
             # colours="black",
+            scale_bar=True,
         )
 
         pdf.savefig(fig)
         plt.close(fig)
```

### Comparing `demesdraw-0.3.1/tests/test_cli.py` & `demesdraw-0.4.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,17 @@
                 f"python -m demesdraw {subcommand} {params} "
                 f"{input_file} {output_file}".split(),
                 check=True,
             )
             assert output_file.exists()
             assert output_file.stat().st_size > 0
 
+    def test_tubes_scale_bar(self):
+        self.test_output_file_is_created("tubes", "--scale-bar")
+
     @pytest.mark.parametrize("subcommand", ["tubes", "size_history"])
     def test_input_from_stdin(self, subcommand):
         input_file = tests.example_files()[0]
         with tempfile.TemporaryDirectory() as tmpdir:
             output_file = pathlib.Path(tmpdir) / "plot.pdf"
             with open(input_file) as f:
                 subprocess.run(
```

### Comparing `demesdraw-0.3.1/tests/test_demesdraw.py` & `demesdraw-0.4.0/tests/test_demesdraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     @pytest.mark.parametrize(
         "labels", ["xticks", "legend", "mid", "xticks-legend", "xticks-mid"]
     )
     @pytest.mark.parametrize("graph", tests.example_graphs())
     def test_labels_params(self, graph, labels):
         self.check_tubes(graph, labels=labels)
 
+    @pytest.mark.parametrize("scale_bar", [True, False])
+    @pytest.mark.parametrize("graph", tests.example_graphs())
+    def test_scale_bar(self, graph, scale_bar):
+        self.check_tubes(graph, scale_bar=scale_bar)
+
     @pytest.mark.parametrize(
         "colours", [None, "black", dict(), dict(A="red", B="blue", C="pink")]
     )
     def test_colours_params(self, colours):
         b = demes.Builder(defaults=dict(epoch=dict(start_size=1000)))
         b.add_deme("A", epochs=[dict(end_time=100)])
         b.add_deme("B", ancestors=["A"])
```

### Comparing `demesdraw-0.3.1/tests/test_import_visibility.py` & `demesdraw-0.4.0/tests/test_import_visibility.py`

 * *Files identical despite different names*

