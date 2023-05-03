# Comparing `tmp/NikeCA-0.1.87.tar.gz` & `tmp/NikeCA-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.87.tar", last modified: Wed May  3 04:39:54 2023, max compression
+gzip compressed data, was "NikeCA-0.1.88.tar", last modified: Wed May  3 05:53:59 2023, max compression
```

## Comparing `NikeCA-0.1.87.tar` & `NikeCA-0.1.88.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.253898 NikeCA-0.1.87/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.87/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 04:39:54.253480 NikeCA-0.1.87/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.87/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 04:39:54.254015 NikeCA-0.1.87/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 04:39:43.000000 NikeCA-0.1.87/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.245957 NikeCA-0.1.87/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.247532 NikeCA-0.1.87/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.249141 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.250823 NikeCA-0.1.87/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 04:39:54.252941 NikeCA-0.1.87/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 04:39:54.000000 NikeCA-0.1.87/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14422 2023-05-03 04:38:16.000000 NikeCA-0.1.87/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    12159 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.87/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.906453 NikeCA-0.1.88/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.88/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 05:53:59.906123 NikeCA-0.1.88/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.88/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 05:53:59.906571 NikeCA-0.1.88/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 05:53:54.000000 NikeCA-0.1.88/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.899979 NikeCA-0.1.88/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.901026 NikeCA-0.1.88/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.901903 NikeCA-0.1.88/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.903650 NikeCA-0.1.88/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 05:53:59.905633 NikeCA-0.1.88/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 05:53:59.000000 NikeCA-0.1.88/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 05:53:59.000000 NikeCA-0.1.88/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 05:53:59.000000 NikeCA-0.1.88/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 05:53:59.000000 NikeCA-0.1.88/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 05:53:59.000000 NikeCA-0.1.88/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14422 2023-05-03 04:38:16.000000 NikeCA-0.1.88/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    12386 2023-05-03 05:53:38.000000 NikeCA-0.1.88/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.88/src/__init__.py
```

### Comparing `NikeCA-0.1.87/LICENSE` & `NikeCA-0.1.88/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/PKG-INFO` & `NikeCA-0.1.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.87
+Version: 0.1.88
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.87/README.md` & `NikeCA-0.1.88/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/setup.py` & `NikeCA-0.1.88/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.87',
+	version='0.1.88',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.87/src/Dashboards/Dashboards.py` & `NikeCA-0.1.88/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.88/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.88/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.88/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.88/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.87
+Version: 0.1.88
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.87/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.88/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.88/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/NikeQA.py` & `NikeCA-0.1.88/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/NikeSF.py` & `NikeCA-0.1.88/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_BuildSearchQuery.py` & `NikeCA-0.1.88/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_GitHub.py` & `NikeCA-0.1.88/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_QA.py` & `NikeCA-0.1.88/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_SearchFiles.py` & `NikeCA-0.1.88/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_SnowflakeData.py` & `NikeCA-0.1.88/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.87/src/_SnowflakeDependencies.py` & `NikeCA-0.1.88/src/_SnowflakeDependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                                ):
 
         if filter_schemas is None:
             filter_schemas = []
 
         d = self.snowflake_dependencies_loop(tables=tables, username=username, warehouse=warehouse, role=role,
                                              database=database, schema=schema)
-        print(d)
+
         # filter out schemas to be divested
         d_final = self.remove_schemas(d_dict=d, schema_list=filter_schemas)
 
         # list column names for the new dataframe and convert the .json file to .csv if the schema name is listed
         # within 10 the previous 10 characters of the table name
         col_names = ['Table', 'Object', 'DDL']
         df_final = self.dict_convert_into_dataframe(d_dict=d_final, cols=col_names, schema_list=filter_schemas)
@@ -257,50 +257,54 @@
         if save_path is not None:
             final_df.to_csv(save_path)
 
         counter = 1
 
         if recursive:
             while len(df_final) > 0:
-                # read the new file created from the above steps to check for sub-dependencies
-                df_final_tables = []
-
-                [df_final_tables.append(v['Object'][v['Object'].right_index('.')+1:]) for k, v in df_final.iterrows()]
-                df_final_tables = list(set(df_final_tables))
-
-                # iterate through the select get_ddl() for the 3375 tables and views in the NGP_DA_PROD database and
-                # look for the dependent table names from the schemas to be divested
-                d = self.snowflake_dependencies_loop(
-                    tables=df_final_tables
-                    , role=role
-                    , database=database
-                    , warehouse=warehouse
-                    ,  username=username)
-
-                # filter out schemas not to save
-                d_final = self.remove_schemas(d_dict=d, schema_list=filter_schemas)
-
-                df_final_schemas = []
-
-                [df_final_schemas.append(str(v['Object']).split('.')[1]) for k, v in final_df.iterrows()]
-
-                df_final_schemas = list(set(df_final_schemas))
-
-                df_final = self.dict_convert_into_dataframe(d_dict=d_final, cols=col_names,
-                                                            schema_list=df_final_schemas)
-
-                df_final.columns = col_names
-
-                for i, v in final_df.iterrows():
-                    for x, y in df_final.iterrows():
-                        df_final.loc[x, 'MergeCol'] = v['Object'][:str(v['Object']).index('.') + 1] + y['Table']
-                final_df = final_df.merge(df_final, left_on='Object', right_on='MergeCol', how='left',
-                                          suffixes=(f'_Round{str(counter)}', f'_Round{str(counter + 1)}'))
-                final_df.drop(columns=['MergeCol'], inplace=True)
-
+                try:
+                    # read the new file created from the above steps to check for sub-dependencies
+                    df_final_tables = []
+
+                    [df_final_tables.append(v['Object'][v['Object'].right_index('.') + 1:]) for k, v in
+                     df_final.iterrows()]
+                    df_final_tables = list(set(df_final_tables))
+
+                    # iterate through the select get_ddl() for the 3375 tables and views in the NGP_DA_PROD database and
+                    # look for the dependent table names from the schemas to be divested
+                    d = self.snowflake_dependencies_loop(
+                        tables=df_final_tables
+                        , role=role
+                        , database=database
+                        , warehouse=warehouse
+                        , username=username)
+
+                    # filter out schemas not to save
+                    d_final = self.remove_schemas(d_dict=d, schema_list=filter_schemas)
+
+                    df_final_schemas = []
+
+                    [df_final_schemas.append(str(v['Object']).split('.')[1]) for k, v in final_df.iterrows()]
+
+                    df_final_schemas = list(set(df_final_schemas))
+
+                    df_final = self.dict_convert_into_dataframe(d_dict=d_final, cols=col_names,
+                                                                schema_list=df_final_schemas)
+
+                    df_final.columns = col_names
+
+                    for i, v in final_df.iterrows():
+                        for x, y in df_final.iterrows():
+                            df_final.loc[x, 'MergeCol'] = v['Object'][:str(v['Object']).index('.') + 1] + y['Table']
+                    final_df = final_df.merge(df_final, left_on='Object', right_on='MergeCol', how='left',
+                                              suffixes=(f'_Round{str(counter)}', f'_Round{str(counter + 1)}'))
+                    final_df.drop(columns=['MergeCol'], inplace=True)
+                except Exception as e:
+                    print(e)
+                    continue
             counter += 1
 
             if save_path is not None:
                 final_df.to_csv(save_path)
 
         print('process complete')
```

### Comparing `NikeCA-0.1.87/src/_SnowflakePull.py` & `NikeCA-0.1.88/src/_SnowflakePull.py`

 * *Files identical despite different names*

