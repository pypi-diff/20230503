# Comparing `tmp/dbt-databricks-1.4.3.tar.gz` & `tmp/dbt-databricks-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.4.3.tar", last modified: Wed Apr 19 19:21:39 2023, max compression
+gzip compressed data, was "dbt-databricks-1.5.0rc1.tar", last modified: Tue May  2 22:21:00 2023, max compression
```

## Comparing `dbt-databricks-1.4.3.tar` & `dbt-databricks-1.5.0rc1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.070120 dbt-databricks-1.4.3/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/MANIFEST.in
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-04-19 19:21:39.069902 dbt-databricks-1.4.3/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-04-19 17:50:57.000000 dbt-databricks-1.4.3/README.md
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.011645 dbt-databricks-1.4.3/dbt/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.011375 dbt-databricks-1.4.3/dbt/adapters/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.029839 dbt-databricks-1.4.3/dbt/adapters/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       23 2023-04-19 19:10:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/column.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    21683 2023-04-19 17:28:05.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/connections.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    19036 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/impl.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    17435 2023-04-19 17:59:31.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/relation.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.012208 dbt-databricks-1.4.3/dbt/include/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.042760 dbt-databricks-1.4.3/dbt/include/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.051440 dbt-databricks-1.4.3/dbt/include/databricks/macros/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     9909 2023-04-19 17:58:37.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.057181 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.062347 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/seed.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.064714 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      475 2023-04-19 17:28:05.000000 dbt-databricks-1.4.3/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.069428 dbt-databricks-1.4.3/dbt_databricks.egg-info/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1389 2023-04-19 19:21:39.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-02-17 19:42:17.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 andre.furlan   (502) staff       (20)       49 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-04-19 19:21:39.070174 dbt-databricks-1.4.3/setup.cfg
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2538 2023-04-19 17:59:55.000000 dbt-databricks-1.4.3/setup.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.339738 dbt-databricks-1.5.0rc1/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5378 2023-05-02 22:21:00.339449 dbt-databricks-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/README.md
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.315986 dbt-databricks-1.5.0rc1/dbt/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.315626 dbt-databricks-1.5.0rc1/dbt/adapters/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.324968 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       25 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/column.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    26590 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.316267 dbt-databricks-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.326407 dbt-databricks-1.5.0rc1/dbt/include/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.329448 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    10178 2023-05-02 22:12:17.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.332059 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.333883 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/seed.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.335116 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.338739 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5378 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       88 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-05-02 22:21:00.339805 dbt-databricks-1.5.0rc1/setup.cfg
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2547 2023-05-02 22:12:17.000000 dbt-databricks-1.5.0rc1/setup.py
```

### Comparing `dbt-databricks-1.4.3/PKG-INFO` & `dbt-databricks-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.4.3
+Version: 1.5.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.4.3/README.md` & `dbt-databricks-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/column.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
             schema_relation = self.Relation.create(
                 database=database,
                 schema=schema,
                 identifier="|".join(table_names),
                 quote_policy=self.config.quoting,
             )
             for relation, information in self._list_relations_with_information(schema_relation):
-                logger.debug("Getting table schema for relation {}", relation)
+                logger.debug("Getting table schema for relation {}", str(relation))
                 columns.extend(self._get_columns_for_catalog(relation, information))
         return Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
 
     def _get_columns_for_catalog(  # type: ignore[override]
         self, relation: DatabricksRelation, information: str
     ) -> Iterable[Dict[str, Any]]:
         columns = self.parse_columns_from_information(relation, information)
```

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/python_submissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 import uuid
 
 from dbt.events import AdapterLogger
 import dbt.exceptions
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.spark import __version__
+from databricks.sdk.core import CredentialsProvider
 
 logger = AdapterLogger("Databricks")
 
 DEFAULT_POLLING_INTERVAL = 10
 SUBMISSION_LANGUAGE = "python"
 DEFAULT_TIMEOUT = 60 * 60 * 24
 DBT_SPARK_VERSION = __version__.version
@@ -377,14 +378,15 @@
                     )
             finally:
                 context.destroy(context_id)
 
 
 class DbtDatabricksBasePythonJobHelper(BaseDatabricksHelper):
     credentials: DatabricksCredentials  # type: ignore[assignment]
+    _credentials_provider: CredentialsProvider = None
 
     def __init__(self, parsed_model: Dict, credentials: DatabricksCredentials) -> None:
         super().__init__(
             parsed_model=parsed_model, credentials=credentials  # type: ignore[arg-type]
         )
 
         self.database = parsed_model.get("database")
@@ -396,16 +398,19 @@
             user_agent = f"{user_agent} ({invocation_env})"
 
         connection_parameters = credentials.connection_parameters.copy()  # type: ignore[union-attr]
 
         http_headers: Dict[str, str] = credentials.get_all_http_headers(
             connection_parameters.pop("http_headers", {})
         )
+        self._credentials_provider = credentials.authenticate(self._credentials_provider)
+        header_factory = self._credentials_provider()
+        headers = header_factory()
 
-        self.auth_header.update({"User-Agent": user_agent, **http_headers})
+        self.auth_header.update({"User-Agent": user_agent, **http_headers, **headers})
 
     @property
     def cluster_id(self) -> Optional[str]:  # type: ignore[override]
         return self.parsed_model["config"].get(
             "cluster_id",
             self.credentials.extract_cluster_id(
                 self.parsed_model["config"].get("http_path", self.credentials.http_path)
```

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,20 @@
 
 {# Persist table-level and column-level constraints. #}
 {% macro persist_constraints(relation, model) %}
   {{ return(adapter.dispatch('persist_constraints', 'dbt')(relation, model)) }}
 {% endmacro %}
 
 {% macro databricks__persist_constraints(relation, model) %}
+  {# Model contracts are not currently supported. #}
+  {%- set contract_config = config.get('contract') -%}
+  {% if contract_config and contract_config.enforced %}
+    {{ exceptions.raise_compiler_error('Model contracts are not currently supported.') }}
+  {% endif %}
+
   {% if config.get('persist_constraints', False) and config.get('file_format', 'delta') == 'delta' %}
     {% do alter_table_add_constraints(relation, model.meta.constraints) %}
     {% do alter_column_set_constraints(relation, model.columns) %}
   {% endif %}
 {% endmacro %}
 
 {% macro optimize(relation) %}
```

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/seed.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.3/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.4.3
+Version: 1.5.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.4.3/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 README.md
 setup.py
 dbt/adapters/databricks/__init__.py
 dbt/adapters/databricks/__version__.py
+dbt/adapters/databricks/auth.py
 dbt/adapters/databricks/column.py
 dbt/adapters/databricks/connections.py
 dbt/adapters/databricks/impl.py
 dbt/adapters/databricks/python_submissions.py
 dbt/adapters/databricks/relation.py
 dbt/adapters/databricks/utils.py
 dbt/include/databricks/__init__.py
```

### Comparing `dbt-databricks-1.4.3/setup.py` & `dbt-databricks-1.5.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,31 +36,32 @@
     except IOError:
         print("Failed to load dbt-databricks version file for packaging.", file=sys.stderr)
         sys.exit(-1)
 
 
 package_name = "dbt-databricks"
 package_version = _get_plugin_version()
-dbt_spark_version = "1.4.1"
 description = """The Databricks adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark~={}".format(dbt_spark_version),
+        "dbt-spark>=1.5.0",
         "databricks-sql-connector>=2.5.0",
+        "databricks-sdk>=0.1.1",
+        "keyring>=23.13.0"
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

