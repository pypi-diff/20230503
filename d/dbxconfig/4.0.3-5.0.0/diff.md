# Comparing `tmp/dbxconfig-4.0.3.tar.gz` & `tmp/dbxconfig-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-4.0.3.tar", last modified: Wed May  3 07:41:46 2023, max compression
+gzip compressed data, was "dbxconfig-5.0.0.tar", last modified: Wed May  3 20:47:28 2023, max compression
```

## Comparing `dbxconfig-4.0.3.tar` & `dbxconfig-5.0.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.462573 dbxconfig-4.0.3/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2658 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1597 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4286 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6649 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/datallake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/dataset_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.462573 dbxconfig-4.0.3/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.339682 dbxconfig-5.0.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3161 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4339 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.339682 dbxconfig-5.0.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/setup.py
```

### Comparing `dbxconfig-4.0.3/PKG-INFO` & `dbxconfig-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 4.0.3
+Version: 5.0.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-4.0.3/README.md` & `dbxconfig-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/_decorators.py` & `dbxconfig-5.0.0/dbxconfig/_decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,41 +3,48 @@
 import logging
 from ._config import Config
 from ._timeslice import Timeslice
 from ._stage_type import StageType
 import os
 
 
-def yetl_flow(stage: StageType, config_path: str = None, pattern: str = None):
+def yetl_flow(
+    stage: StageType,
+    project: str,
+    pipeline: str = None,
+    config_path: str = None,
+):
     def decorate(function):
         def wrap_function(*args, **kwargs):
-            configure_logging()
+            configure_logging(project)
             _logger = logging.getLogger(__name__)
 
-            _pattern = pattern
-            if not _pattern:
-                _pattern = function.__name__
+            _pipeline = pipeline
+            if not _pipeline:
+                _pipeline = function.__name__
 
-            _logger.info(f"Loading pipeline configuration {_pattern}")
+            _logger.info(f"Loading pipeline configuration {_pipeline}")
 
             _config_path = config_path
             if not config_path:
-                _config_path = os.getenv(YETL_CONFIG, "../config")
+                _config_path = os.getenv(YETL_CONFIG, "./config")
 
             timeslice = kwargs.get("timeslice", Timeslice(day="*", month="*", year="*"))
             if "timeslice" in kwargs.keys():
                 del kwargs["timeslice"]
 
             try:
                 table = kwargs["table"]
                 del kwargs["table"]
             except KeyError as e:
                 raise Exception(f"{e} is a required argument for a yetl flow function")
 
-            config = Config(pattern=_pattern, config_path=_config_path)
+            config = Config(
+                project=project, pipeline=_pipeline, config_path=_config_path
+            )
             table_mapping = config.get_table_mapping(
                 timeslice=timeslice, stage=stage, table=table
             )
             _logger.info(f"Calling function {function.__name__}")
             ret = function(
                 *args,
                 table_mapping=table_mapping,
```

### Comparing `dbxconfig-4.0.3/dbxconfig/_spark_context.py` & `dbxconfig-5.0.0/dbxconfig/_spark_context.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/_tables.py` & `dbxconfig-5.0.0/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/_timeslice.py` & `dbxconfig-5.0.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/_utils.py` & `dbxconfig-5.0.0/dbxconfig/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,20 @@
     _logger = logging.getLogger(__name__)
     if not os.path.isabs(path):
         path = os.path.join(root, path)
     _logger.debug(f"Absolute config path {path}")
     return path
 
 
-def get_config_path(path: str):
+def get_config_path(project: str, path: str):
     _logger = logging.getLogger(__name__)
     if not path:
         path = os.getenv(YETL_CONFIG, "./config")
     path = os.path.abspath(path)
+    path = os.path.join(path, project)
     _logger.info(f"Absolute root config path {path}")
     return path
 
 
 def load_schema(path: str):
     _logger = logging.getLogger(__name__)
     schema = load_yaml(path)
```

### Comparing `dbxconfig-4.0.3/dbxconfig/datallake.py` & `dbxconfig-5.0.0/dbxconfig/datallake.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     predicate = " and ".join(predicates)
 
     return predicate
 
 
 def table_exists(database: str, table: str):
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
     table_exists = (
         spark.sql(f"SHOW TABLES in {database};")
         .where(f"tableName='{table}' AND !isTemporary")
         .count()
         == 1
     )
     return table_exists
@@ -55,25 +55,25 @@
 
     sql_path = ""
     if path:
         sql_path = f"USING DELTA LOCATION '{path}';"
 
         sql = f"{sql}\n{sql_path}\n{sql_properties}"
 
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
     _logger.debug(f"{sql}")
     spark.sql(sql)
 
     return sql
 
 
 def create_database(database: str):
     _logger.debug(f"Creating database if not exists `{database}`")
     sql = f"CREATE DATABASE IF NOT EXISTS {database}"
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
     _logger.debug(sql)
     spark.sql(sql)
     return sql
 
 
 def alter_table_drop_constraint(database: str, table: str, name: str):
     return f"ALTER TABLE `{database}`.`{table}` DROP CONSTRAINT {name};"
@@ -86,15 +86,15 @@
 def alter_table_set_tblproperties(database: str, table: str, properties: str):
     return f"ALTER TABLE `{database}`.`{table}` SET TBLPROPERTIES ({properties});"
 
 
 def get_table_properties(database: str, table: str):
     _logger.debug(f"getting existing table properties for table {database}.{table}")
 
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
 
     df: DataFrame = spark.sql(f"SHOW TBLPROPERTIES `{database}`.`{table}`").collect()
     tbl_properties = {
         c.asDict()["key"]: c.asDict()["value"]
         for c in df
         if not c["key"].startswith("delta.constraints")
     }
@@ -123,24 +123,24 @@
         predicate = f" WHERE {predicate}"
         sql = f"{sql}{predicate}"
 
     if zorder_by:
         sql_zorderby = ",".join([f"`{z}`" for z in zorder_by])
         sql = f"{sql} ZORDER BY ({sql_zorderby})"
 
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
     _logger.debug(f"optimizing table {database}.{table}\n{sql}")
     spark.sql(sql)
 
 
 def get_table_details(database: str, table: str):
     _logger.debug(
         f"getting existing table details and partitions for table {database}.{table}"
     )
-    spark = get_spark_context(project="dbxconfig")
+    spark = get_spark_context(project="test_project")
 
     df: DataFrame = spark.sql(
         f"DESCRIBE TABLE EXTENDED `{database}`.`{table}`"
     ).collect()
 
     # get the details into a dictionary
     details = {c.asDict()["col_name"]: c.asDict()["data_type"] for c in df}
```

### Comparing `dbxconfig-4.0.3/dbxconfig/dataset/_dataset.py` & `dbxconfig-5.0.0/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/dataset/_deltalake.py` & `dbxconfig-5.0.0/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/dataset/_factory.py` & `dbxconfig-5.0.0/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/dataset/_read.py` & `dbxconfig-5.0.0/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-5.0.0/dbxconfig/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-4.0.3/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-5.0.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 4.0.3
+Version: 5.0.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-4.0.3/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-5.0.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 dbxconfig/__init__.py
 dbxconfig/_config.py
 dbxconfig/_decorators.py
 dbxconfig/_logging_config.py
+dbxconfig/_project.py
 dbxconfig/_spark_context.py
 dbxconfig/_stage_type.py
 dbxconfig/_table_mapping.py
 dbxconfig/_tables.py
 dbxconfig/_timeslice.py
 dbxconfig/_utils.py
 dbxconfig/datallake.py
```

### Comparing `dbxconfig-4.0.3/setup.py` & `dbxconfig-5.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="4.0.3",
+    version="5.0.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

