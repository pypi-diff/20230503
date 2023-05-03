# Comparing `tmp/NikeCA-0.1.85.tar.gz` & `tmp/NikeCA-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.85.tar", last modified: Thu Apr 27 15:57:54 2023, max compression
+gzip compressed data, was "NikeCA-0.1.86.tar", last modified: Wed May  3 02:42:00 2023, max compression
```

## Comparing `NikeCA-0.1.85.tar` & `NikeCA-0.1.86.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.575787 NikeCA-0.1.85/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.85/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-04-27 15:57:54.575460 NikeCA-0.1.85/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.85/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-27 15:57:54.575885 NikeCA-0.1.85/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2468 2023-04-27 15:57:26.000000 NikeCA-0.1.85/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.568361 NikeCA-0.1.85/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.569618 NikeCA-0.1.85/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.570758 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.572585 NikeCA-0.1.85/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5985 2023-04-24 17:37:55.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-24 17:31:51.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.575034 NikeCA-0.1.85/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1154 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      416 2023-04-24 07:31:10.000000 NikeCA-0.1.85/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23731 2023-04-24 08:02:12.000000 NikeCA-0.1.85/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-04-27 15:54:21.000000 NikeCA-0.1.85/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.160733 NikeCA-0.1.86/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.86/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 02:42:00.160280 NikeCA-0.1.86/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.86/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 02:42:00.160855 NikeCA-0.1.86/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 02:41:31.000000 NikeCA-0.1.86/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.152863 NikeCA-0.1.86/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.153880 NikeCA-0.1.86/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.154912 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.156664 NikeCA-0.1.86/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:42:00.159521 NikeCA-0.1.86/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 02:41:59.000000 NikeCA-0.1.86/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    12159 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.86/src/__init__.py
```

### Comparing `NikeCA-0.1.85/LICENSE` & `NikeCA-0.1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/PKG-INFO` & `NikeCA-0.1.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.85
+Version: 0.1.86
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.85/README.md` & `NikeCA-0.1.86/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/setup.py` & `NikeCA-0.1.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.85',
+	version='0.1.86',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
@@ -66,14 +66,15 @@
 		"jupyter_server==2.3.0",
 		"jupyter_server_fileid==0.8.0",
 		"jupyter_server_terminals==0.4.4",
 		"jupyter_server_ydoc==0.6.1",
 		"jupyterlab==3.6.1",
 		"jupyterlab-pygments==0.2.2",
 		"jupyterlab_server==2.19.0",
+		"links-from-link-header==0.1.0",
 		"lz4==4.3.2",
 		"numpy==1.23.4",
 		"oauthlib==3.2.2",
 		"oscrypto==1.3.0",
 		"pandas==1.5.3",
 		"polars==0.17.9",
 		"pyarrow==10.0.1",
```

### Comparing `NikeCA-0.1.85/src/Dashboards/Dashboards.py` & `NikeCA-0.1.86/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.86/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.86/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,14 @@
                 , start_date: str = '1900-01-01'
                 , end_date: str = '9999-12-31'
                 ):
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
-        import os
-        print(os.system('pwd'))
-        print(config.sections())
         b = config['telemetry_product_usage'].get('col_b')
 
         if order_by is None:
             order_by = config['telemetry_product_usage'].get('order_by')
         else:
             order_by = ', '.join(order_by)
```

### Comparing `NikeCA-0.1.85/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.86/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.85
+Version: 0.1.86
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.85/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.86/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.86/src/NikeCA.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 jupyter_server==2.3.0
 jupyter_server_fileid==0.8.0
 jupyter_server_terminals==0.4.4
 jupyter_server_ydoc==0.6.1
 jupyterlab==3.6.1
 jupyterlab-pygments==0.2.2
 jupyterlab_server==2.19.0
+links-from-link-header==0.1.0
 lz4==4.3.2
 numpy==1.23.4
 oauthlib==3.2.2
 oscrypto==1.3.0
 pandas==1.5.3
 polars==0.17.9
 pyarrow==10.0.1
```

### Comparing `NikeCA-0.1.85/src/NikeQA.py` & `NikeCA-0.1.86/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/NikeSF.py` & `NikeCA-0.1.86/src/NikeSF.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
                  table: str = None, column_name: str = None, col_and_or: str = 'AND', get_ex_val: bool = None,
                  like_flag: bool = False, sample_table: bool = False, sample_val: bool = False,
                  table_sample: dict = None, dtypes_conv=None, query='', separate_dataframes: bool = False,
                  tables: list | str | None = None, save_path: str | None = None, date_min: str | None = None,
-                 date_max: str | None = None, column_filters: list | None = None, polars: bool = False):
+                 date_max: str | None = None, column_filters: list | None = None, polars: bool = False,
+                 filter_schemas: list | None = None, recursive: bool = False):
         """
         Parameters:
 
             username (str): The Snowflake account username.
             warehouse (str): The Snowflake warehouse to use.
             role (str): The Snowflake role to use.
             database (str, optional): The Snowflake database to use (default is None).
@@ -60,14 +61,16 @@
         self.__separate_dataframes = separate_dataframes
         self.__tables = tables
         self.__save_path = save_path
         self.__date_min = date_min
         self.__date_max = date_max
         self.__column_filters = column_filters
         self.__polars = polars
+        self.__filter_schemas = filter_schemas
+        self.__recursive = recursive
 
     # Getter and Setter Methods for Instance Variables
     @property
     def username(self):
         return self.__username
 
     @username.setter
@@ -238,14 +241,30 @@
     def polars(self):
         return self.__polars
 
     @polars.setter
     def polars(self, value):
         self.__polars = value
 
+    @property
+    def filter_schemas(self):
+        return self.__filter_schemas
+
+    @filter_schemas.setter
+    def filter_schemas(self, value):
+        self.__filter_schemas = value
+
+    @property
+    def recursive(self):
+        return self.__recursive
+
+    @recursive.setter
+    def recursive(self, value):
+        self.__recursive = value
+
     def build_search_query(self
                            , inp_db: str = None
                            , schema: str = None
                            , table: str = None
                            , column_name=None
                            , like_flag: bool = False
                            , col_and_or: str = 'AND'
@@ -479,19 +498,23 @@
     def snowflake_dependencies(self,
                                tables: str | list | None = None,
                                username: str | None = None,
                                warehouse: str | None = None,
                                role: str | None = None,
                                database: str | None = None,
                                schema: str | list | None = None,
-                               save_path: str = None
+                               save_path: str = None,
+                               filter_schemas: list | None = None,
+                               recursive: bool = False
                                ):
 
         """
 
+        :param recursive:
+        :param filter_schemas:
         :param save_path:
         :param tables:
         :param username:
         :param warehouse:
         :param role:
         :param database:
         :param schema:
@@ -508,18 +531,23 @@
             role = self.__role
         if database is None:
             database = self.__database
         if schema is None:
             schema = self.__schema
         if save_path is None:
             save_path = self.__save_path
+        if filter_schemas is None:
+            filter_schemas = self.__filter_schemas
+        if not recursive:
+            recursive = self.__recursive
 
         return SnowflakeData.snowflake_dependencies(self, tables=tables, username=username,
                                                     warehouse=warehouse, role=role, database=database,
-                                                    schema=schema, save_path=save_path)
+                                                    schema=schema, save_path=save_path, filter_schemas=filter_schemas,
+                                                    recursive=recursive)
 
     def imp_summary_dashboard(self
                               , username: str | None = None
                               , warehouse: str | None = None
                               , database: str | None = None
                               , role: str | None = None
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.1.85/src/_BuildSearchQuery.py` & `NikeCA-0.1.86/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/_GitHub.py` & `NikeCA-0.1.86/src/_GitHub.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         return d
 
     def get_repo_list(self, git_username: str = None, pat: str | None = None, org_name: str | None = None,
                       repo_list_filename: str | None = None):
         import json
         import requests
         from requests.auth import HTTPBasicAuth
-        import links_from_header
+        # import links_from_header
 
         respget = lambda url: requests.get(url, auth=HTTPBasicAuth(git_username, pat))
 
         myorgname = org_name
         nexturl = f"https://api.github.com/orgs/{myorgname}/repos?per_page=100"
 
         while nexturl:
```

### Comparing `NikeCA-0.1.85/src/_QA.py` & `NikeCA-0.1.86/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/_SearchFiles.py` & `NikeCA-0.1.86/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/_SnowflakeData.py` & `NikeCA-0.1.86/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.85/src/_SnowflakeDependencies.py` & `NikeCA-0.1.86/src/_SnowflakePull.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,184 +1,211 @@
 
 
-class SnowflakeDependencies:
+class SnowflakePull:
 
-    def snowflake_dependencies(self,
-                               tables: str | list,
-                               username: str,
-                               warehouse: str,
-                               role: str,
-                               database: str | None = None,
-                               schema: str | list | None = None,
-                               save_path: str | None = None):
+    import pandas
+
+    def snowflake_pull(self, query: str | dict | None, un, wh, db, role, schema=None, table=None,
+                       sample_table: bool = False, sample_val: bool = False, table_sample: dict = None,
+                       dtypes_conv=None, separate_dataframes: bool = True, polars: bool = False): # -> pandas.DataFrame:
 
         """
-        Searches the snowflake database and finds instances where the table is referenced and where the reference is not
-            in the actual creation of the table itself
+        function: pulls snowflake data
+
+        dependencies: [
+            pandas,
+            snowflake.connector,
+            time,
+            datetime.datetime
+        ]
+
+        :param polars:
+        :param separate_dataframes:
+        :param table:
+        :param schema:
+        :param query: str | dict
+            SQL query to run on Snowflake
+                    E.G. query = "SELECT * FROM  NGP_DA_PROD.POS.TO_DATE_AGG_CHANNEL_CY"
+            Can also be multiple queries in the form of a dictionary
+                    E.G. query = {"df1": "SELECT * FROM  NGP_DA_PROD.POS.TO_DATE_AGG_CHANNEL_CY", "df "SELECT TOP 2 * \
+                    FROM  NGP_DA_PROD.POS.TO_DATE_AGG_CHANNEL_CY"}
+
+        :param un: str
+            Nike Snowflake Username
+                "USERNAME"
+
+        :param db: str, default 'NA'
+            Name of the Database
+
+        :param wh: str
+            Name of the Wharehouse
+            e.g. "DA_DSM_SCANALYTICS_REPORTING_PROD"
+
+        :param role: str
+            Name of the role under which you are running Snowflake
+                "DF_######"
+
+        :param sample_table: bool, default: False
+
+        :param sample_val: bool, default: False
+
+        :param table_sample: dict, default: None
+            later
+                if table_sample = None
+                    table_sample = {'db': None, 'schema': None, 'table': None, 'col': None}
 
-        :param save_path: (str | None) The path to save the output.
-        :param tables: (str | list): The list of tables or views to fetch DDL for.
-        :param username: username for Snowflake
-        :param warehouse: warehouse for Snowflake
-        :param role: role for Snowflake
-        :param database: database to search in must provide
-        :param schema: filling this in can really help to speed up the query
-        :return: pandas Dataframe
-
-        This function is used to fetch the DDL of tables and views from Snowflake.
-
-        Parameters:
-            tables (str | list): The list of tables or views to fetch DDL for.
-            username (str): The username of the Snowflake user.
-            warehouse (str): The warehouse to use for the connection.
-            role (str): The role of the Snowflake user.
-            database (str | None): The database to use for the connection.
-            schema (str | list | None): The schema to use for the connection.
-            save_path (str | None): The path to save the output.
+        :param dtypes_conv: default: None
 
-        Returns:
-            dict: A dictionary containing the DDL of the tables and views.
+        :return: pandas.DataFrame
         """
 
         # snowflake connection packages:
         import pandas as pd
         import polars as pl
         import snowflake.connector
         import time
-        import json
-        import os
-
-        if type(tables) == str:
-            tables = [tables]
 
-        print('opening snowflake connection...')
+        if table_sample is not None:
+            table_sample = {'db': None, 'schema': None, 'table': None, 'col': None}
 
-        cnn = snowflake.connector.connect(
-            user=username,
-            account='nike',
-            authenticator='externalbrowser',
-            role=role,
-            warehouse=warehouse,
-        )
-        cs = cnn.cursor()
-        process_complete = 0
-        process_pass = 0
-        counter = 0
-
-        # fetch schema and table names
-        query = 'SELECT * FROM ' + database + '.INFORMATION_SCHEMA.TABLES'
-        if schema is not None:
-            if type(schema) == str:
-                schema = [schema]
-            query = query + " WHERE TABLE_SCHEMA IN ('" + schema[0] + "'"
-            if len(schema) > 1:
-                for i in schema[1:]:
-                    query = query + ", '" + i + "'"
-            query = query + ')'
-
-        cs.execute(query)
-        df_tables = cs.fetch_pandas_all()
-
-        query_ddl = {}
-
-        for k, i in df_tables.iterrows():
-            if i['TABLE_TYPE'] == 'VIEW':
-                query_ddl[i['TABLE_CATALOG'] + '.' + i['TABLE_SCHEMA'] + '.' + i['TABLE_NAME']] = \
-                    "SELECT GET_DDL('" + i['TABLE_TYPE'] + "', '" + i['TABLE_CATALOG'] + '.' + i[
-                        'TABLE_SCHEMA'] + '.' \
-                    + i['TABLE_NAME'] + "')"
-            elif i['TABLE_TYPE'] == 'BASE TABLE':
-                query_ddl[i['TABLE_CATALOG'] + '.' + i['TABLE_SCHEMA'] + '.' + i['TABLE_NAME']] = \
-                    "SELECT GET_DDL('TABLE', '" + i['TABLE_CATALOG'] + '.' + i['TABLE_SCHEMA'] + '.' + \
-                    i['TABLE_NAME'] + "')"
-
-        df = pd.DataFrame([query_ddl]).T
-
-        df_index = df.index
-
-        df_return = pd.DataFrame(index=df_index)
-        df_return['sfqid'] = ''
-
-        queries = len(df)
-        print('Pulling ' + str(queries) + ' queries')
-
-        query_list = []
-        db_list = []
-        complete = []
-
-        for item in range(queries):
-            query_list.append(item)
-            db_list.append(item)
-            complete.append(0)
-
-        for k, v in df.iterrows():
-            sql = v[0]
-            cs.execute_async(sql)
-            query_list[counter] = cs.sfqid
-            df_return['sfqid'][k] = cs.sfqid
-            counter += 1
-        counter = 1
-        if save_path is not None:
-            if os.path.isfile(save_path):
-                with open(save_path) as f:
-                    d = json.load(f)
-            else:
-                d = {}
+        # --> take a random sample from a table in snowflake
+        query = f'''SELECT * FROM {table_sample['db']}.{table_sample['schema']}.{table_sample['table']} LIMIT 100''' \
+            if sample_table else query
+
+        # --> take a random sample of a column from a table in snowflake
+        query = f'''SELECT DISTINCT 
+                {table_sample['col']} 
+            FROM 
+                {table_sample['db']}.{table_sample['schema']}.{table_sample['table']} 
+            ORDER BY 1 LIMIT 10''' \
+            if sample_val else query
+
+        recs = False
+
+        df = pd.DataFrame()
+
+        if type(query) == dict:
+
+            df = pd.DataFrame([query]).T
+            df_index = df.index
+            print(df_index)
+
+            df2 = pl.from_pandas(df)
+            print(df2)
+
+            df_return = pd.DataFrame(index=df.index)
+            df_return['sfqid'] = ''
+
+            queries = len(df)
+            print('Pulling ' + str(queries) + ' queries')
+
+            query_list = []
+            db_list = []
+            complete = []
+
+            for item in range(queries):
+                query_list.append(item)
+                db_list.append(item)
+                complete.append(0)
+
+            print('opening snowflake connection...')
+
+            try:
+                cnn = snowflake.connector.connect(
+                    user=un,
+                    account='nike',
+                    authenticator='externalbrowser',
+                    role=role,
+                    warehouse='POS_REPORT_PROD'
+                )
+
+                cs = cnn.cursor()
+                process_complete = 0
+                process_pass = 0
+                counter = 0
+
+                for k, v in df.iterrows():
+                    sql = v[0]
+                    cs.execute_async(sql)
+                    query_list[counter] = cs.sfqid
+                    df_return['sfqid'][k] = cs.sfqid
+                    counter += 1
+                dfs = {}
+                while process_complete == 0:
+                    item = -1
+                    process_pass += 1
+                    if sum(complete) == queries or process_pass == 10:
+                        process_complete = 1
+                    for result in query_list:
+                        item += 1
+                        if complete[item] == 0:
+                            status = cnn.get_query_status_throw_if_error(result)
+                            print('the status for ' + df_return[df_return['sfqid'] == result].index[0] + ' is ' +
+                                  str(status))
+                            if str(status) == 'QueryStatus.SUCCESS':
+                                complete[item] = 1
+                                cs.get_results_from_sfqid(result)
+                                if separate_dataframes:
+
+                                    recs = True
+                                    dfs[df_return[df_return['sfqid'] == result].index[0]] = cs.fetch_pandas_all()
+
+                                else:
+                                    df = pd.concat([df, cs.fetch_pandas_all()])
+                            else:
+                                time.sleep(.25)
+            except Exception as e:
+                print(e)
+            finally:
+                cnn.close()
+                print('process complete')
         else:
-            d = {}
+            # connection settings
+            from snowflake.connector.converter_null import SnowflakeNoConverterToPython
+            conn = snowflake.connector.connect(
+                user=un,
+                account='nike',
+
+                # opens separate browser window to confirm authentication
+                authenticator='externalbrowser',
+                warehouse=wh,
+                database=db,
+                role=role,
+                converter_class=SnowflakeNoConverterToPython
+            )
+
+            # connect to snowflake using conn variables
+            cur = conn.cursor()
+
+            try:
+                cur.execute(query)  # execute sql, store into-->
+
+            # final data pull --> allows datatype-memory optimization
+                df = pl.DataFrame
+                if polars:
+                    df = cur.fetch_arrow_all()
+
+                else:
+                    df = cur.fetch_pandas_all()
+                print(df)
+
+            except snowflake.connector.errors.ProgrammingError:
+                print(f'Could not retrieve:\n\t {query}')
+
+            except TypeError:
+                print(f"""Could not retrieve:\n\t{query}\n\nbecause TypeError: NoneType""")
+
+            # --> allows metadata querying
+            except Exception as e:
+                print(e)
+                temp_df = cur.fetchall()  # return data
+                cols = [x.name for x in cur.description]  # get column names
+                df = pd.DataFrame(temp_df, columns=cols)  # create dataset
+
+            conn.close()
+            cur.close()
+        if recs:
+            return [dfs[k] for k in df_index]
 
-        for table in tables:
-            d[table] = {}
-        while process_complete == 0:
-            item = -1
-            process_pass += 1
-            if sum(complete) == queries or process_pass == 1000:
-                process_complete = 1
-            for result in query_list:
-                item += 1
-                if complete[item] == 0:
-                    print('Running ' + df_return[df_return['sfqid'] == result].index[0])
-                    try:
-                        status = cnn.get_query_status_throw_if_error(result)
-
-                    except snowflake.connector.errors.ProgrammingError:
-                        print(f"""Could not retrieve:
-                            {df_return[df_return['sfqid'] == result].index[0]}
-                            
-                            because of snowflake.connector.errors.ProgrammingError""")
-                        complete[item] = 1
-                        continue
-
-                    except TypeError:
-                        print(f"""Could not retrieve:
-                            {df_return[df_return['sfqid'] == result].index[0]}
-                        
-                        because TypeError: NoneType""")
-                        complete[item] = 1
-                        continue
-
-                    print('the status for ' + df_return[df_return['sfqid'] == result].index[0] + ' is ' +
-                          str(status) + ' ' + str(counter))
-                    if str(status) == 'QueryStatus.SUCCESS':
-                        complete[item] = 1
-                        cs.get_results_from_sfqid(result)
-                        data = cs.fetch_pandas_all()
-                        for table in tables:
-                            try:
-                                if table.upper() + ' ' in data.iloc[0, 0][data.iloc[0, 0].upper().index(
-                                        table.upper()):data.iloc[0, 0].upper().index(table.upper()) + len(table) + 1]\
-                                        and table.upper() not in data.iloc[0, 0][:data.iloc[0, 0].index('(')]:
-                                    d[table][df_return[df_return['sfqid'] == result].index[0]] = data.to_dict('index')
-                            except ValueError:
-                                continue
-                    else:
-                        time.sleep(.1)
-                counter += 1
-        cnn.close()
-
-        if save_path is not None:
-            with open(save_path, "w+") as f:
-                json.dump(d, f, indent=4)
+        return df
 
-        print('process complete')
 
-        return d
```

