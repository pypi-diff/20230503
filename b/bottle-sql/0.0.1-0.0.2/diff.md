# Comparing `tmp/bottle_sql-0.0.1.tar.gz` & `tmp/bottle_sql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bottle_sql-0.0.1.tar", last modified: Tue May  2 04:46:28 2023, max compression
+gzip compressed data, was "/home/renningert/workspace/bottle-plugins/bottle-sql/dist/.tmp-b7mew671/bottle_sql-0.0.2.tar", last modified: Wed May  3 19:34:45 2023, max compression
```

## Comparing `bottle_sql-0.0.1.tar` & `bottle_sql-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     1068 2023-05-01 22:46:58.000000 bottle_sql-0.0.1/LICENSE.txt
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     1055 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/PKG-INFO
--rw-rw-r--   0 renningert  (1000) renningert  (1000)      682 2023-05-02 03:58:13.000000 bottle_sql-0.0.1/README.md
--rw-rw-r--   0 renningert  (1000) renningert  (1000)      471 2023-05-02 04:20:10.000000 bottle_sql-0.0.1/pyproject.toml
--rw-rw-r--   0 renningert  (1000) renningert  (1000)       38 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/setup.cfg
-drwxrwxr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-02 04:46:28.269220 bottle_sql-0.0.1/src/
-drwxrwxr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/src/bottle_sql/
--rw-rw-r--   0 renningert  (1000) renningert  (1000)       25 2023-05-01 22:46:58.000000 bottle_sql-0.0.1/src/bottle_sql/__init__.py
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     3467 2023-05-02 00:29:24.000000 bottle_sql-0.0.1/src/bottle_sql/bottle_sql.py
-drwxrwxr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/src/bottle_sql.egg-info/
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     1055 2023-05-02 04:46:28.000000 bottle_sql-0.0.1/src/bottle_sql.egg-info/PKG-INFO
--rw-rw-r--   0 renningert  (1000) renningert  (1000)      320 2023-05-02 04:46:28.000000 bottle_sql-0.0.1/src/bottle_sql.egg-info/SOURCES.txt
--rw-rw-r--   0 renningert  (1000) renningert  (1000)        1 2023-05-02 04:46:28.000000 bottle_sql-0.0.1/src/bottle_sql.egg-info/dependency_links.txt
--rw-rw-r--   0 renningert  (1000) renningert  (1000)        7 2023-05-02 04:46:28.000000 bottle_sql-0.0.1/src/bottle_sql.egg-info/requires.txt
--rw-rw-r--   0 renningert  (1000) renningert  (1000)       11 2023-05-02 04:46:28.000000 bottle_sql-0.0.1/src/bottle_sql.egg-info/top_level.txt
-drwxrwxr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-02 04:46:28.273220 bottle_sql-0.0.1/tests/
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     1674 2023-05-02 01:13:18.000000 bottle_sql-0.0.1/tests/test_sql.py
--rw-rw-r--   0 renningert  (1000) renningert  (1000)     1637 2023-05-01 22:46:58.000000 bottle_sql-0.0.1/tests/test_sqlite.py
+drwxr-xr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     1068 2023-05-01 14:38:47.000000 bottle_sql-0.0.2/LICENSE.txt
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     1078 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/PKG-INFO
+-rw-r--r--   0 renningert  (1000) renningert  (1000)      706 2023-05-02 15:31:51.000000 bottle_sql-0.0.2/README.md
+-rw-r--r--   0 renningert  (1000) renningert  (1000)      483 2023-05-03 19:33:01.000000 bottle_sql-0.0.2/pyproject.toml
+-rw-r--r--   0 renningert  (1000) renningert  (1000)       38 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/setup.cfg
+drwxr-xr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/src/
+drwxr-xr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/src/bottle_sql/
+-rw-r--r--   0 renningert  (1000) renningert  (1000)       25 2023-05-01 15:45:53.000000 bottle_sql-0.0.2/src/bottle_sql/__init__.py
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     3523 2023-05-02 15:31:20.000000 bottle_sql-0.0.2/src/bottle_sql/bottle_sql.py
+drwxr-xr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/src/bottle_sql.egg-info/
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     1078 2023-05-03 19:34:45.000000 bottle_sql-0.0.2/src/bottle_sql.egg-info/PKG-INFO
+-rw-r--r--   0 renningert  (1000) renningert  (1000)      320 2023-05-03 19:34:45.000000 bottle_sql-0.0.2/src/bottle_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 renningert  (1000) renningert  (1000)        1 2023-05-03 19:34:45.000000 bottle_sql-0.0.2/src/bottle_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 renningert  (1000) renningert  (1000)       15 2023-05-03 19:34:45.000000 bottle_sql-0.0.2/src/bottle_sql.egg-info/requires.txt
+-rw-r--r--   0 renningert  (1000) renningert  (1000)       11 2023-05-03 19:34:45.000000 bottle_sql-0.0.2/src/bottle_sql.egg-info/top_level.txt
+drwxr-xr-x   0 renningert  (1000) renningert  (1000)        0 2023-05-03 19:34:45.929390 bottle_sql-0.0.2/tests/
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     1674 2023-05-02 15:30:15.000000 bottle_sql-0.0.2/tests/test_sql.py
+-rw-r--r--   0 renningert  (1000) renningert  (1000)     1637 2023-05-01 20:48:39.000000 bottle_sql-0.0.2/tests/test_sqlite.py
```

### Comparing `bottle_sql-0.0.1/LICENSE.txt` & `bottle_sql-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bottle_sql-0.0.1/PKG-INFO` & `bottle_sql-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bottle_sql
-Version: 0.0.1
+Version: 0.0.2
 Summary: SQL plugin for Bottle
 Author-email: TJ Renninger <renninger12@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # BottleSQL
 SQL plugin for Bottle. Supports MySQL/MariaDB and SQLite.
 
 ## Installation
 ### PyPi
 ``` bash
-pip install <TODO>
+pip install pip install bottle-sql==0.0.1
 ```
 ### Source
 ```bash
 wget https://raw.githubusercontent.com/thepure12/bottle-sql/main/src/bottle_sql/bottle_sql.py
 ```
 
 ## Usage
```

### Comparing `bottle_sql-0.0.1/README.md` & `bottle_sql-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BottleSQL
 SQL plugin for Bottle. Supports MySQL/MariaDB and SQLite.
 
 ## Installation
 ### PyPi
 ``` bash
-pip install <TODO>
+pip install pip install bottle-sql==0.0.1
 ```
 ### Source
 ```bash
 wget https://raw.githubusercontent.com/thepure12/bottle-sql/main/src/bottle_sql/bottle_sql.py
 ```
 
 ## Usage
@@ -28,8 +28,8 @@
 from bottle import Bottle
 from bottle_sql import sqlitePlugin
 
 app = Bottle()
 dbfile= ":memory:"
 sql_plugin = sqlitePlugin(dbfile)
 app.install(sql_plugin)
-```
+```
```

### Comparing `bottle_sql-0.0.1/src/bottle_sql/bottle_sql.py` & `bottle_sql-0.0.2/src/bottle_sql/bottle_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,17 +100,20 @@
                 conn.close()
             return rv
 
         return wrapper
 
 
 def sqlPlugin(
-    user=None, password="", host=None, database=None, dictcursor=True
+    user=None, password="", host=None, database=None, dictrows=True
 ) -> SQLPlugin:
     return SQLPlugin(
         Engine.SQL,
         {"user": user, "password": password, "host": host, "database": database},
+        dictrows=dictrows,
     )
 
 
-def sqlitePlugin(database, dictcursor=True) -> SQLPlugin:
-    return SQLPlugin(Engine.SQLITE, sql_config={"database": database})
+def sqlitePlugin(database, dictrows=True) -> SQLPlugin:
+    return SQLPlugin(
+        Engine.SQLITE, sql_config={"database": database}, dictrows=dictrows
+    )
```

### Comparing `bottle_sql-0.0.1/src/bottle_sql.egg-info/PKG-INFO` & `bottle_sql-0.0.2/src/bottle_sql.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bottle-sql
-Version: 0.0.1
+Version: 0.0.2
 Summary: SQL plugin for Bottle
 Author-email: TJ Renninger <renninger12@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # BottleSQL
 SQL plugin for Bottle. Supports MySQL/MariaDB and SQLite.
 
 ## Installation
 ### PyPi
 ``` bash
-pip install <TODO>
+pip install pip install bottle-sql==0.0.1
 ```
 ### Source
 ```bash
 wget https://raw.githubusercontent.com/thepure12/bottle-sql/main/src/bottle_sql/bottle_sql.py
 ```
 
 ## Usage
```

### Comparing `bottle_sql-0.0.1/tests/test_sql.py` & `bottle_sql-0.0.2/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `bottle_sql-0.0.1/tests/test_sqlite.py` & `bottle_sql-0.0.2/tests/test_sqlite.py`

 * *Files identical despite different names*

