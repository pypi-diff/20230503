# Comparing `tmp/questdb-connect-0.0.34.tar.gz` & `tmp/questdb-connect-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.34.tar", last modified: Wed May  3 12:24:52 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.35.tar", last modified: Wed May  3 13:03:37 2023, max compression
```

## Comparing `questdb-connect-0.0.34.tar` & `questdb-connect-0.0.35.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 12:24:52.058012 questdb-connect-0.0.34/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.34/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-03 12:24:52.057860 questdb-connect-0.0.34/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3718 2023-05-03 11:11:17.000000 questdb-connect-0.0.34/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2510 2023-05-03 12:21:25.000000 questdb-connect-0.0.34/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-03 12:24:52.058047 questdb-connect-0.0.34/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 12:24:52.053941 questdb-connect-0.0.34/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 12:24:52.056027 questdb-connect-0.0.34/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1960 2023-05-03 09:57:40.000000 questdb-connect-0.0.34/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11566 2023-05-03 12:23:45.000000 questdb-connect-0.0.34/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.34/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.34/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.34/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 12:24:52.056978 questdb-connect-0.0.34/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-03 12:24:52.000000 questdb-connect-0.0.34/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 12:24:52.057572 questdb-connect-0.0.34/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.34/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.34/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.34/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 13:03:37.377445 questdb-connect-0.0.35/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.35/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-03 13:03:37.377314 questdb-connect-0.0.35/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3718 2023-05-03 11:11:17.000000 questdb-connect-0.0.35/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2510 2023-05-03 13:00:13.000000 questdb-connect-0.0.35/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-03 13:03:37.377480 questdb-connect-0.0.35/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 13:03:37.373021 questdb-connect-0.0.35/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 13:03:37.374786 questdb-connect-0.0.35/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1960 2023-05-03 09:57:40.000000 questdb-connect-0.0.35/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11566 2023-05-03 12:23:45.000000 questdb-connect-0.0.35/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.35/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10828 2023-05-03 13:03:25.000000 questdb-connect-0.0.35/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.35/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 13:03:37.376036 questdb-connect-0.0.35/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4425 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-03 13:03:37.000000 questdb-connect-0.0.35/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-03 13:03:37.376853 questdb-connect-0.0.35/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.35/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.35/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.35/tests/test_types.py
```

### Comparing `questdb-connect-0.0.34/LICENSE` & `questdb-connect-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/PKG-INFO` & `questdb-connect-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.34
+Version: 0.0.35
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.34/README.md` & `questdb-connect-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/pyproject.toml` & `questdb-connect-0.0.35/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.34"
+version = "0.0.35"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.34/src/questdb_connect/__init__.py` & `questdb-connect-0.0.35/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/src/questdb_connect/dialect.py` & `questdb-connect-0.0.35/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/src/questdb_connect/function_names.py` & `questdb-connect-0.0.35/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.35/src/questdb_connect/superset_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
+from superset.sql_parse import ParsedQuery
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
 
 from . import remove_public_schema, types
 from .function_names import FUNCTION_NAMES
 
+
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
@@ -47,14 +49,15 @@
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
     time_secondary_columns = True
     max_column_name_length = 120
     try_remove_schema_from_table_name = True
     supports_dynamic_schema = False
+    allow_dml = True
     _time_grain_expressions = {
         None: '{col}',
         'PT1S': "date_trunc('second', {col})",
         'PT5S': "date_trunc('second', {col}) + 5000000",
         'PT30S': "date_trunc('second', {col}) + 30000000",
         'PT1M': "date_trunc('minute', {col})",
         'PT5M': "date_trunc('minute', {col}) + 300000000",
@@ -244,7 +247,11 @@
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
+
+    @classmethod
+    def is_readonly_query(cls, parsed_query: ParsedQuery) -> bool:
+        return False
```

### Comparing `questdb-connect-0.0.34/src/questdb_connect/types.py` & `questdb-connect-0.0.35/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.35/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.34
+Version: 0.0.35
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.34/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.35/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/tests/test_dialect.py` & `questdb-connect-0.0.35/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/tests/test_superset.py` & `questdb-connect-0.0.35/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.34/tests/test_types.py` & `questdb-connect-0.0.35/tests/test_types.py`

 * *Files identical despite different names*

