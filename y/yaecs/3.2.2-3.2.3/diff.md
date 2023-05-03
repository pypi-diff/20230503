# Comparing `tmp/yaecs-3.2.2.tar.gz` & `tmp/yaecs-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.2.2.tar", last modified: Wed May  3 09:23:11 2023, max compression
+gzip compressed data, was "yaecs-3.2.3.tar", last modified: Wed May  3 12:04:15 2023, max compression
```

## Comparing `yaecs-3.2.2.tar` & `yaecs-3.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.775797 yaecs-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 09:22:54.000000 yaecs-3.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.767798 yaecs-3.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 09:22:54.000000 yaecs-3.2.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-03 09:22:54.000000 yaecs-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-03 09:22:54.000000 yaecs-3.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-03 09:22:54.000000 yaecs-3.2.2/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 09:22:54.000000 yaecs-3.2.2/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-03 09:22:54.000000 yaecs-3.2.2/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 09:22:54.000000 yaecs-3.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 09:22:54.000000 yaecs-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 09:23:11.775797 yaecs-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-03 09:22:54.000000 yaecs-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 09:22:54.000000 yaecs-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 09:22:54.000000 yaecs-3.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-03 09:22:54.000000 yaecs-3.2.2/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:23:11.775797 yaecs-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 09:22:54.000000 yaecs-3.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 09:22:54.000000 yaecs-3.2.2/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.767798 yaecs-3.2.2/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-03 09:22:54.000000 yaecs-3.2.2/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-03 09:22:54.000000 yaecs-3.2.2/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-03 09:22:54.000000 yaecs-3.2.2/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.771798 yaecs-3.2.2/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-03 09:22:54.000000 yaecs-3.2.2/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.775797 yaecs-3.2.2/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.775797 yaecs-3.2.2/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    47188 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-03 09:22:54.000000 yaecs-3.2.2/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:23:11.775797 yaecs-3.2.2/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 09:23:11.000000 yaecs-3.2.2/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.800347 yaecs-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 12:03:52.000000 yaecs-3.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.792347 yaecs-3.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 12:03:52.000000 yaecs-3.2.3/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-03 12:03:52.000000 yaecs-3.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-03 12:03:52.000000 yaecs-3.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-03 12:03:52.000000 yaecs-3.2.3/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 12:03:52.000000 yaecs-3.2.3/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-03 12:03:52.000000 yaecs-3.2.3/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 12:03:52.000000 yaecs-3.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:03:52.000000 yaecs-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 12:04:15.800347 yaecs-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-03 12:03:52.000000 yaecs-3.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 12:03:52.000000 yaecs-3.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 12:03:52.000000 yaecs-3.2.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-03 12:03:52.000000 yaecs-3.2.3/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:04:15.800347 yaecs-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 12:03:52.000000 yaecs-3.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 12:03:52.000000 yaecs-3.2.3/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.792347 yaecs-3.2.3/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.800347 yaecs-3.2.3/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47630 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.2.2/.github/workflows/pipy_deployment.yaml` & `yaecs-3.2.3/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/.gitignore` & `yaecs-3.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/.pylintrc` & `yaecs-3.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/COPYING.LESSER.md` & `yaecs-3.2.3/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/COPYING.md` & `yaecs-3.2.3/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/DOCUMENTATION_WIP.md` & `yaecs-3.2.3/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/LICENSE.md` & `yaecs-3.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/PKG-INFO` & `yaecs-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.2
+Version: 3.2.3
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.2/README.md` & `yaecs-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/pyproject.toml` & `yaecs-3.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/resources/yaecs_constructor_overview.png` & `yaecs-3.2.3/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/setup.py` & `yaecs-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/short-readme.md` & `yaecs-3.2.3/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/unittests/config/conftest.py` & `yaecs-3.2.3/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/unittests/config/test_config.py` & `yaecs-3.2.3/unittests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/unittests/config/utils.py` & `yaecs-3.2.3/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/usage_example/configs/project_config.py` & `yaecs-3.2.3/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/usage_example/main.py` & `yaecs-3.2.3/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/usage_example/project_utils/utils.py` & `yaecs-3.2.3/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/__init__.py` & `yaecs-3.2.3/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config.py` & `yaecs-3.2.3/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config_base.py` & `yaecs-3.2.3/yaecs/config/config_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,24 @@
                                  "after using any constructor.\nYou can remove the 'config.merge_from_command_line()' "
                                  "line from your code now :) it's redundant.")
         to_merge = self._gather_command_line_dict(string_to_merge)
         if to_merge:
             self._manual_merge(to_merge, do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process,
                                source='command line')
 
+    @staticmethod
+    def _added_pre_processing():
+        """ Will contain pre-processing function added via self.add_processing_function_all. """
+        return {}
+
+    @staticmethod
+    def _added_post_processing():
+        """ Will contain post-processing function added via self.add_processing_function_all. """
+        return {}
+
     def _check_for_unlinked_sub_configs(self) -> None:
         """ Used to raise an error when unlinked sub-configs are declared. """
         all_configs = self.get_all_sub_configs()
         linked_configs = self.get_all_linked_sub_configs()
         for i in all_configs:
             found_correspondence = False
             for j in linked_configs:
@@ -743,15 +753,16 @@
                 recursive_set_attribute(self, set_name, self._process_parameter(name, self[name], "post", order))
         post_processed = [param for param in modified if param in self._pre_postprocessing_values]
         if post_processed and self._verbose:
             YAECS_LOGGER.info(f"Performed post-processing for modified parameters {post_processed}.")
 
     def _prepare_processing_functions(self, processing_type: str) -> None:
         """ Sets self._pre/post_processing_functions from the user-provided functions. """
-        processing_functions = getattr(self, f"parameters_{processing_type}_processing")()
+        processing_functions = {**getattr(self, f"parameters_{processing_type}_processing")(),
+                                **getattr(self, f"_added_{processing_type}_processing")()}
         for key, value in processing_functions.items():
 
             if not isinstance(value, (Callable, Iterable)):
                 raise TypeError(f"Invalid {processing_type}-processing functions defined for param '{key}' : "
                                 "the function should be declared as either a function or an iterable of functions, "
                                 "optionally containing one order value.")
```

### Comparing `yaecs-3.2.2/yaecs/config/config_convenience.py` & `yaecs-3.2.3/yaecs/config/config_convenience.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config_getters.py` & `yaecs-3.2.3/yaecs/config/config_getters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config_hooks.py` & `yaecs-3.2.3/yaecs/config/config_hooks.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config_processing_functions.py` & `yaecs-3.2.3/yaecs/config/config_processing_functions.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/config/config_setters.py` & `yaecs-3.2.3/yaecs/config/config_setters.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import logging
 from typing import Any, Callable, Dict, TYPE_CHECKING, Union
 
-from ..yaecs_utils import Priority, set_function_attribute, TypeHint
+from ..yaecs_utils import TypeHint
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigSettersMixin:
@@ -54,35 +54,37 @@
         :param param_name: parameter(s) to which to add a postprocessing function. Expects paths with respect to the
         main config.
         :param function_to_add: postprocessing function to add, using the generic name "function" if it has no name
         :param processing_type: choose between 'pre' to add a pre-processing function or 'post' to add a post-processing
         function
         """
         if isinstance(function_to_add, str):
-            check_function = getattr(self.__class__, function_to_add[len("_tagged_method_"):])
+            check_function = self._assigned_as_yaml_tags[function_to_add[len("_tagged_method_"):]][0]
         else:
             check_function = function_to_add
         if hasattr(check_function, "assigned_yaml_tag"):
             if check_function.assigned_yaml_tag[1] != processing_type:
                 name = "unknown_function" if not hasattr(check_function, "__name__") else check_function.__name__
                 YAECS_LOGGER.warning(f"WARNING : processing function {name} is recommended to use "
                                      f"as {check_function.assigned_yaml_tag[1]}-processing function, "
                                      f"but was declared as {processing_type}-processing function.")
         # Add to main config
         self._main_config.add_processing_function(param_name, function_to_add, processing_type)
         # Add to current sub-configs
         for subconfig in self._main_config.get_all_sub_configs():
             subconfig.add_processing_function(param_name, function_to_add, processing_type)
         # Add to future sub-configs
-        attribute = f"parameters_{processing_type}_processing"
-        current_processing = object.__getattribute__(self, attribute)()
+        attribute = f"_{processing_type}_processing_functions"
+        current_processing = getattr(self, attribute)
+        attribute = f"_added_{processing_type}_processing"
+        current_added_processing = getattr(self, attribute)()
         set_name = param_name
-        while set_name in current_processing:
+        while set_name in current_processing or set_name in current_added_processing:
             set_name = set_name + " "
-        new_processing = {set_name: function_to_add, **current_processing}
+        new_processing = {set_name: function_to_add, **current_added_processing}
         setattr(self.__class__, attribute, lambda self: new_processing)
 
     def add_type_hint(self, name: str, type_hint: TypeHint) -> None:
         """
         Adds a type hint for a parameter to the list of type hints for automatic type checks.
         :param name: full path of the param in the main config
         :param type_hint: type of the param
```

### Comparing `yaecs-3.2.2/yaecs/config_history.py` & `yaecs-3.2.3/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/experiment.py` & `yaecs-3.2.3/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/pytorch_lightning_utils.py` & `yaecs-3.2.3/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/user_utils.py` & `yaecs-3.2.3/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs/yaecs_utils.py` & `yaecs-3.2.3/yaecs/yaecs_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.2/yaecs.egg-info/PKG-INFO` & `yaecs-3.2.3/yaecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.2
+Version: 3.2.3
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.2/yaecs.egg-info/SOURCES.txt` & `yaecs-3.2.3/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

