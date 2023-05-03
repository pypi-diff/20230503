# Comparing `tmp/circuitpython-mag-cal-1.1.0.tar.gz` & `tmp/circuitpython-mag-cal-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mag-cal-1.1.0.tar", last modified: Fri Apr 28 20:11:11 2023, max compression
+gzip compressed data, was "circuitpython-mag-cal-1.1.1.tar", last modified: Wed May  3 11:17:14 2023, max compression
```

## Comparing `circuitpython-mag-cal-1.1.0.tar` & `circuitpython-mag-cal-1.1.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.573021 circuitpython-mag-cal-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/howto.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/examples/mag_cal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/mag_cal/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    24919 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/nm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/rbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.842670 circuitpython-mag-cal-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.846670 circuitpython-mag-cal-1.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.846670 circuitpython-mag-cal-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.846670 circuitpython-mag-cal-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.846670 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-03 11:17:14.000000 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-03 11:17:14.000000 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:17:14.000000 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 11:17:14.000000 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 11:17:14.000000 circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/howto.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/examples/mag_cal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/mag_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25232 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/mag_cal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.846670 circuitpython-mag-cal-1.1.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:17:14.850670 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ab.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ai.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ai.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bh.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bi.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ee.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/fb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/fb.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/jd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-03 11:16:57.000000 circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/jd.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-03 11:17:07.000000 circuitpython-mag-cal-1.1.1/tests/test_sensor.py
```

### Comparing `circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mag-cal-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/.gitignore` & `circuitpython-mag-cal-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/.pre-commit-config.yaml` & `circuitpython-mag-cal-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/.pylintrc` & `circuitpython-mag-cal-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/CODE_OF_CONDUCT.md` & `circuitpython-mag-cal-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/LICENSE` & `circuitpython-mag-cal-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-mag-cal-1.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/LICENSES/MIT.txt` & `circuitpython-mag-cal-1.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/LICENSES/Unlicense.txt` & `circuitpython-mag-cal-1.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/PKG-INFO` & `circuitpython-mag-cal-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.0
+Version: 1.1.1
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.0/README.rst` & `circuitpython-mag-cal-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/PKG-INFO` & `circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.0
+Version: 1.1.1
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/SOURCES.txt` & `circuitpython-mag-cal-1.1.1/circuitpython_mag_cal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico` & `circuitpython-mag-cal-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/docs/conf.py` & `circuitpython-mag-cal-1.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 # Show the docstring from both the class and its __init__() method.
 autoclass_content = "both"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 autodoc_mock_imports = ["ulab"]
+autodoc_member_order = "bysource"
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
```

### Comparing `circuitpython-mag-cal-1.1.0/docs/howto.rst` & `circuitpython-mag-cal-1.1.1/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/docs/index.rst` & `circuitpython-mag-cal-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/examples/mag_cal_simpletest.py` & `circuitpython-mag-cal-1.1.1/examples/mag_cal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/__init__.py` & `circuitpython-mag-cal-1.1.1/mag_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/axes.py` & `circuitpython-mag-cal-1.1.1/mag_cal/axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/calibration.py` & `circuitpython-mag-cal-1.1.1/mag_cal/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     # work with normal numpy
     import numpy as np
 except ImportError:
     # or work with ulab if we are in CircuitPython
     from ulab import numpy as np
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/furbrain/CircuitPython_mag_cal.git"
 
 
 def _vector_from_matrices(matrix: np.ndarray, i: int, j: int):
     return np.array([x[i, j] for x in matrix])
 
 
@@ -35,22 +35,22 @@
     Object representing a magnetometer and accelerometer calibration
     """
 
     MAGNETOMETER = 1
     ACCELEROMETER = 2
     BOTH = MAGNETOMETER | ACCELEROMETER
 
-    ELLIPSOID = 0  #: Fit to Ellipsoid
-    AXIS_CORRECTION = 1  #: Fit to ellipsoid then correct any axis misalignment
-    NON_LINEAR = (
-        2  #: as per `AXIS_CORRECTION` and then do correction for non-linear effects
-    )
-    FAST_NON_LINEAR = (
-        3  #: as per `AXIS_CORRECTION` and then do quick non-linear correction
-    )
+    ELLIPSOID = 0
+    """Fit to Ellipsoid"""
+    AXIS_CORRECTION = 1
+    """Fit to ellipsoid then correct any axis misalignment"""
+    NON_LINEAR = 2
+    """as per `AXIS_CORRECTION` and then do correction for non-linear effects"""
+    FAST_NON_LINEAR = 3
+    """as per `AXIS_CORRECTION` and then do quick non-linear correction"""
 
     def __init__(self, mag_axes: str = "+X+Y+Z", grav_axes: str = None):
         """
         Create an object representing the calibration coefficients for a combined
         magnetometer and accelerometer
 
         :param str mag_axes: A string representing how your magnetometer is mounted with respect to
@@ -64,53 +64,26 @@
         """
         if grav_axes is None:
             grav_axes = mag_axes
         self.mag = Sensor(axes=mag_axes)
         self.grav = Sensor(axes=grav_axes)
         self.ready = False
 
-    def as_dict(self) -> Dict:
-        """
-        Convert the current calibration to a dictionary, suitable for serialising via json.
-
-        :return: The calibration as a dictionary
-        :rtype: dict
-        """
-        dct = {
-            "mag": self.mag.as_dict(),
-            "grav": self.grav.as_dict(),
-            "ready": self.ready,
-        }
-        return dct
-
-    @classmethod
-    def from_dict(cls, dct: Dict) -> "Calibration":
-        """
-        Create a Calibration object based on a dict previously produced by `as_dict`
-
-        :param dict dct: dict to instantiate
-        :return: Calibration object
-        """
-        instance = cls()
-        instance.mag = Sensor.from_dict(dct["mag"])
-        instance.grav = Sensor.from_dict(dct["grav"])
-        instance.ready = dct["ready"]
-        return instance
-
     def calibrate(
         self,
         mag_data: np.ndarray,
         grav_data: np.ndarray,
         routine: int = FAST_NON_LINEAR,
     ):
         """
         Perform a full calibration, with an algorithm depending on the value of ``routine``. If
         you select a routine other than `ELLIPSOID` you must provide at least one run
         of at least four shots in the same direction with varying amonts of roll. Ideally two sets
         of eight readings, but this is not vital.
+
         :param np.ndarray mag_data: Numpy array of magnetic readings of shape (N,3)
         :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
         :param routine: what level of calibration to perform:
 
           * `ELLIPSOID`: Simplest form of calibration, very fast, does not require any sets of
             readings to be aligned. Does not correct for misalignment between pointer and sensors.
           * `AXIS_CORRECTION`: This routine performs the `ELLIPSOID` and then applies a
@@ -127,24 +100,67 @@
         :return: Measure of error: percentage error of fit for `ELLIPSOID`,
           standard deviation of error in degrees for other methods. Normally <1 degree is
           acceptable, <0.5 degrees is good.
         """
         self.fit_ellipsoid(mag_data, grav_data)
         if routine >= self.AXIS_CORRECTION:
             runs = self.find_similar_shots(mag_data, grav_data)
+            if len(runs) == 0:
+                raise ValueError("No runs of shots all in the same direction found")
             paired_data = [(mag_data[a:b], grav_data[a:b]) for a, b in runs]
             self.fit_to_axis(paired_data)
             if routine == self.NON_LINEAR:
                 self.fit_non_linear(paired_data)
             elif routine == self.FAST_NON_LINEAR:
                 self.fit_non_linear_quick(paired_data)
             return self.accuracy(paired_data)
         # just ellipsod fit done, so use uniformity measure
         return np.mean(self.uniformity(mag_data, grav_data))
 
+    def get_angles(self, mag, grav) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Get device azimuth(bearing), inclination, and roll, given the magnetic and gravity readings
+
+        :param np.ndarray mag: Magnetic readings, either as numpy array or sequence of 3 floats
+        :param np.ndarray grav: Gravity readings, either as numpy array or sequence of 3 floats
+        :return: (azimuth, inclination, roll) in degrees
+        """
+
+        matrix = self.get_orientation_matrix(mag, grav)
+        azimuth, inclination, roll = self.matrix_to_angles(matrix)
+        return azimuth, inclination, roll
+
+    def as_dict(self) -> Dict:
+        """
+        Convert the current calibration to a dictionary, suitable for serialising via json.
+
+        :return: The calibration as a dictionary
+        :rtype: dict
+        """
+        dct = {
+            "mag": self.mag.as_dict(),
+            "grav": self.grav.as_dict(),
+            "ready": self.ready,
+        }
+        return dct
+
+    @classmethod
+    def from_dict(cls, dct: Dict) -> "Calibration":
+        """
+        Create a Calibration object based on a dict previously produced by `as_dict`
+
+        :param dict dct: dict to instantiate
+        :return: Calibration object
+        """
+        instance = cls()
+        instance.mag = Sensor.from_dict(dct["mag"])
+        instance.grav = Sensor.from_dict(dct["grav"])
+        instance.ready = dct["ready"]
+        return instance
+
     def fit_ellipsoid(
         self, mag_data: np.ndarray, grav_data: np.ndarray
     ) -> Tuple[float, float]:
         """
         Take multiple sets of readings in various directions. You can then use this function
         to determine an ideal set of calibration coefficients
 
@@ -154,44 +170,14 @@
           Lower numbers are better
         """
         mag_accuracy = self.mag.fit_ellipsoid(mag_data)
         grav_accuracy = self.grav.fit_ellipsoid(grav_data)
         self.ready = True
         return mag_accuracy, grav_accuracy
 
-    def accuracy(self, data) -> float:
-        """
-        Calculate average accuracy for a set of multiple readings taken
-
-        :param data: A list of paired magnetic and gravity readings e.g.:
-          ``[(mag_data1, grav_data1), (mag_data2, grav_data2)]``, where ``mag_data1`` and
-          ``grav_data1`` is a (N,3) numpy array of readings around the axis in the first
-          direction, and ``mag_data2`` and ``grav_data2`` is a (M,3) numpy array of readings around
-          the specified axis in another direction.
-        :return: Average standard deviation of readings in degrees
-        """
-        results = 0
-        for mag, grav in data:
-            orientation = self.get_orientation_vector(mag, grav)
-            stds = np.std(orientation, axis=0, ddof=1)
-            results += np.linalg.norm(stds)
-        return np.degrees(results / len(data))
-
-    def uniformity(self, mag_data, grav_data):
-        """
-        Check the uniformity of the data - how well the calibrated data points fit on
-        a sphere of radius 1.0
-
-        :param np.ndarray mag_data: Numpy array of magnetic readings of shape (N,3)
-        :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
-        :return: (mag_accuracy, grav_accuracy) How well the calibrated model fits the data.
-          Lower numbers are better
-        """
-        return self.mag.uniformity(mag_data), self.grav.uniformity(grav_data)
-
     def fit_to_axis(self, data, axis="Y") -> float:
         """
         Take multiple reading with the device pointing in the same direction, but rotated around
         ``axis``. You can repeat this with several directions. This function will take
         this data and ensure that your sensors aligned relative to each other. This function
         requires that you have run `Calibration.fit_ellipsoid` beforehand.
 
@@ -323,14 +309,44 @@
         params = self._get_lstsq_non_linear_params(param_count, expected_mags, raw_mags)
         all_params = np.zeros(param_count * 3)
         all_params[:param_count] = params[:param_count]
         all_params[-param_count:] = params[-param_count:]
         self.mag.set_non_linear_params(all_params)
         return self.accuracy(data)
 
+    def accuracy(self, data) -> float:
+        """
+        Calculate average accuracy for a set of multiple readings taken
+
+        :param data: A list of paired magnetic and gravity readings e.g.:
+          ``[(mag_data1, grav_data1), (mag_data2, grav_data2)]``, where ``mag_data1`` and
+          ``grav_data1`` is a (N,3) numpy array of readings around the axis in the first
+          direction, and ``mag_data2`` and ``grav_data2`` is a (M,3) numpy array of readings around
+          the specified axis in another direction.
+        :return: Average standard deviation of readings in degrees
+        """
+        results = 0
+        for mag, grav in data:
+            orientation = self.get_orientation_vector(mag, grav)
+            stds = np.std(orientation, axis=0, ddof=1)
+            results += np.linalg.norm(stds)
+        return np.degrees(results / len(data))
+
+    def uniformity(self, mag_data, grav_data):
+        """
+        Check the uniformity of the data - how well the calibrated data points fit on
+        a sphere of radius 1.0
+
+        :param np.ndarray mag_data: Numpy array of magnetic readings of shape (N,3)
+        :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
+        :return: (mag_accuracy, grav_accuracy) How well the calibrated model fits the data.
+          Lower numbers are better
+        """
+        return self.mag.uniformity(mag_data), self.grav.uniformity(grav_data)
+
     @staticmethod
     def _get_lstsq_non_linear_params(param_count, expected_mags, raw_mags):
         """
         Create a set of non-linear parameters given a set of expected magnetometer readings
         and the actual magnetometer readings
 
         :param param_count: Number of parameters to use per sensor
@@ -412,27 +428,14 @@
         north = normalise(cross(upward, east))
         if len(north.shape) > 1:
             orientation = [np.array([e, n, u]) for e, n, u in zip(east, north, upward)]
         else:
             orientation = np.array((east, north, upward))
         return orientation
 
-    def get_angles(self, mag, grav) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """
-        Get device azimuth(bearing) and inclination, given the magnetic and gravity readings
-
-        :param np.ndarray mag: Magnetic readings, either as numpy array or sequence of 3 floats
-        :param np.ndarray grav: Gravity readings, either as numpy array or sequence of 3 floats
-        :return: (azimuth, inclination, roll) in degrees
-        """
-
-        matrix = self.get_orientation_matrix(mag, grav)
-        azimuth, inclination, roll = self.matrix_to_angles(matrix)
-        return azimuth, inclination, roll
-
     @staticmethod
     def matrix_to_angles(matrix: np.ndarray):
         """
         Extract the rotation angles from a matrix. Angles are "zxy" rotations (azimuth, pitch, roll)
 
         :param np.ndarray matrix:
         :return: azimuth, pitch, roll
@@ -448,15 +451,18 @@
             m11 = matrix[1, 1]
             m21 = matrix[2, 1]
             m20 = matrix[2, 0]
             m22 = matrix[2, 2]
         theta1 = np.arctan2(m01, m11)
         theta2 = np.arctan2(m21 * np.cos(theta1), m11)
         theta3 = np.arctan2(-m20, m22)
-        azimuth = np.degrees(theta1) % 360
+        if not isinstance(theta1, np.ndarray):
+            azimuth = float(np.degrees(theta1)) % 360
+        else:
+            azimuth = np.array([x % 360 for x in np.degrees(theta1)])
         inclination = (
             (np.degrees(theta2) + 90) % 180
         ) - 90  # force to be in range -90,+90
         roll = np.degrees(theta3)
         return azimuth, inclination, roll
 
     @classmethod
@@ -495,21 +501,23 @@
         return [cls.angles_to_matrix(*args) for args in zip(azimuth, inclination, roll)]
 
     def find_similar_shots(
         self, mag: np.ndarray, grav: np.ndarray, precision=30, min_run=4
     ):
         """
         Find runs of shots that are within precision degrees of each other
+
         :param mag: numpy array of magnetic data
         :param grav: numpy array of accelerometer data
         :param precision: number of degrees shots should be within
         :param min_run: minimum length of run to find
         :return: list of start and finish indices for each run
         """
-        azimuths, inclinations, _ = self.get_angles(mag, grav)
+        angles = [self.get_angles(m, g) for m, g in zip(mag, grav)]
+        azimuths, inclinations, _ = zip(*angles)
         groups = []
         i = 0
         while i < len(azimuths) - min_run:
             for j in reversed(range(i + min_run, len(azimuths) + 1)):
                 if self._is_a_run(azimuths[i:j], inclinations[i:j], precision):
                     groups.append([i, j])
                     i = j
```

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/lstsq.py` & `circuitpython-mag-cal-1.1.1/mag_cal/lstsq.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/nm.py` & `circuitpython-mag-cal-1.1.1/mag_cal/nm.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/rbf.py` & `circuitpython-mag-cal-1.1.1/mag_cal/rbf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/sensor.py` & `circuitpython-mag-cal-1.1.1/mag_cal/sensor.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/mag_cal/utils.py` & `circuitpython-mag-cal-1.1.1/mag_cal/utils.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/pyproject.toml` & `circuitpython-mag-cal-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mag-cal"
 description = "Calibrate magnetometer and accelerometer readings"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_mag_cal"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ab.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ai.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bh.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/bi.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/ee.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/fb.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/hj2.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json` & `circuitpython-mag-cal-1.1.1/tests/fixtures/cal_data/jd.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/test_axes.py` & `circuitpython-mag-cal-1.1.1/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/test_calibration.py` & `circuitpython-mag-cal-1.1.1/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.0/tests/test_sensor.py` & `circuitpython-mag-cal-1.1.1/tests/test_sensor.py`

 * *Files identical despite different names*

