# Comparing `tmp/cca_zoo-1.9.0.tar.gz` & `tmp/cca_zoo-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-1.9.0.tar", last modified: Mon Oct  4 23:03:45 2021, max compression
+gzip compressed data, was "dist/cca_zoo-1.9.1.tar", last modified: Sun Nov  7 17:40:01 2021, max compression
```

## Comparing `cca_zoo-1.9.0.tar` & `cca_zoo-1.9.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5398 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8360 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/data/simulated.py
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/data/toy.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/_dcca_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13982 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/architectures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/dcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/dccae.py
--rw-r--r--   0 runner    (1001) docker     (121)    13897 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/deepwrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/dtcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/dvcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/objectives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/deepmodels/splitae.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43156 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/model_selection/_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/models/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7738 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/cca_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/gcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    29499 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/innerloop.py
--rw-r--r--   0 runner    (1001) docker     (121)    29327 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/iterative.py
--rw-r--r--   0 runner    (1001) docker     (121)     8899 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/mcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/rcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    11527 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/models/tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/probabilisticmodels/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/probabilisticmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/probabilisticmodels/vcca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    15510 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (121)    11239 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/test/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/utils/check_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-10-04 23:03:34.000000 cca_zoo-1.9.0/cca_zoo/utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/cca_zoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 23:03:45.000000 cca_zoo-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-10-04 23:03:44.000000 cca_zoo-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5398 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8360 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/simulated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9341 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/toy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/_dcca_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13982 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dccae.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13897 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/deepwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dtcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5780 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/splitae.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43156 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/model_selection/_search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7738 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/cca_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/gcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29499 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/innerloop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29327 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8899 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/mcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4885 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/ncca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8478 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/rcca.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11527 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/vcca.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15510 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11239 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2849 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/check_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/setup.py
```

### Comparing `cca_zoo-1.9.0/PKG-INFO` & `cca_zoo-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca_zoo
-Version: 1.9.0
+Version: 1.9.1
 Summary: Canonical Correlation Analysis Zoo: CCA, GCCA, MCCA, DCCA, DGCCA, DVCCA, DCCAE, KCCA and regularised variants including sparse CCA , ridge CCA and elastic CCA
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/303801602.svg)](https://zenodo.org/badge/latestdoi/303801602)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/master/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-1.9.0/README.md` & `cca_zoo-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/data/simulated.py` & `cca_zoo-1.9.1/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/data/toy.py` & `cca_zoo-1.9.1/cca_zoo/data/toy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/data/utils.py` & `cca_zoo-1.9.1/cca_zoo/data/utils.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/_dcca_base.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/_dcca_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/architectures.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/dcca.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/dcca_noi.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/dccae.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/deepwrapper.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/deepwrapper.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/dtcca.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/dvcca.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/objectives.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/deepmodels/splitae.py` & `cca_zoo-1.9.1/cca_zoo/deepmodels/splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/model_selection/_search.py` & `cca_zoo-1.9.1/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/cca_base.py` & `cca_zoo-1.9.1/cca_zoo/models/cca_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/gcca.py` & `cca_zoo-1.9.1/cca_zoo/models/gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/innerloop.py` & `cca_zoo-1.9.1/cca_zoo/models/innerloop.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/iterative.py` & `cca_zoo-1.9.1/cca_zoo/models/iterative.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/mcca.py` & `cca_zoo-1.9.1/cca_zoo/models/mcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/rcca.py` & `cca_zoo-1.9.1/cca_zoo/models/rcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/models/tcca.py` & `cca_zoo-1.9.1/cca_zoo/models/tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/probabilisticmodels/vcca.py` & `cca_zoo-1.9.1/cca_zoo/probabilisticmodels/vcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/test/test_data.py` & `cca_zoo-1.9.1/cca_zoo/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/test/test_deepmodels.py` & `cca_zoo-1.9.1/cca_zoo/test/test_deepmodels.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from cca_zoo.deepmodels import DCCA, DCCAE, DVCCA, DCCA_NOI, DTCCA, SplitAE, DeepWrapper
 from cca_zoo.deepmodels import objectives, architectures
 from cca_zoo.models import CCA
 
 manual_seed(0)
 rng = check_random_state(0)
 X = rng.rand(200, 10)
-Y = rng.rand(200, 10)
-Z = rng.rand(200, 10)
+Y = rng.rand(200, 12)
+Z = rng.rand(200, 14)
 X_conv = rng.rand(100, 1, 16, 16)
 Y_conv = rng.rand(100, 1, 16, 16)
 train_dataset = data.CCA_Dataset([X, Y])
 
 
 def test_input_types():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     # DCCA
     dcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.CCA,
     )
 
@@ -85,15 +85,15 @@
 def test_DCCA_methods_cpu():
     latent_dims = 4
     cca_model = CCA(latent_dims=latent_dims).fit((X, Y))
     device = "cpu"
     epochs = 100
     # DCCA
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     dcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.CCA,
     )
     optimizer = optim.SGD(dcca_model.parameters(), lr=1e-2)
     dcca_model = DeepWrapper(dcca_model, device=device, optimizer=optimizer)
@@ -102,15 +102,15 @@
             np.testing.assert_array_less(
                 cca_model.score((X, Y)).sum(), dcca_model.score((X, Y)).sum()
             )
             is None
     )
     # DGCCA
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     dgcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.GCCA,
     )
     optimizer = optim.SGD(dgcca_model.parameters(), lr=1e-2)
     dgcca_model = DeepWrapper(dgcca_model, device=device, optimizer=optimizer)
@@ -119,15 +119,15 @@
             np.testing.assert_array_less(
                 cca_model.score((X, Y)).sum(), dgcca_model.score((X, Y)).sum()
             )
             is None
     )
     # DMCCA
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     dmcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.MCCA,
     )
     optimizer = optim.SGD(dmcca_model.parameters(), lr=1e-2)
     dmcca_model = DeepWrapper(dmcca_model, device=device, optimizer=optimizer)
@@ -136,35 +136,35 @@
             np.testing.assert_array_less(
                 cca_model.score((X, Y)).sum(), dmcca_model.score((X, Y)).sum()
             )
             is None
     )
     # DCCA_NOI
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     dcca_noi_model = DCCA_NOI(
         latent_dims, X.shape[0], encoders=[encoder_1, encoder_2], rho=0
     )
-    optimizer = optim.Adam(dcca_noi_model.parameters(), lr=1e-2)
+    optimizer = optim.Adam(dcca_noi_model.parameters(), lr=1e-3)
     dcca_noi_model = DeepWrapper(dcca_noi_model, device=device, optimizer=optimizer)
     dcca_noi_model.fit((X, Y), epochs=epochs)
     assert (
             np.testing.assert_array_less(
                 cca_model.score((X, Y)).sum(), dcca_noi_model.score((X, Y)).sum()
             )
             is None
     )
 
 
 def test_DTCCA_methods_cpu():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(latent_dims=10, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=10, feature_size=10)
-    encoder_3 = architectures.Encoder(latent_dims=10, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=10, feature_size=12)
+    encoder_3 = architectures.Encoder(latent_dims=10, feature_size=14)
     # DTCCA
     dtcca_model = DTCCA(latent_dims=latent_dims, encoders=[encoder_1, encoder_2])
 
     dtcca_model = DeepWrapper(dtcca_model, device=device)
     dtcca_model.fit((X, Y), epochs=20)
     # DCCA
     dcca_model = DCCA(
@@ -177,15 +177,15 @@
     dcca_model.fit((X, Y), epochs=20)
 
 
 def test_scheduler():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     # DCCA
     dcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.CCA,
     )
     optimizer = optim.Adam(dcca_model.parameters(), lr=1e-4)
@@ -197,16 +197,16 @@
     dcca_model.fit((X, Y), epochs=20)
 
 
 def test_DGCCA_methods_cpu():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_3 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_3 = architectures.Encoder(latent_dims=latent_dims, feature_size=14)
     # DTCCA
     dtcca_model = DTCCA(latent_dims=latent_dims, encoders=[encoder_1, encoder_2])
 
     dtcca_model = DeepWrapper(dtcca_model, device=device)
     dtcca_model.fit((X, Y, Z))
     # DGCCA
     dgcca_model = DCCA(
@@ -228,17 +228,17 @@
     dmcca_model.fit((X, Y, Z))
 
 
 def test_DCCAE_methods_cpu():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     decoder_1 = architectures.Decoder(latent_dims=latent_dims, feature_size=10)
-    decoder_2 = architectures.Decoder(latent_dims=latent_dims, feature_size=10)
+    decoder_2 = architectures.Decoder(latent_dims=latent_dims, feature_size=12)
     # DCCAE
     dccae_model = DCCAE(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
 
@@ -274,21 +274,21 @@
 def test_DVCCA_methods_cpu():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(
         latent_dims=latent_dims, feature_size=10, variational=True
     )
     encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dims=latent_dims, feature_size=12, variational=True
     )
     decoder_1 = architectures.Decoder(
         latent_dims=latent_dims, feature_size=10, norm_output=True
     )
     decoder_2 = architectures.Decoder(
-        latent_dims=latent_dims, feature_size=10, norm_output=True
+        latent_dims=latent_dims, feature_size=12, norm_output=True
     )
     # DVCCA
     dvcca_model = DVCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
@@ -300,27 +300,27 @@
 def test_DVCCA_p_methods_cpu():
     latent_dims = 2
     device = "cpu"
     encoder_1 = architectures.Encoder(
         latent_dims=latent_dims, feature_size=10, variational=True
     )
     encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dims=latent_dims, feature_size=12, variational=True
     )
     private_encoder_1 = architectures.Encoder(
         latent_dims=latent_dims, feature_size=10, variational=True
     )
     private_encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dims=latent_dims, feature_size=12, variational=True
     )
     decoder_1 = architectures.Decoder(
         latent_dims=2 * latent_dims, feature_size=10, norm_output=True
     )
     decoder_2 = architectures.Decoder(
-        latent_dims=2 * latent_dims, feature_size=10, norm_output=True
+        latent_dims=2 * latent_dims, feature_size=12, norm_output=True
     )
     # DVCCA
     dvcca_model = DVCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
         private_encoders=[private_encoder_1, private_encoder_2],
@@ -330,15 +330,15 @@
     dvcca_model.fit((X, Y))
 
 
 def test_DCCA_methods_gpu():
     latent_dims = 2
     device = "cuda"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     # DCCA
     dcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         objective=objectives.CCA,
     )
 
@@ -371,16 +371,16 @@
     dcca_noi_model.fit((X, Y))
 
 
 def test_DGCCA_methods_gpu():
     latent_dims = 2
     device = "cuda"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_3 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_3 = architectures.Encoder(latent_dims=latent_dims, feature_size=14)
     # DGCCA
     dgcca_model = DCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2, encoder_3],
         objective=objectives.GCCA,
     )
 
@@ -397,17 +397,17 @@
     dmcca_model.fit((X, Y, Z))
 
 
 def test_DCCAE_methods_gpu():
     latent_dims = 2
     device = "cuda"
     encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
+    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
     decoder_1 = architectures.Decoder(latent_dims=latent_dims, feature_size=10)
-    decoder_2 = architectures.Decoder(latent_dims=latent_dims, feature_size=10)
+    decoder_2 = architectures.Decoder(latent_dims=latent_dims, feature_size=12)
     # DCCAE
     dccae_model = DCCAE(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
 
@@ -418,38 +418,38 @@
 def test_DVCCA_methods_gpu():
     latent_dims = 2
     device = "cuda"
     encoder_1 = architectures.Encoder(
         latent_dims=latent_dims, feature_size=10, variational=True
     )
     encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dims=latent_dims, feature_size=12, variational=True
     )
     decoder_1 = architectures.Decoder(
         latent_dims=latent_dims, feature_size=10, norm_output=True
     )
     decoder_2 = architectures.Decoder(
-        latent_dims=latent_dims, feature_size=10, norm_output=True
+        latent_dims=latent_dims, feature_size=12, norm_output=True
     )
     # DVCCA
     dvcca_model = DVCCA(
         latent_dims=latent_dims,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
 
     dvcca_model = DeepWrapper(dvcca_model, device=device)
     dvcca_model.fit((X, Y))
 
 
 def test_linear():
     encoder_1 = architectures.LinearEncoder(latent_dims=1, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=1, feature_size=10)
+    encoder_2 = architectures.LinearEncoder(latent_dims=1, feature_size=12)
     dcca_model = DCCA(latent_dims=1, encoders=[encoder_1, encoder_2])
-    dcca_model = DeepWrapper(dcca_model).fit((X, Y), epochs=35)
+    dcca_model = DeepWrapper(dcca_model).fit((X, Y), epochs=40)
     cca = CCA().fit((X, Y))
     # check linear encoder with SGD matches vanilla linear CCA
     assert (
             np.testing.assert_array_almost_equal(
                 cca.score((X, Y)), dcca_model.score((X, Y)), decimal=2
             )
             is None
```

### Comparing `cca_zoo-1.9.0/cca_zoo/test/test_models.py` & `cca_zoo-1.9.1/cca_zoo/test/test_models.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/utils/check_values.py` & `cca_zoo-1.9.1/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo/utils/plotting.py` & `cca_zoo-1.9.1/cca_zoo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-1.9.0/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-1.9.1/cca_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 1.9.0
+Version: 1.9.1
 Summary: Canonical Correlation Analysis Zoo: CCA, GCCA, MCCA, DCCA, DGCCA, DVCCA, DCCAE, KCCA and regularised variants including sparse CCA , ridge CCA and elastic CCA
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/303801602.svg)](https://zenodo.org/badge/latestdoi/303801602)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/master/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-1.9.0/cca_zoo.egg-info/SOURCES.txt` & `cca_zoo-1.9.1/cca_zoo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 cca_zoo/model_selection/_search.py
 cca_zoo/models/__init__.py
 cca_zoo/models/cca_base.py
 cca_zoo/models/gcca.py
 cca_zoo/models/innerloop.py
 cca_zoo/models/iterative.py
 cca_zoo/models/mcca.py
+cca_zoo/models/ncca.py
 cca_zoo/models/rcca.py
 cca_zoo/models/tcca.py
 cca_zoo/probabilisticmodels/__init__.py
 cca_zoo/probabilisticmodels/vcca.py
 cca_zoo/test/__init__.py
 cca_zoo/test/test_data.py
 cca_zoo/test/test_deepmodels.py
```

### Comparing `cca_zoo-1.9.0/setup.py` & `cca_zoo-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open("./requirements/deep.txt", "r") as f:
     EXTRA_PACKAGES['deep'] = f.read()
 with open("./requirements/probabilistic.txt", "r") as f:
     EXTRA_PACKAGES['probabilistic'] = f.read()
 
 setup(
     name='cca_zoo',
-    version='1.9.0',
+    version='1.9.1',
     include_package_data=True,
     keywords='cca',
     packages=find_packages(),
     url='https://github.com/jameschapman19/cca_zoo',
     license='MIT',
     author='jameschapman',
     description=(
```

