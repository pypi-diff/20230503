# Comparing `tmp/NikeCA-0.1.86.tar.gz` & `tmp/NikeCA-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.86.tar", last modified: Wed May  3 02:42:00 2023, max compression
+gzip compressed data, was "NikeCA-0.1.87.tar", last modified: Wed May  3 04:39:54 2023, max compression
```

## Comparing `NikeCA-0.1.86.tar` & `NikeCA-0.1.87.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.160733 NikeCA-0.1.86/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.86/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 02:42:00.160280 NikeCA-0.1.86/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.86/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 02:42:00.160855 NikeCA-0.1.86/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 02:41:31.000000 NikeCA-0.1.86/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.152863 NikeCA-0.1.86/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.153880 NikeCA-0.1.86/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.154912 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.156664 NikeCA-0.1.86/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.159521 NikeCA-0.1.86/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    12159 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.253898 NikeCA-0.1.87/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.87/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 04:39:54.253480 NikeCA-0.1.87/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.87/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 04:39:54.254015 NikeCA-0.1.87/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 04:39:43.000000 NikeCA-0.1.87/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.245957 NikeCA-0.1.87/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.247532 NikeCA-0.1.87/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.249141 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.250823 NikeCA-0.1.87/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.252941 NikeCA-0.1.87/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14422 2023-05-03 04:38:16.000000 NikeCA-0.1.87/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    12159 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/__init__.py
```

### Comparing `NikeCA-0.1.86/LICENSE` & `NikeCA-0.1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/PKG-INFO` & `NikeCA-0.1.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.86
+Version: 0.1.87
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.86/README.md` & `NikeCA-0.1.87/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/setup.py` & `NikeCA-0.1.87/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.86',
+	version='0.1.87',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.86/src/Dashboards/Dashboards.py` & `NikeCA-0.1.87/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.87/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.87/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.87/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.87/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.86
+Version: 0.1.87
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.86/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.87/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.87/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/NikeQA.py` & `NikeCA-0.1.87/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/NikeSF.py` & `NikeCA-0.1.87/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_BuildSearchQuery.py` & `NikeCA-0.1.87/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_GitHub.py` & `NikeCA-0.1.87/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_QA.py` & `NikeCA-0.1.87/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_SearchFiles.py` & `NikeCA-0.1.87/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_SnowflakeData.py` & `NikeCA-0.1.87/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,24 @@
                     print(f"Could not pull {row['COLUMN_NAME']} for table: {row['TABLE_NAME']}")
                     print(e)
                     continue
 
         return results_fin
 
     def snowflake_dependencies(self, tables: str | list, username: str, warehouse: str, role: str,
-                               database: str | None = None, schema: str | list | None = None, save_path: str = None):
+                               database: str | None = None, schema: str | list | None = None, save_path: str = None,
+                               filter_schemas: list | None = None, recursive: bool = False):
 
         return _SnowflakeDependencies.SnowflakeDependencies.snowflake_dependencies(self, tables=tables,
                                                                                    username=username,
                                                                                    warehouse=warehouse, role=role,
                                                                                    database=database, schema=schema,
-                                                                                   save_path=save_path)
+                                                                                   save_path=save_path,
+                                                                                   filter_schemas=filter_schemas,
+                                                                                   recursive=recursive)
 
     def optimize_tbl_mem(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
                          table_name: str = None, pull_all_cols=True, run_debugging: bool = False,
                          query=None):
 
         import numpy as np
         from NikeQA import QA
```

### Comparing `NikeCA-0.1.86/src/_SnowflakeDependencies.py` & `NikeCA-0.1.87/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.86/src/_SnowflakePull.py` & `NikeCA-0.1.87/src/_SnowflakePull.py`

 * *Files identical despite different names*

