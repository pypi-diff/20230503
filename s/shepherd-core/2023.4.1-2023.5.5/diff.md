# Comparing `tmp/shepherd_core-2023.4.1.tar.gz` & `tmp/shepherd_core-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.4.1.tar", last modified: Thu Apr 13 21:00:36 2023, max compression
+gzip compressed data, was "shepherd_core-2023.5.5.tar", last modified: Wed May  3 19:29:44 2023, max compression
```

## Comparing `shepherd_core-2023.4.1.tar` & `shepherd_core-2023.5.5.tar`

### file list

```diff
@@ -1,18 +1,77 @@
-drwxrwxrwx   0 hans      (1000) hans      (1000)        0 2023-04-13 21:00:36.525268 shepherd_core-2023.4.1/
--rwxrwxrwx   0 hans      (1000) hans      (1000)     2127 2023-04-13 21:00:36.525268 shepherd_core-2023.4.1/PKG-INFO
--rwxrwxrwx   0 hans      (1000) hans      (1000)      807 2023-04-13 15:14:18.000000 shepherd_core-2023.4.1/README.md
--rwxrwxrwx   0 hans      (1000) hans      (1000)       84 2023-04-12 21:01:39.000000 shepherd_core-2023.4.1/pyproject.toml
--rwxrwxrwx   0 hans      (1000) hans      (1000)     1630 2023-04-13 21:00:36.526268 shepherd_core-2023.4.1/setup.cfg
-drwxrwxrwx   0 hans      (1000) hans      (1000)        0 2023-04-13 21:00:36.515848 shepherd_core-2023.4.1/shepherd_core/
--rwxrwxrwx   0 hans      (1000) hans      (1000)      545 2023-04-13 14:28:48.000000 shepherd_core-2023.4.1/shepherd_core/__init__.py
--rwxrwxrwx   0 hans      (1000) hans      (1000)     1901 2023-04-12 20:42:18.000000 shepherd_core-2023.4.1/shepherd_core/calibration.py
--rwxrwxrwx   0 hans      (1000) hans      (1000)     1403 2023-04-12 21:18:43.000000 shepherd_core-2023.4.1/shepherd_core/logger.py
--rwxrwxrwx   0 hans      (1000) hans      (1000)    12336 2023-04-13 14:27:29.000000 shepherd_core-2023.4.1/shepherd_core/reader.py
--rwxrwxrwx   0 hans      (1000) hans      (1000)    13623 2023-04-12 20:52:53.000000 shepherd_core-2023.4.1/shepherd_core/writer.py
-drwxrwxrwx   0 hans      (1000) hans      (1000)        0 2023-04-13 21:00:36.524268 shepherd_core-2023.4.1/shepherd_core.egg-info/
--rwxrwxrwx   0 hans      (1000) hans      (1000)     2127 2023-04-13 21:00:36.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/PKG-INFO
--rwxrwxrwx   0 hans      (1000) hans      (1000)      387 2023-04-13 21:00:36.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/SOURCES.txt
--rwxrwxrwx   0 hans      (1000) hans      (1000)        1 2023-04-13 21:00:36.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/dependency_links.txt
--rwxrwxrwx   0 hans      (1000) hans      (1000)      117 2023-04-13 21:00:36.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/requires.txt
--rwxrwxrwx   0 hans      (1000) hans      (1000)       14 2023-04-13 21:00:36.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/top_level.txt
--rwxrwxrwx   0 hans      (1000) hans      (1000)        1 2023-04-13 20:57:51.000000 shepherd_core-2023.4.1/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.445703 shepherd_core-2023.5.5/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/content/virtual_source_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/experiment/target_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/model_virtualSourceDoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.449703 shepherd_core-2023.5.5/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/programmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.453703 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:29:44.000000 shepherd_core-2023.5.5/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:44.457703 shepherd_core-2023.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-03 19:29:32.000000 shepherd_core-2023.5.5/tests/test_testbed_models.py
```

### Comparing `shepherd_core-2023.4.1/PKG-INFO` & `shepherd_core-2023.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.4.1
+Version: 2023.5.5
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -35,15 +35,17 @@
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
 [![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This Python Module bundles data-models and file-access-routines that are used by several codebases. Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
+This Python Module bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+
+Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
 
 ---
 
 **Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
 
 **Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
```

### Comparing `shepherd_core-2023.4.1/README.md` & `shepherd_core-2023.5.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Shepherd - Core
-
-[![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
-[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
-[![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-This Python Module bundles data-models and file-access-routines that are used by several codebases. Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
-
----
-
-**Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
-
-**Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
-
----
+# Shepherd - Core
+
+[![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
+[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
+[![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+This Python Module bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+
+Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
+
+---
+
+**Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
+
+**Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
+
+---
```

### Comparing `shepherd_core-2023.4.1/setup.cfg` & `shepherd_core-2023.5.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -37,33 +37,33 @@
 include_package_data = True
 python_requires = >= 3.7
 install_requires = 
 	h5py
 	numpy
 	pyYAML
 	chromalog
+	pydantic[email]<2.0.0
 
 [options.extras_require]
 dev = 
 	black
 	pylint
 	flake8
 	twine
 	pre-commit
 	pyright
 test = 
 	pytest
-	pytest-click
 	coverage
 
 [options.packages.find]
 where = .
 
 [options.package_data]
-* = README.md
+* = README.md,*.yaml
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 addopts = -vvv
```

### Comparing `shepherd_core-2023.4.1/shepherd_core/calibration.py` & `shepherd_core-2023.5.5/shepherd_core/calibration.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-""" Helper-FNs to convert values between raw/int and physical si-units
-
-"""
-from typing import Dict
-from typing import TypeVar
-
-import numpy as np
-from numpy.typing import NDArray
-
-# TODO: build
-#  - unit-converter-class that takes cal-pairs (gain, offset)
-#  - cal-class that takes dict of pairs and builds complete converter
-
-cal_default: Dict[str, Dict[str, float]] = {
-    "voltage": {"gain": 3 * 1e-9, "offset": 0.0},  # allows 0 - 12 V in 3 nV-Steps
-    "current": {"gain": 250 * 1e-12, "offset": 0.0},  # allows 0 - 1 A in 250 pA - Steps
-    "time": {"gain": 1e-9, "offset": 0.0},
-    # SI-value [SI-Unit] = raw-value * gain + offset
-}
-
-T_calc = TypeVar("T_calc", NDArray[np.float64], float)
-
-
-def raw_to_si(values_raw: T_calc, cal: Dict[str, float]) -> T_calc:
-    """Helper to convert between physical units and raw unsigned integers
-
-    :param values_raw: number or numpy array with raw values
-    :param cal: calibration-dict with entries for gain and offset
-    :return: converted number or array
-    """
-    values_si = values_raw * cal["gain"] + cal["offset"]
-    if isinstance(values_si, np.ndarray):
-        values_si[values_si < 0.0] = 0.0
-        # if pyright still complains, cast with .astype(float)
-    else:
-        values_si = float(max(values_si, 0.0))
-    return values_si
-
-
-def si_to_raw(values_si: T_calc, cal: Dict[str, float]) -> T_calc:
-    """Helper to convert between physical units and raw unsigned integers
-
-    :param values_si: number or numpy array with values in physical units
-    :param cal: calibration-dict with entries for gain and offset
-    :return: converted number or array
-    """
-    values_raw = (values_si - cal["offset"]) / cal["gain"]
-    if isinstance(values_raw, np.ndarray):
-        values_raw[values_raw < 0.0] = 0.0
-    else:
-        values_raw = max(values_raw, 0.0)
-    return values_raw
+""" Helper-FNs to convert values between raw/int and physical si-units
+
+"""
+from typing import Dict
+from typing import TypeVar
+
+import numpy as np
+from numpy.typing import NDArray
+
+# TODO: build
+#  - unit-converter-class that takes cal-pairs (gain, offset)
+#  - cal-class that takes dict of pairs and builds complete converter
+
+cal_default: Dict[str, Dict[str, float]] = {
+    "voltage": {"gain": 3 * 1e-9, "offset": 0.0},  # allows 0 - 12 V in 3 nV-Steps
+    "current": {"gain": 250 * 1e-12, "offset": 0.0},  # allows 0 - 1 A in 250 pA - Steps
+    "time": {"gain": 1e-9, "offset": 0.0},
+    # SI-value [SI-Unit] = raw-value * gain + offset
+}
+
+T_calc = TypeVar("T_calc", NDArray[np.float64], float)
+
+
+def raw_to_si(values_raw: T_calc, cal: Dict[str, float]) -> T_calc:
+    """Helper to convert between physical units and raw unsigned integers
+
+    :param values_raw: number or numpy array with raw values
+    :param cal: calibration-dict with entries for gain and offset
+    :return: converted number or array
+    """
+    values_si = values_raw * cal["gain"] + cal["offset"]
+    if isinstance(values_si, np.ndarray):
+        values_si[values_si < 0.0] = 0.0
+        # if pyright still complains, cast with .astype(float)
+    else:
+        values_si = float(max(values_si, 0.0))
+    return values_si
+
+
+def si_to_raw(values_si: T_calc, cal: Dict[str, float]) -> T_calc:
+    """Helper to convert between physical units and raw unsigned integers
+
+    :param values_si: number or numpy array with values in physical units
+    :param cal: calibration-dict with entries for gain and offset
+    :return: converted number or array
+    """
+    values_raw = (values_si - cal["offset"]) / cal["gain"]
+    if isinstance(values_raw, np.ndarray):
+        values_raw[values_raw < 0.0] = 0.0
+    else:
+        values_raw = max(values_raw, 0.0)
+    return values_raw
```

### Comparing `shepherd_core-2023.4.1/shepherd_core/writer.py` & `shepherd_core-2023.5.5/shepherd_core/writer.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-"""
-Writer that inherits from Reader-Baseclass
-"""
-import logging
-import math
-from itertools import product
-from pathlib import Path
-from typing import Optional
-from typing import Union
-
-import h5py
-import numpy as np
-import yaml
-
-from .calibration import cal_default
-from .calibration import si_to_raw
-from .reader import BaseReader
-
-
-def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
-    """finds an unused filename in case it already exists
-
-    :param base_path: file-path to test
-    :param suffix: file-suffix
-    :return: new non-existing path
-    """
-    counter = 0
-    while True:
-        path = Path(base_path).with_suffix(f".{counter}{suffix}")
-        if not path.exists():
-            return path
-        counter += 1
-
-
-class BaseWriter(BaseReader):
-    """Stores data for Shepherd in HDF5 format
-
-    Args:
-        file_path: (Path) Name of the HDF5 file that data will be written to
-        mode: (str) Indicates if this is data from harvester or emulator
-        datatype: (str) choose type: ivsample (most common), ivcurve or isc_voc
-        window_samples: (int) windows size for the datatype ivcurve
-        cal_data: (CalibrationData) Data is written as raw ADC
-            values. We need calibration data in order to convert to physical
-            units later.
-        modify_existing: (bool) explicitly enable modifying existing file
-            otherwise a unique name will be found
-        compression: (str) use either None, lzf or "1" (gzips compression level)
-        verbose: (bool) provides more info instead of just warnings / errors
-    """
-
-    # choose lossless compression filter
-    # - lzf:  low to moderate compression, VERY fast, no options
-    #         -> 20 % cpu overhead for half the filesize
-    # - gzip: good compression, moderate speed, select level from 1-9, default is 4
-    #         -> lower levels seem fine
-    #         -> _algo=number instead of "gzip" is read as compression level for gzip
-    # -> comparison / benchmarks https://www.h5py.org/lzf/
-    comp_default: int = 1
-    mode_default: str = "harvester"
-    datatype_default: str = "ivsample"
-
-    _chunk_shape: tuple = (BaseReader.samples_per_buffer,)
-
-    def __init__(
-        self,
-        file_path: Path,
-        mode: Optional[str] = None,
-        datatype: Optional[str] = None,
-        window_samples: Optional[int] = None,
-        cal_data: Optional[dict] = None,
-        modify_existing: bool = False,
-        compression: Union[None, str, int] = "default",
-        verbose: Optional[bool] = True,
-    ):
-        file_path = Path(file_path)
-        self._modify = modify_existing
-
-        if not hasattr(self, "_logger"):
-            self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
-        # -> logger gets configured in reader()
-
-        if self._modify or not file_path.exists():
-            self._file_path: Path = file_path
-            self._logger.info("Storing data to   '%s'", self._file_path)
-        else:
-            base_dir = file_path.resolve().parents[0]
-            self._file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
-            self._logger.warning(
-                "File %s already exists -> " "storing under %s instead",
-                file_path,
-                self._file_path.name,
-            )
-
-        if not isinstance(mode, (str, type(None))):
-            raise TypeError(f"Can't handle type '{type(mode)}' for mode [str, None]")
-        if isinstance(mode, str) and mode not in self.mode_dtype_dict:
-            raise ValueError(
-                f"Can't handle mode '{mode}' " f"(choose one of {self.mode_dtype_dict})"
-            )
-        if not isinstance(window_samples, (int, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(window_samples)}' for window_samples [int, None]"
-            )
-        if not isinstance(cal_data, (dict, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(cal_data)}' for cal_data [dict, None]"
-            )
-
-        if not isinstance(datatype, (str, type(None))):
-            raise TypeError(
-                f"Can't handle type '{type(datatype)}' for datatype [str, None]"
-            )
-
-        _dtypes = self.mode_dtype_dict[self.mode_default if (mode is None) else mode]
-        if isinstance(datatype, str) and datatype not in _dtypes:
-            raise ValueError(
-                f"Can't handle value '{datatype}' of datatype "
-                f"(choose one of {_dtypes})"
-            )
-
-        if self._modify:
-            self._mode = mode
-            self._cal = (
-                cal_data if isinstance(cal_data, dict) else cal_default
-            )  # TODO: switch to pydantic
-            self._datatype = datatype
-            self._window_samples = window_samples
-        else:
-            self._mode = mode if isinstance(mode, str) else self.mode_default
-            self._cal = cal_data if isinstance(cal_data, dict) else cal_default
-            self._datatype = (
-                datatype if isinstance(datatype, str) else self.datatype_default
-            )
-            self._window_samples = (
-                window_samples if isinstance(window_samples, int) else 0
-            )
-
-        if compression in [None, "lzf", 1]:  # order of recommendation
-            self._compression_algo = compression
-        else:
-            self._compression_algo = self.comp_default
-
-        # open file
-        if self._modify:
-            self.h5file = h5py.File(self._file_path, "r+")  # = rw
-        else:
-            self.h5file = h5py.File(self._file_path, "w")  # write, truncate if exist
-            self._create_skeleton()
-
-        # Store the mode in order to allow user to differentiate harvesting vs emulation data
-        if isinstance(self._mode, str) and self._mode in self.mode_dtype_dict:
-            self.h5file.attrs["mode"] = self._mode
-
-        if (
-            isinstance(self._datatype, str)
-            and self._datatype in self.mode_dtype_dict[self.get_mode()]
-        ):
-            self.h5file["data"].attrs["datatype"] = self._datatype
-        elif not self._modify:
-            self._logger.error("datatype invalid? '%s' not written", self._datatype)
-
-        if isinstance(self._window_samples, int):
-            self.h5file["data"].attrs["window_samples"] = self._window_samples
-
-        if self._cal is not None:
-            for channel, parameter in product(
-                ["current", "voltage"], ["gain", "offset"]
-            ):
-                self.h5file["data"][channel].attrs[parameter] = self._cal[channel][
-                    parameter
-                ]
-        super().__init__(file_path=None, verbose=verbose)
-
-    def __enter__(self):
-        super().__enter__()
-        return self
-
-    def __exit__(self, *exc):  # type: ignore
-        self._align()
-        self._refresh_file_stats()
-        self._logger.info(
-            "closing hdf5 file, %s s iv-data, size = %s MiB, rate = %s KiB/s",
-            self.runtime_s,
-            round(self.file_size / 2**20, 3),
-            round(self.data_rate / 2**10),
-        )
-        self.is_valid()
-        self.h5file.close()
-
-    def _create_skeleton(self) -> None:
-        """Initializes the structure of the HDF5 file
-
-        HDF5 is hierarchically structured and before writing data, we have to
-        setup this structure, i.e. creating the right groups with corresponding
-        data types. We will store 3 types of data in a database: The
-        actual IV samples recorded either from the harvester (during recording)
-        or the target (during emulation). Any log messages, that can be used to
-        store relevant events or tag some parts of the recorded data.
-
-        """
-        # Store voltage and current samples in the data group,
-        # both are stored as 4 Byte unsigned int
-        gp_data = self.h5file.create_group("data")
-        # the size of window_samples-attribute in harvest-data indicates ivcurves as input
-        # -> emulator uses virtual-harvester, field will be adjusted by .embed_config()
-        gp_data.attrs["window_samples"] = 0
-
-        gp_data.create_dataset(
-            "time",
-            (0,),
-            dtype="u8",
-            maxshape=(None,),
-            chunks=self._chunk_shape,
-            compression=self._compression_algo,
-        )
-        gp_data["time"].attrs["unit"] = "ns"
-        gp_data["time"].attrs["description"] = "system time [ns]"
-
-        gp_data.create_dataset(
-            "current",
-            (0,),
-            dtype="u4",
-            maxshape=(None,),
-            chunks=self._chunk_shape,
-            compression=self._compression_algo,
-        )
-        gp_data["current"].attrs["unit"] = "A"
-        gp_data["current"].attrs["description"] = "current [A] = value * gain + offset"
-
-        gp_data.create_dataset(
-            "voltage",
-            (0,),
-            dtype="u4",
-            maxshape=(None,),
-            chunks=self._chunk_shape,
-            compression=self._compression_algo,
-        )
-        gp_data["voltage"].attrs["unit"] = "V"
-        gp_data["voltage"].attrs["description"] = "voltage [V] = value * gain + offset"
-
-    def append_iv_data_raw(
-        self,
-        timestamp_ns: Union[np.ndarray, float, int],
-        voltage: np.ndarray,
-        current: np.ndarray,
-    ) -> None:
-        """Writes raw data to database
-
-        Args:
-            timestamp_ns: just start of buffer or whole ndarray
-            voltage: ndarray as raw unsigned integers
-            current: ndarray as raw unsigned integers
-        """
-        len_new = min(voltage.size, current.size)
-
-        if isinstance(timestamp_ns, float):
-            timestamp_ns = int(timestamp_ns)
-        if isinstance(timestamp_ns, int):
-            time_series_ns = self.sample_interval_ns * np.arange(len_new).astype("u8")
-            timestamp_ns = timestamp_ns + time_series_ns
-        if isinstance(timestamp_ns, np.ndarray):
-            len_new = min(len_new, timestamp_ns.size)
-        else:
-            self._logger.error("timestamp-data was not usable")
-            return
-
-        len_old = self.ds_time.shape[0]
-
-        # resize dataset
-        self.ds_time.resize((len_old + len_new,))
-        self.ds_voltage.resize((len_old + len_new,))
-        self.ds_current.resize((len_old + len_new,))
-
-        # append new data
-        self.ds_time[len_old : len_old + len_new] = timestamp_ns[:len_new]
-        self.ds_voltage[len_old : len_old + len_new] = voltage[:len_new]
-        self.ds_current[len_old : len_old + len_new] = current[:len_new]
-
-    def append_iv_data_si(
-        self,
-        timestamp: Union[np.ndarray, float],
-        voltage: np.ndarray,
-        current: np.ndarray,
-    ) -> None:
-        """Writes data (in SI / physical unit) to file, but converts it to raw-data first
-
-           SI-value [SI-Unit] = raw-value * gain + offset,
-
-        Args:
-            timestamp: python timestamp (time.time()) in seconds (si-unit)
-                       -> provide start of buffer or whole ndarray
-            voltage: ndarray in physical-unit V
-            current: ndarray in physical-unit A
-        """
-        timestamp = timestamp * 10**9
-        voltage = si_to_raw(voltage, self._cal["voltage"])
-        current = si_to_raw(current, self._cal["current"])
-        self.append_iv_data_raw(timestamp, voltage, current)
-
-    def _align(self) -> None:
-        """Align datasets with buffer-size of shepherd"""
-        self._refresh_file_stats()
-        n_buff = self.ds_time.size / self.samples_per_buffer
-        size_new = int(math.floor(n_buff) * self.samples_per_buffer)
-        if size_new < self.ds_time.size:
-            if self.samplerate_sps < 95_000:
-                self._logger.debug("skipped alignment due to altered samplerate")
-                return
-            self._logger.info(
-                "aligning with buffer-size, discarding last %s entries",
-                self.ds_time.size - size_new,
-            )
-            self.ds_time.resize((size_new,))
-            self.ds_voltage.resize((size_new,))
-            self.ds_current.resize((size_new,))
-
-    def __setitem__(self, key: str, item):  # type: ignore
-        """A convenient interface to store relevant key-value data (attribute) if H5-structure"""
-        return self.h5file.attrs.__setitem__(key, item)
-
-    def set_config(self, data: dict) -> None:
-        """Important Step to get a self-describing Output-File
-
-        :param data: from virtual harvester or converter / source
-        """
-        self.h5file["data"].attrs["config"] = yaml.safe_dump(
-            data, default_flow_style=False, sort_keys=False
-        )
-        if "window_samples" in data:
-            self.set_window_samples(data["window_samples"])
-
-    def set_window_samples(self, samples: int = 0) -> None:
-        """parameter essential for ivcurves
-
-        :param samples: length of window / voltage sweep
-        """
-        self.h5file["data"].attrs["window_samples"] = samples
-
-    def set_hostname(self, name: str) -> None:
-        """option to distinguish the host, target or data-source in the testbed
-            -> perfect for plotting later
-
-        :param name: something unique, or "artificial" in case of generated content
-        """
-        self.h5file.attrs["hostname"] = name
+"""
+Writer that inherits from Reader-Baseclass
+"""
+import logging
+import math
+from itertools import product
+from pathlib import Path
+from typing import Optional
+from typing import Union
+
+import h5py
+import numpy as np
+import yaml
+
+from .calibration import cal_default
+from .calibration import si_to_raw
+from .reader import BaseReader
+
+
+def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
+    """finds an unused filename in case it already exists
+
+    :param base_path: file-path to test
+    :param suffix: file-suffix
+    :return: new non-existing path
+    """
+    counter = 0
+    while True:
+        path = Path(base_path).with_suffix(f".{counter}{suffix}")
+        if not path.exists():
+            return path
+        counter += 1
+
+
+class BaseWriter(BaseReader):
+    """Stores data for Shepherd in HDF5 format
+
+    Args:
+        file_path: (Path) Name of the HDF5 file that data will be written to
+        mode: (str) Indicates if this is data from harvester or emulator
+        datatype: (str) choose type: ivsample (most common), ivcurve or isc_voc
+        window_samples: (int) windows size for the datatype ivcurve
+        cal_data: (CalibrationData) Data is written as raw ADC
+            values. We need calibration data in order to convert to physical
+            units later.
+        modify_existing: (bool) explicitly enable modifying existing file
+            otherwise a unique name will be found
+        compression: (str) use either None, lzf or "1" (gzips compression level)
+        verbose: (bool) provides more info instead of just warnings / errors
+    """
+
+    # choose lossless compression filter
+    # - lzf:  low to moderate compression, VERY fast, no options
+    #         -> 20 % cpu overhead for half the filesize
+    # - gzip: good compression, moderate speed, select level from 1-9, default is 4
+    #         -> lower levels seem fine
+    #         -> _algo=number instead of "gzip" is read as compression level for gzip
+    # -> comparison / benchmarks https://www.h5py.org/lzf/
+    comp_default: int = 1
+    mode_default: str = "harvester"
+    datatype_default: str = "ivsample"
+
+    _chunk_shape: tuple = (BaseReader.samples_per_buffer,)
+
+    def __init__(
+        self,
+        file_path: Path,
+        mode: Optional[str] = None,
+        datatype: Optional[str] = None,
+        window_samples: Optional[int] = None,
+        cal_data: Optional[dict] = None,
+        modify_existing: bool = False,
+        compression: Union[None, str, int] = "default",
+        verbose: Optional[bool] = True,
+    ):
+        file_path = Path(file_path)
+        self._modify = modify_existing
+
+        if not hasattr(self, "_logger"):
+            self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
+        # -> logger gets configured in reader()
+
+        if self._modify or not file_path.exists():
+            self._file_path: Path = file_path
+            self._logger.info("Storing data to   '%s'", self._file_path)
+        else:
+            base_dir = file_path.resolve().parents[0]
+            self._file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
+            self._logger.warning(
+                "File %s already exists -> " "storing under %s instead",
+                file_path,
+                self._file_path.name,
+            )
+
+        if not isinstance(mode, (str, type(None))):
+            raise TypeError(f"Can't handle type '{type(mode)}' for mode [str, None]")
+        if isinstance(mode, str) and mode not in self.mode_dtype_dict:
+            raise ValueError(
+                f"Can't handle mode '{mode}' " f"(choose one of {self.mode_dtype_dict})"
+            )
+        if not isinstance(window_samples, (int, type(None))):
+            raise TypeError(
+                f"Can't handle type '{type(window_samples)}' for window_samples [int, None]"
+            )
+        if not isinstance(cal_data, (dict, type(None))):
+            raise TypeError(
+                f"Can't handle type '{type(cal_data)}' for cal_data [dict, None]"
+            )
+
+        if not isinstance(datatype, (str, type(None))):
+            raise TypeError(
+                f"Can't handle type '{type(datatype)}' for datatype [str, None]"
+            )
+
+        _dtypes = self.mode_dtype_dict[self.mode_default if (mode is None) else mode]
+        if isinstance(datatype, str) and datatype not in _dtypes:
+            raise ValueError(
+                f"Can't handle value '{datatype}' of datatype "
+                f"(choose one of {_dtypes})"
+            )
+
+        if self._modify:
+            self._mode = mode
+            self._cal = (
+                cal_data if isinstance(cal_data, dict) else cal_default
+            )  # TODO: switch to pydantic
+            self._datatype = datatype
+            self._window_samples = window_samples
+        else:
+            self._mode = mode if isinstance(mode, str) else self.mode_default
+            self._cal = cal_data if isinstance(cal_data, dict) else cal_default
+            self._datatype = (
+                datatype if isinstance(datatype, str) else self.datatype_default
+            )
+            self._window_samples = (
+                window_samples if isinstance(window_samples, int) else 0
+            )
+
+        if compression in [None, "lzf", 1]:  # order of recommendation
+            self._compression_algo = compression
+        else:
+            self._compression_algo = self.comp_default
+
+        # open file
+        if self._modify:
+            self.h5file = h5py.File(self._file_path, "r+")  # = rw
+        else:
+            self.h5file = h5py.File(self._file_path, "w")  # write, truncate if exist
+            self._create_skeleton()
+
+        # Store the mode in order to allow user to differentiate harvesting vs emulation data
+        if isinstance(self._mode, str) and self._mode in self.mode_dtype_dict:
+            self.h5file.attrs["mode"] = self._mode
+
+        if (
+            isinstance(self._datatype, str)
+            and self._datatype in self.mode_dtype_dict[self.get_mode()]
+        ):
+            self.h5file["data"].attrs["datatype"] = self._datatype
+        elif not self._modify:
+            self._logger.error("datatype invalid? '%s' not written", self._datatype)
+
+        if isinstance(self._window_samples, int):
+            self.h5file["data"].attrs["window_samples"] = self._window_samples
+
+        if self._cal is not None:
+            for channel, parameter in product(
+                ["current", "voltage"], ["gain", "offset"]
+            ):
+                self.h5file["data"][channel].attrs[parameter] = self._cal[channel][
+                    parameter
+                ]
+        super().__init__(file_path=None, verbose=verbose)
+
+    def __enter__(self):
+        super().__enter__()
+        return self
+
+    def __exit__(self, *exc):  # type: ignore
+        self._align()
+        self._refresh_file_stats()
+        self._logger.info(
+            "closing hdf5 file, %s s iv-data, size = %s MiB, rate = %s KiB/s",
+            self.runtime_s,
+            round(self.file_size / 2**20, 3),
+            round(self.data_rate / 2**10),
+        )
+        self.is_valid()
+        self.h5file.close()
+
+    def _create_skeleton(self) -> None:
+        """Initializes the structure of the HDF5 file
+
+        HDF5 is hierarchically structured and before writing data, we have to
+        setup this structure, i.e. creating the right groups with corresponding
+        data types. We will store 3 types of data in a database: The
+        actual IV samples recorded either from the harvester (during recording)
+        or the target (during emulation). Any log messages, that can be used to
+        store relevant events or tag some parts of the recorded data.
+
+        """
+        # Store voltage and current samples in the data group,
+        # both are stored as 4 Byte unsigned int
+        gp_data = self.h5file.create_group("data")
+        # the size of window_samples-attribute in harvest-data indicates ivcurves as input
+        # -> emulator uses virtual-harvester, field will be adjusted by .embed_config()
+        gp_data.attrs["window_samples"] = 0
+
+        gp_data.create_dataset(
+            "time",
+            (0,),
+            dtype="u8",
+            maxshape=(None,),
+            chunks=self._chunk_shape,
+            compression=self._compression_algo,
+        )
+        gp_data["time"].attrs["unit"] = "ns"
+        gp_data["time"].attrs["description"] = "system time [ns]"
+
+        gp_data.create_dataset(
+            "current",
+            (0,),
+            dtype="u4",
+            maxshape=(None,),
+            chunks=self._chunk_shape,
+            compression=self._compression_algo,
+        )
+        gp_data["current"].attrs["unit"] = "A"
+        gp_data["current"].attrs["description"] = "current [A] = value * gain + offset"
+
+        gp_data.create_dataset(
+            "voltage",
+            (0,),
+            dtype="u4",
+            maxshape=(None,),
+            chunks=self._chunk_shape,
+            compression=self._compression_algo,
+        )
+        gp_data["voltage"].attrs["unit"] = "V"
+        gp_data["voltage"].attrs["description"] = "voltage [V] = value * gain + offset"
+
+    def append_iv_data_raw(
+        self,
+        timestamp_ns: Union[np.ndarray, float, int],
+        voltage: np.ndarray,
+        current: np.ndarray,
+    ) -> None:
+        """Writes raw data to database
+
+        Args:
+            timestamp_ns: just start of buffer or whole ndarray
+            voltage: ndarray as raw unsigned integers
+            current: ndarray as raw unsigned integers
+        """
+        len_new = min(voltage.size, current.size)
+
+        if isinstance(timestamp_ns, float):
+            timestamp_ns = int(timestamp_ns)
+        if isinstance(timestamp_ns, int):
+            time_series_ns = self.sample_interval_ns * np.arange(len_new).astype("u8")
+            timestamp_ns = timestamp_ns + time_series_ns
+        if isinstance(timestamp_ns, np.ndarray):
+            len_new = min(len_new, timestamp_ns.size)
+        else:
+            self._logger.error("timestamp-data was not usable")
+            return
+
+        len_old = self.ds_time.shape[0]
+
+        # resize dataset
+        self.ds_time.resize((len_old + len_new,))
+        self.ds_voltage.resize((len_old + len_new,))
+        self.ds_current.resize((len_old + len_new,))
+
+        # append new data
+        self.ds_time[len_old : len_old + len_new] = timestamp_ns[:len_new]
+        self.ds_voltage[len_old : len_old + len_new] = voltage[:len_new]
+        self.ds_current[len_old : len_old + len_new] = current[:len_new]
+
+    def append_iv_data_si(
+        self,
+        timestamp: Union[np.ndarray, float],
+        voltage: np.ndarray,
+        current: np.ndarray,
+    ) -> None:
+        """Writes data (in SI / physical unit) to file, but converts it to raw-data first
+
+           SI-value [SI-Unit] = raw-value * gain + offset,
+
+        Args:
+            timestamp: python timestamp (time.time()) in seconds (si-unit)
+                       -> provide start of buffer or whole ndarray
+            voltage: ndarray in physical-unit V
+            current: ndarray in physical-unit A
+        """
+        timestamp = timestamp * 10**9
+        voltage = si_to_raw(voltage, self._cal["voltage"])
+        current = si_to_raw(current, self._cal["current"])
+        self.append_iv_data_raw(timestamp, voltage, current)
+
+    def _align(self) -> None:
+        """Align datasets with buffer-size of shepherd"""
+        self._refresh_file_stats()
+        n_buff = self.ds_time.size / self.samples_per_buffer
+        size_new = int(math.floor(n_buff) * self.samples_per_buffer)
+        if size_new < self.ds_time.size:
+            if self.samplerate_sps < 95_000:
+                self._logger.debug("skipped alignment due to altered samplerate")
+                return
+            self._logger.info(
+                "aligning with buffer-size, discarding last %s entries",
+                self.ds_time.size - size_new,
+            )
+            self.ds_time.resize((size_new,))
+            self.ds_voltage.resize((size_new,))
+            self.ds_current.resize((size_new,))
+
+    def __setitem__(self, key: str, item):  # type: ignore
+        """A convenient interface to store relevant key-value data (attribute) if H5-structure"""
+        return self.h5file.attrs.__setitem__(key, item)
+
+    def set_config(self, data: dict) -> None:
+        """Important Step to get a self-describing Output-File
+
+        :param data: from virtual harvester or converter / source
+        """
+        self.h5file["data"].attrs["config"] = yaml.safe_dump(
+            data, default_flow_style=False, sort_keys=False
+        )
+        if "window_samples" in data:
+            self.set_window_samples(data["window_samples"])
+
+    def set_window_samples(self, samples: int = 0) -> None:
+        """parameter essential for ivcurves
+
+        :param samples: length of window / voltage sweep
+        """
+        self.h5file["data"].attrs["window_samples"] = samples
+
+    def set_hostname(self, name: str) -> None:
+        """option to distinguish the host, target or data-source in the testbed
+            -> perfect for plotting later
+
+        :param name: something unique, or "artificial" in case of generated content
+        """
+        self.h5file.attrs["hostname"] = name
```

### Comparing `shepherd_core-2023.4.1/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.5.5/shepherd_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.4.1
+Version: 2023.5.5
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -35,15 +35,17 @@
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
 [![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This Python Module bundles data-models and file-access-routines that are used by several codebases. Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
+This Python Module bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+
+Users probably want to use the [datalib](https://pypi.org/project/shepherd_data).
 
 ---
 
 **Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
 
 **Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
```

