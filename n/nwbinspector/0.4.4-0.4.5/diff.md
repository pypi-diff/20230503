# Comparing `tmp/nwbinspector-0.4.4.tar.gz` & `tmp/nwbinspector-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwbinspector-0.4.4.tar", last modified: Thu May  5 13:56:22 2022, max compression
+gzip compressed data, was "dist/nwbinspector-0.4.5.tar", last modified: Wed May 11 15:10:09 2022, max compression
```

## Comparing `nwbinspector-0.4.4.tar` & `nwbinspector-0.4.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector/checks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/general.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/image_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/nwb_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6690 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/nwbfile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/ogen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/ophys.py
--rw-r--r--   0 runner    (1001) docker     (121)     8288 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/checks/time_series.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    13558 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/inspector_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector/internal_configs/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/internal_configs/dandi.inspector_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    21874 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/nwbinspector.py
--rw-r--r--   0 runner    (1001) docker     (121)     7485 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/register_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/nwbinspector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/nwbinspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/test_check_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    24264 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (121)     7034 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/test_register_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     8217 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/true_nwbinspector_default_report.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 13:56:22.000000 nwbinspector-0.4.4/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_image_series.py
--rw-r--r--   0 runner    (1001) docker     (121)    12611 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_nwbfile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (121)    12951 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-05-05 13:56:11.000000 nwbinspector-0.4.4/tests/unit_tests/test_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector/
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/image_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/nwb_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6690 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/nwbfile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8288 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/checks/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)    13558 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/inspector_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector/internal_configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/internal_configs/dandi.inspector_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    21874 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/nwbinspector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7485 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/register_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/nwbinspector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/nwbinspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/test_check_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24264 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7034 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/test_register_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8217 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/true_nwbinspector_default_report.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 15:10:09.000000 nwbinspector-0.4.5/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_image_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12611 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_nwbfile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12951 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-05-11 15:10:03.000000 nwbinspector-0.4.5/tests/unit_tests/test_time_series.py
```

### Comparing `nwbinspector-0.4.4/PKG-INFO` & `nwbinspector-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwbinspector
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tool to inspect NWB files for best practices compliance.
 Home-page: https://github.com/NeurodataWithoutBorders/nwbinspector
 Author: Ryan Ly, Ben Dichter, and Cody Baker.
 Author-email: rly@lbl.gov, ben.dichter@gmail.com, cody.baker@catalystneuro.com
 License: BSD-3-Clause
 Description: <img src="docs/logo/logo.png" width="300">
```

### Comparing `nwbinspector-0.4.4/README.md` & `nwbinspector-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/license.txt` & `nwbinspector-0.4.5/license.txt`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/behavior.py` & `nwbinspector-0.4.5/nwbinspector/checks/behavior.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Check if a SpatialSeries has the correct dimensions."""
     if len(spatial_series.data.shape) > 1 and spatial_series.data.shape[1] > 3:
         return InspectorMessage(
             message="SpatialSeries should have 1 column (x), 2 columns (x, y), or 3 columns (x, y, z)."
         )
 
 
-@register_check(importance=Importance.BEST_PRACTICE_VIOLATION, neurodata_type=SpatialSeries)
+@register_check(importance=Importance.BEST_PRACTICE_VIOLATION, neurodata_type=CompassDirection)
 def check_compass_direction_unit(compass_direction: CompassDirection):
     for spatial_series in compass_direction.spatial_series.values():
         if spatial_series.unit not in ("degrees", "radians"):
             yield InspectorMessage(
                 message=f"SpatialSeries objects inside a CompassDirection object should be angular and should have a "
                 f"unit of 'degrees' or 'radians', but '{spatial_series.name}' has units '{spatial_series.unit}'."
             )
```

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/ecephys.py` & `nwbinspector-0.4.5/nwbinspector/checks/ecephys.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/general.py` & `nwbinspector-0.4.5/nwbinspector/checks/general.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/image_series.py` & `nwbinspector-0.4.5/nwbinspector/checks/image_series.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/nwb_containers.py` & `nwbinspector-0.4.5/nwbinspector/checks/nwb_containers.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/nwbfile_metadata.py` & `nwbinspector-0.4.5/nwbinspector/checks/nwbfile_metadata.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/ogen.py` & `nwbinspector-0.4.5/nwbinspector/checks/ogen.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/ophys.py` & `nwbinspector-0.4.5/nwbinspector/checks/ophys.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/tables.py` & `nwbinspector-0.4.5/nwbinspector/checks/tables.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/checks/time_series.py` & `nwbinspector-0.4.5/nwbinspector/checks/time_series.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/config.schema.json` & `nwbinspector-0.4.5/nwbinspector/config.schema.json`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/inspector_tools.py` & `nwbinspector-0.4.5/nwbinspector/inspector_tools.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/internal_configs/dandi.inspector_config.yaml` & `nwbinspector-0.4.5/nwbinspector/internal_configs/dandi.inspector_config.yaml`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/nwbinspector.py` & `nwbinspector-0.4.5/nwbinspector/nwbinspector.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/register_checks.py` & `nwbinspector-0.4.5/nwbinspector/register_checks.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/tools.py` & `nwbinspector-0.4.5/nwbinspector/tools.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector/utils.py` & `nwbinspector-0.4.5/nwbinspector/utils.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/nwbinspector.egg-info/PKG-INFO` & `nwbinspector-0.4.5/nwbinspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwbinspector
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tool to inspect NWB files for best practices compliance.
 Home-page: https://github.com/NeurodataWithoutBorders/nwbinspector
 Author: Ryan Ly, Ben Dichter, and Cody Baker.
 Author-email: rly@lbl.gov, ben.dichter@gmail.com, cody.baker@catalystneuro.com
 License: BSD-3-Clause
 Description: <img src="docs/logo/logo.png" width="300">
```

### Comparing `nwbinspector-0.4.4/nwbinspector.egg-info/SOURCES.txt` & `nwbinspector-0.4.5/nwbinspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/setup.py` & `nwbinspector-0.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Get the long description from the README file
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="nwbinspector",
-    version="0.4.4",
+    version="0.4.5",
     description="Tool to inspect NWB files for best practices compliance.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ryan Ly, Ben Dichter, and Cody Baker.",
     author_email="rly@lbl.gov, ben.dichter@gmail.com, cody.baker@catalystneuro.com",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `nwbinspector-0.4.4/tests/test_check_configuration.py` & `nwbinspector-0.4.5/tests/test_check_configuration.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/test_inspector.py` & `nwbinspector-0.4.5/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/test_register_check.py` & `nwbinspector-0.4.5/tests/test_register_check.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/test_tools.py` & `nwbinspector-0.4.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/test_utils.py` & `nwbinspector-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/true_nwbinspector_default_report.txt` & `nwbinspector-0.4.5/tests/true_nwbinspector_default_report.txt`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_behavior.py` & `nwbinspector-0.4.5/tests/unit_tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_containers.py` & `nwbinspector-0.4.5/tests/unit_tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_ecephys.py` & `nwbinspector-0.4.5/tests/unit_tests/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_general.py` & `nwbinspector-0.4.5/tests/unit_tests/test_general.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_image_series.py` & `nwbinspector-0.4.5/tests/unit_tests/test_image_series.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_nwbfile_metadata.py` & `nwbinspector-0.4.5/tests/unit_tests/test_nwbfile_metadata.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_ogen.py` & `nwbinspector-0.4.5/tests/unit_tests/test_ogen.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_ophys.py` & `nwbinspector-0.4.5/tests/unit_tests/test_ophys.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_tables.py` & `nwbinspector-0.4.5/tests/unit_tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `nwbinspector-0.4.4/tests/unit_tests/test_time_series.py` & `nwbinspector-0.4.5/tests/unit_tests/test_time_series.py`

 * *Files identical despite different names*

