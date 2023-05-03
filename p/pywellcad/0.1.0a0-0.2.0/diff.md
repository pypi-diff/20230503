# Comparing `tmp/pywellcad-0.1.0a0.tar.gz` & `tmp/pywellcad-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Projects\pywellcad\dist\tmpqcmu6usa\pywellcad-0.1.0a0.tar", last modified: Thu Feb 10 11:41:05 2022, max compression
+gzip compressed data, was "C:\Projects\pywellcad\dist\.tmp-bs586v8y\pywellcad-0.2.0.tar", last modified: Wed May  3 13:47:18 2023, max compression
```

## Comparing `pywellcad-0.1.0a0.tar` & `pywellcad-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-02-10 11:41:05.086284 pywellcad-0.1.0a0/
--rw-rw-rw-   0        0        0       80 2022-02-10 08:00:59.000000 pywellcad-0.1.0a0/.gitignore
--rw-rw-rw-   0        0        0     1565 2021-11-24 11:08:07.000000 pywellcad-0.1.0a0/LICENSE.txt
--rw-rw-rw-   0        0        0       49 2022-01-17 15:04:12.000000 pywellcad-0.1.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     2770 2022-02-10 11:41:05.087303 pywellcad-0.1.0a0/PKG-INFO
--rw-rw-rw-   0        0        0     2309 2022-02-10 09:02:07.000000 pywellcad-0.1.0a0/README.md
--rw-rw-rw-   0        0        0      149 2021-11-24 11:08:07.000000 pywellcad-0.1.0a0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-02-10 11:41:05.000230 pywellcad-0.1.0a0/pywellcad.egg-info/
--rw-rw-rw-   0        0        0     2770 2022-02-10 11:41:03.000000 pywellcad-0.1.0a0/pywellcad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2022-02-10 11:41:04.000000 pywellcad-0.1.0a0/pywellcad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-10 11:41:03.000000 pywellcad-0.1.0a0/pywellcad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-01 07:44:06.000000 pywellcad-0.1.0a0/pywellcad.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2022-02-10 11:41:03.000000 pywellcad-0.1.0a0/pywellcad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-02-10 11:41:03.000000 pywellcad-0.1.0a0/pywellcad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      579 2022-02-10 11:41:05.089420 pywellcad-0.1.0a0/setup.cfg
--rw-rw-rw-   0        0        0       37 2021-11-24 11:08:07.000000 pywellcad-0.1.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-10 11:41:05.003220 pywellcad-0.1.0a0/wellcad/
--rw-rw-rw-   0        0        0       17 2022-01-17 15:04:13.000000 pywellcad-0.1.0a0/wellcad/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-10 11:41:05.084297 pywellcad-0.1.0a0/wellcad/com/
--rw-rw-rw-   0        0        0      816 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/__init__.py
--rw-rw-rw-   0        0        0     8895 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_application.py
--rw-rw-rw-   0        0        0   155867 2022-02-10 11:14:21.000000 pywellcad-0.1.0a0/wellcad/com/_borehole.py
--rw-rw-rw-   0        0        0      622 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_comment_box.py
--rw-rw-rw-   0        0        0      870 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_cross_section_box.py
--rw-rw-rw-   0        0        0     4388 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_depth.py
--rw-rw-rw-   0        0        0     2445 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_dispatch_wrapper.py
--rw-rw-rw-   0        0        0     1689 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_drill_item.py
--rw-rw-rw-   0        0        0     5092 2022-02-10 11:14:21.000000 pywellcad-0.1.0a0/wellcad/com/_equipment_item.py
--rw-rw-rw-   0        0        0     2825 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_font.py
--rw-rw-rw-   0        0        0     1695 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_fossil_item.py
--rw-rw-rw-   0        0        0   115540 2022-02-01 13:39:56.000000 pywellcad-0.1.0a0/wellcad/com/_genpy_dump.py
--rw-rw-rw-   0        0        0     3678 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_header.py
--rw-rw-rw-   0        0        0     1056 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_interval_item.py
--rw-rw-rw-   0        0        0     1903 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_litho_bed.py
--rw-rw-rw-   0        0        0     1605 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_litho_dictionary.py
--rw-rw-rw-   0        0        0     1298 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_litho_pattern.py
--rw-rw-rw-   0        0        0    76749 2022-02-10 11:14:21.000000 pywellcad-0.1.0a0/wellcad/com/_log.py
--rw-rw-rw-   0        0        0     1233 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_marker_item.py
--rw-rw-rw-   0        0        0      891 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_odbc.py
--rw-rw-rw-   0        0        0     5280 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_page.py
--rw-rw-rw-   0        0        0     1229 2022-01-19 13:44:07.000000 pywellcad-0.1.0a0/wellcad/com/_polar_and_rose_box.py
--rw-rw-rw-   0        0        0     1618 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_stacking_pattern_item.py
--rw-rw-rw-   0        0        0    11640 2022-02-10 11:14:21.000000 pywellcad-0.1.0a0/wellcad/com/_structure.py
--rw-rw-rw-   0        0        0    13377 2022-02-10 08:01:00.000000 pywellcad-0.1.0a0/wellcad/com/_title.py
--rw-rw-rw-   0        0        0    11891 2022-02-10 11:14:21.000000 pywellcad-0.1.0a0/wellcad/com/_workspace.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.916174 pywellcad-0.2.0/
+-rw-rw-rw-   0        0        0      217 2023-05-03 13:38:48.000000 pywellcad-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1565 2021-11-24 11:08:07.000000 pywellcad-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       49 2022-01-17 15:04:12.000000 pywellcad-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2751 2023-05-03 13:47:18.918174 pywellcad-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2023-04-18 06:11:17.000000 pywellcad-0.2.0/README.md
+-rw-rw-rw-   0        0        0      149 2021-11-24 11:08:07.000000 pywellcad-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.648294 pywellcad-0.2.0/pywellcad.egg-info/
+-rw-rw-rw-   0        0        0     2751 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-05-03 13:47:18.000000 pywellcad-0.2.0/pywellcad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-10-01 07:44:06.000000 pywellcad-0.2.0/pywellcad.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      579 2023-05-03 13:47:18.929174 pywellcad-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2021-11-24 11:08:07.000000 pywellcad-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.654069 pywellcad-0.2.0/wellcad/
+-rw-rw-rw-   0        0        0       17 2023-03-20 09:55:35.000000 pywellcad-0.2.0/wellcad/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.910194 pywellcad-0.2.0/wellcad/com/
+-rw-rw-rw-   0        0        0      816 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/__init__.py
+-rw-rw-rw-   0        0        0     8895 2023-05-03 12:03:11.000000 pywellcad-0.2.0/wellcad/com/_application.py
+-rw-rw-rw-   0        0        0   170263 2023-05-03 13:38:49.000000 pywellcad-0.2.0/wellcad/com/_borehole.py
+-rw-rw-rw-   0        0        0      622 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_comment_box.py
+-rw-rw-rw-   0        0        0      870 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_cross_section_box.py
+-rw-rw-rw-   0        0        0     4388 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_depth.py
+-rw-rw-rw-   0        0        0     2445 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_dispatch_wrapper.py
+-rw-rw-rw-   0        0        0     1689 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_drill_item.py
+-rw-rw-rw-   0        0        0     5092 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_equipment_item.py
+-rw-rw-rw-   0        0        0     2825 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_font.py
+-rw-rw-rw-   0        0        0     1695 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_fossil_item.py
+-rw-rw-rw-   0        0        0     3678 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_header.py
+-rw-rw-rw-   0        0        0     1056 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_interval_item.py
+-rw-rw-rw-   0        0        0     1903 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_litho_bed.py
+-rw-rw-rw-   0        0        0     1605 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_litho_dictionary.py
+-rw-rw-rw-   0        0        0     1298 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_litho_pattern.py
+-rw-rw-rw-   0        0        0    77009 2023-05-03 12:03:11.000000 pywellcad-0.2.0/wellcad/com/_log.py
+-rw-rw-rw-   0        0        0     1233 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_marker_item.py
+-rw-rw-rw-   0        0        0      891 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_odbc.py
+-rw-rw-rw-   0        0        0     5280 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_page.py
+-rw-rw-rw-   0        0        0     1229 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_polar_and_rose_box.py
+-rw-rw-rw-   0        0        0     1618 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_stacking_pattern_item.py
+-rw-rw-rw-   0        0        0    11640 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_structure.py
+-rw-rw-rw-   0        0        0    13377 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_title.py
+-rw-rw-rw-   0        0        0    12431 2023-05-03 13:38:49.000000 pywellcad-0.2.0/wellcad/com/_workspace.py
```

### Comparing `pywellcad-0.1.0a0/LICENSE.txt` & `pywellcad-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/PKG-INFO` & `pywellcad-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.1.0a0
+Version: 0.2.0
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pywellcad
@@ -42,23 +41,22 @@
 
 ```python
 import wellcad.com
 
 app = wellcad.com.Application()
 sample_file_path = r"C:\Program Files\Advanced Logic Technology\WellCAD\Samples\Classic Sample.wcl"
 borehole = app.open_borehole(sample_file_path)
-gr_log = borehole.log("GR")
+gr_log = borehole.get_log("GR")
 gr_log.file_export(r"C:\Temp", "sample_gr", "csv")
 ```
 
 A comprehensive set of documentation can be found [here](https://pywellcad.readthedocs.io/).
 
 ## Contributing
 
 If you have problems or suggestions, please feel free to open an issue here on GitHub. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please note, initial development of this library was done using a self-hosted Git platform ([Gitea](https://gitea.io/en-us/)), so you may not have access to older issues/PRs.
 
 ## License
 
 pywellcad is licensed under the [BSD 3-clause](https://choosealicense.com/licenses/bsd-3-clause/) license.
-
```

### Comparing `pywellcad-0.1.0a0/README.md` & `pywellcad-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```python
 import wellcad.com
 
 app = wellcad.com.Application()
 sample_file_path = r"C:\Program Files\Advanced Logic Technology\WellCAD\Samples\Classic Sample.wcl"
 borehole = app.open_borehole(sample_file_path)
-gr_log = borehole.log("GR")
+gr_log = borehole.get_log("GR")
 gr_log.file_export(r"C:\Temp", "sample_gr", "csv")
 ```
 
 A comprehensive set of documentation can be found [here](https://pywellcad.readthedocs.io/).
 
 ## Contributing
```

### Comparing `pywellcad-0.1.0a0/pywellcad.egg-info/PKG-INFO` & `pywellcad-0.2.0/pywellcad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.1.0a0
+Version: 0.2.0
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # pywellcad
@@ -42,23 +41,22 @@
 
 ```python
 import wellcad.com
 
 app = wellcad.com.Application()
 sample_file_path = r"C:\Program Files\Advanced Logic Technology\WellCAD\Samples\Classic Sample.wcl"
 borehole = app.open_borehole(sample_file_path)
-gr_log = borehole.log("GR")
+gr_log = borehole.get_log("GR")
 gr_log.file_export(r"C:\Temp", "sample_gr", "csv")
 ```
 
 A comprehensive set of documentation can be found [here](https://pywellcad.readthedocs.io/).
 
 ## Contributing
 
 If you have problems or suggestions, please feel free to open an issue here on GitHub. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please note, initial development of this library was done using a self-hosted Git platform ([Gitea](https://gitea.io/en-us/)), so you may not have access to older issues/PRs.
 
 ## License
 
 pywellcad is licensed under the [BSD 3-clause](https://choosealicense.com/licenses/bsd-3-clause/) license.
-
```

### Comparing `pywellcad-0.1.0a0/pywellcad.egg-info/SOURCES.txt` & `pywellcad-0.2.0/pywellcad.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 wellcad/com/_cross_section_box.py
 wellcad/com/_depth.py
 wellcad/com/_dispatch_wrapper.py
 wellcad/com/_drill_item.py
 wellcad/com/_equipment_item.py
 wellcad/com/_font.py
 wellcad/com/_fossil_item.py
-wellcad/com/_genpy_dump.py
 wellcad/com/_header.py
 wellcad/com/_interval_item.py
 wellcad/com/_litho_bed.py
 wellcad/com/_litho_dictionary.py
 wellcad/com/_litho_pattern.py
 wellcad/com/_log.py
 wellcad/com/_marker_item.py
```

### Comparing `pywellcad-0.1.0a0/setup.cfg` & `pywellcad-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/__init__.py` & `pywellcad-0.2.0/wellcad/com/__init__.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_application.py` & `pywellcad-0.2.0/wellcad/com/_application.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_borehole.py` & `pywellcad-0.2.0/wellcad/com/_borehole.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
                          "FilterImageLog", "ApplyConditionalTesting", "RQD", "GrainSizeSorting", "StackTraces",
                          "AverageFilterFWSLog", "FreqFilterFwsLog", "ApplyStandOffCorrection",
                          "CompensatedVelocity", "ApplySemblanceProcessing", "ProcessReflectedTubeWave",
                          "PickFirstArrival", "PickE1Arrival", "ExtractE1Amplitude", "AdjustPickToExtremum",
                          "ExtractWindowPeakAmplitude", "ApplyNaturalGammaBoreholeCorrection",
                          "ApplyTotalGammaCalibration", "CorrectDeadSensor", "CalculateFluidVelocity",
                          "CalculateApparentMetalLoss", "GetLog", "CreateNewWorkspace",  "Workspace", "FileExport",
-                         "ConvertLogTo", "FilterLog", "ResampleLog", "InterpolateLog", "ElogCorrection", "NMRFluidVolumes",)
+                         "ConvertLogTo", "FilterLog", "ResampleLog", "InterpolateLog", "ElogCorrection",
+                         "NMRFluidVolumes", "ROPAverage", "SharpenRGBLog", "RetinexFilterRGBLog", )
 
     @property
     def name(self):
         """str: The title of a borehole document."""
         return self._dispatch.Name
 
     @name.setter
@@ -417,15 +418,15 @@
             If not provided, the current top depth of the document will be used.
         bottom_depth : float, optional
             The bottom depth of the printed depth interval.
             If not provided, the current bottom depth of the document will be used.
         nb_of_copies : int, optional
             The number of copies to be printed.
         """
-        self._dispatch.DoPrint(self, enable_dialog, top_depth, bottom_depth, nb_of_copies)
+        self._dispatch.DoPrint(enable_dialog, top_depth, bottom_depth, nb_of_copies)
 
     def read_database(self, script_path):
         """Opens and interprets an SQL script to download data from a database.
 
         Parameters
         ----------
         script_path : str
@@ -727,16 +728,14 @@
         bool
             True if successful, False otherwise.
         """
         return self._dispatch.ApplyTemplate(path, prompt_if_not_found, create_new_logs, create_new_layers,
                                             apply_annotation_settings, replace_header, keep_charts, new_charts,
                                             overwrite_workspaces, new_workspaces, delete_non_associated_logs, config)
 
-    # Common log edition
-
     def slice_log(self, log, slice_depth, create_top=None, create_bottom=None, keep_original=None):
         """Allows the separation of the log data into a top and bottom section. New logs can be created \
         holding the data of the top and bottom parts of the data set.
 
         Parameters
         ----------
         log : str or int
@@ -850,16 +849,14 @@
         user_defined_intervals : bool, optional
             If set to False the intervals will be loaded from a reference log.
         interval_log : str or int, optional
             The title or the zero based index of the log containing the reference intervals.
         """
         self._dispatch.FillLog(log, top_depth, bottom_depth, step, thickness, user_defined_intervals, interval_log)
 
-    # Common log processes
-
     def filter_log(self, log, prompt_user=None, config=None):
         """Calculates a new filtered data set of a Well Log.
 
         Parameters
         ----------
         log : str or int
             The title or the zero based index of the log.
@@ -1006,20 +1003,89 @@
         config : str, optional
             Path to a configuration file or a parameter string. The
             configuration file can contain the following options:
 
             .. code-block:: ini
 
                 [AnalysisLogNormalize]
-                ComponentsToDelete=20,05#1,Artifacts
+                ComponentsToDelete= 20, 05#1, Artifacts (Codes of the patterns to be
+                removed separated by commas)
                 CreateNewLog=yes
-                NormalizeAt100=yes
+                At100=yes
         """
         self._dispatch.Normalize(log, prompt_user, config)
 
+    def tvd(self, log=None, prompt_user=None, config=None):
+        """Calculates a TVD either from another TVD log (Depth Log) or from a tilt log (Well Log).
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [TVD]
+                Output=TVD /Elevation
+                ExtrapolateBack=yes /no
+                TVDAtZero=0.0
+
+        Returns
+        -------
+        Log
+            The newly created Log containing the TVD data.
+        """
+        return Log(self._dispatch.TVD(log, prompt_user, config))
+
+    def rop_average(self, log=None, prompt_user=None, config=None):
+        """Computes the average rate of penetration over specified depth intervals
+        for a Mud Log or a Well Log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ROPAverage]
+                ReferenceInterval=Litho ; log title or constant value indicating the interval height
+                OutputLogAsGraphic=no
+                OutputLogAsText=yes
+                DepthRange=Maximum ;Maximum, UserDefined, Zones, LogZones
+                TopDepth=105
+                BottomDepth=120
+                ;LogZones : top1, bot1, top2, bot2, ... topN, botN
+                LogZones=
+                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                LogZonesDepthRange=Litho,06,05#1
+
+        Returns
+        -------
+        Log
+            The newly created Log.
+        """
+        return Log(self._dispatch.ROPAverage(log, prompt_user, config))
+
     def unit_conversion(self, log=None, prompt_user=None, config=None):
         """Converts the units used in a log.
 
         Units are organized in categories (e.g. Length, Weight or Temperature).
 
         Parameters
         ----------
@@ -1135,14 +1201,42 @@
         Returns
         -------
         Log
             An object of the interpolated log.
         """
         return Log(self._dispatch.InterpolateLog(log, prompt_user, config))
 
+    def auto_joint_detection(self, log, prompt_user=None, config=None):
+        """Detects the joints from the main log (data source) used
+        in the workspace.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                Sensitivity = 5
+                TopAndBottom = yes
+        """
+        self._dispatch.AutoJointDetection(log, prompt_user, config)
+
     def calculate_borehole_deviation(self, prompt_user=None, config=None):
         """Calculates borehole Azimuth, RBR and Tilt from magnetometer and inclinometer / accelerometer data.
 
         Parameters
         ----------
         prompt_user : bool, optional
             Whether dialog boxes are displayed to interact with the user.
@@ -1186,14 +1280,68 @@
             If set to ``False`` the processing parameters will be retrieved from the specified
             configuration.  If no configuration has been specified, default values will be used.
             Default is True.
         config : str, optional
             Path to a configuration file or a parameter string. The
             configuration file can contain the following options:
 
+            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
+
+            .. code-block:: ini
+
+                [VolumeProcess]
+                ; OuterDiam, InnerDiam : name of a well log, img log or a constant value
+                ; OuterDiamUnit, InnerDiamUnit : inch or mm, default to mm
+                ; OuterDiam1, InnerDiam1 : name of a well log, img log or a constant value.
+                ; Use either OuterDiam, InnerDiam or OuterDiam1, InnerDiam1 but not both !
+                ; OuterDiamUnit1, InnerDiamUnit1 : inch or mm, default to mm.
+                ; Use either OuterDiamUnit, InnerDiamUnit or OuterDiamUnit1, InnerDiamUnit1 but not both !
+                ; OuterDiam2, InnerDiam2 : name of a well log
+                ; OuterDiamUnit2, InnerDiamUnit2 : inch or mm, default to mm
+                ; IntervalRef : name of a well log or value (if value, in depth units of the borehole doc)
+                ; DepthRange : Maximum, UserDefined, Zones, LogZones
+                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                OuterDiam=
+                OuterDiamUnit=mm
+                InnerDiam=
+                InnerDiamUnit=mm
+                OuterDiam1=w_diam_ext
+                OuterDiamUnit1=mm
+                OuterDiam2=
+                OuterDiamUnit2=mm
+                OuterDiam3=
+                OuterDiamUnit3=mm
+                OuterDiam4=
+                OuterDiamUni4t=mm
+                InnerDiamUnit=mm
+                InnerDiam1=
+                InnerDiamUnit1=mm
+                OuterDiamAsDiameter=yes
+                InnerDiamAsDiameter=yes
+                AnnularVolume=no
+                BottomToTop=yes
+                VolumeUnit=litre
+                DisplayTick=no
+                SmallTickFreq=1
+                MediumTickFreq=10
+                LargeTickFreq=100
+                DisplayNumerical=no
+                NumericalFreq=10
+                DisplayInterval=no
+                IntervalRef=10
+                DisplayCurve=yes
+                DepthRange=Maximum
+                TopDepth=10
+                BottomDepth=19
+                ZonesDepthRange=
+                LogZonesDepthRange=Litho,06,05#1
+
+
+            For WellCAD version 5.5 and 5.6, use this configuration instead:
+
             .. code-block:: ini
 
                 [VolumeProcess]
                 InnerDiam = 100 / log name
                 InnerDiamUnit = mm/in/cm/ft/yd
                 OuterDiam = 110 / log name
                 OuterDiamUnit = mm/in/cm/ft/yd
@@ -1208,15 +1356,14 @@
                 NumericalFreq = 10
                 DisplayCurve = yes/no
                 DisplayInterval = yes/no
                 IntervalRef = 10
                 MaxDepthRange = yes/no
                 TopDepth = 0.0
                 BottomDepth = 123.5
-
         """
         self._dispatch.CalculateBoreholeVolume(prompt_user, config)
 
     def calculate_borehole_coordinates(self, prompt_user=None, config=None):
         """Calculates the deviation path coordinates Northing, Easting and TVD.
 
         Parameters
@@ -1360,14 +1507,42 @@
         -------
         Log
             The resulting log.
         """
 
         return Log(self._dispatch.StackTraces(is_spectrum, log, prompt_user, config))
 
+    def slice_traces(self, log=None, prompt_user=None, config=None):
+        """Allows the user to keep only a portion of a FWS log's traces. Updates the log in place.
+        
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SliceTraces]
+                start = 0  ; in log units
+                end = 0  ; in log units
+        """
+
+        self._dispatch.SliceTraces(log, prompt_user, config)
+
     def apply_conditional_testing(self, log_if=None, log_then=None, prompt_user=None, config=None):
         """Applies conditional testing (If-Then-Else) to image log
         values.
 
         Parameters
         ----------
         log_if : str or int, optional
@@ -1552,15 +1727,15 @@
                 InclYPositive = yes / no
                 InclZPositive = yes / no
                 IsAccelerometer = yes / no
                 MarkerPosition = 180.2
         """
         self._dispatch.OrientImageToNorth(log, prompt_user, config)
 
-    def extract_image_log_image_statistics(self, log=None, prompt_user=None, config=None):
+    def extract_image_log_statistics(self, log=None, prompt_user=None, config=None):
         """Extracts minimum, maximum, average, median and other
         statistical values fulfilling an optional condition from each
         image log trace.
 
         Parameters
         ----------
         log : str or int, optional
@@ -1930,15 +2105,71 @@
         prompt_user : bool, optional
             Whether dialog boxes are displayed to interact with
             the user. If set to False, the new brightness and
             contrast values will be determined automatically.
         """
         self._dispatch.AdjustImageBrightnessAndContrast(log, prompt_user)
 
-    def extract_structure_interval_statistics(self, log=None, prompt_user=None, config=None):
+    def retinex_filter_rgb_log(self, log=None, prompt_user=None, config=None):
+        """Applies a retinex filter to the RGB log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Not Used for this function.
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+
+        return Log(self._dispatch.RetinexFilterRGBLog(log, prompt_user, config))
+
+    def sharpen_rgb_log(self, log=None, prompt_user=None, config=None):
+        """Sharpens the RGB log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Not Used for this function.
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+
+        return Log(self._dispatch.SharpenRGBLog(log, prompt_user, config))
+
+    def extract_structure_interval_statistic(self, log=None, prompt_user=None, config=None):
         """Allows determination of statistical values (e.g. frequency
         of dips) per interval from a structure log.
 
         Parameters
         ----------
         log : str or int, optional
             Zero based index (integer) or title (string) of
@@ -1975,15 +2206,15 @@
                 OutputAverageLength = yes / no
                 OutputMinOpening = yes / no
                 OutputMaxOpening = yes / no
 
         Returns
         -------
         Log
-            One of the computed log.  #TODO figure out which
+            One of the computed log.
         """
         return Log(self._dispatch.ExtractStructureIntervalStatistic(log, prompt_user, config))
 
     def rqd(self, log=None, prompt_user=None, config=None):
         """Computes the Rock Quality Designation from the structure
         picks in a Structure Log.
 
@@ -2280,17 +2511,51 @@
                 SteelVelocity = VelocityLog / 5200
                 SteelVelocityUnit= m/s
                 CurveOutput = yes / no
                 ImageOutput = yes / no
         """
         self._dispatch.CalculateCasingThickness(log, prompt_user, config)
 
+    def cased_hole_ultrasonics(self, wavelet_log=None, zone_log=None, prompt_user=None, config=None):
+        """Processes ultrasonic waveforms from a wavelet log using the processing parameters from a zone log.
+
+        Parameters
+        ----------
+        wavelet_log : int or str, optional
+            Zero based index or title of the wavelet log to process.
+            If not provided, the process dialog box will be displayed.
+        zone_log : int or str, optional
+            Zero based index or title of the zone log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CasedHoleUltrasonics]
+                ; Thickness : output the thickness as an image log
+                ; Cadi  : output the cadi as an image log
+                ; Score  : output the score as an image log
+                Thickness = yes / no
+                Cadi = yes / no
+                Score = yes / no
+        """
+        self._dispatch.CasedHoleUltrasonics(wavelet_log, zone_log, prompt_user, config)
+
     def calculate_apparent_metal_loss(self, log=None, prompt_user=None, config=None):
         """Calculates an apparent metal loss value for each trace of radius values stored in an image log.
 
+        Note: This function is deprecated in WellCAD 5.7 and onwards. Please use calculate_apparent_metal_loss_ex instead.
+
         Parameters
         ----------
         log : int or str, optional
             Zero based index or title of the log to process.
             If not provided, the process dialog box will be displayed.
         prompt_user : bool, optional
             Whether dialog boxes are displayed to interact with the user.
@@ -2311,14 +2576,59 @@
         Returns
         -------
         Log
             A log giving the metal loss.
         """
         return Log(self._dispatch.CalculateApparentMetalLoss(log, prompt_user, config))
 
+    def calculate_apparent_metal_loss_ex(self, log=None, prompt_user=None, config=None):
+        """Calculates an apparent metal loss value for each trace of radius/thickness values stored in an
+        image log or well log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, either here or in the config, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [MetalLoss]
+                ; ID : name of a well log or img log
+                ; Thickness : name of a well log or img log
+                ; NomOD : name of a well log or value
+                ; NomThickness : name of a well log or value
+                ; NomODUnit, NomThicknessUnit : inch or mm, default to mm
+                ; DepthRange : Maximum, UserDefined, Zones, LogZones
+                ; ZonesDepthRange : top1, bot1, top2, bot2, ... topN, botN
+                ; LogZonesDepthRange = logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                ID=
+                Thickness=
+                NomOD=50
+                NomODUnit=mm
+                NomThickness=10
+                NomThicknessUnit=mm
+                DepthRange=Maximum
+                TopDepth = 10
+                BottomDepth = 19
+                ZonesDepthRange=
+                LogZonesDepthRange = Litho,06,05#1
+        """
+        self._dispatch.CalculateApparentMetalLossEx(log, prompt_user, config)
+
     def radius_to_from_diameter(self, log=None, prompt_user=None, config=None):
         """Converts values data in an Image log from radius to diameter values or vice versa.
 
         Parameters
         ----------
         log : int or str
             Zero based index or title of the log to process.
@@ -3674,16 +3984,14 @@
         -------
         Log
             A Log object of the resulting hydraulic conductivity.
         """
 
         return Log(self._dispatch.HydraulicConductivity(log, prompt_user, config))
 
-    # CoreCAD processes
-
     def extract_grain_size_statistics(self, log=None, prompt_user=None, config=None):
         """Computes statistics from a grain size distribution curve.
 
         Parameters
         ----------
         log : int or str, optional
             Zero based index or title of the log containing the grain size values.
@@ -3747,16 +4055,14 @@
         -------
         Log
             A log containing the sorted values
         """
 
         return Log(self._dispatch.GrainSizeSorting(log_min, log_max, prompt_user, config))
 
-    # Protection options
-
     def enable_protection(self, enable, password):
         """Changes the protection status of a document using a password
 
         Parameters
         ----------
         enable : bool
             Set to True to protect the borehole document.
@@ -3839,8 +4145,51 @@
         enable : bool
             Set to True to allow edition of the document header data.
         password : str
             The password used to allow this option.
         """
 
         self._dispatch.AllowModifyHeadersContent(enable, password)
-        
+
+    def set_metadata(self, id, value):
+        """Sets a metadata value. If the id doesn't exist, this will create it and set the value.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+        value : str
+            The value to set the metadata to.
+        """
+
+        self._dispatch.SetMetadata(id, value)
+
+    def get_metadata(self, id):
+        """Gets the value metadata value.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+
+        Returns
+        -------
+        str
+            The value associated with the metadata.
+        """
+
+        return self._dispatch.GetMetadata(id)
+
+    def delete_metadata(self, id):
+        """Removes a metadata id and value pair.
+        Warning: if this metadata is used within a header, the metadata id will remain valid and it's value will be set to null.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+        """
+
+        self._dispatch.DeleteMetadata(id)
```

### Comparing `pywellcad-0.1.0a0/wellcad/com/_comment_box.py` & `pywellcad-0.2.0/wellcad/com/_comment_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_cross_section_box.py` & `pywellcad-0.2.0/wellcad/com/_cross_section_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_depth.py` & `pywellcad-0.2.0/wellcad/com/_depth.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_dispatch_wrapper.py` & `pywellcad-0.2.0/wellcad/com/_dispatch_wrapper.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_drill_item.py` & `pywellcad-0.2.0/wellcad/com/_drill_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_equipment_item.py` & `pywellcad-0.2.0/wellcad/com/_equipment_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_font.py` & `pywellcad-0.2.0/wellcad/com/_font.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_fossil_item.py` & `pywellcad-0.2.0/wellcad/com/_fossil_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_header.py` & `pywellcad-0.2.0/wellcad/com/_header.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_interval_item.py` & `pywellcad-0.2.0/wellcad/com/_interval_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_litho_bed.py` & `pywellcad-0.2.0/wellcad/com/_litho_bed.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_litho_dictionary.py` & `pywellcad-0.2.0/wellcad/com/_litho_dictionary.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_litho_pattern.py` & `pywellcad-0.2.0/wellcad/com/_litho_pattern.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_log.py` & `pywellcad-0.2.0/wellcad/com/_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         right : float
             The position of the right side of the log column as a fraction of
             the document width.
         """
         self._dispatch.SetPosition(left, right)
 
     @property
-    def type(self):  # TODO: new lineation log should be added to documentation
+    def type(self):
         """int: The log type index.
 
         Log types are one of the below:
 
         * Undefined = 0
         * Well log = 1
         * Formula log = 2
@@ -199,14 +199,15 @@
         * Polar & Rose log = 20
         * Cross log = 21
         * OLE log = 22
         * Shading log = 23
         * Marker log = 24
         * Breakout log = 25
         * Bio log = 26
+        * Lineation log = 27
         """
         return self._dispatch.Type
 
     @property
     def hide_log_title(self):
         """bool: Whether the log title is hidden."""
         return self._dispatch.HideLogTitle
@@ -226,15 +227,15 @@
 
     @property
     def log_background_color(self):
         """int: The background color of the log column.
         
         Colours are specified as a 32 bit integer with an ``xBGR`` structure.
         Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
+        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
         """
         return self._dispatch.LogBackgroundColor
 
     @log_background_color.setter
     def log_background_color(self, value):
         self._dispatch.LogBackgroundColor = value
 
@@ -267,15 +268,15 @@
 
     @property
     def border_color(self):
         """int: The border color of the log column.
         
         Colours are specified as a 32 bit integer with an ``xBGR`` structure.
         Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
+        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
         """
         return self._dispatch.BorderColor
 
     @border_color.setter
     def border_color(self, value):
         self._dispatch.BorderColor = value
 
@@ -533,15 +534,17 @@
         ----------
         index : int
             Zero based index of the data to be retrieved.
         
         Returns
         -------
         float
-            The depth of the log data at the specified index.
+            The depth of the log data at the specified index. If the index is
+            out of bounds, this will be 0.0 for a Mud Log, and an extrapolated
+            value for a Well Log.
         """
         return self._dispatch.DataDepth(index)
 
     def insert_data(self, index, value):
         """Inserts a new data value at the specified index.
 
         If necessary existing data points will be shifted.
@@ -666,15 +669,15 @@
 
     @property
     def pen_color(self):
         """int: The pen color for a Well or Mud log.
         
         Colours are specified as a 32 bit integer with an ``xBGR`` structure.
         Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
+        values.  Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
         """
         return self._dispatch.PenColor
 
     @pen_color.setter
     def pen_color(self, color):
         self._dispatch.PenColor = color
 
@@ -755,14 +758,15 @@
     @property
     def shading(self):
         """int: The shading position used in a Well or Mud Log.
         
         * None = 0
         * Left = 1
         * Right = 2
+        * Full = 3
         """
         return self._dispatch.Shading
 
     @shading.setter
     def shading(self, position):
         self._dispatch.Shading = position
 
@@ -1845,15 +1849,15 @@
         ----------
         depth : float
             The depth of the Polar & Rose box to be removed in
             current depth units.
         """
         self._dispatch.RemoveSchmitBoxAtDepth(depth)
 
-    def cross_box(self, index):  # the example in the Automation module is wrong
+    def cross_box(self, index):
         """Gets a Cross Box object from the Cross Section Log at the specified index.
 
         Parameters
         ----------
         index : int
             Zero based index of the box to be retrieved.
 
@@ -2234,15 +2238,15 @@
         * 4: cross
         * 5: diagonal cross
 
         If an invalid style is set, nothing will happen.
         """
         return self._dispatch.BackgroundHatchStyle
 
-    @background_hatch_style.setter  # code number 4 is missing
+    @background_hatch_style.setter
     def background_hatch_style(self, code):
         self._dispatch.BackgroundHatchStyle = code
 
     @property
     def background_style(self):
         """int: The background style for the Engineering Log.
 
@@ -2298,15 +2302,15 @@
         export : bool
             Set this boolean to True to allow the modification of log data. Set it to False to protect the data.
         password : str
             the password needed to make changes to the protection level.
         """
         self._dispatch.AllowModifyLogData(export, password)
 
-    def allow_modify_log_settings(self, export, password):  # TDOD Duplicate
+    def allow_modify_log_settings(self, export, password):
         """When dealing with a protected document you can use this method to enable / disable the option
         to change the settings of a log. This assumes you are in possession of the password.
 
         Parameters
         ----------
         export : bool
             Set this boolean to True to allow access to the log settings. Set it to False to protect the log settings.
```

### Comparing `pywellcad-0.1.0a0/wellcad/com/_marker_item.py` & `pywellcad-0.2.0/wellcad/com/_marker_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_odbc.py` & `pywellcad-0.2.0/wellcad/com/_odbc.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_page.py` & `pywellcad-0.2.0/wellcad/com/_page.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_polar_and_rose_box.py` & `pywellcad-0.2.0/wellcad/com/_polar_and_rose_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_stacking_pattern_item.py` & `pywellcad-0.2.0/wellcad/com/_stacking_pattern_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_structure.py` & `pywellcad-0.2.0/wellcad/com/_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ._dispatch_wrapper import DispatchWrapper
 
 
 class Structure(DispatchWrapper):
-    """ Structures are picked features (strata, lineations, fractures, breakouts) within a Structure, Lineation
+    r"""Structures are picked features (strata, lineations, fractures, breakouts) within a Structure, Lineation
     or Breakout Log.
 
     Sinusoidal structures (for example factures crossing a borehole) can be partial with only limited visible portions.
     Lineations are penetrative linear elements within a rock and can be of various origin (mineral lineation, fold axis etc.)
     Breakouts structures are vertical fractures caused by compression forces on the borehole walls.
     Their length, aperture and orientation helps to understand the constraints applied to the rock formation.
```

### Comparing `pywellcad-0.1.0a0/wellcad/com/_title.py` & `pywellcad-0.2.0/wellcad/com/_title.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.1.0a0/wellcad/com/_workspace.py` & `pywellcad-0.2.0/wellcad/com/_workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,40 +247,57 @@
 
         Returns
         -------
         bool
             Always returns True except for the WellCAD Reader and
             Demo version for which the function returns False.
         """
-        self._dispatch.ApplyTemplate(path, prompt_if_not_found, config_file_name)
+        return self._dispatch.ApplyTemplate(path, prompt_if_not_found, config_file_name)
 
     def auto_joint_detection(self, config_file_name):
         """Detects the joints from the main log (data source) used
         in the workspace.
 
         Parameters
         ----------
-        config_file_name : str
-            \*.ini file containing the processing parameters.
-            Read the WellCAD Help for information on the
-            syntax of the file.
+        config_file_name : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                Sensitivity = 5
+                TopAndBottom = yes
+
+            For WellCAD version 5.5 and 5.6, use this configuration instead:
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                JointHeight=0.5
+                Sensitivity=100
         """
         self._dispatch.AutoJointDetection(config_file_name)
 
     def add_joint_log_to_b_hole(self):
         """Adds the Marker Log from the Casing Integrity
         Workspace displaying the casing joints back to the
         borehole document.
         """
         self._dispatch.AddJointLogToBHole()
 
     def add_engin_log_from_driller_casing_table_to_b_hole(self):
         """Adds the Engineering Log from the Navigation Bar
         of the Casing Integrity Workspace displaying the
         drillers casing info back to the borehole document.
+
+        Note: this function is deprecated in WellCAD 5.7 and onwards
         """
         self._dispatch.AddEnginLogFromDrillerCasingTableToBHole()
 
     def add_engin_log_from_logger_casing_table_to_b_hole(self):
         """Adds the Engineering Log from the Navigation Bar
         of the Casing Integrity Workspace displaying the
         casing info derived from the logged data back to the
```

