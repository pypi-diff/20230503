# Comparing `tmp/trusspy-1.0.3.tar.gz` & `tmp/trusspy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trusspy-1.0.3.tar", last modified: Wed Mar 15 22:39:56 2023, max compression
+gzip compressed data, was "trusspy-1.0.4.tar", last modified: Wed May  3 19:44:34 2023, max compression
```

## Comparing `trusspy-1.0.3.tar` & `trusspy-1.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.726243 trusspy-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    33206 2023-03-15 22:39:45.000000 trusspy-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43380 2023-03-15 22:39:56.726243 trusspy-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-03-15 22:39:45.000000 trusspy-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-15 22:39:46.000000 trusspy-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:39:56.726243 trusspy-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.718242 trusspy-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/external_force.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/core/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy/elements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/elements/element_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_extforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/handlers/handler_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy/materials/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/materials/material_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    24745 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.726243 trusspy-1.0.3/src/trusspy/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19226 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/solvers/tpsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/solvers/zerosearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.726243 trusspy-1.0.3/src/trusspy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/tools/helper_functions2.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/tools/movie_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-03-15 22:39:46.000000 trusspy-1.0.3/src/trusspy/tools/plot_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.722242 trusspy-1.0.3/src/trusspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43380 2023-03-15 22:39:56.000000 trusspy-1.0.3/src/trusspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-15 22:39:56.000000 trusspy-1.0.3/src/trusspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:39:56.000000 trusspy-1.0.3/src/trusspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-15 22:39:56.000000 trusspy-1.0.3/src/trusspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 22:39:56.000000 trusspy-1.0.3/src/trusspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:39:56.726243 trusspy-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e101_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e102_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e102_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e103_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e10x_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e10xx_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e201_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e202_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_e302_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_eADV_A_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_eNTA_A_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_eNTA_A_model_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_eNTA_A_model_python2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_eNTA_X_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-15 22:39:46.000000 trusspy-1.0.3/tests/test_stiffness_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.771091 trusspy-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    33206 2023-05-03 19:44:23.000000 trusspy-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43484 2023-05-03 19:44:34.771091 trusspy-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-03 19:44:23.000000 trusspy-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 19:44:24.000000 trusspy-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:44:34.771091 trusspy-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.759091 trusspy-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.759091 trusspy-1.0.4/src/trusspy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.763090 trusspy-1.0.4/src/trusspy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/external_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/core/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.763090 trusspy-1.0.4/src/trusspy/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/elements/element_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.763090 trusspy-1.0.4/src/trusspy/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_extforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/handlers/handler_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.767090 trusspy-1.0.4/src/trusspy/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/materials/material_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.767090 trusspy-1.0.4/src/trusspy/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19226 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/solvers/tpsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/solvers/zerosearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.767090 trusspy-1.0.4/src/trusspy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/tools/helper_functions2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/tools/movie_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-03 19:44:24.000000 trusspy-1.0.4/src/trusspy/tools/plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.763090 trusspy-1.0.4/src/trusspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43484 2023-05-03 19:44:34.000000 trusspy-1.0.4/src/trusspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 19:44:34.000000 trusspy-1.0.4/src/trusspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:44:34.000000 trusspy-1.0.4/src/trusspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 19:44:34.000000 trusspy-1.0.4/src/trusspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 19:44:34.000000 trusspy-1.0.4/src/trusspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:34.771091 trusspy-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e101_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e102_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e102_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e103_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e10x_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e10xx_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e201_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e202_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_e302_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_eADV_A_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_eNTA_A_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_eNTA_A_model_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_eNTA_A_model_python2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_eNTA_X_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 19:44:24.000000 trusspy-1.0.4/tests/test_stiffness_function.py
```

### Comparing `trusspy-1.0.3/LICENSE` & `trusspy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/PKG-INFO` & `trusspy-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trusspy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Truss Solver for Python
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -663,14 +663,16 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
+<img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/>
+
 **TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
```

### Comparing `trusspy-1.0.3/README.md` & `trusspy-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
+<img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/>
+
 **TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
```

### Comparing `trusspy-1.0.3/pyproject.toml` & `trusspy-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/core/analysis.py` & `trusspy-1.0.4/src/trusspy/core/analysis.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/core/boundary.py` & `trusspy-1.0.4/src/trusspy/core/boundary.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/core/element.py` & `trusspy-1.0.4/src/trusspy/core/element.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/core/external_force.py` & `trusspy-1.0.4/src/trusspy/core/external_force.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/core/node.py` & `trusspy-1.0.4/src/trusspy/core/node.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/elements/element_definition.py` & `trusspy-1.0.4/src/trusspy/elements/element_definition.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_boundary.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_boundary.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_element.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_element.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_extforce.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_extforce.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_node.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_node.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_result.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_result.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/handlers/handler_settings.py` & `trusspy-1.0.4/src/trusspy/handlers/handler_settings.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/materials/material_definition.py` & `trusspy-1.0.4/src/trusspy/materials/material_definition.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/model.py` & `trusspy-1.0.4/src/trusspy/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,15 +672,15 @@
         p_elements(self, config)
 
     def plt_extforces(self, config="undeformed"):
         p_extforces(self, config)
 
     def plot_model(
         self,
-        config="both",
+        config=["deformed"],
         view="xz",
         contour=None,
         lim_scale=1.2,
         force_scale=0.5,
         nodesize=10,
         cbar_limits="auto",
         inc=-1,
@@ -696,33 +696,35 @@
             cbar_limits,
             inc,
         )
         return fig, ax
 
     def plot_movie(
         self,
-        config="both",
+        config=["deformed"],
         view="xz",
         contour=None,
         lim_scale=1.2,
         force_scale=0.5,
         nodesize=10,
         cbar_limits="auto",
         incs="all",
+        **kwargs,
     ):
         p_movie(
             self,
             config,
             view,
             contour,
             lim_scale,
             force_scale,
             nodesize,
             cbar_limits,
             incs,
+            **kwargs,
         )
 
     def plot_history(
         self,
         nodes=[1, 1],
         increments=None,
         X="Displacement X",
```

### Comparing `trusspy-1.0.3/src/trusspy/solvers/tpsolver.py` & `trusspy-1.0.4/src/trusspy/solvers/tpsolver.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/solvers/zerosearch.py` & `trusspy-1.0.4/src/trusspy/solvers/zerosearch.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/tools/helper_functions2.py` & `trusspy-1.0.4/src/trusspy/tools/helper_functions2.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/src/trusspy/tools/movie_generator.py` & `trusspy-1.0.4/src/trusspy/tools/movie_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 import os
 from shutil import rmtree
 
 import imageio
 
 
-def png_to_gif(workdir=r"figures/", png_subdir=r"png/", gif_subdir=r"gif/"):
+def png_to_gif(workdir=r"figures/", png_subdir=r"png/", gif_subdir=r"gif/", **kwargs):
     png_dir = workdir + png_subdir
     gif_dir = workdir + gif_subdir
     images = []
 
     if os.path.isdir(gif_dir):
         rmtree(gif_dir)
     os.mkdir(gif_dir)
 
     for file_name in sorted(os.listdir(png_dir)):
         if file_name.endswith(".png"):
             file_path = os.path.join(png_dir, file_name)
             images.append(imageio.imread(file_path))
-    imageio.mimwrite(gif_dir + r"movie.gif", images, fps=5, subrectangles=True)
+    imageio.mimwrite(
+        gif_dir + r"movie.gif", images, subrectangles=True, **kwargs
+    )
```

### Comparing `trusspy-1.0.3/src/trusspy/tools/plot_utilities.py` & `trusspy-1.0.4/src/trusspy/tools/plot_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,30 +162,32 @@
             )
 
     if force_scale is not None and ("deformed" in config or "undeformed" in config):
         # these are matplotlib.patch.Patch properties
         props = dict(boxstyle="round", facecolor="C2", alpha=0.25)
         if view == "3d":
             ax.text2D(
-                0.3,
-                1.05,
+                0.5,
+                0.95,
                 textstr,
                 transform=ax.transAxes,
                 fontsize=11,
                 verticalalignment="top",
+                horizontalalignment="center",
                 bbox=props,
             )
         else:
             ax.text(
-                0.05,
+                0.5,
                 0.95,
                 textstr,
                 transform=ax.transAxes,
                 fontsize=11,
                 verticalalignment="top",
+                horizontalalignment="center",
                 bbox=props,
             )
 
     if len(plt.gca().yaxis.get_label().get_text()) == 0:
         str_ins = ""
     else:
         str_ins = ", "
@@ -212,14 +214,15 @@
     view="xz",
     contour=None,
     lim_scale=1.5,
     force_scale=0.5,
     nodesize=10,
     cbar_limits="auto",
     incs="all",
+    **kwargs,
 ):
     if incs == "all":
         if self.Settings.nsteps > 1:
             b = 0
             for s in range(self.Settings.nsteps):
                 b += self.Settings.incs[s]
         else:
@@ -238,15 +241,15 @@
 
         self.plot_model(
             config, view, contour, lim_scale, force_scale, nodesize, cbar_limits, i
         )
         plt.savefig("figures/png/fig_{:03d}.png".format(i), dpi=200)
         plt.close("all")
 
-    png_to_gif()
+    png_to_gif(**kwargs)
 
 
 def p_path(self, nodepath, increment=-1, Y="Displacement X", fig=None, ax=None):
     # loop over increments
     xx = []
     yy = []
     dir_dict = {"X": 0, "Y": 1, "Z": 2}
```

### Comparing `trusspy-1.0.3/src/trusspy.egg-info/PKG-INFO` & `trusspy-1.0.4/src/trusspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trusspy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Truss Solver for Python
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -663,14 +663,16 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/trusspy.svg)](https://pypi.python.org/pypi/trusspy/) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/trusspy/main?labpath=docs%2Fexamples%2Fe101_nb_interactive.ipynb) [![Documentation Status](https://readthedocs.org/projects/trusspy/badge/?version=latest)](https://trusspy.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/trusspy/branch/main/graph/badge.svg?token=2Z0ZKOUKPW)](https://codecov.io/gh/adtzlr/trusspy) [![DOI](https://zenodo.org/badge/145743574.svg)](https://zenodo.org/badge/latestdoi/145743574) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
+<img src="https://raw.githubusercontent.com/adtzlr/trusspy/main/docs/_static/logo.png" height="80px"/>
+
 **TrussPy** is a 3D **Truss**-Solver written in **Py**-thon which is capable of material and geometric nonlinearities. It uses an object-oriented approach to structure the code in meaningful classes, attributes and methods. TrussPy contains both multistep functionality (multiple loadcase analysis with sequenced external forces) and an adaptive method to control incremental stepwidths. Input files may be written in Excel or directly in Python. A simple post-processing inside TrussPy is directly available via Matplotlib. Model Plots whether in undeformed or deformed configuration with optional contour plots on element forces are easy to show. They may also be generated for a series of increments and saved as a GIF Movie. Last but not least History (a.k.a. x-y) Plots for a series of increments or Path Plots along a given node path may be generated for nodal properties (displacements, forces) or global quantities like the Load-Proportionality-Factor (LPF).
    
 Official Documentation: http://trusspy.readthedocs.io/
 
 # Installation
 Use `pip` to install TrussPy
```

### Comparing `trusspy-1.0.3/src/trusspy.egg-info/SOURCES.txt` & `trusspy-1.0.4/src/trusspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e101_model.py` & `trusspy-1.0.4/tests/test_e101_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e102_model.py` & `trusspy-1.0.4/tests/test_e102_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e102_model_python.py` & `trusspy-1.0.4/tests/test_e102_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e103_model_python.py` & `trusspy-1.0.4/tests/test_e103_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e10x_model.py` & `trusspy-1.0.4/tests/test_e10x_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e10xx_model.py` & `trusspy-1.0.4/tests/test_e10xx_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e201_model.py` & `trusspy-1.0.4/tests/test_e201_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e202_model.py` & `trusspy-1.0.4/tests/test_e202_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_e302_model.py` & `trusspy-1.0.4/tests/test_e302_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_eADV_A_model_python.py` & `trusspy-1.0.4/tests/test_eADV_A_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_eNTA_A_model.py` & `trusspy-1.0.4/tests/test_eNTA_A_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_eNTA_A_model_python.py` & `trusspy-1.0.4/tests/test_eNTA_A_model_python.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_eNTA_A_model_python2.py` & `trusspy-1.0.4/tests/test_eNTA_A_model_python2.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_eNTA_X_model.py` & `trusspy-1.0.4/tests/test_eNTA_X_model.py`

 * *Files identical despite different names*

### Comparing `trusspy-1.0.3/tests/test_stiffness_function.py` & `trusspy-1.0.4/tests/test_stiffness_function.py`

 * *Files identical despite different names*

