# Comparing `tmp/tmmc-lnpy-0.2.2.tar.gz` & `tmp/tmmc-lnpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmmc-lnpy-0.2.2.tar", last modified: Thu Apr  6 00:17:05 2023, max compression
+gzip compressed data, was "tmmc-lnpy-0.3.0.tar", last modified: Wed May  3 03:05:36 2023, max compression
```

## Comparing `tmmc-lnpy-0.2.2.tar` & `tmmc-lnpy-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,96 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:05.011173 tmmc-lnpy-0.2.2/
--rw-r--r--   0 wpk      (42033)    36681     1324 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681     1336 2023-04-04 22:04:31.000000 tmmc-lnpy-0.2.2/.gitignore
--rw-r--r--   0 wpk      (42033)    36681     2863 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     6734 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681       59 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/HISTORY.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      330 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     8345 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/Makefile
--rw-r--r--   0 wpk      (42033)    36681     6086 2023-04-06 00:17:05.011432 tmmc-lnpy-0.2.2/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     3368 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:04.973558 tmmc-lnpy-0.2.2/environment/
--rw-r--r--   0 wpk      (42033)    36681     1121 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      252 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      120 2023-04-05 16:50:00.000000 tmmc-lnpy-0.2.2/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       76 2023-04-06 00:12:02.000000 tmmc-lnpy-0.2.2/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      728 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      422 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       27 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      149 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      158 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     4176 2023-04-06 00:12:02.000000 tmmc-lnpy-0.2.2/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681      387 2023-04-06 00:17:05.012301 tmmc-lnpy-0.2.2/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-06 00:12:02.000000 tmmc-lnpy-0.2.2/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:04.958479 tmmc-lnpy-0.2.2/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:04.976102 tmmc-lnpy-0.2.2/src/lnPi/
--rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnPi/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnPi/collectionlnpiutils.py
--rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnPi/stability.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:04.993250 tmmc-lnpy-0.2.2/src/lnpy/
--rw-r--r--   0 wpk      (42033)    36681     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     3478 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/bracket.py
--rw-r--r--   0 wpk      (42033)    36681     6004 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/cached_decorators.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:05.000149 tmmc-lnpy-0.2.2/src/lnpy/data/
--rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.2.2/src/lnpy/data/hsmix_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    38953 2022-09-28 17:20:41.000000 tmmc-lnpy-0.2.2/src/lnpy/data/lj_sub_example.json
--rw-r--r--   0 wpk      (42033)    36681    38751 2022-09-28 17:20:41.000000 tmmc-lnpy-0.2.2/src/lnpy/data/lj_sup_example.json
--rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.2.2/src/lnpy/data/ljmix_sup_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    61595 2022-09-28 17:20:41.000000 tmmc-lnpy-0.2.2/src/lnpy/data/watermof_example.json
--rw-r--r--   0 wpk      (42033)    36681    34464 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/ensembles.py
--rw-r--r--   0 wpk      (42033)    36681     4997 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/examples.py
--rw-r--r--   0 wpk      (42033)    36681    13241 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/extensions.py
--rw-r--r--   0 wpk      (42033)    36681    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/lnpicollectionutils.py
--rw-r--r--   0 wpk      (42033)    36681    18821 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/lnpidata.py
--rw-r--r--   0 wpk      (42033)    36681    22910 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/lnpienergy.py
--rw-r--r--   0 wpk      (42033)    36681    26231 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/lnpiseries.py
--rw-r--r--   0 wpk      (42033)    36681    15177 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/maskedlnpi_legacy.py
--rw-r--r--   0 wpk      (42033)    36681     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/molfrac.py
--rw-r--r--   0 wpk      (42033)    36681     3361 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/options.py
--rw-r--r--   0 wpk      (42033)    36681    20723 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/segment.py
--rw-r--r--   0 wpk      (42033)    36681    26451 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/stability.py
--rw-r--r--   0 wpk      (42033)    36681    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/src/lnpy/utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:05.010842 tmmc-lnpy-0.2.2/src/tmmc_lnpy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     1423 2023-04-06 00:17:04.000000 tmmc-lnpy-0.2.2/src/tmmc_lnpy.egg-info/SOURCES.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:05.005576 tmmc-lnpy-0.2.2/tests/
--rw-r--r--   0 wpk      (42033)    36681     2531 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/tests/test_hs_mix.py
--rw-r--r--   0 wpk      (42033)    36681       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.2.2/tests/test_import.py
--rw-r--r--   0 wpk      (42033)    36681     1843 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/tests/test_lj_mix_0.py
--rw-r--r--   0 wpk      (42033)    36681     5231 2023-04-05 21:34:43.000000 tmmc-lnpy-0.2.2/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033)    36681     5834 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/tests/test_single_comp_sub.py
--rw-r--r--   0 wpk      (42033)    36681     5072 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/tests/test_single_comp_super.py
--rw-r--r--   0 wpk      (42033)    36681     2801 2023-04-04 21:54:21.000000 tmmc-lnpy-0.2.2/tests/test_water_cluster.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:17:05.010230 tmmc-lnpy-0.2.2/tests/water_cluster/
--rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/data_0.csv
--rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/data_0_dw.csv
--rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/data_1.csv
--rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/data_1_dw.csv
--rw-r--r--   0 wpk      (42033)    36681      367 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/water_MOF_ensemble.json
--rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.2.2/tests/water_cluster/water_MOF_example.csv
--rw-r--r--   0 wpk      (42033)    36681     3991 2023-04-06 00:12:02.000000 tmmc-lnpy-0.2.2/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.321590 tmmc-lnpy-0.3.0/
+-rw-r--r--   0 wpk      (42033)    36681     1478 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681     1324 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3681 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.3.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     1834 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9178 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11319 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     7758 2023-05-03 03:05:36.322018 tmmc-lnpy-0.3.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     3274 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.249916 tmmc-lnpy-0.3.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.250654 tmmc-lnpy-0.3.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.252360 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.266048 tmmc-lnpy-0.3.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      961 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      317 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment.yaml
+-rw-r--r--   0 wpk      (42033)    36681     6157 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.272827 tmmc-lnpy-0.3.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      396 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681      290 2023-05-03 03:05:36.323648 tmmc-lnpy-0.3.0/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.0/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.236716 tmmc-lnpy-0.3.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.276264 tmmc-lnpy-0.3.0/src/lnPi/
+-rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/collectionlnpiutils.py
+-rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/stability.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.291583 tmmc-lnpy-0.3.0/src/lnpy/
+-rw-r--r--   0 wpk      (42033)    36681     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/bracket.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.297421 tmmc-lnpy-0.3.0/src/lnpy/data/
+-rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.0/src/lnpy/data/hsmix_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/lj_sub_example.json
+-rw-r--r--   0 wpk      (42033)    36681    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/lj_sup_example.json
+-rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.0/src/lnpy/data/ljmix_sup_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/watermof_example.json
+-rw-r--r--   0 wpk      (42033)    36681     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/ensembles.py
+-rw-r--r--   0 wpk      (42033)    36681     4997 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/examples.py
+-rw-r--r--   0 wpk      (42033)    36681    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/extensions.py
+-rw-r--r--   0 wpk      (42033)    36681    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpicollectionutils.py
+-rw-r--r--   0 wpk      (42033)    36681    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpidata.py
+-rw-r--r--   0 wpk      (42033)    36681    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpienergy.py
+-rw-r--r--   0 wpk      (42033)    36681    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpiseries.py
+-rw-r--r--   0 wpk      (42033)    36681    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/maskedlnpi_legacy.py
+-rw-r--r--   0 wpk      (42033)    36681     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/molfrac.py
+-rw-r--r--   0 wpk      (42033)    36681     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/options.py
+-rw-r--r--   0 wpk      (42033)    36681    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/segment.py
+-rw-r--r--   0 wpk      (42033)    36681    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/stability.py
+-rw-r--r--   0 wpk      (42033)    36681    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/utils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.305162 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     7758 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2061 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-14 22:53:56.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033)    36681      112 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       10 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.312001 tmmc-lnpy-0.3.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_hs_mix.py
+-rw-r--r--   0 wpk      (42033)    36681       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.3.0/tests/test_import.py
+-rw-r--r--   0 wpk      (42033)    36681     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_lj_mix_0.py
+-rw-r--r--   0 wpk      (42033)    36681     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033)    36681     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_single_comp_sub.py
+-rw-r--r--   0 wpk      (42033)    36681     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_single_comp_super.py
+-rw-r--r--   0 wpk      (42033)    36681     2801 2023-04-15 00:15:07.000000 tmmc-lnpy-0.3.0/tests/test_water_cluster.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.320558 tmmc-lnpy-0.3.0/tests/water_cluster/
+-rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_0.csv
+-rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_0_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_1.csv
+-rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_1_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_ensemble.json
+-rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_example.csv
+-rw-r--r--   0 wpk      (42033)    36681     3774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tox.ini
```

### Comparing `tmmc-lnpy-0.2.2/.cruft.json` & `tmmc-lnpy-0.3.0/.cruft.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8432017543859649%*

 * *Differences: {"'commit'": "'cb20a32f67dadb4142be54898a87de1efdce6bd6'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(4, 'docs/_static/css/*'), (5, "*

 * *              "'docs/_static/js/*'), (6, 'changelog.d/templates/*'), (7, "*

 * *              "'changelog.d/templates/auto-changlog/*')]}}}",*

 * * "'skip'": "{insert: [(1, 'docs/examples/usage/demo.ipynb'), (2, 'examples/usage/demo.ipynb'), (3, "*

 * *           "'docs/examples/example-usage.md')], delete: [4, 3, 2, 1]}"}*

```diff
@@ -1,17 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "7a176a00a6d92c034b696c2a8a672bac5a6d5aab",
+    "commit": "cb20a32f67dadb4142be54898a87de1efdce6bd6",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
-                "docs/_templates/autodocsumm/*.rst"
+                "docs/_templates/autodocsumm/*.rst",
+                "docs/_static/css/*",
+                "docs/_static/js/*",
+                "changelog.d/templates/*",
+                "changelog.d/templates/auto-changlog/*"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
@@ -28,14 +32,13 @@
             "use_pytest": "y",
             "version": "0.0.1"
         }
     },
     "directory": null,
     "skip": [
         "src/lnpy/__init__.py",
-        "environment.yaml",
-        "docs/api.md",
-        "docs/index.md",
-        "docs/spelling_wordlist.txt"
+        "docs/examples/usage/demo.ipynb",
+        "examples/usage/demo.ipynb",
+        "docs/examples/example-usage.md"
     ],
     "template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git"
 }
```

### Comparing `tmmc-lnpy-0.2.2/.gitignore` & `tmmc-lnpy-0.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
-dist-conda/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -103,11 +102,11 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
-/docs/generated/
+/docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/
-/docs/reference/generated
+/dist-conda/*
+!/dist-conda/Makefile
```

### Comparing `tmmc-lnpy-0.2.2/.pre-commit-config.yaml` & `tmmc-lnpy-0.3.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,136 @@
 ---
 # pre-commit install
 # pre-commit run --all-files
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+default_install_hook_types:
+  - pre-commit
+  - commit-msg
 repos:
+  #* Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-yaml
-        #     args: [--unsafe]
-  # Ruff
+      - id: check-json
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+  #* Formatting
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v3.0.0-alpha.6"
+    hooks:
+      - id: prettier
+        stages: [commit]
+        additional_dependencies:
+          - prettier-plugin-toml
+        exclude: ^examples/archived/|^src/lnpy/data/|^tests/water_cluster/
+  #** markdown
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.6.0
+    hooks:
+      - id: markdownlint-cli2
+        args: ["--style prettier"]
+  #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.254'
+    rev: "v0.0.261"
     hooks:
       - id: ruff
-        args: ["--fix"]
-  # isort should run before black as black sometimes tweaks the isort output
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        stages: [manual]
-  # https://github.com/python/black#version-control-integration
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
-      - id: black-jupyter
+      # - id: black-jupyter
+      # Move to just black.  use nbqa for notebook formatting
+      - id: black
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"  # replace with latest tag on GitHub
+    rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==23.1.0
+          - black==23.3.0
         exclude: ^README.md
-  - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: blackdoc
-        additional_dependencies: ["black==23.1.0"]
-      - id: blackdoc-autoupdate-black
-  - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+      - id: nbqa-ruff
+        additional_dependencies: [ruff]
+        exclude: ^examples/archived/
+      - id: nbqa-black
+        additional_dependencies: [black]
+
+  #* Commit message
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v3.0.1
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+
+  #* Manual Linting
+  - repo: local
     hooks:
-      - id: codespell
-        types_or: [python, rst, markdown, cython, c]
-        additional_dependencies: [tomli]
-        args: [-I, docs/spelling_wordlist.txt]
+      - id: mypy
+        name: mypy
+        entry: tox
+        args: ["-e", "lint-mypy"]
+        language: system
+        pass_filenames: false
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
+      - id: pyright
+        name: pyright
+        entry: pyright
+        args: []
+        language: system
+        pass_filenames: true
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
         stages: [manual]
-  # this should be run before flake8 to
-  # this should be run externally
-  # messes up too many things
-  # - repo: https://github.com/PyCQA/docformatter
-  #   rev: v1.5.0
-  #   hooks:
-  #     - id: docformatter
-  #       args: [--in-place]
+  # isort, pyupgrade, flake8 defer to ruff
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        stages: [manual]
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        stages: [manual]
+        args: [--py38-plus]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         stages: [manual]
-        additional_dependencies: [flake8-docstrings]
+        additional_dependencies:
+          - flake8-docstrings
+          - Flake8-pyproject
+          # - pep8-naming
+          # - flake8-rst-docstrings
         exclude: ^tests/|^src/lnpy/tests/|^docs/conf.py|^setup.py
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: mypy
-        # `properies` & `asv_bench` are copied from setup.cfg.
-        # `_typed_ops.py` is added since otherwise mypy will complain (but notably only in pre-commit)
-        exclude: properties|asv_bench|_typed_ops.py|conf.py
-        # This is slow and so we take it out of the fast-path; requires passing
-        # `--hook-stage manual` to pre-commit
+      - id: nbqa-pyupgrade
+        additional_dependencies: [pyupgrade]
         stages: [manual]
-        additional_dependencies: [types-pkg_resources, typing-extensions==3.10.0.0, numpy]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+        args: [--py38-plus]
+      - id: nbqa-isort
+        additional_dependencies: [isort]
+        stages: [manual]
+  #** spelling
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
     hooks:
-      - id: pyupgrade
+      - id: codespell
+        types_or: [python, rst, markdown, cython, c]
+        additional_dependencies: [tomli]
+        args: [-I, docs/spelling_wordlist.txt]
         stages: [manual]
-        args:
-          - --py38-plus
-          # remove on f-strings in Py3.7
-          - --keep-percent-format
```

### Comparing `tmmc-lnpy-0.2.2/LICENSE` & `tmmc-lnpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/Makefile` & `tmmc-lnpy-0.3.0/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 endef
 export BROWSER_PYSCRIPT
 
 define PRINT_HELP_PYSCRIPT
 import re, sys
 
 for line in sys.stdin:
-	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
+	match = re.match(r'^([a-zA-Z_/.-]+):.*?## (.*)$$', line)
 	if match:
 		target, help = match.groups()
 		print("%-20s %s" % (target, help))
 endef
 export PRINT_HELP_PYSCRIPT
 
 BROWSER := python -c "$$BROWSER_PYSCRIPT"
@@ -50,54 +50,64 @@
 
 
 
 
 ################################################################################
 # utilities
 ################################################################################
-.PHONY: lint pre-commit-init pre-commit-run pre-commit-run-all pre-commit-lint-extra pre-commit-codespell init
-
-lint: ## check style with flake8
-	flake8 cmomy tests
-
+.PHONY: pre-commit-init pre-commit pre-commit-all
 pre-commit-init: ## install pre-commit
 	pre-commit install
 
-pre-commit-run: ## run pre-commit
+pre-commit: ## run pre-commit
 	pre-commit run
 
-pre-commit-run-all: ## run pre-commit on all files
+pre-commit-all: ## run pre-commit on all files
 	pre-commit run --all-files
 
-pre-commit-manual: ## run pre-commit manual flags
-	pre-commit run --hook-stage manual
+.PHONY: pre-commit-lint pre-commit-lint-notebooks pre-commit-prettier pre-commit-lint-markdown
+pre-commit-lint: ## run ruff and black on on all files
+	pre-commit run --all-files ruff
+	pre-commit run --all-files black
+	pre-commit run --all-files blacken-docs
+
+pre-commit-lint-notebooks: ## Run nbqa linting
+	pre-commit run --all-files nbqa-ruff
+	pre-commit run --all-files nbqa-black
+
+pre-commit-prettier: ## run prettier on all files.
+	pre-commit run --all-files prettier
+
+pre-commit-lint-markdown: ## run markdown linter.
+	pre-commit run --all-files --hook-stage manual markdownlint-cli2
 
-pre-commit-lint-extra: ## run all linting
+.PHONY: pre-commit-lint-extra pre-commit-mypy pre-commit-codespell
+pre-commit-lint-extra: ## run all extra linting (isort, flake8, pyupgrade, nbqa isort and pyupgrade)
 	pre-commit run --all-files --hook-stage manual isort
 	pre-commit run --all-files --hook-stage manual flake8
 	pre-commit run --all-files --hook-stage manual pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-isort
 
 pre-commit-mypy: ## run mypy
 	pre-commit run --all-files --hook-stage manual mypy
 
+pre-commit-pyright: ## run pyright
+	pre-commit run --all-files --hook-stage manual pyright
+
 pre-commit-codespell: ## run codespell. Note that this imports allowed words from docs/spelling_wordlist.txt
 	pre-commit run --all-files --hook-stage manual codespell
 
-.git: ## init git
-	git init
-
-init: .git pre-commit-init ## run git-init pre-commit
-
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo lnpy-env > .venv
+	echo $${PWD}/.tox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -127,28 +137,40 @@
 	python -c 'import lnpy; print(lnpy.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
+ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
+PRETTIER = bash scripts/run-prettier.sh
 
-environment/dev.yaml: environment.yaml environment/dev-extras.yaml ## build development yaml file
+environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
 	conda-merge $^ > $@
+	$(PRETTIER) $@
+
+environment/dev.yaml: ## development environment yaml file
+environment/test.yaml: ## testing environment yaml file
+enviornment/docs.yaml: ## docs environment yaml file
 
-environment/docs.yaml: environment.yaml environment/docs-extras.yaml ## build docs yaml file
-	conda-merge $^ > $@
 
-environment/test.yaml: environment.yaml environment/test-extras.yaml ## build test yaml file
+# special for linters
+environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
+	echo $^
 	conda-merge $^ > $@
+	$(PRETTIER) $@
 
-.PHONY: environment-files
+ENVIRONMENTS += environment/lint.yaml
 
-environment-files: environment/dev.yaml environment/docs.yaml environment/test.yaml ## rebuild all environment files
+.PHONY: environment-files-clean
+environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
+	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
+.PHONY: environment-files-build
+environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
 
 ################################################################################
 # virtual env
 ################################################################################
 .PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
 
 mamba-env: environment.yaml ## create base environment
@@ -162,98 +184,136 @@
 
 mamba-dev-update: environment/dev.yaml ## update development environment
 	mamba env update -f $<
 
 ################################################################################
 # TOX
 ###############################################################################
-tox_posargs?=-v
-TOX=CONDA_EXE=mamba tox $(tox_posargs)
+tox_args?=-v
+version?=
+TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
+
+.PHONY: tox-ipykernel-display-name
+tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
+	bash ./scripts/tox-ipykernel-display-name.sh lnpy
+
+## dev env
+.PHONY: dev-env
+dev-env: environment/dev.yaml ## create development environment using tox
+	tox -e dev
 
 ## testing
-
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox
+test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
 	$(TOX) -- $(posargs)
 
-
 ## docs
-.PHONY: docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-open docs-live docs-clean-build docs-linkcheck
-posargs=
+.PHONY: docs-examples-symlink
+docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
+	bash ./scripts/docs-examples-symlinks.sh
+
+
+.PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use posargs=... to override stuff
-	$(TOX) -e $@ -- $(posargs)
+docs-release: ## release docs.  use release_args=... to override stuff
+	$(TOX) -e docs -- release
+docs-command: ## run command with command=...
+	$(TOX) -e docs -- command
+
+.PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e $@ -- $(posargs)
-docs-nist-pages: ## do both build and releas
-	$(TOX) -e $@ -- $(posargs)
-docs-live: ## use autobuild for docs
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- spelling
+docs-livehtml: ## use autobuild for docs
+	$(TOX) -e docs -- livehtml
 docs-open: ## open the build
 	$(BROWSER) docs/_build/html/index.html
 docs-linkcheck: ## check links
-	$(TOX) -e docs-build -- linkcheck
+	$(TOX) -e docs -- linkcheck
 
-docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-live: environment/docs.yaml
+docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
+## linting
+.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
+lint-mypy: ## run mypy mypy_args=...
+	$(TOX) -e lint -- mypy
+lint-pyright: ## run pyright pyright_args=...
+	$(TOX) -e lint -- pyright
+lint-pytype: ## run pytype pytype_args=...
+	$(TOX) -e lint -- pytype
+lint-all:
+	$(TOX) -e lint -- all
+lint-command:
+	$(TOX) -e lint -- command
+
+lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
 
 ## distribution
-.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-conda-recipe dist-conda-build
+.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
-posargs=
-dist-pypi-build: ## build dist, can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-testrelease: ## test release on testpypi. can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
+dist-pypi-build: ## build dist
+	$(TOX) -e dist-pypi -- build
+dist-pypi-testrelease: ## test release on testpypi
+	$(TOX) -e dist-pypi -- testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-build dist-pypi-testrelease dist-pypi-release: environment/dist-pypi.yaml
+	$(TOX) -e dist-pypi -- release
+dist-pypi-command: ## run command with command=...
+	$(TOX) -e dist-pypi -- command
+dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
+.PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e dist-conda -- recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(pasargs)
-dist-conda-build dist-conda-recipe: environment/dist-conda.yaml
+	$(TOX) -e dist-conda -- build
+dist-conda-command: ## run command with command=...
+	$(TOX) -e dist-conda -- command
+dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
-.PHONY: test-dist-pypi-remote test-dist-conda-remote test-dist-pypi-local test-dist-conda-local
+.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-test-dist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
+testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-test-dist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
+testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
+testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 
-
-test-dist-pypi: environment/test.
-
+testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
 
 ## list all options
 .PHONY: tox-list
-
 tox-list:
 	$(TOX) -a
 
 
 ################################################################################
 # installation
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
 	pip install . --no-deps
 
 install-dev: ## install development version (run clean?)
 	pip install -e . --no-deps
+
+
+################################################################################
+# other tools
+################################################################################
+
+# Note that this requires `auto-changelog`, which can be installed with pip(x)
+auto-changelog: ## autogenerate changelog and print to stdout
+	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
+
+commitizen-changelog:
+	cz changelog --unreleased-version unreleased --dry-run --incremental
```

### Comparing `tmmc-lnpy-0.2.2/PKG-INFO` & `tmmc-lnpy-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,147 +1,222 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.2.2
+Version: 0.3.0
 Summary: Analysis of lnPi results from TMMC simulation
 Home-page: https://github.com/usnistgov/tmmc-lnpy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
-Project-URL: Homepage, https://github.com/usnistgov/tmmc-lnpy
-Project-URL: Documentation, https://pages.nist.gov/tmmc-lnpy/
-Project-URL: Source, https://github.com/usnistgov/tmmc-lnpy
+Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
+Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!--
+  For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/tmmc-lnpy
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/tmmc-lnpy
-<!-- [pypi-badge]: https://badge.fury.io/py/tmmc-lnpy -->
 [pypi-link]: https://pypi.org/project/tmmc-lnpy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/tmmc-lnpy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/tmmc-lnpy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/tmmc-lnpy
 [conda-link]: https://anaconda.org/wpk-nist/tmmc-lnpy
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
+[license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
+<!-- other links -->
 
 # `tmmc-lnpy`
 
+A Python package for stuff.
+
 ## Overview
 
 A package to analyze $\ln \Pi(N)$ data from Transition Matrix Monte Carlo
-simulation.  The main output from TMMC simulations, $\ln \Pi(N)$, provides a means to calculate a host of thermodynamic
-properties.  Moreover, if $\ln \Pi(N)$ is calculated at a specific chemical potential, it can be reweighted to provide
+simulation. The main output from TMMC simulations, $\ln \Pi(N)$, provides a
+means to calculate a host of thermodynamic properties. Moreover, if $\ln \Pi(N)$
+is calculated at a specific chemical potential, it can be reweighted to provide
 thermodynamic information at a different chemical potential
 
-
-
-
 ## Features
 
-``tmmc-lnpy`` provides a wide array of routines to analyze $\ln \Pi(N)$.  These include:
-
-* Reweighting to arbitrary chemical potential
-* Segmenting $\ln \Pi(N)$ (to identify unique phases)
-* Containers for interacting with several values of $\ln \Pi(N)$ in a vectorized way.
-* Calculating thermodynamic properties from these containers
-* Calculating limits of stability, and phase equilibrium
+`tmmc-lnpy` provides a wide array of routines to analyze $\ln \Pi(N)$. These
+include:
 
+- Reweighting to arbitrary chemical potential
+- Segmenting $\ln \Pi(N)$ (to identify unique phases)
+- Containers for interacting with several values of $\ln \Pi(N)$ in a vectorized
+  way.
+- Calculating thermodynamic properties from these containers
+- Calculating limits of stability, and phase equilibrium
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following
 
-``` bash
+```bash
 pip install tmmc-lnpy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist tmmc-lnpy
 ```
 
 ## Example usage
 
-Note that the distribution name ``tmmc-lnpy`` is different than the import name ``lnpy`` due to name clashing on pypi.
+Note that the distribution name `tmmc-lnpy` is different than the import name
+`lnpy` due to name clashing on pypi.
 
-``` python
+```python
 import lnpy
 import lnpy.examples
 
 ref = lnpy.examples.load_example_maskddata('lj_sub')
 ```
 
-
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `tmmc-lnpy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
-This package is used for with [thermoextrap](https://github.com/usnistgov/thermo-extrap) to analyze thermodynamically extrapolated macro state probability distributions.
+This package is used for with
+[thermoextrap](https://github.com/usnistgov/thermo-extrap) to analyze
+thermodynamically extrapolated macro state probability distributions.
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
-# History
+# Changelog
+
+Changelog for `lnpy`
+
+## Unreleased
+
+See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
+
+<!-- scriv-insert-here -->
+
+## v0.3.0 — 2023-05-02
+
+### Added
+
+- Added support for python3.11
+
+- Moved `_docstrings` -> `docstrings` to make available
+- Moved from local docfiller to module_utilities.docfiller
+- Moved from local cached module to module-utilities.cached
+- Add support for python3.11
+
+Full set of changes:
+[`v0.2.2...0.3.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.2...0.3.0)
+
+### Changed
+
+- Update package layout
+- New linters via pre-commit
+- Development env now handled by tox
+
+## v0.2.2 - 2023-04-05
+
+Full set of changes:
+[`v0.2.1...v0.2.2`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.1...v0.2.2)
+
+## v0.2.1 - 2023-04-04
+
+Full set of changes:
+[`v0.2.0...v0.2.1`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.2.0...v0.2.1)
+
+## v0.2.0 - 2023-04-04
+
+Full set of changes:
+[`v0.1.5...v0.2.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.5...v0.2.0)
+
+## v0.1.5 - 2022-09-28
+
+Full set of changes:
+[`v0.1.4...v0.1.5`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.4...v0.1.5)
+
+## v0.1.4 - 2022-09-26
+
+Full set of changes:
+[`v0.1.3...v0.1.4`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.3...v0.1.4)
+
+## v0.1.3 - 2022-09-15
+
+Full set of changes:
+[`v0.1.2...v0.1.3`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.2...v0.1.3)
+
+## v0.1.2 - 2022-09-14
+
+Full set of changes:
+[`v0.1.1...v0.1.2`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.1...v0.1.2)
+
+## v0.1.1 - 2022-09-13
+
+Full set of changes:
+[`v0.1.0...v0.1.1`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.1.0...v0.1.1)
+
+## v0.1.0 - 2022-09-13
 
-## 0.1.1 (2022-09-12)
+Full set of changes:
+[`v0.0.1...v0.1.0`](https://github.com/usnistgov/tmmc-lnpy/compare/v0.0.1...v0.1.0)
 
-- First release on PyPI.
+## v0.0.1 - 2022-09-13
 
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmmc-lnpy-0.2.2/README.md` & `tmmc-lnpy-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!--
+  For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/tmmc-lnpy
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/tmmc-lnpy
-<!-- [pypi-badge]: https://badge.fury.io/py/tmmc-lnpy -->
 [pypi-link]: https://pypi.org/project/tmmc-lnpy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/tmmc-lnpy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/tmmc-lnpy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/tmmc-lnpy
 [conda-link]: https://anaconda.org/wpk-nist/tmmc-lnpy
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
+[license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
+<!-- other links -->
 
 # `tmmc-lnpy`
 
+A Python package for stuff.
+
 ## Overview
 
 A package to analyze $\ln \Pi(N)$ data from Transition Matrix Monte Carlo
-simulation.  The main output from TMMC simulations, $\ln \Pi(N)$, provides a means to calculate a host of thermodynamic
-properties.  Moreover, if $\ln \Pi(N)$ is calculated at a specific chemical potential, it can be reweighted to provide
+simulation. The main output from TMMC simulations, $\ln \Pi(N)$, provides a
+means to calculate a host of thermodynamic properties. Moreover, if $\ln \Pi(N)$
+is calculated at a specific chemical potential, it can be reweighted to provide
 thermodynamic information at a different chemical potential
 
-
-
-
 ## Features
 
-``tmmc-lnpy`` provides a wide array of routines to analyze $\ln \Pi(N)$.  These include:
-
-* Reweighting to arbitrary chemical potential
-* Segmenting $\ln \Pi(N)$ (to identify unique phases)
-* Containers for interacting with several values of $\ln \Pi(N)$ in a vectorized way.
-* Calculating thermodynamic properties from these containers
-* Calculating limits of stability, and phase equilibrium
+`tmmc-lnpy` provides a wide array of routines to analyze $\ln \Pi(N)$. These
+include:
 
+- Reweighting to arbitrary chemical potential
+- Segmenting $\ln \Pi(N)$ (to identify unique phases)
+- Containers for interacting with several values of $\ln \Pi(N)$ in a vectorized
+  way.
+- Calculating thermodynamic properties from these containers
+- Calculating limits of stability, and phase equilibrium
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following
 
-``` bash
+```bash
 pip install tmmc-lnpy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist tmmc-lnpy
 ```
 
 ## Example usage
 
-Note that the distribution name ``tmmc-lnpy`` is different than the import name ``lnpy`` due to name clashing on pypi.
+Note that the distribution name `tmmc-lnpy` is different than the import name
+`lnpy` due to name clashing on pypi.
 
-``` python
+```python
 import lnpy
 import lnpy.examples
 
 ref = lnpy.examples.load_example_maskddata('lj_sub')
 ```
 
-
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `tmmc-lnpy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
-This package is used for with [thermoextrap](https://github.com/usnistgov/thermo-extrap) to analyze thermodynamically extrapolated macro state probability distributions.
+This package is used for with
+[thermoextrap](https://github.com/usnistgov/thermo-extrap) to analyze
+thermodynamically extrapolated macro state probability distributions.
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
```

### Comparing `tmmc-lnpy-0.2.2/environment/dev-extras.yaml` & `tmmc-lnpy-0.3.0/environment/dev-extras.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 dependencies:
-    # numerics/tests
-    - matplotlib
-    # - dask
-    - netcdf4
-    # - pandas
-    # development
-    # - isort
-    # - black
-    # - blackdoc
-    # - flake8
-    # testing
-    - pytest
-    - pytest-cov
-    - pytest-xdist
-    # - tox-conda
-    # specials
-    # - pre-commit
-    # repl
-    - ipython
-    - ipykernel
-    - ipywidgets
-    # build
-    - setuptools-scm
-    # - setuptools
-    # - twine
-    # - setuptools_scm_git_archive
-    # - build
-    # conda specific
-    # - conda-build
-    # - anaconda-client
-    # - greyskull
-    # doc stuff
-    # - sphinx
-    # - sphinx_rtd_theme
-    # - recommonmark # if want markdown
-    # - nbsphinx # if want notebooks
-    # - sphinxcontrib-spelling
-    # - sphinx-toolbox
-    # lsp stuff
-    # - autoflake
-    # - pyls-mypy
-    # - pyls-black
-    # - pyls-isort
-    # mypy
-    # - mypy
-    # - pytest-mypy
-    # # Monkeytype: autocreate type hints
-    # - MonkeyType
-    # - pip
-    # - pip:
-            # - mypy-extensions
-            # - pytest-monkeytype
-            # - flake8-mypy
-            # - attr-utils
-            # spelling?
-            # - pyenchant
+  # numerics/tests
+  - matplotlib
+  # - dask
+  - netcdf4
+  # - pandas
+  # development
+  # - isort
+  # - black
+  # - blackdoc
+  # - flake8
+  # testing
+  - pytest
+  - pytest-cov
+  - pytest-xdist
+  # - tox-conda
+  # specials
+  # - pre-commit
+  # repl
+  - ipython
+  - ipykernel
+  - ipywidgets
+  # build
+  - setuptools-scm
+  # - setuptools
+  # - twine
+  # - setuptools_scm_git_archive
+  # - build
+  # conda specific
+  # - conda-build
+  # - anaconda-client
+  # - greyskull
+  # doc stuff
+  # - sphinx
+  # - sphinx_rtd_theme
+  # - recommonmark # if want markdown
+  # - nbsphinx # if want notebooks
+  # - sphinxcontrib-spelling
+  # - sphinx-toolbox
+  # lsp stuff
+  # - autoflake
+  # - pyls-mypy
+  # - pyls-black
+  # - pyls-isort
+  # mypy
+  # - mypy
+  # - pytest-mypy
+  # # Monkeytype: autocreate type hints
+  # - MonkeyType
+  # - pip
+  # - pip:
+  # - mypy-extensions
+  # - pytest-monkeytype
+  # - flake8-mypy
+  # - attr-utils
+  # spelling?
+  # - pyenchant
```

### Comparing `tmmc-lnpy-0.2.2/environment/docs-extras.yaml` & `tmmc-lnpy-0.3.0/environment/docs-extras.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 channels:
   - conda-forge
 dependencies:
-    - setuptools-scm
-    - ipython
-    - matplotlib
-    - ipywidgets
-    ## package deps
-    # - matplotlib
-    # - pandas
-    - pip
-    - pip:
-        - pyenchant
-        # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
-        - ghp-import
-        - sphinx
-        ## themes
-        - sphinx-book-theme
-        ## error with == 0.13.3
-        - pydata-sphinx-theme==0.13.1
-        ## optionals
-        # sphinx-design
-        - sphinx-copybutton
-        - sphinxcontrib-spelling
-        # sphinxext-rediraffe
-        ## autobuild
-        - sphinx-autobuild
-        ## myst
-        # myst-parser
-        - myst-nb
-        ## others
-        - autodocsumm
+  - setuptools-scm
+  - ipython
+  - matplotlib
+  - ipywidgets
+  ## package deps
+  # - matplotlib
+  # - pandas
+  - pip
+  - pip:
+      - pyenchant
+      # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
+      - ghp-import
+      - sphinx
+      ## themes
+      - sphinx-book-theme
+      ## error with == 0.13.3
+      - pydata-sphinx-theme==0.13.1
+      ## optionals
+      # sphinx-design
+      - sphinx-copybutton
+      - sphinxcontrib-spelling
+      # sphinxext-rediraffe
+      ## autobuild
+      - sphinx-autobuild
+      ## myst
+      # myst-parser
+      - myst-nb
+      ## others
+      - autodocsumm
```

### Comparing `tmmc-lnpy-0.2.2/src/lnPi/__init__.py` & `tmmc-lnpy-0.3.0/src/lnPi/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/__init__.py` & `tmmc-lnpy-0.3.0/src/lnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/bracket.py` & `tmmc-lnpy-0.3.0/src/lnpy/bracket.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/data/hsmix_example.json.gz` & `tmmc-lnpy-0.3.0/src/lnpy/data/hsmix_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/data/lj_sub_example.json` & `tmmc-lnpy-0.3.0/src/lnpy/data/lj_sub_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/data/lj_sup_example.json` & `tmmc-lnpy-0.3.0/src/lnpy/data/lj_sup_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/data/ljmix_sup_example.json.gz` & `tmmc-lnpy-0.3.0/src/lnpy/data/ljmix_sup_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/data/watermof_example.json` & `tmmc-lnpy-0.3.0/src/lnpy/data/watermof_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/ensembles.py` & `tmmc-lnpy-0.3.0/src/lnpy/ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Ensemble averages (:mod:`~lnpy.ensembles`)
 ==========================================
 """
-from functools import lru_cache, wraps
+from functools import lru_cache, partial, wraps
 
 import numpy as np
-
-# import pandas as pd
 import xarray as xr
+from module_utilities import cached
 
-from .cached_decorators import gcached_use_cache as gcached
 from .lnpidata import MaskedlnPiDelayed, lnPiMasked
 from .lnpiseries import lnPiCollection
 from .maskedlnpi_legacy import MaskedlnPiLegacy
 from .utils import dim_to_suffix_dataset
 
+# always check_use_cache here.
+cached_prop = partial(cached.prop, check_use_cache=True)
+cached_meth = partial(cached.meth, check_use_cache=True)
+
 
 ###############################################################################
 # xlnPi wrapper
 @lru_cache(maxsize=10)
 def _get_indices(shape):
     return np.indices(shape)
 
@@ -75,48 +77,48 @@
             self.dims_rec = [rec_name]
 
         self.n_name = n_name
         self.dims_n = [f"{n_name}_{i}" for i in range(self.ndim)]
         self.dims_lnz = [f"{lnz_name}_{i}" for i in range(self.ndim)]
         self.dims_comp = [comp_name]
 
-    @gcached()
+    @cached_prop
     def coords_n(self):
         return {
             k: xr.DataArray(_get_range(n), dims=k, attrs={"long_name": rf"${k}$"})
             for k, n in zip(self.dims_n, self.shape)
         }
 
-    @gcached(prop=False)
+    @cached_meth
     def attrs(self, *args):
         d = {
             "dims_n": self.dims_n,
             "dims_lnz": self.dims_lnz,
             "dims_comp": self.dims_comp,
             "dims_state": self.dims_lnz + list(args),
         }
 
         if self.dims_rec is not None:
             d["dims_rec"] = self.dims_rec
         return d
 
-    @gcached(prop=False)
+    @cached_meth
     def ncoords(self, coords_n=False):
         if coords_n:
             coords = self.coords_n
         else:
             coords = None
         return xr.DataArray(
             _get_indices(self.shape),
             dims=self.dims_comp + self.dims_n,
             coords=coords,
             name=self.n_name,
         )
 
-    @gcached(prop=False)
+    @cached_meth
     def ncoords_tot(self, coords_n=False):
         return self.ncoords(coords_n).sum(self.dims_comp)
 
     def wrap_data(self, data, coords_n=False, coords=None, **kwargs):
         if coords is None:
             coords = {}
 
@@ -208,19 +210,19 @@
     def _use_cache(self):
         return getattr(self._parent, "_use_cache", False)
 
     @property
     def _xarray_unstack(self):
         return getattr(self._parent, "_xarray_unstack", True)
 
-    @gcached()
+    @cached_prop
     def _standard_attrs(self):
         return self._wrapper.attrs(*self._parent.state_kws.keys())
 
-    # @gcached() to much memory
+    # @cached_prop to much memory
     @property
     def _rec_coords(self):
         if self._rec_name is None:
             return dict(self._parent._index_dict(), **self._parent.state_kws)
         else:
             return {
                 self._parent._concat_dim: self._parent.index,
@@ -272,19 +274,19 @@
         return self._parent.state_kws["beta"]
 
     @property
     def volume(self):
         """System volume :math:`V`."""
         return self._parent.state_kws["volume"]
 
-    @gcached()
+    @cached_prop
     def coords_state(self):
         return {k: self.pi_norm.coords[k] for k in self.dims_state}
 
-    @gcached()
+    @cached_prop
     @xr_name(r"$\beta {\bf \mu}$")
     def betamu(self):
         r"""Scaled chemical potential :math:`\beta \mu`"""
         return self._wrapper.wrap_lnz(self._parent._lnz_tot, coords=self._rec_coords)
 
     @property
     @xr_name(r"$\ln\beta{\bf\mu}$")
@@ -304,15 +306,15 @@
         """
         return self._wrapper.wrap_lnpi(
             self._parent._lnpi_tot(fill_value),
             coords=self._rec_coords,
             **self._parent.state_kws,
         )  # .assign_coords(**self._rec_coords)
 
-    @gcached()
+    @cached_prop
     def _pi_params(self):
         pi_norm, pi_sum, lnpi_zero = self._parent._pi_params(-np.inf)
 
         pi_sum = self._wrapper.wrap_lnpi_0(
             pi_sum, name="pi_sum", coords=self._rec_coords
         )
 
@@ -481,39 +483,39 @@
 
         return xr.dot(self.pi_norm, xx, yy, dims=self.dims_n, **self._xarray_dot_kws)
 
     def pipe(self, func, *args, **kwargs):
         """Apply function to `self`"""
         return func(self, *args, **kwargs)
 
-    @gcached()
+    @cached_prop
     @xr_name(r"${\bf n}(\mu,V,T)$")
     def nvec(self):
         r"""Average number of particles of each component :math:`\overline{{\bf N}}`"""
         return self._mean_pi(self.ncoords)
 
-    @gcached()
+    @cached_prop
     @xr_name(r"$n(\mu,V,T)$")
     def ntot(self):
         r"""Average total number of particles :math:`\overline{N}`"""
         return self._mean_pi(self.ncoords_tot)
 
     @property
     @xr_name(r"${\bf x}(\mu,V,T)$")
     def molfrac(self):
         r"""Average molfrac for each components :math:`{\bf x} = \overline{{\bf N}} / N`"""
         return self.nvec.pipe(lambda x: x / x.sum(self.dims_comp))
 
-    @gcached()
+    @cached_prop
     @xr_name(r"$var[{\bf n}(\mu,V,T)]$")
     def nvec_var(self):
         r"""Variance in particle number :math:`{\rm var}\, \bf{N}`"""
         return self.var_pi(self.ncoords)
 
-    @gcached()
+    @cached_prop
     @xr_name(r"$var[n(\mu,V,T)]$")
     def ntot_var(self):
         r"""Variance in total number of particles :math:`{\rm var}\, N`"""
         return self.var_pi(self.ncoords_tot)
 
     @property
     @xr_name(r"${\bf \rho}(\mu,V,T)$")
@@ -540,30 +542,30 @@
     # def edge_distance(self, ref, *args, **kwargs):
     #     """distance from endpoint"""
 
     #     return xr.DataArray([x.edge_distance(ref) for x in self._parent],
     #                         dims=self.dims_rec,
     #                         coords=self._rec_coords)
 
-    @gcached(prop=False)
+    @cached_meth
     def _argmax_indexer(self):
         x = self.pi_norm.values
         xx = x.reshape(x.shape[0], -1)
         idx_flat = xx.argmax(-1)
         indexer = np.unravel_index(idx_flat, x.shape[1:])
         return indexer
 
-    @gcached()
+    @cached_prop
     def _argmax_indexer_dict(self):
         return {
             k: xr.DataArray(v, dims=self._parent._concat_dim)
             for k, v in zip(self.dims_n, self._argmax_indexer())
         }
 
-    @gcached()
+    @cached_prop
     def _sample_indexer_dict(self):
         return {
             self._parent._concat_dim: xr.DataArray(
                 range(len(self._parent)), dims=self._parent._concat_dim
             )
         }
 
@@ -587,15 +589,15 @@
     def pi_norm_max(self, add_n_coords=True):
         r"""Maximum value :math:`\max_N \Pi_{\rm norm}(N, meta)`"""
         out = self.pi_norm.isel(**self._sample_argmax_indexer_dict)
         if add_n_coords:
             out = out.assign_coords(**self._argmax_indexer_dict)
         return out
 
-    @gcached(prop=False)
+    @cached_meth
     def argmax(self):
         return np.array(self._argmax_indexer()).T
 
     @xr_name("distance from upper edge")
     def edge_distance(self, ref, *args, **kwargs):
         """Distance from argmax(lnPi) to endpoint"""
         out = ref.edge_distance_matrix[self._argmax_indexer()]
@@ -622,15 +624,15 @@
         else:
             assert val is not None
 
         e = xr.DataArray(ref.edge_distance_matrix, dims=self.dims_n)
         mask = self.pi_norm > val
         return e.where(mask).min(self.dims_n)
 
-    @gcached(prop=False)
+    @cached_meth
     @xr_name(r"$\beta \Omega(\mu,V,T)$", standard_name="grand_potential")
     def _betaOmega(self, lnpi_zero=None):
         if lnpi_zero is None:
             lnpi_zero = self._lnpi_zero
         return lnpi_zero - np.log(self.pi_sum)
 
     def betaOmega(self, lnpi_zero=None):
@@ -645,15 +647,15 @@
         # Note.  Put calculation in _betaOmega
         # because so many other things
         # call it with lnpi_zero set to None
         # so end up with copies of the same
         # thing in cache
         return self._betaOmega(lnpi_zero)
 
-    @gcached()
+    @cached_prop
     @xr_name(r"${\rm PE}(\mu,V,T)$", standard_name="potential_energy")
     def PE(self):
         r"""Potential energy :math:`\overline{PE}`"""
 
         # if betaPE available, use that:
 
         if hasattr(self._parent, "_series"):
@@ -693,21 +695,21 @@
     ################################################################################
     # Other properties
     @xr_name(r"$\beta\omega(\mu,V,T)$", standard_name="grand_potential_per_particle")
     def betaOmega_n(self, lnpi_zero=None):
         r"""Grand potential per particle :math:`\beta \Omega / \overline{N}`"""
         return self.betaOmega(lnpi_zero) / self.ntot
 
-    # @gcached(prop=False)
+    # @cached_meth
     @xr_name(r"$\beta p(\mu,V,T)V$")
     def betapV(self, lnpi_zero=None):
         r""":math:`\beta p V = - \beta \Omega`"""
         return -self.betaOmega(lnpi_zero)
 
-    @gcached()
+    @cached_prop
     @xr_name("mask_stable", description="True where state is most stable")
     def mask_stable(self):
         """Masks are True where values are stable. Only works for unstacked data."""
         if not self._xarray_unstack:
             # raise Value'only mask with unstack')
             pv = self.betapV()
             sample = self._parent._concat_dim
@@ -716,15 +718,15 @@
                 .pipe(lambda x: x.max("phase") == x)
                 .stack(sample=pv.indexes[sample].names)
                 .loc[pv.indexes["sample"]]
             )
         else:
             return self.betapV().pipe(lambda x: x.max("phase") == x)
 
-    # @gcached(prop=False)
+    # @cached_meth
     @xr_name(r"$\beta p(\mu,V,T)/\rho$", standard_name="compressibility_factor")
     def Z(self, lnpi_zero=None):
         r"""Compressibility factor :math:`\beta p / \rho`"""
         return -self.betaOmega_n(lnpi_zero)
 
     @xr_name(r"$p(\mu,V,T)$")
     def pressure(self, lnpi_zero=None):
@@ -899,34 +901,34 @@
         r""":class:`~xarray.DataArray` view of :math:`\ln Pi(N)`"""
         return self._xge.lnpi(fill_value=fill_value)
 
     @property
     def _xarray_unstack(self):
         return getattr(self._parent, "_xarray_unstack", True)
 
-    @gcached()
+    @cached_prop
     def ncoords(self):
         """Coordinate vector `dims_n`"""
         return (
             self._xge.ncoords
             # NOTE: if don't use '.values', then get extra coords don't want
             .where(~self._xge.lnpi(np.nan).isnull().values)
         )
 
     @property
     def nvec(self):
         r"""Number of particles for each components :math:`{\bf N}`"""
         return self.ncoords.rename("nvec")
 
-    @gcached()
+    @cached_prop
     def ntot(self):
         """Total number of particles :math:`N`"""
         return self.ncoords.sum(self._xge.dims_comp)
 
-    @gcached(prop=False)
+    @cached_meth
     @xr_name(r"$\beta F({\bf n},V,T)$", standard_name="helmholtz_free_energy")
     def _betaF(self, lnpi_zero=None):
         """Helmholtz free energy"""
         x = self._parent.xge
 
         if lnpi_zero is None:
             lnpi_zero = self._parent.data.ravel()[0]
@@ -946,15 +948,15 @@
     @xr_name(
         r"$\beta F({\bf n},V,T)/n$", standard_name="helmholtz_free_energy_per_particle"
     )
     def betaF_n(self, lnpi_zero=None):
         r"""Scaled Helmholtz free energy per particle :math:`\beta F / N`"""
         return self.betaF(lnpi_zero) / self.ntot
 
-    @gcached()
+    @cached_prop
     @xr_name(r"${\rm PE}({\bf n},V,T)/n$", standard_name="potential_energy")
     def PE(self):
         """Internal Energy :math:`PE`"""
         # if betaPE available, use that:
         PE = self._parent.extra_kws.get("PE", None)
         if PE is None:
             raise AttributeError('must set "PE" in "extra_kws" of lnPiMasked')
@@ -986,15 +988,15 @@
         return self.betaE(ndim) - self.betaF(lnpi_zero)
 
     @xr_name(r"$S({\bf n},V,T)/(n k_{rm B})$")
     def S_n(self, ndim=3, lnpi_zero=None):
         r"""Entropy per particle :math:`S / (N k_{\rm B})`"""
         return self.S(ndim, lnpi_zero) / self.ntot
 
-    @gcached(prop=False)
+    @cached_meth
     @xr_name(r"$\beta {\bf\mu}({bf n},V,T)$", standard_name="absolute_activity")
     def _betamu(self, lnpi_zero=None):
         return xr.concat(
             [self.betaF(lnpi_zero).differentiate(n) for n in self._xge.dims_n],
             dim=self._xge.dims_comp[0],
         ).assign_attrs(self._xge._standard_attrs)
 
@@ -1004,15 +1006,15 @@
 
     @property
     @xr_name(r"${\bf \rho}({\bf n},V,T)$")
     def dens(self):
         r"""Density :math:`\rho = N / V`"""
         return self.ncoords / self._xge.volume
 
-    @gcached(prop=False)
+    @cached_meth
     @xr_name(r"$\beta\Omega({\bf n},V,T)$")
     def _betaOmega(self, lnpi_zero=None):
         """Calculate beta * Omega = betaF - lnz .dot. N"""
         return self.betaF(lnpi_zero) - (self.betamu(lnpi_zero) * self.ncoords).sum(
             self._xge.dims_comp
         )
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/examples.py` & `tmmc-lnpy-0.3.0/src/lnpy/examples.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/extensions.py` & `tmmc-lnpy-0.3.0/src/lnpy/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 This is inspired by xarray accessors.
 """
 
 import warnings
 from itertools import chain
 from operator import attrgetter
 
-from .cached_decorators import gcached
+from module_utilities import cached
+
 from .utils import get_tqdm_calc as get_tqdm
 from .utils import parallel_map_attr, parallel_map_call
 
 
 class AccessorRegistrationWarning(Warning):
     """Warning for conflicts in accessor registration."""
 
@@ -61,15 +62,15 @@
 
     Notes
     -----
     This gets deleted if self._cache is cleared.
     If you only want to create it once, then use the Single access wrapper below
     """
 
-    @gcached(key=name, prop=True)
+    @cached.prop(key=name)
     @wraps(accessor)
     def _get_prop(self):
         return accessor(self)
 
     return _get_prop
 
 
@@ -176,15 +177,15 @@
     def __init__(self, parent, items, desc=None):
         self.parent = parent
         self.items = items
         self.desc = desc
         self._cache = {}
         self._use_joblib = getattr(self.parent, "_USE_JOBLIB_", False)
 
-    @gcached(prop=False)
+    @cached.meth
     def __call__(self, *args, **kwargs):
         # get value
         seq = get_tqdm(self.items, desc=self.desc)
         # results = [x(*args, **kwargs) for x in seq]
         results = parallel_map_call(seq, self._use_joblib, *args, **kwargs)
         if hasattr(self.parent, "wrap_list_results"):
             results = self.parent.wrap_list_results(results)
@@ -283,36 +284,36 @@
     """Get top level property from items"""
 
     if cache_list is not None and name in cache_list:
         cache = True
     else:
         cache = False
 
-    # @gcached(key=name, prop=True)
+    # @cached.prop(key=name)
     def _get_prop(self):
         results = [getattr(x, name) for x in self]
         if callable(results[0]):
             results = _CallableListResults(self, results)
         else:
             if hasattr(self, "wrap_list_results"):
                 results = self.wrap_list_results(results)
         return results
 
     if cache:
-        _get_prop = gcached(key=name, prop=True)(_get_prop)
+        _get_prop = cached.prop(key=name)(_get_prop)
     else:
         _get_prop = property(_get_prop)
 
     return _get_prop
 
 
 def _CachedListAccessorWrapper(name, cache_list=None):
     """Wrap List accessor in cached property"""
 
-    @gcached(key=name, prop=True)
+    @cached.prop(key=name)
     def _get_prop(self):
         return _ListAccessor(
             self, [getattr(x, name) for x in self], cache_list=cache_list
         )
 
     return _get_prop
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/lnpicollectionutils.py` & `tmmc-lnpy-0.3.0/src/lnpy/lnpicollectionutils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/lnpidata.py` & `tmmc-lnpy-0.3.0/src/lnpy/lnpidata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 ################################################################################
 # Delayed
 from functools import lru_cache
 
 import numpy as np
 import pandas as pd
+from module_utilities import cached
 
-from ._docstrings import docfiller_shared
-from .cached_decorators import gcached
+from .docstrings import docfiller_shared
 from .extensions import AccessorMixin
 from .utils import labels_to_masks, masks_change_convention
 
 # from scipy.ndimage import filters
 
 
 @lru_cache(maxsize=20)
@@ -394,15 +394,15 @@
 
         return pi_norm, pi_sum, lnpi_zero
 
     @property
     def _lnz_tot(self):
         return self.lnz
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_argmax(self, *args, **kwargs):
         """
         Calculate index of maximum of masked data.
 
         Parameters
         ----------
         *args
@@ -413,15 +413,15 @@
         See Also
         --------
         numpy.ma.MaskedArray.argmax
         numpy.unravel_index
         """
         return np.unravel_index(self.ma.argmax(*args, **kwargs), self.shape)
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_max(self, *args, **kwargs):
         """
         Calculate index of maximum of masked data.
 
         Parameters
         ----------
         *args
@@ -431,20 +431,20 @@
 
         See Also
         --------
         numpy.ma.MaskedArray.max
         """
         return self.ma[self.local_argmax(*args, **kwargs)]
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_maxmask(self, *args, **kwargs):
         """Calculate mask where ``self.ma == self.local_max()``"""
         return self.ma == self.local_max(*args, **kwargs)
 
-    @gcached()
+    @cached.prop
     def edge_distance_matrix(self):
         """
         Matrix of distance from each element to a background (i.e., masked) point.
 
         See Also
         --------
         lnpy.utils.distance_matrix
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/lnpienergy.py` & `tmmc-lnpy-0.3.0/src/lnpy/lnpienergy.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """
 import itertools
 import warnings
 
 import numpy as np
 import pandas as pd
 import xarray as xr
+from module_utilities import cached
 from skimage import segmentation
 
-from ._docstrings import docfiller_shared
-from .cached_decorators import gcached
+from .docstrings import docfiller_shared
 from .lnpiseries import lnPiCollection
 from .utils import get_tqdm_calc as get_tqdm
 from .utils import labels_to_masks, masks_change_convention, parallel_map_func_starargs
 
 
 def find_boundaries(masks, mode="thick", connectivity=None, **kws):
     """
@@ -389,20 +389,20 @@
             features=features,
             convention="image",
             include_boundary=include_boundary,
             **kwargs,
         )
         return cls(data=data, masks=masks, connectivity=connectivity)
 
-    @gcached()
+    @cached.prop
     def _data_max(self):
         """For lnPi data, find absolute argmax and max"""
         return find_masked_extrema(self.data, self.masks)
 
-    @gcached(prop=False)
+    @cached.meth
     def _boundary_max(self, method="exact"):
         """
         Find argmax along boundaries of regions.
         Corresponds to argmin(w)
 
         if method == 'exact', then find the boundary of each region
         and find max.  then find min of those maxes.
@@ -469,15 +469,15 @@
         return np.nan_to_num(-self._boundary_max()[1], nan=np.inf)
 
     @property
     def w_argtran(self):
         """Location of `w_tran`"""
         return self._boundary_max()[0]
 
-    @gcached()
+    @cached.prop
     def delta_w(self):
         """Transition energy ``delta_w[i, j] = w_tran[i, j] - w_min[i]``."""
         return self.w_tran - self.w_min
 
     def merge_regions(
         self,
         nfeature_max=None,
@@ -595,15 +595,15 @@
             indexes.append(phases.index)
             masks = [x.mask for x in phases.values]
             ws.append(
                 wFreeEnergy(data=phases.iloc[0].data, masks=masks, convention=False)
             )
         return indexes, ws
 
-    @gcached()
+    @cached.prop
     def _data(self):
         indexes, ws = self._get_items_ws()
         seq = get_tqdm(zip(indexes, ws), total=len(ws), desc="wFreeEnergyCollection")
         out = parallel_map_func_starargs(
             _get_w_data, items=seq, use_joblib=self._use_joblib, total=len(ws)
         )
 
@@ -701,26 +701,26 @@
 
     Notes
     -----
     This is accessed through :attr:`lnpy.lnpiseries.lnPiCollection.wfe_phases`
 
     """
 
-    @gcached()
+    @cached.prop
     def dwx(self):
         index = list(self._parent.index.get_level_values("phase"))
         masks = [x.mask for x in self._parent]
         w = wFreeEnergy(data=self._parent.iloc[0].data, masks=masks, convention=False)
 
         dw = w.w_tran - w.w_min
         dims = ["phase", "phase_nebr"]
         coords = dict(zip(dims, [index] * 2))
         return xr.DataArray(dw, dims=dims, coords=coords)
 
-    @gcached()
+    @cached.prop
     def dw(self):
         """Series representation of delta_w"""
         return self.dwx.to_series()
 
     def get_dw(self, idx, idx_nebr=None):
         dw = self.dwx
         index = dw.indexes["phase"]
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/lnpiseries.py` & `tmmc-lnpy-0.3.0/src/lnpy/lnpiseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Collection of lnPi objects (:mod:`~lnpy.lnpiseries`)
 ====================================================
 """
 
 import numpy as np
 import pandas as pd
 import xarray as xr
+from module_utilities import cached
 
-from .cached_decorators import gcached
 from .extensions import AccessorMixin
 from .utils import get_tqdm_build as get_tqdm
 from .utils import labels_to_masks, masks_to_labels
 from .utils import parallel_map_build as parallel_map
 
 
 class SeriesWrapper(AccessorMixin):
@@ -482,15 +482,15 @@
                 assert lnpi.state_kws == state_kws
                 assert lnpi.shape == shape
                 # would like to do this, but
                 # fails for parallel builds
                 # assert lnpi._base is _base
 
     # repr
-    @gcached()
+    @cached.prop
     def _lnz_series(self):
         return self._series.apply(lambda x: x.lnz)
 
     def __repr__(self):
         return f"<class {self.__class__.__name__}>\n{repr(self._lnz_series)}"
 
     def __str__(self):
@@ -502,15 +502,15 @@
         return self.iloc[0].state_kws
 
     @property
     def nlnz(self):
         """Number of unique lnzs"""
         return len(self.index.droplevel("phase").drop_duplicates())
 
-    @gcached()
+    @cached.prop
     def index_frame(self):
         """
         Values (from :class:`xarray.DataArray`) for each sample.
 
         includes a column 'lnz_index' which is the unique lnz values
         regardless of phase
         """
@@ -550,15 +550,15 @@
             index = index.levels[level_idx]
         return index
 
     def get_index_level(self, level="phase"):
         """Get index values for specified level"""
         return self._get_level(level=level)
 
-    # @gcached()
+    # @cached.prop
     @property
     def _nrec(self):
         return len(self._series)
 
     def _lnpi_tot(self, fill_value=None):
         # old method
         # return np.stack([x.filled() for x in self])
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/maskedlnpi_legacy.py` & `tmmc-lnpy-0.3.0/src/lnpy/maskedlnpi_legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Legacy lnPi array routines (:mod:`~lnpy.maskedlnpi_legacy`)
 ===========================================================
 """
 from warnings import warn
 
 import numpy as np
 import pandas as pd
+from module_utilities import cached
 from scipy import ndimage
 
-from .cached_decorators import gcached
 from .extensions import AccessorMixin
 from .utils import labels_to_masks, masks_change_convention
 
 # NOTE : This is a rework of core.
 # [ ] : split xarray functionality into wrapper(s)
 # [ ] : split splitting into separate classes
 
@@ -169,51 +169,51 @@
         p = "MaskedlnPi(\n" + "\n".join([indent + x for x in L]) + "\n)"
 
         return p
 
     def __str__(self):
         return f"MaskedlnPi(lnz={str(self.lnz)})"
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_argmax(self, *args, **kwargs):
         return np.unravel_index(self.argmax(*args, **kwargs), self.shape)
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_max(self, *args, **kwargs):
         return self[self.local_argmax(*args, **kwargs)]
 
-    # @gcached(prop=False)
+    # @cached.meth
     def local_maxmask(self, *args, **kwargs):
         return self == self.local_max(*args, **kwargs)
 
-    @gcached()
+    @cached.prop
     def edge_distance_matrix(self):
         """Matrix of distance from upper bound"""
         from .utils import distance_matrix
 
         return distance_matrix(~self.mask)
 
     def edge_distance(self, ref, *args, **kwargs):
         return ref.edge_distance_matrix[self.local_argmax(*args, **kwargs)]
 
     # make these top level
-    # @gcached()
+    # @cached.prop
     # @property
     # def pi(self):
     #     """
     #     basic pi = exp(lnpi)
     #     """
     #     pi = np.exp(self - self.local_max())
     #     return pi
 
-    # @gcached()
+    # @cached.prop
     # def pi_sum(self):
     #     return self.pi.sum()
 
-    # @gcached(prop=False)
+    # @cached.meth
     # def betaOmega(self, lnpi_zero=None):
     #     if lnpi_zero is None:
     #         lnpi_zero = self.data.ravel()[0]
     #     zval = lnpi_zero - self.local_max()
     #     return  (zval - np.log(self.pi_sum))
 
     def __setitem__(self, index, value):
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/molfrac.py` & `tmmc-lnpy-0.3.0/src/lnpy/molfrac.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/options.py` & `tmmc-lnpy-0.3.0/src/lnpy/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 """
 Options (:mod:`~lnpy.options`)
 ==============================
 """
 
-import os
-
 TQDM_USE = "tqdm_use"
 TQDM_LEN_CALC = "tqdm_len_calc"
 TQDM_LEN_BUILD = "tqdm_len_build"
 TQDM_LEAVE = "tqdm_leave"
 TQDM_BAR = "tqdm_bar"
 
 JOBLIB_USE = "joblib_use"
 JOBLIB_N_JOBS = "joblib_n_jobs"
 JOBLIB_BACKEND = "joblib_backend"
 JOBLIB_KWS = "joblib_kws"
 JOBLIB_LEN_CALC = "joblib_len_calc"
 JOBLIB_LEN_BUILD = "joblib_len_build"
 
-DOC_SUB = "doc_sub"
-
-try:
-    # Default to setting docs
-    _DOC_SUB = os.getenv("LNPI_DOC_SUB", "True").lower() not in ("0", "f", "false")
-except KeyError:
-    _DOC_SUB = True
-
 
 OPTIONS = {
     TQDM_USE: True,
     TQDM_LEN_CALC: 100,
     TQDM_LEN_BUILD: 500,
     TQDM_LEAVE: False,
     TQDM_BAR: "default",
     JOBLIB_USE: True,
     JOBLIB_N_JOBS: -1,
     JOBLIB_BACKEND: None,
     JOBLIB_KWS: {},
     JOBLIB_LEN_CALC: 200,
     JOBLIB_LEN_BUILD: 500,
-    DOC_SUB: _DOC_SUB,
 }
 
 _isbool = lambda x: isinstance(x, bool)
 _isint = lambda x: isinstance(x, int)
 _isstr = lambda x: isinstance(x, str)
 
 _isstr_or_None = lambda x: isinstance(x, str) or x is None
@@ -56,15 +45,14 @@
     TQDM_BAR: lambda x: x in ["default", "text", "notebook"],
     JOBLIB_USE: _isbool,
     JOBLIB_N_JOBS: _isint,
     JOBLIB_BACKEND: _isstr_or_None,
     JOBLIB_KWS: lambda x: isinstance(x, dict),
     JOBLIB_LEN_CALC: _isint,
     JOBLIB_LEN_BUILD: _isint,
-    DOC_SUB: _isbool,
 }
 
 _SETTERS = {}
 
 
 class set_options:
     """
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/segment.py` & `tmmc-lnpy-0.3.0/src/lnpy/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,67 +12,58 @@
 
 import warnings
 from collections.abc import Iterable
 from functools import lru_cache
 
 import bottleneck
 import numpy as np
+from module_utilities.docfiller import DocFiller
 from skimage import feature, morphology, segmentation
 
-from ._docstrings import _prepare_shared_docs, _shared_docs, docfiller
+from .docstrings import DOCFILLER_SHARED
 from .lnpienergy import wFreeEnergy
 from .lnpiseries import lnPiCollection
 
 # * Common doc strings
+_docstrings_local = r"""
+Parameters
+----------
+data : array-like
+    Image data to analyze
+min_distance : int or sequence of int, optional
+    min_distance parameter.  If sequence, then call
+    :func:`~skimage.feature.peak_local_max` until number of peaks ``<=num_peaks_max``.
+    Default value is ``(5, 10, 15, 20, 25)``.
+connectivity_morphology | connectivity : int, optional
+    Maximum number of orthogonal hops to consider a pixel/voxel as a neighbor.
+    Accepted values are ranging from 1 to ``input.ndim``. If ``None``, a full
+    connectivity of ``input.ndim`` is used.
+connectivity_watershed | connectivity : ndarray, optional
+    An array with the same number of dimensions as image whose non-zero
+    elements indicate neighbors for connection. Following the scipy convention,
+    default is a one-connected array of the dimension of the image.
+num_peaks_max : int, optional
+    Max number of maxima/peaks to find. If not specified, any number of peaks allowed.
+peak_style | style : {'indices', 'mask', 'marker'}
+    Controls output style
+
+    * indices : indices of peaks
+    * mask : array of bool marking peak locations
+    * marker : array of int
+markers : int, or ndarray of int, optional
+    Same shape as image. The desired number of markers, or an array marking the
+    basins with the values to be assigned in the label matrix. Zero means not a
+    marker. If None (no markers given), the local minima of the image are used
+    as markers.
+"""
 
-_shared_docs_local = {
-    "data": """
-    data : array-like
-        Image data to analyze
-    """,
-    "min_distance": r"""
-    min_distance : int or sequence of int, optional
-        min_distance parameter.  If sequence, then call
-        :func:`~skimage.feature.peak_local_max` until number of peaks ``<=num_peaks_max``.
-        Default value is ``(5, 10, 15, 20, 25)``.
-    """,
-    "connectivity_morphology": """
-    connectivity : int, optional
-        Maximum number of orthogonal hops to consider a pixel/voxel as a neighbor.
-        Accepted values are ranging from 1 to ``input.ndim``. If ``None``, a full connectivity of ``input.ndim`` is used.
-    """,
-    "connectivity_watershed": """
-    connectivity : ndarray, optional
-        An array with the same number of dimensions as image whose non-zero elements indicate neighbors for connection.
-        Following the scipy convention, default is a one-connected array of the dimension of the image.
-    """,
-    "num_peaks_max": """
-    num_peaks_max : int, optional
-        Max number of maxima/peaks to find. If not specified, any number of peaks allowed.
-    """,
-    "peak_style": """
-    style : {'indices', 'mask', 'marker'}
-        Controls output style
-
-        * indices : indices of peaks
-        * mask : array of bool marking peak locations
-        * marker : array of int
-
-    """,
-    "markers": """
-    markers : int, or ndarray of int, optional
-        Same shape as image. The desired number of markers, or an array marking the basins with the values to be assigned in the label matrix.
-        Zero means not a marker. If None (no markers given), the local minima of the image are used as markers.
-    """,
-}
 
-_shared_docs_local = _prepare_shared_docs(_shared_docs_local)
-docfiller_shared = docfiller(**(dict(_shared_docs, **_shared_docs_local)))
+DOCFILLER_LOCAL = DocFiller.from_docstring(_docstrings_local, combine_keys="parameters")
 
-# docfiller_shared = docfiller(**dict(_shared_docs, **_prepare_shared_docs(_shared_docs_local)))
+docfiller_shared = DOCFILLER_SHARED.append(DOCFILLER_LOCAL)()
 
 
 @docfiller_shared
 def peak_local_max_adaptive(
     data,
     mask=None,
     min_distance=None,
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/stability.py` & `tmmc-lnpy-0.3.0/src/lnpy/stability.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 ================================================
 
 Calculation of spinodal and binodal
 """
 import itertools
 
 import numpy as np
+from module_utilities import cached
 from scipy import optimize
 
-from .cached_decorators import gcached
 from .lnpiseries import lnPiCollection
 
 
 # ###############################################################################
 # Spinodal routines
 def _initial_bracket_spinodal_right(
     C,
@@ -580,15 +580,15 @@
         concat_kws = dict(names=[self._NAME], **concat_kws)
         kwargs = dict(self.access_kws, **kwargs)
         # return self._parent.concat_like(items, **concat_kws)
         # s = pd.concat({k:v._series for k,v in items}, **concat_kws)
         # return self._parent.new_like(s)
         return self._parent.concat(items, concat_kws=concat_kws, **kwargs)
 
-    @gcached()
+    @cached.prop
     def access(self):
         """View (:class:`lnpy.lnpiseries.lnPiCollection`) of stability"""
         return self._get_access()
 
     def __getitem__(self, idx):
         return self._items[idx]
 
@@ -707,15 +707,15 @@
             out[idx] = s
             info[idx] = r
 
         if unstack is None:
             unstack = self._parent._xarray_unstack
         self.set_access_kws(unstack=unstack)
 
-        converged = all([x.converged for x in info.values()])
+        converged = all(x.converged for x in info.values())
         if raise_unconverged and not converged:
             raise ValueError("Spinodal calculation did not converge")
 
         if inplace:
             self._items = out
             self._info = info
             # if append:
@@ -845,15 +845,15 @@
                 build_kws=build_kws,
                 **kwargs,
             )
             out[idx] = s
             info[idx] = r
             index[idx] = ids
 
-        converged = all([x.converged for x in info.values()])
+        converged = all(x.converged for x in info.values())
         if raise_unconverged and not converged:
             raise ValueError("Binodal calculation did not converge")
 
         if unstack is None:
             unstack = self._parent._xarray_unstack
         self.set_access_kws(unstack=unstack)
```

### Comparing `tmmc-lnpy-0.2.2/src/lnpy/utils.py` & `tmmc-lnpy-0.3.0/src/lnpy/utils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tests/test_hs_mix.py` & `tmmc-lnpy-0.3.0/tests/test_hs_mix.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 import lnpy
 import lnpy.stability
 
-path_data = Path(__file__).parent / "../examples/HS_mix"
+path_data = Path(__file__).parent / "../examples/archived/HS_mix"
 
 
 # function to tag 'LD' and 'HD' phases
 def tag_phases2(x):
     if len(x) > 2:
         raise ValueError("bad tag function")
     argmax0 = np.array([xx.local_argmax()[0] for xx in x])
```

### Comparing `tmmc-lnpy-0.2.2/tests/test_lj_mix_0.py` & `tmmc-lnpy-0.3.0/tests/test_lj_mix_0.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import lnpy
 
-path_data = Path(__file__).parent / "../examples/LJ_mix"
+path_data = Path(__file__).parent / "../examples/archived/LJ_mix"
 
 
 @pytest.fixture
 def ref():
     path = path_data / "ljmix4_full.t080.v512.r1.lnpi_o.dat.gz"
     temp = 0.8
     state_kws = {"temp": temp, "beta": 1.0 / temp, "volume": 512}
```

### Comparing `tmmc-lnpy-0.2.2/tests/test_lnPi.py` & `tmmc-lnpy-0.3.0/tests/test_lnPi.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import lnPi
 
-path_data = Path(__file__).parent / "../examples/LJ_cfs_2.5sig"
+path_data = Path(__file__).parent / "../examples/archived/LJ_cfs_2.5sig"
 
 
 def get_lnz(path):
     kB = 1.3806503e-23  # J/K
     kg = 1.66054e-27  # 1/amu
     hPlanck = 6.62606876e-34  # Js
```

### Comparing `tmmc-lnpy-0.2.2/tests/test_single_comp_sub.py` & `tmmc-lnpy-0.3.0/tests/test_single_comp_sub.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         raise ValueError("bad tag function")
     argmax0 = np.array([xx.local_argmax()[0] for xx in x])
     return np.where(argmax0 <= x[0].shape[0] / 2, 0, 1)
 
 
 from pathlib import Path
 
-path_data = Path(__file__).parent / "../examples/LJ_cfs_2.5sig"
+path_data = Path(__file__).parent / "../examples/archived/LJ_cfs_2.5sig"
 
 
 def get_lnz(path):
     kB = 1.3806503e-23  # J/K
     kg = 1.66054e-27  # 1/amu
     hPlanck = 6.62606876e-34  # Js
```

### Comparing `tmmc-lnpy-0.2.2/tests/test_single_comp_super.py` & `tmmc-lnpy-0.3.0/tests/test_single_comp_super.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import lnpy
 
-path_data = Path(__file__).parent / "../examples/LJ_cfs_2.5sig"
+path_data = Path(__file__).parent / "../examples/archived/LJ_cfs_2.5sig"
 
 
 def get_lnz(path):
     kB = 1.3806503e-23  # J/K
     kg = 1.66054e-27  # 1/amu
     hPlanck = 6.62606876e-34  # Js
```

### Comparing `tmmc-lnpy-0.2.2/tests/test_water_cluster.py` & `tmmc-lnpy-0.3.0/tests/test_water_cluster.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tests/water_cluster/data_0.csv` & `tmmc-lnpy-0.3.0/tests/water_cluster/data_0.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tests/water_cluster/data_1.csv` & `tmmc-lnpy-0.3.0/tests/water_cluster/data_1.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tests/water_cluster/data_1_dw.csv` & `tmmc-lnpy-0.3.0/tests/water_cluster/data_1_dw.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tests/water_cluster/water_MOF_example.csv` & `tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_example.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.2.2/tox.ini` & `tmmc-lnpy-0.3.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,136 @@
 [tox]
-skipsdist=True
+isolated_build = True
 requires = tox-conda
 envlist =
         # test
-        py3{8, 9, 10}-tests
-
+        test-py3{8, 9, 10, 11}
 
 [base]
 package_name = tmmc-lnpy
 import_name  = lnpy
 build_python = python3.10
 conda_env            = {toxinidir}/environment.yaml
 conda_env_dev        = {toxinidir}/environment/dev.yaml
 conda_env_test       = {toxinidir}/environment/test.yaml
 conda_env_docs       = {toxinidir}/environment/docs.yaml
 conda_env_dist_pypi  = {toxinidir}/environment/dist-pypi.yaml
 conda_env_dist_conda = {toxinidir}/environment/dist-conda.yaml
+conda_env_lint       = {toxinidir}/environment/lint.yaml
 conda_channels =
     wpk-nist
     conda-forge
 conda_deps_test =
 allowlist_externals =
     bash
-    open
-    cat
-    rm
-    echo
-    mkdir
     make
 commands_test_check =
     python --version
     python -c 'import {[base]import_name}; print( {[base]import_name}.__version__)'
     bash -ec 'echo $PWD'
-    echo {posargs:{toxinidir}}
-
 
 [testenv]
+passenv =
+        SETUPTOOLS_SCM_PRETEND_VERSION
+        command
+        mypy_args
+        pyright_args
+        pytype_args
+        release_args
+        project_name
+        TEST_VERSION
 usedevelop =
-    tests: True
+    test: True
 conda_env =
-    tests: {[base]conda_env_test}
+    test: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
     {[base]commands_test_check}
-    pytest {posargs}
+    {posargs:pytest}
 
+[testenv:dev]
+description =
+    Create development environment.
+usedevelop = True
+basepython = {[base]build_python}
+conda_env = {[base]conda_env_dev}
+envdir = {toxworkdir}/dev
+commands =
+    {posargs:bash -ec 'conda list'}
 
-# Build documentation
-[testenv:docs-{build, release, clean, command, spelling, live, open, make}]
+[testenv:docs]
 description =
-    build: build documentation.
-    release: create documentation branch.
-    clean: clean build.
-    spelling: run spell checking on documentation and docstrings.
-    command: run arbitrary command
-    live: use sphinx-autobuild
-    make: run arbitrary make command from docs/Makefile.  Passes in posargs
+    Runs make in docs directory.
+    For example, 'tox -e docs -- html' -> 'make -C docs html'.
+    With 'release' option, you can set the message with 'message=...' in posargs.
 usedevelop = True
 envdir     = {toxworkdir}/docs
 basepython = {[base]build_python}
 conda_env  = {[base]conda_env_docs}
 changedir  = {toxinidir}/docs
 commands =
-    build: bash -c "echo $PWD"
-    build: make {posargs:html}
-    open: open {toxinidir}/docs/_build/html/index.html
-    release: ghp-import -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
-    clean: make allclean
-    spelling: make spelling
-    command: {posargs}
-    live: make livehtml
-    make: make {posargs}
+    make {posargs:html}
 
-# create pypi dist
-[testenv:dist-pypi-{build, testrelease, release}]
+[testenv:dist-pypi]
 description  =
-    build: build distribution.
-    testrelease: upload to testpypi
-    release: upload to pypi
+    Runs make -f scrips/dist-pypi.mk posargs
+    For example, 'tox -e dist-pypi -- build' -> 'make -f scripts/dist-pypi.mk build'
 skip_install = True
 envdir       = {toxworkdir}/dist-pypi
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_pypi}
 changedir    = {toxinidir}
 commands     =
-    build: rm -rf {toxinidir}/dist
-    build: python -m build --outdir "{toxinidir}/dist/"
-
-    testrelease: twine upload --repository testpypi {toxinidir}/dist/*
-    release: twine upload {toxinidir}/dist/*
-
+    make -f {toxinidir}/scripts/dist-pypi.mk {posargs:build}
 
-# create conda dist
-[testenv:dist-conda-{recipe, build, command}]
+[testenv:dist-conda]
 description  =
-    recipe: build conda recipe using grayskull
+    Runs make -C dist-conda posargs
+    recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}/dist-conda
 commands     =
-    recipe: rm -rf {toxinidir}/dist-conda/{[base]package_name}
-    recipe: grayskull pypi {posargs:{[base]package_name}}
-    recipe: cat {[base]package_name}/meta.yaml
-
-    build: rm -rf build
-    build: mkdir -p build
-    build: conda mambabuild --output-folder=build --no-anaconda-upload .
-    command: {posargs:python}
+    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={[base]package_name}
 
-
-# test pypi/conda install from local/remote
-[testenv:test-dist-{pypi, conda}-{local,remote}-py3{8,9,10}]
+[testenv:testdist-{pypi, conda}-{local,remote}-py3{8, 9, 10, 11}]
 conda_channels =
     {[base]conda_channels}
-description  =
+description =
     Test install from
     pypi: pypi
     conda: conda
     using either
     local: local
     remote: remote
     versions.
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote: {[base]package_name}
+    conda-remote: {[base]package_name}{env:TEST_VERSION:''}
     conda-local: {posargs}
 deps =
-    pypi-remote: {[base]package_name}
+    pypi-remote: {[base]package_name}{env:TEST_VERSION:''}
     pypi-local: {posargs}
 
-
-# Test pip installed dependencies
-[testenv:test-pip-py3{8,9,10}]
+[testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
 conda_env    = {toxinidir}/environment/test-extras.yaml
+
+[testenv:lint]
+description =
+    Run linters
+    For example, 'tox -e lint -- mypy mypy_args=...' runs 'mypy $mypy_args'
+conda_env = {[base]conda_env_lint}
+usedevelop = True
+envdir     = {toxworkdir}/lint
+basepython = {[base]build_python}
+commands =
+    make -f {toxinidir}/scripts/lint.mk {posargs:mypy}
```

