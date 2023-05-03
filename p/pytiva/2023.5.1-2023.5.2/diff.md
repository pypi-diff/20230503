# Comparing `tmp/pytiva-2023.5.1.tar.gz` & `tmp/pytiva-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiva-2023.5.1.tar", last modified: Wed May  3 15:46:07 2023, max compression
+gzip compressed data, was "pytiva-2023.5.2.tar", last modified: Wed May  3 18:45:52 2023, max compression
```

## Comparing `pytiva-2023.5.1.tar` & `pytiva-2023.5.2.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.244635 pytiva-2023.5.1/
--rw-rw-r--   0 tj        (1000) tj        (1000)    35149 2022-11-20 20:53:47.000000 pytiva-2023.5.1/LICENSE
--rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 15:46:07.244635 pytiva-2023.5.1/PKG-INFO
--rw-rw-r--   0 tj        (1000) tj        (1000)      292 2023-04-30 15:42:01.000000 pytiva-2023.5.1/README.md
--rw-rw-r--   0 tj        (1000) tj        (1000)      700 2023-05-03 15:37:50.000000 pytiva-2023.5.1/pyproject.toml
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.236635 pytiva-2023.5.1/pytiva/
--rw-rw-r--   0 tj        (1000) tj        (1000)      148 2023-04-21 18:01:43.000000 pytiva-2023.5.1/pytiva/__init__.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.236635 pytiva-2023.5.1/pytiva/activity/
--rw-rw-r--   0 tj        (1000) tj        (1000)    11122 2023-04-21 19:12:18.000000 pytiva-2023.5.1/pytiva/activity/ActivityDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      102 2022-11-11 19:52:47.000000 pytiva-2023.5.1/pytiva/activity/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1801 2023-04-08 15:20:20.000000 pytiva-2023.5.1/pytiva/activity/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/anesthesia/
--rw-rw-r--   0 tj        (1000) tj        (1000)     3045 2023-04-24 20:11:34.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1988 2023-03-29 01:52:22.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4555 2023-02-14 16:40:11.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      370 2023-04-01 21:59:08.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseStaffingDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      882 2023-04-01 22:53:53.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)    13292 2023-04-24 20:09:40.000000 pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaStudy.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2816 2023-04-30 15:32:20.000000 pytiva-2023.5.1/pytiva/anesthesia/EventActivityDefinition.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      465 2023-02-14 22:04:16.000000 pytiva-2023.5.1/pytiva/anesthesia/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1571 2023-02-05 18:43:13.000000 pytiva-2023.5.1/pytiva/anesthesia/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/dataset/
--rw-rw-r--   0 tj        (1000) tj        (1000)     5720 2023-04-30 15:37:19.000000 pytiva-2023.5.1/pytiva/dataset/DataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      950 2023-04-09 22:37:45.000000 pytiva-2023.5.1/pytiva/dataset/TimeSeriesDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)       78 2023-04-08 14:19:31.000000 pytiva-2023.5.1/pytiva/dataset/__init__.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/pytiva.egg-info/
--rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 15:46:07.000000 pytiva-2023.5.1/pytiva/pytiva.egg-info/PKG-INFO
--rw-rw-r--   0 tj        (1000) tj        (1000)     1363 2023-05-03 15:46:07.000000 pytiva-2023.5.1/pytiva/pytiva.egg-info/SOURCES.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)        1 2023-05-03 15:46:07.000000 pytiva-2023.5.1/pytiva/pytiva.egg-info/dependency_links.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)       56 2023-05-03 15:46:07.000000 pytiva-2023.5.1/pytiva/pytiva.egg-info/top_level.txt
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/staffing/
--rw-rw-r--   0 tj        (1000) tj        (1000)      273 2023-04-08 15:01:52.000000 pytiva-2023.5.1/pytiva/staffing/CapacityTSDS.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3042 2022-11-04 18:22:16.000000 pytiva-2023.5.1/pytiva/staffing/ProviderShift.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3401 2023-04-09 22:37:51.000000 pytiva-2023.5.1/pytiva/staffing/ResourceAssignmentDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      242 2023-04-01 22:25:45.000000 pytiva-2023.5.1/pytiva/staffing/StaffingDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      293 2023-04-08 15:02:09.000000 pytiva-2023.5.1/pytiva/staffing/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4987 2023-04-07 21:12:34.000000 pytiva-2023.5.1/pytiva/staffing/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/utils/
--rw-rw-r--   0 tj        (1000) tj        (1000)       21 2023-02-01 23:16:37.000000 pytiva-2023.5.1/pytiva/utils/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4094 2023-03-28 16:03:27.000000 pytiva-2023.5.1/pytiva/utils/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.240635 pytiva-2023.5.1/pytiva/viz/
--rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-04-21 19:08:41.000000 pytiva-2023.5.1/pytiva/viz/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2536 2023-04-23 00:26:25.000000 pytiva-2023.5.1/pytiva/viz/gantt.py
--rw-rw-r--   0 tj        (1000) tj        (1000)       38 2023-05-03 15:46:07.244635 pytiva-2023.5.1/setup.cfg
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 15:46:07.244635 pytiva-2023.5.1/tests/
--rw-rw-r--   0 tj        (1000) tj        (1000)     1342 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_ProviderShift.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3293 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_ResourceAssignmentDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      963 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_activity.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1676 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_activity_unduplication_with_meds.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      982 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_anesthesia.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1371 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_anesthesia_case_events_dataset.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1849 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_anesthesia_study.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2590 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_dataset.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3532 2023-05-03 15:27:47.000000 pytiva-2023.5.1/tests/test_gantt.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      192 2023-04-09 20:16:13.000000 pytiva-2023.5.1/tests/test_staffing.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3983 2023-04-23 01:25:52.000000 pytiva-2023.5.1/tests/testconfig.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.270932 pytiva-2023.5.2/
+-rw-rw-r--   0 tj        (1000) tj        (1000)    35149 2022-11-20 20:53:47.000000 pytiva-2023.5.2/LICENSE
+-rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 18:45:52.270932 pytiva-2023.5.2/PKG-INFO
+-rw-rw-r--   0 tj        (1000) tj        (1000)      292 2023-04-30 15:42:01.000000 pytiva-2023.5.2/README.md
+-rw-rw-r--   0 tj        (1000) tj        (1000)      801 2023-05-03 18:43:34.000000 pytiva-2023.5.2/pyproject.toml
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.210932 pytiva-2023.5.2/pytiva/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      148 2023-04-21 18:01:43.000000 pytiva-2023.5.2/pytiva/__init__.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.214932 pytiva-2023.5.2/pytiva/activity/
+-rw-rw-r--   0 tj        (1000) tj        (1000)    11122 2023-04-21 19:12:18.000000 pytiva-2023.5.2/pytiva/activity/ActivityDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      102 2022-11-11 19:52:47.000000 pytiva-2023.5.2/pytiva/activity/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1801 2023-04-08 15:20:20.000000 pytiva-2023.5.2/pytiva/activity/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.222932 pytiva-2023.5.2/pytiva/anesthesia/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3045 2023-04-24 20:11:34.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1988 2023-03-29 01:52:22.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4555 2023-02-14 16:40:11.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      370 2023-04-01 21:59:08.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseStaffingDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      882 2023-04-01 22:53:53.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)    13292 2023-04-24 20:09:40.000000 pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaStudy.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2816 2023-04-30 15:32:20.000000 pytiva-2023.5.2/pytiva/anesthesia/EventActivityDefinition.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      465 2023-02-14 22:04:16.000000 pytiva-2023.5.2/pytiva/anesthesia/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1571 2023-02-05 18:43:13.000000 pytiva-2023.5.2/pytiva/anesthesia/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.226932 pytiva-2023.5.2/pytiva/dataset/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     5720 2023-04-30 15:37:19.000000 pytiva-2023.5.2/pytiva/dataset/DataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      950 2023-04-09 22:37:45.000000 pytiva-2023.5.2/pytiva/dataset/TimeSeriesDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)       78 2023-04-08 14:19:31.000000 pytiva-2023.5.2/pytiva/dataset/__init__.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.238932 pytiva-2023.5.2/pytiva/pytiva.egg-info/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 18:45:52.000000 pytiva-2023.5.2/pytiva/pytiva.egg-info/PKG-INFO
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1416 2023-05-03 18:45:52.000000 pytiva-2023.5.2/pytiva/pytiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)        1 2023-05-03 18:45:52.000000 pytiva-2023.5.2/pytiva/pytiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-05-03 18:45:52.000000 pytiva-2023.5.2/pytiva/pytiva.egg-info/requires.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)       47 2023-05-03 18:45:52.000000 pytiva-2023.5.2/pytiva/pytiva.egg-info/top_level.txt
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.250932 pytiva-2023.5.2/pytiva/staffing/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      273 2023-04-08 15:01:52.000000 pytiva-2023.5.2/pytiva/staffing/CapacityTSDS.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3042 2022-11-04 18:22:16.000000 pytiva-2023.5.2/pytiva/staffing/ProviderShift.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3401 2023-04-09 22:37:51.000000 pytiva-2023.5.2/pytiva/staffing/ResourceAssignmentDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      242 2023-04-01 22:25:45.000000 pytiva-2023.5.2/pytiva/staffing/StaffingDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      293 2023-04-08 15:02:09.000000 pytiva-2023.5.2/pytiva/staffing/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4987 2023-04-07 21:12:34.000000 pytiva-2023.5.2/pytiva/staffing/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.254932 pytiva-2023.5.2/pytiva/utils/
+-rw-rw-r--   0 tj        (1000) tj        (1000)       21 2023-02-01 23:16:37.000000 pytiva-2023.5.2/pytiva/utils/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4094 2023-03-28 16:03:27.000000 pytiva-2023.5.2/pytiva/utils/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.254932 pytiva-2023.5.2/pytiva/viz/
+-rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-04-21 19:08:41.000000 pytiva-2023.5.2/pytiva/viz/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2536 2023-04-23 00:26:25.000000 pytiva-2023.5.2/pytiva/viz/gantt.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-05-03 18:43:10.000000 pytiva-2023.5.2/requirements.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)       38 2023-05-03 18:45:52.270932 pytiva-2023.5.2/setup.cfg
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 18:45:52.266932 pytiva-2023.5.2/tests/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1342 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_ProviderShift.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3293 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_ResourceAssignmentDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      963 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_activity.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1676 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_activity_unduplication_with_meds.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      982 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_anesthesia.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1371 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_anesthesia_case_events_dataset.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1849 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_anesthesia_study.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2590 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_dataset.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3532 2023-05-03 15:27:47.000000 pytiva-2023.5.2/tests/test_gantt.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      192 2023-04-09 20:16:13.000000 pytiva-2023.5.2/tests/test_staffing.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3983 2023-04-23 01:25:52.000000 pytiva-2023.5.2/tests/testconfig.py
```

### Comparing `pytiva-2023.5.1/LICENSE` & `pytiva-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/PKG-INFO` & `pytiva-2023.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiva
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Python Tools for Investigation and Visualziing Activity within anesthesia records
 Author-email: TJ Biel <tjbiel85@gmail.com>
 Project-URL: Homepage, https://github.com/tjbiel85/pytiva
 Project-URL: Bug Tracker, https://github.com/tjbiel85/pytiva/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pytiva-2023.5.1/pyproject.toml` & `pytiva-2023.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytiva"
-version = "2023.5.1"
+version = "2023.5.2"
 authors = [
     { name="TJ Biel", email="tjbiel85@gmail.com" },
 ]
 description = "Python Tools for Investigation and Visualziing Activity within anesthesia records"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
+dynamic = ["dependencies"]
 
-[tool.setuptools]
-package-dir = { "" = "pytiva"}
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
+[tool.setuptools.packages.find]
+where = ["pytiva"]
 
 [project.urls]
 "Homepage" = "https://github.com/tjbiel85/pytiva"
 "Bug Tracker" = "https://github.com/tjbiel85/pytiva/issues"
```

### Comparing `pytiva-2023.5.1/pytiva/activity/ActivityDataSet.py` & `pytiva-2023.5.2/pytiva/activity/ActivityDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/activity/utils.py` & `pytiva-2023.5.2/pytiva/activity/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseDataSet.py` & `pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py` & `pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py` & `pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaDataSet.py` & `pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/AnesthesiaStudy.py` & `pytiva-2023.5.2/pytiva/anesthesia/AnesthesiaStudy.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/EventActivityDefinition.py` & `pytiva-2023.5.2/pytiva/anesthesia/EventActivityDefinition.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/anesthesia/utils.py` & `pytiva-2023.5.2/pytiva/anesthesia/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/dataset/DataSet.py` & `pytiva-2023.5.2/pytiva/dataset/DataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/dataset/TimeSeriesDataSet.py` & `pytiva-2023.5.2/pytiva/dataset/TimeSeriesDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/pytiva.egg-info/PKG-INFO` & `pytiva-2023.5.2/pytiva/pytiva.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiva
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Python Tools for Investigation and Visualziing Activity within anesthesia records
 Author-email: TJ Biel <tjbiel85@gmail.com>
 Project-URL: Homepage, https://github.com/tjbiel85/pytiva
 Project-URL: Bug Tracker, https://github.com/tjbiel85/pytiva/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pytiva-2023.5.1/pytiva/pytiva.egg-info/SOURCES.txt` & `pytiva-2023.5.2/pytiva/pytiva.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 pytiva/__init__.py
 pytiva/activity/ActivityDataSet.py
 pytiva/activity/__init__.py
 pytiva/activity/utils.py
 pytiva/anesthesia/AnesthesiaCaseDataSet.py
 pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py
 pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py
@@ -16,14 +17,15 @@
 pytiva/anesthesia/utils.py
 pytiva/dataset/DataSet.py
 pytiva/dataset/TimeSeriesDataSet.py
 pytiva/dataset/__init__.py
 pytiva/pytiva.egg-info/PKG-INFO
 pytiva/pytiva.egg-info/SOURCES.txt
 pytiva/pytiva.egg-info/dependency_links.txt
+pytiva/pytiva.egg-info/requires.txt
 pytiva/pytiva.egg-info/top_level.txt
 pytiva/staffing/CapacityTSDS.py
 pytiva/staffing/ProviderShift.py
 pytiva/staffing/ResourceAssignmentDataSet.py
 pytiva/staffing/StaffingDataSet.py
 pytiva/staffing/__init__.py
 pytiva/staffing/utils.py
```

### Comparing `pytiva-2023.5.1/pytiva/staffing/ProviderShift.py` & `pytiva-2023.5.2/pytiva/staffing/ProviderShift.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/staffing/ResourceAssignmentDataSet.py` & `pytiva-2023.5.2/pytiva/staffing/ResourceAssignmentDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/staffing/utils.py` & `pytiva-2023.5.2/pytiva/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/utils/utils.py` & `pytiva-2023.5.2/pytiva/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/pytiva/viz/gantt.py` & `pytiva-2023.5.2/pytiva/viz/gantt.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_ProviderShift.py` & `pytiva-2023.5.2/tests/test_ProviderShift.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_ResourceAssignmentDataSet.py` & `pytiva-2023.5.2/tests/test_ResourceAssignmentDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_activity.py` & `pytiva-2023.5.2/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_activity_unduplication_with_meds.py` & `pytiva-2023.5.2/tests/test_activity_unduplication_with_meds.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_anesthesia.py` & `pytiva-2023.5.2/tests/test_anesthesia.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_anesthesia_case_events_dataset.py` & `pytiva-2023.5.2/tests/test_anesthesia_case_events_dataset.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_anesthesia_study.py` & `pytiva-2023.5.2/tests/test_anesthesia_study.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_dataset.py` & `pytiva-2023.5.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/test_gantt.py` & `pytiva-2023.5.2/tests/test_gantt.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.1/tests/testconfig.py` & `pytiva-2023.5.2/tests/testconfig.py`

 * *Files identical despite different names*

