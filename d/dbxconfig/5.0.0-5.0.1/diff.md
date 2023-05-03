# Comparing `tmp/dbxconfig-5.0.0.tar.gz` & `tmp/dbxconfig-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-5.0.0.tar", last modified: Wed May  3 20:47:28 2023, max compression
+gzip compressed data, was "dbxconfig-5.0.1.tar", last modified: Wed May  3 20:56:10 2023, max compression
```

## Comparing `dbxconfig-5.0.0.tar` & `dbxconfig-5.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.339682 dbxconfig-5.0.0/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3161 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4339 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/datallake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/dataset/dataset_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:47:28.339682 dbxconfig-5.0.0/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 20:47:28.000000 dbxconfig-5.0.0/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 20:47:28.343682 dbxconfig-5.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 20:46:37.000000 dbxconfig-5.0.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:56:10.366899 dbxconfig-5.0.1/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3161 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4339 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 20:56:10.000000 dbxconfig-5.0.1/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 20:56:10.370899 dbxconfig-5.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 20:55:12.000000 dbxconfig-5.0.1/setup.py
```

### Comparing `dbxconfig-5.0.0/PKG-INFO` & `dbxconfig-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.0
+Version: 5.0.1
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.0/README.md` & `dbxconfig-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_config.py` & `dbxconfig-5.0.1/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_decorators.py` & `dbxconfig-5.0.1/dbxconfig/_decorators.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_logging_config.py` & `dbxconfig-5.0.1/dbxconfig/_logging_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_project.py` & `dbxconfig-5.0.1/dbxconfig/_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,12 +41,12 @@
             self.config_path, self.databricks_queries.replace("./", "")
         )
 
     config_path: str = Field(...)
     name: str = Field(...)
     sql: str = Field(default="./sql")
     pipelines: str = Field(default="./pipelines")
-    databricks_notebooks: str = Field(default="./Databricks/Notebooks")
-    databricks_workflows: str = Field(default="./Databricks/Workflows")
-    databricks_queries: str = Field(default="./Databricks/Queries")
+    databricks_notebooks: str = Field(default="./databricks/notebooks")
+    databricks_workflows: str = Field(default="./databricks/workflows")
+    databricks_queries: str = Field(default="./databricks/queries")
 
     spark: SparkConfig = Field(default=SparkConfig())
```

### Comparing `dbxconfig-5.0.0/dbxconfig/_spark_context.py` & `dbxconfig-5.0.1/dbxconfig/_spark_context.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_tables.py` & `dbxconfig-5.0.1/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_timeslice.py` & `dbxconfig-5.0.1/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/_utils.py` & `dbxconfig-5.0.1/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/datallake.py` & `dbxconfig-5.0.1/dbxconfig/datallake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/dataset/_dataset.py` & `dbxconfig-5.0.1/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/dataset/_deltalake.py` & `dbxconfig-5.0.1/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/dataset/_factory.py` & `dbxconfig-5.0.1/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/dataset/_read.py` & `dbxconfig-5.0.1/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-5.0.1/dbxconfig/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-5.0.1/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.0
+Version: 5.0.1
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.0/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-5.0.1/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.0/setup.py` & `dbxconfig-5.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="5.0.0",
+    version="5.0.1",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

