# Comparing `tmp/magnumnp-1.0.8.tar.gz` & `tmp/magnumnp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnumnp-1.0.8.tar", last modified: Mon Feb 27 15:01:13 2023, max compression
+gzip compressed data, was "magnumnp-1.0.9.tar", last modified: Wed May  3 15:33:07 2023, max compression
```

## Comparing `magnumnp-1.0.8.tar` & `magnumnp-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.222425 magnumnp-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-02-27 15:00:56.000000 magnumnp-1.0.8/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35069 2023-02-27 15:00:56.000000 magnumnp-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6135 2023-02-27 15:01:13.222425 magnumnp-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5642 2023-02-27 15:00:56.000000 magnumnp-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.217424 magnumnp-1.0.8/magnumnp/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.219424 magnumnp-1.0.8/magnumnp/common/
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/decorated_tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     7290 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/material.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     4781 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/state.py
--rw-rw-rw-   0 root         (0) root         (0)    38962 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/tabulate.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/time_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/common/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.220425 magnumnp-1.0.8/magnumnp/field_terms/
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5554 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/anisotropy.py
--rw-rw-rw-   0 root         (0) root         (0)     7910 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/demag.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/demagPBC.py
--rw-rw-rw-   0 root         (0) root         (0)     6605 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/dmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2110 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/exchangePBC.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/external.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/field_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     6127 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/oersted.py
--rw-rw-rw-   0 root         (0) root         (0)     4937 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/rkky.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/field_terms/spintorque.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.221425 magnumnp-1.0.8/magnumnp/loggers/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/loggers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/loggers/field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/loggers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/loggers/scalar_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.221425 magnumnp-1.0.8/magnumnp/solvers/
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/llg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.221425 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/rkf45.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/scipy_ode.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/scipy_odeint.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/ode_solvers/torchdiffeq.py
--rw-rw-rw-   0 root         (0) root         (0)     3313 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/solvers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.222425 magnumnp-1.0.8/magnumnp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/utils/imaging_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-02-27 15:00:56.000000 magnumnp-1.0.8/magnumnp/utils/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 15:01:13.218424 magnumnp-1.0.8/magnumnp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6135 2023-02-27 15:01:13.000000 magnumnp-1.0.8/magnumnp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1411 2023-02-27 15:01:13.000000 magnumnp-1.0.8/magnumnp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 15:01:13.000000 magnumnp-1.0.8/magnumnp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-02-27 15:01:13.000000 magnumnp-1.0.8/magnumnp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-27 15:01:13.000000 magnumnp-1.0.8/magnumnp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 15:01:13.222425 magnumnp-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-02-27 15:01:06.000000 magnumnp-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.837859 magnumnp-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-03 15:32:50.000000 magnumnp-1.0.9/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35069 2023-05-03 15:32:50.000000 magnumnp-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-05-03 15:33:07.837859 magnumnp-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2023-05-03 15:32:50.000000 magnumnp-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.832859 magnumnp-1.0.9/magnumnp/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.834859 magnumnp-1.0.9/magnumnp/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/decorated_tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/material.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     6630 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/state.py
+-rw-rw-rw-   0 root         (0) root         (0)    38962 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/tabulate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/time_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/common/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.835859 magnumnp-1.0.9/magnumnp/field_terms/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5554 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/anisotropy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demagPBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     7456 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/demag_nonequidistant.py
+-rw-rw-rw-   0 root         (0) root         (0)     6605 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/dmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     2110 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/exchangePBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/external.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/field_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6325 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/oersted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4937 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/rkky.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/field_terms/spintorque.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.835859 magnumnp-1.0.9/magnumnp/loggers/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/loggers/scalar_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/solvers/
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/llg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/rkf45.py
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_odeint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/ode_solvers/torchdiffeq.py
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/solvers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.836860 magnumnp-1.0.9/magnumnp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/imaging_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-05-03 15:32:51.000000 magnumnp-1.0.9/magnumnp/utils/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:33:07.832859 magnumnp-1.0.9/magnumnp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-03 15:33:07.000000 magnumnp-1.0.9/magnumnp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 15:33:07.837859 magnumnp-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-03 15:33:01.000000 magnumnp-1.0.9/setup.py
```

### Comparing `magnumnp-1.0.8/LICENSE` & `magnumnp-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/PKG-INFO` & `magnumnp-1.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1
-Name: magnumnp
-Version: 1.0.8
-Summary: magnum.np finite-difference package for the solution of micromagnetic problems
-Home-page: http://gitlab.com/magnum.np/magnum.np
-Author: Florian Bruckner
-Author-email: florian.bruckner@univie.ac.at
-Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
-Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-magnum.np 1.0.8
+magnum.np 1.0.9
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -34,15 +21,22 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [Standard Problem #4](demos/sp4/run.ipynb)
+   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
@@ -65,15 +59,15 @@
 
     pip install -e .
 
 Note that a default version of [pytorch](http://www.pytorch.org) is included in magnum.np's dependecy list. If you would like to uses a specific pytorch version (fitting your installed CUDA library) it needs to be installed in advance.
 
 ### run remotely via Google Colab
 ---------------------------------
-Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](http://colab.research.google.com). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
+Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](https://drive.google.com/drive/folders/1Ymvx9bi0qQqW-zlOws0ahFJqoE3JCFd9?usp=share_link). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
 
 Some jupyter-notebook examples are included in the [demo](demos/README.md) directory, which also include links to Colab, where they can directly be run without any local installation.
 
 
 Example
 -------
 The following demo code shows the solution of the muMAG Standard Problem #5 and can be found in the demos directory:
```

### Comparing `magnumnp-1.0.8/README.md` & `magnumnp-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-magnum.np 1.0.8
+Metadata-Version: 2.1
+Name: magnumnp
+Version: 1.0.9
+Summary: magnum.np finite-difference package for the solution of micromagnetic problems
+Home-page: http://gitlab.com/magnum.np/magnum.np
+Author: Florian Bruckner
+Author-email: florian.bruckner@univie.ac.at
+Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
+Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+magnum.np 1.0.9
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -21,15 +34,22 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [Standard Problem #4](demos/sp4/run.ipynb)
+   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
@@ -52,15 +72,15 @@
 
     pip install -e .
 
 Note that a default version of [pytorch](http://www.pytorch.org) is included in magnum.np's dependecy list. If you would like to uses a specific pytorch version (fitting your installed CUDA library) it needs to be installed in advance.
 
 ### run remotely via Google Colab
 ---------------------------------
-Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](http://colab.research.google.com). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
+Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](https://drive.google.com/drive/folders/1Ymvx9bi0qQqW-zlOws0ahFJqoE3JCFd9?usp=share_link). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
 
 Some jupyter-notebook examples are included in the [demo](demos/README.md) directory, which also include links to Colab, where they can directly be run without any local installation.
 
 
 Example
 -------
 The following demo code shows the solution of the muMAG Standard Problem #5 and can be found in the demos directory:
```

### Comparing `magnumnp-1.0.8/magnumnp/__init__.py` & `magnumnp-1.0.9/magnumnp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """magnum.np main module"""
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 import magnumnp.common.logging as logging
 import torch
-#torch.set_default_dtype(torch.float64)
+torch.set_default_dtype(torch.float64)
 
-# monkey patch older torch version without compile
-if not hasattr(torch, "compile"):
-    def fake_compile(func):
-        return func
-    logging.warning("PyTorch version < 2.0 does not support 'torch.compile'! Switch to pytorch 2.0 in order get maximum performance!")
+# monkey patch torch versions < 2.0 or on Windows
+try:
+   def fake_compile(func):
+       return func
+
+   @torch.compile
+   def dummy_function():
+      return
+   dummy_function()
+except Exception as e:
     torch.compile = fake_compile
+    logging.warning(e)
+
 
 try:
     import setproctitle
     setproctitle.setproctitle("magnumnp")
 
     from magnumnp.common import *
     from magnumnp.field_terms import *
```

### Comparing `magnumnp-1.0.8/magnumnp/common/__init__.py` & `magnumnp-1.0.9/magnumnp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/common/constants.py` & `magnumnp-1.0.9/magnumnp/common/constants.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/common/decorated_tensor.py` & `magnumnp-1.0.9/magnumnp/common/time_interpolator.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,39 +12,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
+import numpy as np
 import torch
+from scipy import interpolate
 
-__all__ = ["DecoratedTensor"]
+__all__ = ["TimeInterpolator"]
 
-class DecoratedTensor(torch.Tensor):
-    @staticmethod
-    def __new__(cls, x, *args, **kwargs): # TODO: is this needed?
-        return super().__new__(cls, x, *args, **kwargs)
-
-    def avg(self, dim=(0,1,2)):
-        if self.dim() <= 1: # e.g. [0,0,1]
-            return self
-        elif self.dim() == 2: # state.m[domain]
-            return self.mean(dim=0)
-        else:
-            return self.mean(dim=dim)
-
-    def average(self, dim=(0,1,2)):
-        return self.avg(dim)
-
-    def normalize(self):
-        self /= torch.linalg.norm(self, dim = -1, keepdim = True)
-        self[...] = torch.nan_to_num(self, posinf=0, neginf=0)
-        return self
+class TimeInterpolator(object):
+    def __init__(self, state, points):
+        self._tp = state.Tensor(list(points.keys()))
+        self._fp = state._tensor(list(points.values()))
+        self._state = state
 
     def __call__(self, t):
-        return self
+        i = torch.searchsorted(self._tp, t) # upper index
+        i = torch.clamp(i, min=1, max=len(self._tp)-1) # extrapolate on bounds
+        tp = self._tp
+        fp = self._fp
+        return fp[i-1] + (t-tp[i-1]) / (tp[i]-tp[i-1]) * (fp[i] - fp[i-1])
 
     @property
-    def torch_tensor(self):
-        ''' return original tensor (in order to apply pytorch.compile) '''
-        return self.as_subclass(torch.Tensor)
+    def final_time(self):
+        return self._tp[-1]
```

### Comparing `magnumnp-1.0.8/magnumnp/common/io.py` & `magnumnp-1.0.9/magnumnp/common/io.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,54 @@
 import torch
 import numpy as np
 import scipy
 import pyvista as pv
 import os
 from . import Mesh, DecoratedTensor
 
-__all__ = ["write_vti", "read_vti", "read_image", "read_mesh"]
+__all__ = ["write_vtr", "write_vti", "read_vti", "read_image", "read_mesh"]
+
+def write_vtr(fields, filename, state = None):
+    dirname = os.path.dirname(filename)
+    if dirname and not os.path.isdir(dirname):
+        os.makedirs(dirname)
+
+    if not (isinstance(fields, list) or isinstance(fields, dict)):
+        fields = [fields]
+    if not isinstance(fields, dict):
+        fields = {"f%03d"%i:f for (i,f) in enumerate(fields)}
+
+    if state is None:
+        n = list(fields.values())[0].shape[:3]
+        dx = (1., 1., 1.)
+        origin = (0., 0., 0.)
+    else:
+        n = state.mesh.n
+        dx = state.mesh.dx
+        origin = state.mesh.origin
+
+    x = torch.hstack([state._tensor([0.]), state.dx[0].cumsum(0)]).cpu().numpy() + state.mesh.origin[0]
+    y = torch.hstack([state._tensor([0.]), state.dx[1].cumsum(0)]).cpu().numpy() + state.mesh.origin[1]
+    z = torch.hstack([state._tensor([0.]), state.dx[2].cumsum(0)]).cpu().numpy() + state.mesh.origin[2]
+
+    grid = pv.RectilinearGrid(x, y, z)
+
+    for name, f in fields.items():
+        if len(f.shape) == 0 or len(f.shape) == 1: # expand constant tensor to tensorfield
+            f = f.expand(n + f.shape)
+        if len(f.shape) == 4 and f.shape[-1] == 1: # remove dim for scalar field (nx,ny,nz,1) => (nx,ny,nz)
+            f = f[: ,:, :, 0]
+        if len(f.shape) == 3: # scalar data
+            grid.cell_data.set_array(f.detach().cpu().numpy().flatten('F'), name)
+        elif len(f.shape) == 4: # vector data
+            grid.cell_data.set_array(f.detach().cpu().numpy().reshape(-1,3,order='F'), name)
+        else:
+            raise ValueError("write_vti: unsupported data format (", name, f.shape, ")")
+    grid.save(filename)
+
 
 def write_vti(fields, filename, state = None):
     r"""
     Write vti files (equidistant rectangular grid, compressed) using pyvista.
 
     :param fields: single torch Tensor or List/Dictionary of tensors to be written
     :type fields: :class:`Tensor`, list, dict
```

### Comparing `magnumnp-1.0.8/magnumnp/common/logging.py` & `magnumnp-1.0.9/magnumnp/common/logging.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/common/mesh.py` & `magnumnp-1.0.9/magnumnp/common/mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,9 @@
         return self.dx[0] * self.dx[1] * self.dx[2]
 
     @property
     def volume(self):
         return self.n[0] * self.n[1] * self.n[2] * self.cell_volume
 
     def __str__(self):
-        return "%dx%dx%d_%gx%gx%g" % (self.n + self.dx)
+        str_dx = ["%g" % dx if isinstance(dx, (float, int)) else "XX" for dx in self.dx]
+        return "%dx%dx%d (size= %s x %s x %s)" % (*self.n, *str_dx)
```

### Comparing `magnumnp-1.0.8/magnumnp/common/tabulate.py` & `magnumnp-1.0.9/magnumnp/common/tabulate.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/common/time_interpolator.py` & `magnumnp-1.0.9/magnumnp/field_terms/field_terms.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-import numpy as np
+from magnumnp.common import constants
 import torch
-from scipy import interpolate
 
-__all__ = ["TimeInterpolator"]
+__all__ = ["FieldTerm", "LinearFieldTerm"]
 
-class TimeInterpolator(object):
-    def __init__(self, state, points):
-        self._tp = state.Tensor(list(points.keys()))
-        self._fp = state._tensor(list(points.values()))
-        self._state = state
+class FieldTerm(object):
+    parameters = []
 
-    def __call__(self, t):
-        i = torch.searchsorted(self._tp, t) # upper index
-        i = torch.clamp(i, min=1, max=len(self._tp)-1) # extrapolate on bounds
-        tp = self._tp
-        fp = self._fp
-        return fp[i-1] + (t-tp[i-1]) / (tp[i]-tp[i-1]) * (fp[i] - fp[i-1])
+    def __init__(self, **kwargs):
+        unknown_params = set(kwargs.keys()) - set(self.parameters)
+        if unknown_params:
+            raise Warning("Got unknown parameters '%s'. Ignoring!" % unknown_params)
+        params = {key:key for key in self.parameters}
+        params.update(kwargs)
+        for key, value in params.items():
+            setattr(self, key, value)
 
-    @property
-    def final_time(self):
-        return self._tp[-1]
+class LinearFieldTerm(FieldTerm):
+    def E(self, state):
+        return -0.5 * constants.mu_0 * state.mesh.cell_volume * torch.sum(state.material["Ms"] * state.m * self.h(state))
```

### Comparing `magnumnp-1.0.8/magnumnp/common/timer.py` & `magnumnp-1.0.9/magnumnp/common/timer.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/__init__.py` & `magnumnp-1.0.9/magnumnp/field_terms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.field_terms.anisotropy import *
 from magnumnp.field_terms.demag import *
+from magnumnp.field_terms.demag_nonequidistant import *
 from magnumnp.field_terms.demagPBC import *
 from magnumnp.field_terms.dmi import *
 from magnumnp.field_terms.exchange import *
 from magnumnp.field_terms.exchangePBC import *
 from magnumnp.field_terms.external import *
 from magnumnp.field_terms.field_terms import *
 from magnumnp.field_terms.oersted import *
 from magnumnp.field_terms.rkky import *
 from magnumnp.field_terms.spintorque import *
 
 __all__ = (anisotropy.__all__ +
            demag.__all__ +
+           demag_nonequidistant.__all__ +
            demagPBC.__all__ +
            dmi.__all__ +
            exchange.__all__ +
            exchangePBC.__all__ +
            external.__all__ +
            field_terms.__all__ +
            oersted.__all__ +
```

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/anisotropy.py` & `magnumnp-1.0.9/magnumnp/field_terms/anisotropy.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/demag.py` & `magnumnp-1.0.9/magnumnp/field_terms/demag.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,45 +13,42 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.common import logging, timedmethod, constants, Timer
+from .field_terms import LinearFieldTerm
 import numpy as np
 import torch
 import torch.fft
 from torch import asinh, atan, sqrt, log, abs
 from time import time
 import os
 
-__all__ = ["DemagField", "newell_f", "newell_g", "dipole_f", "dipole_g"]
+__all__ = ["DemagField", "newell_f", "newell_g", "dipole_f", "dipole_g", "newell_N"]
 
-def newell_f(points):
-    x = abs(points[:,:,:,0])
-    y = abs(points[:,:,:,1])
-    z = abs(points[:,:,:,2])
+def newell_f(x, y, z):
+    x, y, z = abs(x), abs(y), abs(z)
 
     result = 1.0 / 6.0 * (2*x**2 - y**2 - z**2) * sqrt(x**2 + y**2 + z**2)
 
     mask = (x**2 + z**2).gt(0)
     result[mask] += (y / 2.0 * (z**2 - x**2) * asinh(y / sqrt(x**2 + z**2)))[mask]
 
     mask = (x**2 + y**2).gt(0)
     result[mask] += (z / 2.0 * (y**2 - x**2) * asinh(z / sqrt(x**2 + y**2)))[mask]
 
     mask = (x * (x**2 + y**2 + z**2)).gt(0)
     result[mask] -= (x * y * z * atan(y*z / (x * sqrt(x**2 + y**2 + z**2))))[mask]
 
     return result
 
-def newell_g(points):
-    x = points[:,:,:,0]
-    y = points[:,:,:,1]
-    z = abs(points[:,:,:,2])
+def newell_g(x, y, z):
+    z = abs(z)
 
     result = - x*y * sqrt(x**2 + y**2 + z**2) / 3.0
 
     mask = (x**2 + y**2).gt(0) # x**2 + y**2 > 0
     result[mask] += (x*y*z * asinh(z / sqrt(x**2 + y**2)))[mask]
 
     mask = (y**2 + z**2).gt(0)
@@ -67,42 +64,45 @@
     result[mask] -= (z * y**2 / 2.0 * atan(x*z / (y * sqrt(x**2 + y**2 + z**2))))[mask]
 
     mask = (x * (x**2 + y**2 + z**2)).ne(0)
     result[mask] -= (z * x**2 / 2.0 * atan(y*z / (x * sqrt(x**2 + y**2 + z**2))))[mask]
 
     return result
 
+def F1(func, x, y, z, dz, dZ):
+    return func(x, y, z      + dZ) \
+         - func(x, y, z          ) \
+         - func(x, y, z - dz + dZ) \
+         + func(x, y, z - dz     )
+
+def F0(func, x, y, z, dy, dY, dz, dZ):
+    return F1(func, x, y      + dY, z, dz, dZ) \
+         - F1(func, x, y,           z, dz, dZ) \
+         - F1(func, x, y - dy + dY, z, dz, dZ) \
+         + F1(func, x, y - dy,      z, dz, dZ)
+
+def newell_N(func, x, y, z, dx, dy, dz, dX, dY, dZ):
+    return F0(func, x,           y, z, dy, dY, dz, dZ) \
+         - F0(func, x - dx,      y, z, dy, dY, dz, dZ) \
+         - F0(func, x + dX,      y, z, dy, dY, dz, dZ) \
+         + F0(func, x - dx + dX, y, z, dy, dY, dz, dZ)
 
-def dipole_f(points):
-    x = points[:,:,:,0]
-    y = points[:,:,:,1]
-    z = points[:,:,:,2]
 
+def dipole_f(x, y, z):
     result = (2.*x**2 - y**2 - z**2) * pow(x**2 + y**2 + z**2, -5./2.)
     result[0,0,0] = 0.
     return result
 
-def dipole_g(points):
-    x = points[:,:,:,0]
-    y = points[:,:,:,1]
-    z = points[:,:,:,2]
-
+def dipole_g(x, y, z):
     result = 3.*x*y * pow(x**2 + y**2 + z**2, -5./2.)
     result[0,0,0] = 0.
     return result
 
 
-complex_dtype = {
-    torch.float: torch.complex,
-    torch.float32: torch.complex64,
-    torch.float64: torch.complex128
-    }
-
-
-class DemagField(object):
+class DemagField(LinearFieldTerm):
     r"""
     Demagnetization Field:
 
     The dipole-dipole interaction gives rise to a long-range interaction.
     The integral formulation of the corresponding Maxwell equations can
     be represented as convolution of the magnetization :math:`\vec{M} = M_s \; \vec{m}` with a proper
     demagnetization kernel :math:`\vec{N}`
@@ -124,61 +124,65 @@
         dx /= dx.min()
 
         # dipole far-field
         shape = [1 if n==1 else 2*n for n in state.mesh.n]
         ij = [torch.fft.fftshift(state._arange(n)) - n//2 for n in shape]
         ij = torch.meshgrid(*ij,indexing='ij')
 
-        r = torch.stack([ij[ind]*dx[ind] for ind in perm], dim=-1)
-        Nc = func_far(r) * np.prod(dx) / (4.*np.pi)
+        xyz = [ij[ind]*dx[ind] for ind in perm]
+        Nc = func_far(*xyz) * np.prod(dx) / (4.*np.pi)
 
         # newell near-field
         n_near = np.minimum(state.mesh.n, self._p)
         N_near = state._zeros([1 if n==1 else 2*n for n in n_near])
         ij = [torch.fft.fftshift(state._arange(n)) - n//2 for n in N_near.shape[:3]]
         ij = torch.meshgrid(*ij,indexing='ij')
 
-        for kl in np.rollaxis(np.indices((2,)*6), 0, 7).reshape(64, 6):
-            k, l = kl[:3], kl[3:]
-            r = torch.stack([(ij[ind] + k[ind] - l[ind])*dx[ind] for ind in perm], dim=-1)
-            N_near[:,:,:] -= (-1)**np.sum(kl) * func_near(r) / (4.*np.pi*np.prod(dx))
+        xyz = [ij[ind]*dx[ind] for ind in perm]
+        dx = [dx[ind] for ind in perm]
+        N_near = -newell_N(func_near, *xyz, *dx, *dx) / (4.*np.pi*np.prod(dx))
 
         Nc[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ] = N_near[:n_near[0]   ,:n_near[1]   ,:n_near[2]   ]
         Nc[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:] = N_near[:n_near[0]   ,:n_near[1]   ,-n_near[2]+1:]
         Nc[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ] = N_near[:n_near[0]   ,-n_near[1]+1:,:n_near[2]   ]
         Nc[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:] = N_near[:n_near[0]   ,-n_near[1]+1:,-n_near[2]+1:]
         Nc[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ] = N_near[-n_near[0]+1:,:n_near[1]   ,:n_near[2]   ]
         Nc[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:] = N_near[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:]
         Nc[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ] = N_near[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ]
         Nc[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:] = N_near[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:]
 
-        return torch.fft.rfftn(Nc, dim = [i for i in range(3) if state.mesh.n[i] > 1]).real.clone()
+        Nc = torch.fft.rfftn(Nc, dim = [i for i in range(3) if state.mesh.n[i] > 1])
+        return Nc.real.clone()
 
     def _init_N(self, state):
+        dtype = state._dtype
+        state._dtype = torch.float64 # always use double precision
         time_kernel = time()
-        Nxx = self._init_N_component(state, [0,1,2], newell_f, dipole_f)
-        Nxy = self._init_N_component(state, [0,1,2], newell_g, dipole_g)
-        Nxz = self._init_N_component(state, [0,2,1], newell_g, dipole_g)
-        Nyy = self._init_N_component(state, [1,2,0], newell_f, dipole_f)
-        Nyz = self._init_N_component(state, [1,2,0], newell_g, dipole_g)
-        Nzz = self._init_N_component(state, [2,0,1], newell_f, dipole_f)
+
+        Nxx = self._init_N_component(state, [0,1,2], newell_f, dipole_f).to(dtype=dtype)
+        Nxy = self._init_N_component(state, [0,1,2], newell_g, dipole_g).to(dtype=dtype)
+        Nxz = self._init_N_component(state, [0,2,1], newell_g, dipole_g).to(dtype=dtype)
+        Nyy = self._init_N_component(state, [1,2,0], newell_f, dipole_f).to(dtype=dtype)
+        Nyz = self._init_N_component(state, [1,2,0], newell_g, dipole_g).to(dtype=dtype)
+        Nzz = self._init_N_component(state, [2,0,1], newell_f, dipole_f).to(dtype=dtype)
 
         self._N = [[Nxx, Nxy, Nxz],
                    [Nxy, Nyy, Nyz],
                    [Nxz, Nyz, Nzz]]
         logging.info(f"[DEMAG]: Time calculation of demag kernel = {time() - time_kernel} s")
+        state._dtype = dtype # restore dtype
 
     @timedmethod
     def h(self, state):
         if not hasattr(self, "_N"):
             self._init_N(state)
 
-        hx = state._zeros(list(self._N[0][0].shape), dtype=complex_dtype[self._N[0][0].dtype])
-        hy = state._zeros(list(self._N[0][0].shape), dtype=complex_dtype[self._N[0][0].dtype])
-        hz = state._zeros(list(self._N[0][0].shape), dtype=complex_dtype[self._N[0][0].dtype])
+        hx = state._zeros(self._N[0][0].shape, dtype=state.complex_dtype)
+        hy = state._zeros(self._N[0][0].shape, dtype=state.complex_dtype)
+        hz = state._zeros(self._N[0][0].shape, dtype=state.complex_dtype)
         for ax in range(3):
             m_pad_fft1D = torch.fft.rfftn(state.material["Ms"] * state.m[:,:,:,(ax,)], dim = [i for i in range(3) if state.mesh.n[i] > 1], s = [2*state.mesh.n[i] for i in range(3) if state.mesh.n[i] > 1]).squeeze(-1)
 
             hx += self._N[0][ax] * m_pad_fft1D
             hy += self._N[1][ax] * m_pad_fft1D
             hz += self._N[2][ax] * m_pad_fft1D
```

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/demagPBC.py` & `magnumnp-1.0.9/magnumnp/field_terms/demagPBC.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/dmi.py` & `magnumnp-1.0.9/magnumnp/field_terms/dmi.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/exchange.py` & `magnumnp-1.0.9/magnumnp/field_terms/exchange.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,28 +43,32 @@
     @timedmethod
     def h(self, state):
         A = state.material[self.A].torch_tensor
         Ms = state.material["Ms"].torch_tensor
         m = state.m.torch_tensor
         if self._domain != None:
             A = A * self._domain[:,:,:,None]
-        h = self._h(m, A, Ms, state)
+        dx = state.dx[0].reshape(-1,1,1,1)
+        dy = state.dx[1].reshape(1,-1,1,1)
+        dz = state.dx[2].reshape(1,1,-1,1)
+        h = self._h(m, A, Ms, dx, dy, dz, state)
         return state.Tensor(h)
 
     @torch.compile
-    def _h(self, m, A, Ms, state):
+    def _h(self, m, A, Ms, dx, dy, dz, state):
         h = state._zeros(state.mesh.n + (3,))
-        A_avg = 2.*A[1:,:,:]*A[:-1,:,:] / (A[1:,:,:]+A[:-1,:,:])
-        h[:-1,:,:,:] += A_avg * m[ 1:,:,:,:] / state.mesh.dx[0]**2 # m_i-1 - m_i
-        h[ 1:,:,:,:] += A_avg * m[:-1,:,:,:] / state.mesh.dx[0]**2 # m_i+1 - m_i
 
-        A_avg = 2.*A[:,1:,:]*A[:,:-1,:] / (A[:,1:,:]+A[:,:-1,:])
-        h[:,:-1,:,:] += A_avg * m[:, 1:,:,:] / state.mesh.dx[1]**2 # m_i-1 - m_i
-        h[:, 1:,:,:] += A_avg * m[:,:-1,:,:] / state.mesh.dx[1]**2 # m_i+1 - m_i
+        A_avg = 2.*A[1:,:,:]*A[:-1,:,:] / (A[1:,:,:]*dx[:-1,:,:,:] + A[:-1,:,:]*dx[1:,:,:,:])
+        h[:-1,:,:,:] += A_avg * (m[ 1:,:,:,:]-m[:-1,:,:,:]) / dx[:-1,:,:,:] # m_i-1 - m_i
+        h[ 1:,:,:,:] += A_avg * (m[:-1,:,:,:]-m[ 1:,:,:,:]) / dx[ 1:,:,:,:] # m_i+1 - m_i
 
-        A_avg = 2.*A[:,:,1:]*A[:,:,:-1] / (A[:,:,1:]+A[:,:,:-1])
-        h[:,:,:-1,:] += A_avg * m[:,:, 1:,:] / state.mesh.dx[2]**2 # m_i-1 - m_i
-        h[:,:, 1:,:] += A_avg * m[:,:,:-1,:] / state.mesh.dx[2]**2 # m_i+1 - m_i
+        A_avg = 2.*A[:,1:,:]*A[:,:-1,:] / (A[:,1:,:]*dy[:,:-1,:,:] + A[:,:-1,:]*dy[:,1:,:,:])
+        h[:,:-1,:,:] += A_avg * (m[:, 1:,:,:]-m[:,:-1,:,:]) / dy[:,:-1,:,:] # m_i-1 - m_i
+        h[:, 1:,:,:] += A_avg * (m[:,:-1,:,:]-m[:, 1:,:,:]) / dy[:, 1:,:,:] # m_i+1 - m_i
+
+        A_avg = 2.*A[:,:,1:]*A[:,:,:-1] / (A[:,:,1:]*dz[:,:,:-1,:] + A[:,:,:-1]*dz[:,:,1:,:])
+        h[:,:,:-1,:] += A_avg * (m[:,:, 1:,:]-m[:,:,:-1,:]) / dz[:,:,:-1,:] # m_i-1 - m_i
+        h[:,:, 1:,:] += A_avg * (m[:,:,:-1,:]-m[:,:, 1:,:]) / dz[:,:, 1:,:] # m_i+1 - m_i
 
         h *= 2. / (constants.mu_0 * Ms)
         h = torch.nan_to_num(h, posinf=0, neginf=0)
         return h
```

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/exchangePBC.py` & `magnumnp-1.0.9/magnumnp/field_terms/exchangePBC.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/external.py` & `magnumnp-1.0.9/magnumnp/field_terms/external.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/oersted.py` & `magnumnp-1.0.9/magnumnp/field_terms/oersted.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,33 +108,36 @@
         Kc[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:] = K_near[-n_near[0]+1:,:n_near[1]   ,-n_near[2]+1:]
         Kc[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ] = K_near[-n_near[0]+1:,-n_near[1]+1:,:n_near[2]   ]
         Kc[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:] = K_near[-n_near[0]+1:,-n_near[1]+1:,-n_near[2]+1:]
 
         return torch.fft.rfftn(Kc, dim = [i for i in range(3) if state.mesh.n[i] > 1])#.real.clone()
 
     def _init_K(self, state):
+        dtype = state._dtype
+        state._dtype = torch.float64 # always use double precision
         time_kernel = time()
-        Kxy = self._init_K_component(state, [0,1,2], krueger_g, dipole_g)
-        Kyz = self._init_K_component(state, [1,2,0], krueger_g, dipole_g)
-        Kxz = self._init_K_component(state, [2,0,1], krueger_g, dipole_g)
+        Kxy = self._init_K_component(state, [0,1,2], krueger_g, dipole_g).to(dtype=dtype)
+        Kyz = self._init_K_component(state, [1,2,0], krueger_g, dipole_g).to(dtype=dtype)
+        Kxz = self._init_K_component(state, [2,0,1], krueger_g, dipole_g).to(dtype=dtype)
 
         self._K = [[  0., -Kxy, +Kxz],
                    [+Kxy,   0., -Kyz],
                    [-Kxz, +Kyz,   0.]]
 
         logging.info(f"[OERSTED]: Time calculation of oersted kernel = {time() - time_kernel} s")
+        state._dtype = dtype # restore dtype
 
     @timedmethod
     def h(self, state):
         if not hasattr(self, "_K"):
             self._init_K(state)
 
-        hx = state._zeros(list(self._K[0][1].shape), dtype=torch.complex128)
-        hy = state._zeros(list(self._K[0][1].shape), dtype=torch.complex128)
-        hz = state._zeros(list(self._K[0][1].shape), dtype=torch.complex128)
+        hx = state._zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+        hy = state._zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+        hz = state._zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
 
         for ax in range(3):
             j_pad_fft1D = torch.fft.rfftn(state.j[:,:,:,ax], dim = [i for i in range(3) if state.mesh.n[i] > 1], s = [2*state.mesh.n[i] for i in range(3) if state.mesh.n[i] > 1])
 
             hx += self._K[0][ax] * j_pad_fft1D
             hy += self._K[1][ax] * j_pad_fft1D
             hz += self._K[2][ax] * j_pad_fft1D
```

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/rkky.py` & `magnumnp-1.0.9/magnumnp/field_terms/rkky.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/field_terms/spintorque.py` & `magnumnp-1.0.9/magnumnp/field_terms/spintorque.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/loggers/__init__.py` & `magnumnp-1.0.9/magnumnp/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/loggers/field_logger.py` & `magnumnp-1.0.9/magnumnp/loggers/field_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,21 @@
             elif isinstance(field, tuple) or isinstance(field, list):
                 name = field[0]
                 value = field[1](state)
             else:
                 raise RuntimeError('Column type not supported.')
             values[name] = value
 
-        filename = "%s_%04d.vti" % (self._filename, self._i // self._every)
-        write_vti(values, filename, state = state)
+        filename = "%s_%04d" % (self._filename, self._i // self._every)
+        state.write_vtk(values, filename)
+
+        if state._is_equidistant:
+            filename += ".vti"
+        else:
+            filename += ".vtr"
         cElementTree.SubElement(self._xmlroot[0], "DataSet", timestep=str(state.t.tolist()), file=os.path.basename(filename))
         with open(self._filename + ".pvd", 'w') as fd:
             fd.write(minidom.parseString(" ".join(cElementTree.tostring(self._xmlroot).decode().replace("\n","").split()).replace("> <", "><")).toprettyxml(indent="  "))
 
     def __lshift__(self, state):
         self.log(state)
```

### Comparing `magnumnp-1.0.8/magnumnp/loggers/logger.py` & `magnumnp-1.0.9/magnumnp/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/loggers/scalar_logger.py` & `magnumnp-1.0.9/magnumnp/loggers/scalar_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/__init__.py` & `magnumnp-1.0.9/magnumnp/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/llg.py` & `magnumnp-1.0.9/magnumnp/solvers/llg.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/ode_solvers/__init__.py` & `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/ode_solvers/rkf45.py` & `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/rkf45.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/ode_solvers/scipy_ode.py` & `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_ode.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/ode_solvers/scipy_odeint.py` & `magnumnp-1.0.9/magnumnp/solvers/ode_solvers/scipy_odeint.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/solvers/string.py` & `magnumnp-1.0.9/magnumnp/solvers/string.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/utils/__init__.py` & `magnumnp-1.0.9/magnumnp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/utils/imaging_tools.py` & `magnumnp-1.0.9/magnumnp/utils/imaging_tools.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp/utils/misc.py` & `magnumnp-1.0.9/magnumnp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.0.8/magnumnp.egg-info/PKG-INFO` & `magnumnp-1.0.9/magnumnp.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.0.8
+Version: 1.0.9
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-magnum.np 1.0.8
+magnum.np 1.0.9
 ===============
 
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
@@ -34,15 +34,22 @@
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
 The following demos are also stored on Google Colab, where they can directly be run without any local installation:
 
-   * [Standard Problem #4](demos/sp4/run.ipynb)
+   * [RKKY](demos/rkky.ipynb) ([Colab] (https://colab.research.google.com/drive/1HZyMxhG1HZCMsbdOohNqfmR0WUnoQ-ux))
+   * [Softmagnetic Composite](demos/softmagnetic_composite.ipynb) ([Colab](https://colab.research.google.com/drive/11dP3VrckM_hc24jP0sHIM_0_MlkNioRV))
+   * [Spin Orbit Torque](demos/sot.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
+   * [Standard Problem #4](demos/sp4.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
+   * [Standard Problem #5](demos/sp5.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
+   * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
+   * [Standard Problem FMR](demos/sp_FMR.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
+
 
 
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
@@ -65,15 +72,15 @@
 
     pip install -e .
 
 Note that a default version of [pytorch](http://www.pytorch.org) is included in magnum.np's dependecy list. If you would like to uses a specific pytorch version (fitting your installed CUDA library) it needs to be installed in advance.
 
 ### run remotely via Google Colab
 ---------------------------------
-Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](http://colab.research.google.com). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
+Magnum.np could also be used without any hardware by executing it remotely on resources provided by [Google Colab](https://drive.google.com/drive/folders/1Ymvx9bi0qQqW-zlOws0ahFJqoE3JCFd9?usp=share_link). The platform offers different runtime types like CPU(None), GPU or TPU. This allows users to directly test magnum.np, whithout needing their own hardware. Advanced users can use Google Colab(Pro), which provides access to current GPUs like the A100.
 
 Some jupyter-notebook examples are included in the [demo](demos/README.md) directory, which also include links to Colab, where they can directly be run without any local installation.
 
 
 Example
 -------
 The following demo code shows the solution of the muMAG Standard Problem #5 and can be found in the demos directory:
```

### Comparing `magnumnp-1.0.8/magnumnp.egg-info/SOURCES.txt` & `magnumnp-1.0.9/magnumnp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 magnumnp/common/tabulate.py
 magnumnp/common/time_interpolator.py
 magnumnp/common/timer.py
 magnumnp/field_terms/__init__.py
 magnumnp/field_terms/anisotropy.py
 magnumnp/field_terms/demag.py
 magnumnp/field_terms/demagPBC.py
+magnumnp/field_terms/demag_nonequidistant.py
 magnumnp/field_terms/dmi.py
 magnumnp/field_terms/exchange.py
 magnumnp/field_terms/exchangePBC.py
 magnumnp/field_terms/external.py
 magnumnp/field_terms/field_terms.py
 magnumnp/field_terms/oersted.py
 magnumnp/field_terms/rkky.py
```

### Comparing `magnumnp-1.0.8/setup.py` & `magnumnp-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='magnumnp',
-      version='v1.0.8',
+      version='v1.0.9',
       description='magnum.np finite-difference package for the solution of micromagnetic problems',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Florian Bruckner',
       author_email='florian.bruckner@univie.ac.at',
       url='http://gitlab.com/magnum.np/magnum.np',
       project_urls = {'Documentation': 'https://magnum.np.gitlab.io/magnum.np/',
```

