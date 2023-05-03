# Comparing `tmp/dbt-redshift-1.5.0rc1.tar.gz` & `tmp/dbt-redshift-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.5.0rc1.tar", last modified: Fri Apr 14 21:19:22 2023, max compression
+gzip compressed data, was "dbt-redshift-1.5.1.tar", last modified: Wed May  3 17:50:00 2023, max compression
```

## Comparing `dbt-redshift-1.5.0rc1.tar` & `dbt-redshift-1.5.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.484236 dbt-redshift-1.5.0rc1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.484236 dbt-redshift-1.5.0rc1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.488236 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 21:19:22.000000 dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:19:22.492236 dbt-redshift-1.5.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-14 21:19:11.000000 dbt-redshift-1.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/setup.py
```

### Comparing `dbt-redshift-1.5.0rc1/LICENSE.md` & `dbt-redshift-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/PKG-INFO` & `dbt-redshift-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0rc1 Summary: The
-Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
-redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.1 Summary: The Redshift
+adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
+Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.5.0rc1/README.md` & `dbt-redshift-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.5.1/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.5.1/dbt/adapters/redshift/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,43 +3,59 @@
 from contextlib import contextmanager
 from typing import NewType, Tuple, Union, Optional, List
 from dataclasses import dataclass, field
 
 import agate
 import sqlparse
 import redshift_connector
+import urllib.request
+import json
 from redshift_connector.utils.oids import get_datatype_name
 
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse, Connection, Credentials
 from dbt.events import AdapterLogger
 import dbt.exceptions
 import dbt.flags
 from dbt.dataclass_schema import FieldEncoder, dbtClassMixin, StrEnum
 from dbt.helper_types import Port
 
-
 logger = AdapterLogger("Redshift")
 
-
 drop_lock: Lock = dbt.flags.MP_CONTEXT.Lock()  # type: ignore
 
-
 IAMDuration = NewType("IAMDuration", int)
 
 
 class IAMDurationEncoder(FieldEncoder):
     @property
     def json_schema(self):
         return {"type": "integer", "minimum": 0, "maximum": 65535}
 
 
 dbtClassMixin.register_field_encoders({IAMDuration: IAMDurationEncoder()})
 
 
+def _get_aws_regions():
+    # Extract the prefixes from the AWS IP ranges JSON to determine the available regions
+    url = "https://ip-ranges.amazonaws.com/ip-ranges.json"
+    response = urllib.request.urlopen(url)
+    data = json.loads(response.read().decode())
+    regions = set()
+
+    for prefix in data["prefixes"]:
+        if prefix["service"] == "AMAZON":
+            regions.add(prefix["region"])
+
+    return regions
+
+
+_AVAILABLE_AWS_REGIONS = _get_aws_regions()
+
+
 class RedshiftConnectionMethod(StrEnum):
     DATABASE = "database"
     IAM = "iam"
 
 
 @dataclass
 class RedshiftCredentials(Credentials):
@@ -56,14 +72,15 @@
     autocreate: bool = False
     db_groups: List[str] = field(default_factory=list)
     ra3_node: Optional[bool] = False
     connect_timeout: int = 30
     role: Optional[str] = None
     sslmode: Optional[str] = None
     retries: int = 1
+    region: Optional[str] = None  # if not provided, will be determined from host
 
     _ALIASES = {"dbname": "database", "pass": "password"}
 
     @property
     def type(self):
         return "redshift"
 
@@ -74,38 +91,64 @@
             "user",
             "database",
             "schema",
             "method",
             "cluster_id",
             "iam_profile",
             "sslmode",
+            "region",
         )
 
     @property
     def unique_field(self) -> str:
         return self.host
 
 
+def _is_valid_region(region):
+    if region is None or len(region) == 0:
+        logger.warning("Couldn't determine AWS regions. Skipping validation to avoid blocking.")
+        return True
+    return region in _AVAILABLE_AWS_REGIONS
+
+
 class RedshiftConnectMethodFactory:
     credentials: RedshiftCredentials
 
     def __init__(self, credentials):
         self.credentials = credentials
 
     def get_connect_method(self):
         method = self.credentials.method
         kwargs = {
             "host": self.credentials.host,
             "database": self.credentials.database,
             "port": self.credentials.port if self.credentials.port else 5439,
             "auto_create": self.credentials.autocreate,
             "db_groups": self.credentials.db_groups,
-            "region": self.credentials.host.split(".")[2],
+            "region": self.credentials.region,
             "timeout": self.credentials.connect_timeout,
         }
+        if kwargs["region"] is None:
+            logger.debug("No region provided, attempting to determine from host.")
+            try:
+                region_value = self.credentials.host.split(".")[2]
+            except IndexError:
+                raise dbt.exceptions.FailedToConnectError(
+                    "No region provided and unable to determine region from host: "
+                    "{}".format(self.credentials.host)
+                )
+
+            kwargs["region"] = region_value
+
+        # Validate the set region
+        if not _is_valid_region(kwargs["region"]):
+            raise dbt.exceptions.FailedToConnectError(
+                "Invalid region provided: {}".format(kwargs["region"])
+            )
+
         if self.credentials.sslmode:
             kwargs["sslmode"] = self.credentials.sslmode
 
         # Support missing 'method' for backwards compatibility
         if method == RedshiftConnectionMethod.DATABASE or method is None:
             # this requirement is really annoying to encode into json schema,
             # so validate it here
@@ -113,15 +156,17 @@
                 raise dbt.exceptions.FailedToConnectError(
                     "'password' field is required for 'database' credentials"
                 )
 
             def connect():
                 logger.debug("Connecting to redshift with username/password based auth...")
                 c = redshift_connector.connect(
-                    user=self.credentials.user, password=self.credentials.password, **kwargs
+                    user=self.credentials.user,
+                    password=self.credentials.password,
+                    **kwargs,
                 )
                 if self.credentials.role:
                     c.cursor().execute("set role {}".format(self.credentials.role))
                 return c
 
         elif method == RedshiftConnectionMethod.IAM:
             if not self.credentials.cluster_id and "serverless" not in self.credentials.host:
```

### Comparing `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.5.1/dbt/adapters/redshift/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.5.1/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.5.1/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.5.1/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.5.1/dbt_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.0rc1 Summary: The
-Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
-redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.1 Summary: The Redshift
+adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
+Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.5.0rc1/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.5.1/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.0rc1/setup.py` & `dbt-redshift-1.5.1/setup.py`

 * *Files identical despite different names*

