# Comparing `tmp/dbxconfig-2.4.0.tar.gz` & `tmp/dbxconfig-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.4.0.tar", last modified: Thu Apr 27 19:37:09 2023, max compression
+gzip compressed data, was "dbxconfig-4.0.3.tar", last modified: Wed May  3 07:41:46 2023, max compression
```

## Comparing `dbxconfig-2.4.0.tar` & `dbxconfig-4.0.3.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      463 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2808 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1264 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5348 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      963 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3232 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.462573 dbxconfig-4.0.3/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2658 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1656 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1597 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4286 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6649 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 07:41:46.462573 dbxconfig-4.0.3/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 07:41:46.000000 dbxconfig-4.0.3/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 07:41:46.466573 dbxconfig-4.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 07:40:49.000000 dbxconfig-4.0.3/setup.py
```

### Comparing `dbxconfig-2.4.0/PKG-INFO` & `dbxconfig-4.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,119 @@
-Metadata-Version: 2.1
-Name: dbxconfig
-Version: 2.4.0
-Summary: Databricks Configuration Framework
-Home-page: https://dbxconfig.readthedocs.io/en/latest/
-Author: Shaun Ryan
-Author-email: shaun_chiburi@hotmail.com
-License: MIT
-Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
-Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # dbxconfig
 
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
 landing:
-  landing_dbx_patterns:
-    customer_details_1: null
-    customer_details_2: null
+  read:
+    landing_dbx_patterns:
+      customer_details_1: null
+      customer_details_2: null
 
 raw:
-  raw_dbx_patterns:
-    customers:
-      ids: id
-      depends_on:
-        - landing.landing_dbx_patterns.customer_details_1
-        - landing.landing_dbx_patterns.customer_details_2
-      warning_thresholds:
-        invalid_ratio: 0.1
-        invalid_rows: 0
-        max_rows: 100
-        min_rows: 5
-      exception_thresholds:
-        invalid_ratio: 0.2
-        invalid_rows: 2
-        max_rows: 1000
-        min_rows: 0
+  delta_lake:
+    raw_dbx_patterns:
+      customers:
+        ids: id
+        depends_on:
+          - landing.landing_dbx_patterns.customer_details_1
+          - landing.landing_dbx_patterns.customer_details_2
+        warning_thresholds:
+          invalid_ratio: 0.1
+          invalid_rows: 0
+          max_rows: 100
+          min_rows: 5
+        exception_thresholds:
+          invalid_ratio: 0.2
+          invalid_rows: 2
+          max_rows: 1000
+          min_rows: 0
+        custom_properties:
+          process_group: 1
 
 base:
-  base_dbx_patterns:
-    customer_details_1:
-      ids: id
-      depends_on:
-        - raw.raw_dbx_patterns.customers
-    customer_details_2:
-      ids: id
-      depends_on:
-        - raw.raw_dbx_patterns.customers
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+      delta.appendOnly: true
+      delta.autoOptimize.autoCompact: true    
+      delta.autoOptimize.optimizeWrite: true  
+      delta.enableChangeDataFeed: false
+    base_dbx_patterns:
+      customer_details_1:
+        ids: id
+        depends_on:
+          - raw.raw_dbx_patterns.customers
+        # delta table properties can be set at stage level or table level
+        # table level properties will overwride stage level properties
+        delta_properties:
+            delta.enableChangeDataFeed: true
+      customer_details_2:
+        ids: id
+        depends_on:
+          - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
 tables: ./tables.yaml
 
 landing:
-  trigger: customerdetailscomplete-{{filename_date_format}}*.flg
-  trigger_type: file
-  database: landing_dbx_patterns
-  table: "{{table}}"
-  container: datalake
-  root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
-  filename: "{{table}}-{{filename_date_format}}*.csv"
-  filename_date_format: "%Y%m%d"
-  path_date_format: "%Y%m%d"
-  format: cloudFiles
-  spark_schema: ../Schema/{{table.lower()}}.yaml
-  options:
-    # autoloader
-    cloudFiles.format: csv
-    cloudFiles.schemaLocation:  "/mnt/{{container}}/checkpoint/{{checkpoint}}"
-    cloudFiles.useIncrementalListing: auto
-    # schema
-    inferSchema: false
-    enforceSchema: true
-    columnNameOfCorruptRecord: _corrupt_record
-    # csv
-    header: false
-    mode: PERMISSIVE
-    encoding: windows-1252
-    delimiter: ","
-    escape: '"'
-    nullValue: ""
-    quote: '"'
-    emptyValue: ""
+  read:
+    trigger: customerdetailscomplete-{{filename_date_format}}*.flg
+    trigger_type: file
+    database: landing_dbx_patterns
+    table: "{{table}}"
+    container: datalake
+    root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
+    filename: "{{table}}-{{filename_date_format}}*.csv"
+    filename_date_format: "%Y%m%d"
+    path_date_format: "%Y%m%d"
+    format: cloudFiles
+    spark_schema: ../Schema/{{table.lower()}}.yaml
+    options:
+      # autoloader
+      cloudFiles.format: csv
+      cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
+      cloudFiles.useIncrementalListing: auto
+      # schema
+      inferSchema: false
+      enforceSchema: true
+      columnNameOfCorruptRecord: _corrupt_record
+      # csv
+      header: false
+      mode: PERMISSIVE
+      encoding: windows-1252
+      delimiter: ","
+      escape: '"'
+      nullValue: ""
+      quote: '"'
+      emptyValue: ""
     
 
 raw:
-  database: raw_dbx_patterns
-  table: "{{table}}"
-  container: datalake
-  root: /mnt/{{container}}/data/raw
-  path: "{{database}}/{{table}}"
-  checkpoint_location: /mnt/{{container}}/checkpoint/{{checkpoint}}
-  options:
-    mergeSchema: true
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+      delta.appendOnly: true
+      delta.autoOptimize.autoCompact: true    
+      delta.autoOptimize.optimizeWrite: true  
+      delta.enableChangeDataFeed: false
+    database: raw_dbx_patterns
+    table: "{{table}}"
+    container: datalake
+    root: /mnt/{{container}}/data/raw
+    path: "{{database}}/{{table}}"
+    options:
+      checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
+      mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from dbxconfig import Config, Timeslice, StageType
```

### Comparing `dbxconfig-2.4.0/dbxconfig/_config.py` & `dbxconfig-4.0.3/dbxconfig/_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-import yaml
 import os
 from .dataset import DataSet
 from ._timeslice import Timeslice
 from ._tables import Tables, _INDEX_WILDCARD
 from ._stage_type import StageType
 from .dataset import dataset_factory
-from ._utils import abs_config_path
+from ._utils import abs_config_path, load_yaml, get_config_path, check_version
+from ._logging_config import configure_logging
 
 
 class Config:
-    _CONFIG_PATH = "./Config/"
-    _ENCODING = "utf-8"
     _TABLES = "tables"
-    _SOURCE_TABLE = "source_table"
+    _CONFIG_PATH = "config_path"
 
     def __init__(self, pattern: str, config_path: str = None):
+        configure_logging()
+
         self.config = self._load_config(pattern, config_path)
         self.tables = self._load_tables()
 
     def _load_config(self, pattern: str, config_path: str):
-        config_path = self._get_config_path(config_path)
+        config_path = get_config_path(config_path)
         config_file = f"{pattern}.yaml"
 
         config_file_path = os.path.join(config_path, config_file)
-
-        with open(config_file_path, "r", encoding=self._ENCODING) as f:
-            config = yaml.safe_load(f)
+        config = load_yaml(config_file_path)
+        check_version(config)
 
         # add the configuration path into the confif dictionart
         # so that it gets passed to table config when created
-        config["config_path"] = config_path
+        config[self._CONFIG_PATH] = config_path
         return config
 
     def _load_tables(self):
-        tables_path = self.config["tables"]
-        tables_path = abs_config_path(self.config["config_path"], self.config["tables"])
+        tables_path = self.config[self._TABLES]
+        tables_path = abs_config_path(
+            self.config[self._CONFIG_PATH], self.config[self._TABLES]
+        )
 
-        with open(tables_path, "r", encoding=self._ENCODING) as f:
-            self.config["tables"] = yaml.safe_load(f)
+        data = load_yaml(tables_path)
+        check_version(data)
+        self.config[self._TABLES] = data
 
         tables = Tables(
-            table_data=self.config["tables"], config_path=self.config["config_path"]
+            table_data=self.config[self._TABLES],
+            config_path=self.config[self._CONFIG_PATH],
         )
-
         return tables
 
-    def _get_config_path(self, config_path: str):
-        if not config_path:
-            config_path = self._CONFIG_PATH
-        config_path = os.path.abspath(config_path)
-        return config_path
-
     def get_table_mapping(
         self,
         timeslice: Timeslice,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
     ):
```

### Comparing `dbxconfig-2.4.0/dbxconfig/_table.py` & `dbxconfig-4.0.3/dbxconfig/dataset/_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from pydantic import BaseModel, Field
-from typing import Union, List, Any, Dict
-from ._stage_type import StageType
+import logging
+from pydantic import BaseModel, Field, PrivateAttr
+from .._utils import JinjaVariables
+from typing import Any, Dict, Union, List
+from .._timeslice import Timeslice
+from .._stage_type import StageType
+from .dataset_type import TableType
 
 
-class ValidationThreshold(BaseModel):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    invalid_ratio: float = Field(default=None)
-    invalid_rows: int = Field(default=None)
-    max_rows: int = Field(default=None)
-    min_rows: int = Field(default=None)
-
-
-class BaseTable(BaseModel):
+class Table(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
     database: str = Field(...)
-    name: str = Field(...)
+    table: str = Field(...)
     id: Union[str, List[str]] = Field(default=[])
-
-
-class Table(BaseTable):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    depends_on: List[str] = Field(default=[])
-    delta_properties: Dict[str, str] = Field(default=None)
     custom_properties: Dict[str, Any] = Field(default=None)
-    warning_thresholds: ValidationThreshold = Field(default=None)
-    exception_thresholds: ValidationThreshold = Field(default=None)
+    table_type: TableType = Field(...)
+
+    def _render(self):
+        pass
 
 
-class TableMapping(BaseModel):
+class DataSet(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
+        self._logger = logging.getLogger(self.__class__.__name__)
+
+    _logger: Any = PrivateAttr(default=None)
+    _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
+    container: str = Field(...)
+    root: str = Field(...)
+    path: str = Field(default=None)
+    options: dict = Field(...)
+    timeslice: Timeslice = Field(...)
+    checkpoint: str = Field(default=None)
+    config_path: str = Field(...)
 
-    destination: Table = Field(...)
-    source: Union[Dict[str, Table], Table] = Field(...)
+    def _render(self):
+        pass
```

### Comparing `dbxconfig-2.4.0/dbxconfig/_tables.py` & `dbxconfig-4.0.3/dbxconfig/_tables.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from pydantic import BaseModel, Field
 from typing import Union, Any, Dict, List
 from ._stage_type import StageType
 import fnmatch
-from ._table import Table, TableMapping
+from ._table_mapping import TableMapping
+from .dataset.dataset_type import TableType
+from .dataset import dataset_factory
+from .dataset._dataset import Table
 
 
 _INDEX_WILDCARD = "*"
 
 
 class Tables(BaseModel):
     def __init__(self, **data: Any) -> None:
@@ -43,46 +46,92 @@
         except Exception as e:
             raise Exception(
                 f"attempted to parse an invalid index {index}. It must be of the form 'stage.database.table'"
             ) from e
 
         return stage, database, table
 
+    def _parse_table_delta_lake_properties(
+        self,
+        table_type: TableType,
+        table_details: dict,
+        merge_properties: dict = {},
+    ):
+        """
+        Parse the delta properties from the tables details if there are any. Merge the into
+        a set of existing properties with the table detail properties taking precedence.
+        """
+        if table_type is TableType.DeltaLakeTable:
+            delta_properties = table_details.get("delta_properties", {})
+            # delta_properties = stage_delta_properties | delta_properties
+            delta_properties = {
+                **merge_properties,
+                **delta_properties,
+            }
+            return delta_properties
+        else:
+            return None
+
+    def _parse_stage_delta_lake_properties(
+        self, table_type: TableType, database_tables: dict
+    ):
+        """Parse delta lake properties from the database table details and remove it"""
+        stage_delta_properties = None
+        if table_type is TableType.DeltaLakeTable:
+            stage_delta_properties = database_tables.get("delta_properties", {})
+            if stage_delta_properties:
+                del database_tables["delta_properties"]
+        return stage_delta_properties
+
+    def _parse_stage_data(self, stage: StageType, stage_data: dict):
+        """
+        loop through the database tables, create the table
+        and add it to the class index.
+        """
+        for table_type, database_tables in stage_data.items():
+            table_type = TableType(table_type)
+            stage_delta_properties = self._parse_stage_delta_lake_properties(
+                table_type, database_tables
+            )
+            for database, tables in database_tables.items():
+                for table, table_details in tables.items():
+                    # flatten the config structure for a table
+                    if not table_details:
+                        table_details = {}
+
+                    delta_properties = self._parse_table_delta_lake_properties(
+                        table_type, table_details, stage_delta_properties
+                    )
+                    if delta_properties:
+                        table_details["delta_properties"] = delta_properties
+                    table_details["table"] = table
+                    table_details["database"] = database
+                    table_details["stage"] = stage
+                    table_details["table_type"] = table_type
+
+                    # create a table object
+
+                    # table = Table(**table_details)
+                    table = dataset_factory.get_table(table_type, table_details)
+
+                    # index the table object
+                    index = f"{stage.name}.{database}.{table.table}"
+                    self.tables_index[index] = table
+
     def _load_index(self):
+        """
+        Parse through the table definitions dictionary and deserialize it
+        into Table objects. The table object are then place in a dictionary for easy
+        lookup with a key = stage.database.table and the value being the table
+        object it self. This dictionary index is held on self.tables_index
+        """
         for stage in StageType:
-            stage_data = self.table_data.get(stage.name)
+            stage_data = self.table_data.get(stage)
             if stage_data:
-                stage_delta_properties = stage_data.get("delta_properties", {})
-
-                for database, tables in stage_data.items():
-                    if database == "delta_properties":
-                        continue
-
-                    for table, table_details in tables.items():
-                        # flatten the config structure for a table
-                        if not table_details:
-                            table_details = {}
-                        delta_properties = table_details.get("delta_properties", {})
-                        # delta_properties = stage_delta_properties | delta_properties
-                        delta_properties = {
-                            **stage_delta_properties,
-                            **delta_properties,
-                        }
-                        table_details["name"] = table
-                        table_details["database"] = database
-                        table_details["stage"] = stage
-                        if delta_properties:
-                            table_details["delta_properties"] = delta_properties
-
-                        # create a table object
-                        table = Table(**table_details)
-
-                        # index the table object
-                        index = f"{stage.name}.{database}.{table.name}"
-                        self.tables_index[index] = table
+                self._parse_stage_data(stage, stage_data)
 
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
@@ -140,15 +189,15 @@
                 do_stage, do_database, do_table = Tables.parse_index(index)
                 table = self.lookup_table(
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
                     first_match=True,
                 )
-                source[table.name] = table
+                source[table.table] = table
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
         if len(list(source.values())) == 1:
             source = list(source.values())[0]
 
         return TableMapping(source=source, destination=destination)
```

### Comparing `dbxconfig-2.4.0/dbxconfig/_timeslice.py` & `dbxconfig-4.0.3/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.4.0/dbxconfig/dataset/_deltalake.py` & `dbxconfig-4.0.3/dbxconfig/dataset/_deltalake.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 import logging
 from pydantic import Field, PrivateAttr
-from .._utils import JinjaVariables, render_jinja
-from typing import Any, Dict, Union
+from .._utils import JinjaVariables, render_jinja, is_databricks
+from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 import os
 from .._stage_type import StageType
-from ._dataset import DataSet
-from .._table import ValidationThreshold
+from ._dataset import DataSet, Table
+from ..datallake import create_database, create_table
 
-try:
-    from databricks.sdk.runtime import *  # noqa F403
-except ModuleNotFoundError:
-    pass
+# try:
+#     from databricks.sdk.runtime import *  # noqa F403
+# except ModuleNotFoundError:
+#     pass
 
 
-class DeltaLake(DataSet):
+class DeltaLakeTable(Table):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+    depends_on: List[str] = Field(default=[])
+    delta_properties: Dict[str, str] = Field(default=None)
+    delta_constraints: Dict[str, str] = Field(default=None)
+    partition_by: List[str] = Field(default=None)
+    z_order_by: List[str] = Field(default=None)
+    create_table: bool = Field(default=True)
+    managed: bool = Field(default=False)
+
+
+class DeltaLake(DataSet, DeltaLakeTable):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
-        self.create_table()
+        self.create_delta_table()
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
-    database: str = Field(...)
-    destination_table: str = Field(...)
-    table: str = Field(...)
-    container: str = Field(...)
-    root: str = Field(...)
-    path: str = Field(...)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
-    checkpoint: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
-    delta_properties: Dict[str, str] = Field(default=None)
     stage: StageType = Field(...)
-    warning_thresholds: ValidationThreshold = Field(default=None)
-    exception_thresholds: ValidationThreshold = Field(default=None)
+    managed: bool = Field(default=False)
+    create_table: bool = Field(default=True)
 
     def _render(self):
         self._replacements = {
-            JinjaVariables.TABLE: self.destination_table,
+            JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
 
         self.root = render_jinja(self.root, self._replacements)
         self.path = render_jinja(self.path, self._replacements)
         self.database = render_jinja(self.database, self._replacements)
         self.table = render_jinja(self.table, self._replacements)
         if self.options:
             for option, value in self.options.items():
                 self.options[option] = render_jinja(value, self._replacements)
 
         self.location = os.path.join(self.root, self.path)
-
-    def create_table(self):
-        table_ddl = f"""
-            CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
-            USING DELTA
-            LOCATION '{self.location}'
-        """
-        # add in the delta properties if there are any
-        if self.delta_properties:
-            tbl_properties = [
-                f"{k.lower()} = {v.lower()}" for k, v in self.delta_properties.items()
-            ]
-            tbl_properties = ", ".join(tbl_properties)
-            table_ddl = f"""{table_ddl}
-            TBLPROPERTIES({tbl_properties})
-            """
-        try:
-            spark.sql(f"CREATE DATABASE IF NOT EXISTS `{self.database}`")  # noqa F821
-            spark.sql(table_ddl)  # noqa F821
-        except NameError:
-            version = os.getenv("DATABRICKS_RUNTIME_VERSION", None)
-            if version:
-                raise Exception("Spark undefined on databricks runtime!")
-            logging.warning(
-                "spark is not defined, skipping Spark operation for testing purposes"
+        if not is_databricks():
+            self.location = f"{self.config_path}/../data{self.location}"
+            self.location = os.path.abspath(self.location)
+
+    def create_delta_table(self):
+        database_table = f"`{self.database}`.`{self.table}`"
+        self._logger.info(f"Creating delta lake table {database_table}")
+        create_database(self.database)
+
+        if self.managed:
+            create_table(
+                database=self.database,
+                table=self.table,
+                delta_properties=self.delta_properties,
+            )
+        else:
+            create_table(
+                database=self.database,
+                table=self.table,
+                delta_properties=self.delta_properties,
+                path=self.location,
             )
```

### Comparing `dbxconfig-2.4.0/dbxconfig/dataset/_read.py` & `dbxconfig-4.0.3/dbxconfig/dataset/_read.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 import logging
-from pydantic import Field, PrivateAttr
+from pydantic import Field, PrivateAttr, BaseModel
 from .._utils import JinjaVariables, render_jinja, get_ddl, load_schema, abs_config_path
 from typing import Any, Dict, List, Union
-from .._timeslice import Timeslice
 from enum import Enum
 import os
 from pyspark.sql.types import StructType
 from pyspark.sql.streaming import StreamingQuery
 from pyspark.sql import DataFrame
 from .._stage_type import StageType
-from ._dataset import DataSet
+from ._dataset import DataSet, Table
 
 
 class TriggerType(Enum):
     File = "file"
 
 
-class Read(DataSet):
+class ValidationThreshold(BaseModel):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+    invalid_ratio: float = Field(default=None)
+    invalid_rows: int = Field(default=None)
+    max_rows: int = Field(default=None)
+    min_rows: int = Field(default=None)
+
+
+class ReadTable(Table):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+    warning_thresholds: ValidationThreshold = Field(default=None)
+    exception_thresholds: ValidationThreshold = Field(default=None)
+    create_table: bool = Field(default=True)
+    managed: bool = Field(default=False)
+
+
+class Read(DataSet, ReadTable):
     _OPTION_CF_SCHEMA_HINTS = "cloudFiles.schemaHints"
     _OPTION_CORRUPT_RECORD_NAME = "columnNameOfCorruptRecord"
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
         self.path = os.path.join(self.root, self.filename)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     trigger: str = Field(default=None)
     trigger_type: TriggerType = Field(default=None)
-    database: str = Field(...)
-    destination_table: str = Field(...)
-    table: str = Field(...)
-    container: str = Field(...)
-    root: str = Field(...)
     filename: str = Field(...)
     filename_date_format: str = Field(...)
     path_date_format: str = Field(...)
-    options: dict = Field(...)
-    timeslice: Timeslice = Field(...)
     format: str = Field(...)
-    path: str = Field(default=None)
     spark_schema: Union[StructType, str] = Field(default=None)
     ddl: List[str] = Field(default=None)
     headerless_ddl: List[str] = Field(default=None)
-    checkpoint: str = Field(default=None)
     stage: StageType = Field(...)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.FILENAME_DATE_FORMAT: self.timeslice.strftime(
                 self.filename_date_format
             ),
             JinjaVariables.PATH_DATE_FORMAT: self.timeslice.strftime(
                 self.path_date_format
             ),
-            JinjaVariables.TABLE: self.destination_table,
+            JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
 
         self.root = render_jinja(self.root, self._replacements)
         self.filename = render_jinja(self.filename, self._replacements)
```

### Comparing `dbxconfig-2.4.0/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-4.0.3/dbxconfig/workflow/_multi_threaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "status": "executing",
         "notebook": notebook.path,
     }
     print(msg["_message"], flush=True)
 
     try:
         result = dbutils.notebook.run(
-            notebook.path, notebook.timeout, notebook.get_parameters()
+            notebook.path, notebook.timeout, notebook.parameters
         )
         msg = {
             "_message": f"Succeeded notebook {notebook.path}",
             "status": "succeeded",
             "notebook": notebook.path,
         }
         print(msg["_message"], flush=True)
```

### Comparing `dbxconfig-2.4.0/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-4.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.4.0
+Version: 4.0.3
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
@@ -18,94 +18,117 @@
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
 landing:
-  landing_dbx_patterns:
-    customer_details_1: null
-    customer_details_2: null
+  read:
+    landing_dbx_patterns:
+      customer_details_1: null
+      customer_details_2: null
 
 raw:
-  raw_dbx_patterns:
-    customers:
-      ids: id
-      depends_on:
-        - landing.landing_dbx_patterns.customer_details_1
-        - landing.landing_dbx_patterns.customer_details_2
-      warning_thresholds:
-        invalid_ratio: 0.1
-        invalid_rows: 0
-        max_rows: 100
-        min_rows: 5
-      exception_thresholds:
-        invalid_ratio: 0.2
-        invalid_rows: 2
-        max_rows: 1000
-        min_rows: 0
+  delta_lake:
+    raw_dbx_patterns:
+      customers:
+        ids: id
+        depends_on:
+          - landing.landing_dbx_patterns.customer_details_1
+          - landing.landing_dbx_patterns.customer_details_2
+        warning_thresholds:
+          invalid_ratio: 0.1
+          invalid_rows: 0
+          max_rows: 100
+          min_rows: 5
+        exception_thresholds:
+          invalid_ratio: 0.2
+          invalid_rows: 2
+          max_rows: 1000
+          min_rows: 0
+        custom_properties:
+          process_group: 1
 
 base:
-  base_dbx_patterns:
-    customer_details_1:
-      ids: id
-      depends_on:
-        - raw.raw_dbx_patterns.customers
-    customer_details_2:
-      ids: id
-      depends_on:
-        - raw.raw_dbx_patterns.customers
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+      delta.appendOnly: true
+      delta.autoOptimize.autoCompact: true    
+      delta.autoOptimize.optimizeWrite: true  
+      delta.enableChangeDataFeed: false
+    base_dbx_patterns:
+      customer_details_1:
+        ids: id
+        depends_on:
+          - raw.raw_dbx_patterns.customers
+        # delta table properties can be set at stage level or table level
+        # table level properties will overwride stage level properties
+        delta_properties:
+            delta.enableChangeDataFeed: true
+      customer_details_2:
+        ids: id
+        depends_on:
+          - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
 tables: ./tables.yaml
 
 landing:
-  trigger: customerdetailscomplete-{{filename_date_format}}*.flg
-  trigger_type: file
-  database: landing_dbx_patterns
-  table: "{{table}}"
-  container: datalake
-  root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
-  filename: "{{table}}-{{filename_date_format}}*.csv"
-  filename_date_format: "%Y%m%d"
-  path_date_format: "%Y%m%d"
-  format: cloudFiles
-  spark_schema: ../Schema/{{table.lower()}}.yaml
-  options:
-    # autoloader
-    cloudFiles.format: csv
-    cloudFiles.schemaLocation:  "/mnt/{{container}}/checkpoint/{{checkpoint}}"
-    cloudFiles.useIncrementalListing: auto
-    # schema
-    inferSchema: false
-    enforceSchema: true
-    columnNameOfCorruptRecord: _corrupt_record
-    # csv
-    header: false
-    mode: PERMISSIVE
-    encoding: windows-1252
-    delimiter: ","
-    escape: '"'
-    nullValue: ""
-    quote: '"'
-    emptyValue: ""
+  read:
+    trigger: customerdetailscomplete-{{filename_date_format}}*.flg
+    trigger_type: file
+    database: landing_dbx_patterns
+    table: "{{table}}"
+    container: datalake
+    root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
+    filename: "{{table}}-{{filename_date_format}}*.csv"
+    filename_date_format: "%Y%m%d"
+    path_date_format: "%Y%m%d"
+    format: cloudFiles
+    spark_schema: ../Schema/{{table.lower()}}.yaml
+    options:
+      # autoloader
+      cloudFiles.format: csv
+      cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
+      cloudFiles.useIncrementalListing: auto
+      # schema
+      inferSchema: false
+      enforceSchema: true
+      columnNameOfCorruptRecord: _corrupt_record
+      # csv
+      header: false
+      mode: PERMISSIVE
+      encoding: windows-1252
+      delimiter: ","
+      escape: '"'
+      nullValue: ""
+      quote: '"'
+      emptyValue: ""
     
 
 raw:
-  database: raw_dbx_patterns
-  table: "{{table}}"
-  container: datalake
-  root: /mnt/{{container}}/data/raw
-  path: "{{database}}/{{table}}"
-  checkpoint_location: /mnt/{{container}}/checkpoint/{{checkpoint}}
-  options:
-    mergeSchema: true
+  delta_lake:
+    # delta table properties can be set at stage level or table level
+    delta_properties:
+      delta.appendOnly: true
+      delta.autoOptimize.autoCompact: true    
+      delta.autoOptimize.optimizeWrite: true  
+      delta.enableChangeDataFeed: false
+    database: raw_dbx_patterns
+    table: "{{table}}"
+    container: datalake
+    root: /mnt/{{container}}/data/raw
+    path: "{{database}}/{{table}}"
+    options:
+      checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
+      mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from dbxconfig import Config, Timeslice, StageType
```

### Comparing `dbxconfig-2.4.0/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-4.0.3/dbxconfig.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 README.md
 setup.py
 dbxconfig/__init__.py
 dbxconfig/_config.py
+dbxconfig/_decorators.py
+dbxconfig/_logging_config.py
+dbxconfig/_spark_context.py
 dbxconfig/_stage_type.py
-dbxconfig/_table.py
+dbxconfig/_table_mapping.py
 dbxconfig/_tables.py
 dbxconfig/_timeslice.py
 dbxconfig/_utils.py
+dbxconfig/datallake.py
 dbxconfig.egg-info/PKG-INFO
 dbxconfig.egg-info/SOURCES.txt
 dbxconfig.egg-info/dependency_links.txt
 dbxconfig.egg-info/not-zip-safe
 dbxconfig.egg-info/requires.txt
 dbxconfig.egg-info/top_level.txt
 dbxconfig/dataset/__init__.py
 dbxconfig/dataset/_dataset.py
 dbxconfig/dataset/_deltalake.py
 dbxconfig/dataset/_factory.py
 dbxconfig/dataset/_read.py
 dbxconfig/dataset/_write.py
+dbxconfig/dataset/dataset_type.py
 dbxconfig/workflow/__init__.py
 dbxconfig/workflow/_multi_threaded.py
 dbxconfig/workflow/_notebook.py
```

### Comparing `dbxconfig-2.4.0/setup.py` & `dbxconfig-4.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.4.0",
+    version="4.0.3",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

