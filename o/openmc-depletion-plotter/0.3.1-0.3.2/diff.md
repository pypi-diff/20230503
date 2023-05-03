# Comparing `tmp/openmc_depletion_plotter-0.3.1.tar.gz` & `tmp/openmc_depletion_plotter-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_depletion_plotter-0.3.1.tar", last modified: Mon Mar 20 12:54:03 2023, max compression
+gzip compressed data, was "openmc_depletion_plotter-0.3.2.tar", last modified: Wed May  3 13:01:41 2023, max compression
```

## Comparing `openmc_depletion_plotter-0.3.1.tar` & `openmc_depletion_plotter-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.771502 openmc_depletion_plotter-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.775502 openmc_depletion_plotter-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1851485 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/chain-nndc-b7.1.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.771502 openmc_depletion_plotter-0.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.775502 openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/plot_activity_vs_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/plot_atoms_vs_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/simulate_silver_depletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/examples/isotope_charts/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts_fisson_irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts_fusion_irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_multiple_isotope_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/simulate_fission_actiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/isotope_charts/simulate_fussion_actiation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/examples/pulse_schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/examples/pulse_schedule/plot_pulse_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.775502 openmc_depletion_plotter-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 12:54:03.000000 openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 12:54:03.779502 openmc_depletion_plotter-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-20 12:53:47.000000 openmc_depletion_plotter-0.3.1/tests/test_python_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.399462 openmc_depletion_plotter-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.387461 openmc_depletion_plotter-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.391461 openmc_depletion_plotter-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-03 13:01:41.399462 openmc_depletion_plotter-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1851485 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/chain-nndc-b7.1.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.387461 openmc_depletion_plotter-0.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.391461 openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/plot_activity_vs_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/plot_atoms_vs_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/simulate_silver_depletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.391461 openmc_depletion_plotter-0.3.2/examples/isotope_charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts_fisson_irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts_fusion_irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_multiple_isotope_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/simulate_fission_actiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/isotope_charts/simulate_fussion_actiation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.395462 openmc_depletion_plotter-0.3.2/examples/pulse_schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/examples/pulse_schedule/plot_pulse_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:01:41.399462 openmc_depletion_plotter-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.387461 openmc_depletion_plotter-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.395462 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.399462 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 13:01:41.000000 openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:01:41.399462 openmc_depletion_plotter-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-03 13:01:12.000000 openmc_depletion_plotter-0.3.2/tests/test_python_api.py
```

### Comparing `openmc_depletion_plotter-0.3.1/.github/workflows/ci.yml` & `openmc_depletion_plotter-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/.github/workflows/python-publish.yml` & `openmc_depletion_plotter-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/.gitignore` & `openmc_depletion_plotter-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/LICENSE.txt` & `openmc_depletion_plotter-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/PKG-INFO` & `openmc_depletion_plotter-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_depletion_plotter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Plot the isotopes present during depletion steps.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_depletion_plotter-0.3.1/README.md` & `openmc_depletion_plotter-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/chain-nndc-b7.1.xml` & `openmc_depletion_plotter-0.3.2/chain-nndc-b7.1.xml`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/plot_activity_vs_time.py` & `openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/plot_activity_vs_time.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/plot_atoms_vs_time.py` & `openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/plot_atoms_vs_time.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/activity_atoms_vs_time/simulate_silver_depletion.py` & `openmc_depletion_plotter-0.3.2/examples/activity_atoms_vs_time/simulate_silver_depletion.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts_fisson_irradiation.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts_fisson_irradiation.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_isotope_charts_fusion_irradiation.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_isotope_charts_fusion_irradiation.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/plot_multiple_isotope_charts.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/plot_multiple_isotope_charts.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/simulate_fission_actiation.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/simulate_fission_actiation.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/isotope_charts/simulate_fussion_actiation.py` & `openmc_depletion_plotter-0.3.2/examples/isotope_charts/simulate_fussion_actiation.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/examples/pulse_schedule/plot_pulse_schedule.py` & `openmc_depletion_plotter-0.3.2/examples/pulse_schedule/plot_pulse_schedule.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/pyproject.toml` & `openmc_depletion_plotter-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/__init__.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/app.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     st.write("<br>", unsafe_allow_html=True)
 
 
 def main():
 
     st.write(
         """
-            👉 Carry out an OpenMC depletion simulation to generate ```depletion_results.h5``` file and ```maerials.xml``` file.
+            👉 Carry out an OpenMC depletion simulation to generate ```depletion_results.h5``` file and ```materials.xml``` file.
 
         """
         # Not got a h5 file handy, right mouse 🖱️ click and save these links
         # [ example 1 ](https://fusion-energy.github.io/openmc_depletion_plottter/examples/csg_tokamak/geometry.xml),
         # [ example 2 ](https://fusion-energy.github.io/openmc_depletion_plottter/examples/csg_cylinder_box/geometry.xml)
     )
 
@@ -92,27 +92,27 @@
             options=("activity", "number of atoms"),
             index=0,
             key="activity_or_atoms",
             help="",
         )
 
         backend = st.sidebar.selectbox(
-            label="Ploting backend",
+            label="Plotting backend",
             options=("matplotlib", "plotly"),
             index=0,
-            key="geometry_ploting_backend",
+            key="geometry_plotting_backend",
             help="Create png images with MatPlotLib or HTML plots with Plotly",
         )
 
         time_units = st.sidebar.selectbox(
             label="Time units",
             options=("s", "min", "h", "d", "a"),
             index=0,
             key="time_units",
-            help="The time units to use on the Y aixs, seconds minutes, hours, days or years",
+            help="The time units to use on the Y axis, seconds minutes, hours, days or years",
         )
 
         x_scale = st.sidebar.selectbox(
             label="X scale",
             options=("linear", "log"),
             index=0,
             key="x_scale",
@@ -150,28 +150,31 @@
             material_index = st.sidebar.number_input(
                 value=0,
                 label="Material index",
                 key="material_index",
                 help="",
             )
         else:
-            raise ValueError("there are no depleted materials in the first time step")
+            raise ValueError(
+                "There are no depleted materials in the first time step"
+            )
         # bug with threshold as it cuts too much
         # threshold = st.sidebar.number_input(
         #     value=0.,
         #     label="Threshold",
         #     key="threshold",
         #     help="",
         # )
 
         include_total = st.sidebar.radio(
             "Include total",
             options=(True, False),
             help="Add a line to the plot showing the total (or sum) of all other lines.",
         )
+
         excluded_material = st.sidebar.radio(
             "Exclude nuclides from undepleted material",
             options=(True, False),
             help="Allows nuclides in the orginal material to be excluded so that the nuclides created during depletion can be clearly shown.",
         )
 
         if excluded_material:
@@ -194,15 +197,15 @@
                 # horizontal_lines
                 show_top=show_top,
                 # threshold
                 material_index=material_index,
                 include_total=include_total,
                 path=materials_file.name,
             )
-        else:
+        elif activity_or_atoms == "number of atoms":
             plot = results.plot_atoms_vs_time(
                 # todo allow no materials to be excluded
                 excluded_material=material_to_exclude,
                 time_units=time_units,
                 # x_axis_title=f'Time [{time_units}]', this the default already
                 # title="Number of of nuclides in material", this is the default
                 x_scale=x_scale,
@@ -210,14 +213,19 @@
                 plotting_backend=backend,
                 path=materials_file.name,
                 include_total=include_total,
                 show_top=show_top,
                 material_index=material_index
                 # threshold=threshold # looks like there is a bug with threshold
             )
+        else:
+            raise ValueError(
+                'activity_or_atoms must be either "activity" or "number of atoms" to plot'
+            )
+
 
         if backend == "matplotlib":
             st.pyplot(plot)
         else:
             # remove log line selector
             plot.layout["updatemenus"] = []
             st.plotly_chart(plot)
```

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/integrators.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/integrators.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/materials.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/materials.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/results.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 from .utils import get_nuclide_atom_densities_from_materials
 from .utils import find_most_abundant_nuclides_in_materials
 from .utils import find_total_nuclides_in_materials
 import plotly.graph_objects as go
 import numpy as np
 import matplotlib.pyplot as plt
 
+lots_of_nuclides = []
+elements = list(openmc.data.ATOMIC_SYMBOL.values())
+for el in elements:
+    for atomic_num in range(1, 1000):
+        lots_of_nuclides.append(f'{el}{atomic_num}')
+
 
 def plot_activity_vs_time(
     self,
     excluded_material=None,
     time_units="d",
     show_top=None,
     x_scale="linear",
@@ -33,15 +39,15 @@
     path="materials.xml",
 ):
 
     time_steps = self.get_times(time_units=time_units)
 
     all_materials = []
     for counter, step in enumerate(time_steps):
-        materials = self.export_to_materials(burnup_index=counter, path=path)[
+        materials = self.export_to_materials(nuc_with_data=lots_of_nuclides,burnup_index=counter, path=path)[
             material_index
         ]
         all_materials.append(materials)
 
     most_active = find_most_active_nuclides_in_materials(
         materials=all_materials, exclude=excluded_material, units=units
     )
@@ -66,15 +72,17 @@
             x_scale=x_scale,
             y_scale=y_scale,
         )
 
         if threshold:
             total = (
                 find_total_activity_in_materials(
-                    materials=all_materials, units=units, exclude=excluded_material
+                    materials=all_materials,
+                    units=units,
+                    exclude=excluded_material
                 ),
             )
             figure.update_layout(yaxis_range=[threshold, max(total)])
         add_scale_buttons(figure, x_scale, y_scale)
 
     elif plotting_backend == "matplotlib":
         plt.cla
@@ -119,15 +127,14 @@
         else:
 
             y=find_total_activity_in_materials(
                 materials=all_materials, units=units, exclude=excluded_material
             )
             plt.plot(time_steps, y, 'k--', label='total')
 
-
     for name, value in horizontal_lines:
         if plotting_backend == "plotly":
             figure.add_trace(
                 go.Scatter(
                     mode="lines",
                     x=[time_steps[0], time_steps[-1]],
                     y=[value, value],
@@ -160,15 +167,15 @@
     path="materials.xml",
 ):
 
     time_steps = self.get_times(time_units=time_units)
 
     all_materials = []
     for counter, step in enumerate(time_steps):
-        materials = self.export_to_materials(burnup_index=counter, path=path)[
+        materials = self.export_to_materials(nuc_with_data=lots_of_nuclides,burnup_index=counter, path=path)[
             material_index
         ]
         all_materials.append(materials)
 
     most_abundant = find_most_abundant_nuclides_in_materials(
         materials=all_materials, exclude=excluded_material
     )
```

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter/utils.py` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter/utils.py`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/PKG-INFO` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc-depletion-plotter
-Version: 0.3.1
+Version: 0.3.2
 Summary: Plot the isotopes present during depletion steps.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_depletion_plotter-0.3.1/src/openmc_depletion_plotter.egg-info/SOURCES.txt` & `openmc_depletion_plotter-0.3.2/src/openmc_depletion_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmc_depletion_plotter-0.3.1/tests/test_python_api.py` & `openmc_depletion_plotter-0.3.2/tests/test_python_api.py`

 * *Files identical despite different names*

