# Comparing `tmp/pfstools-0.2.2.tar.gz` & `tmp/pfstools-0.2.3.tar.gz`

## Comparing `pfstools-0.2.2.tar` & `pfstools-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pfstools-0.2.2/requirements.txt
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pfstools-0.2.2/testing.ipynb
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pfstools-0.2.2/pfstools/__init__.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 pfstools-0.2.2/pfstools/output.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 pfstools-0.2.2/pfstools/sql.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pfstools-0.2.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pfstools-0.2.2/LICENSE
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pfstools-0.2.2/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pfstools-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 pfstools-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pfstools-0.2.3/requirements.txt
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pfstools-0.2.3/testing.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/__init__.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/output.py
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/sql.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/tools.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pfstools-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pfstools-0.2.3/LICENSE
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pfstools-0.2.3/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pfstools-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 pfstools-0.2.3/PKG-INFO
```

### Comparing `pfstools-0.2.2/pfstools/output.py` & `pfstools-0.2.3/pfstools/output.py`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.2/pfstools/sql.py` & `pfstools-0.2.3/pfstools/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         db : 'str' =''):
 
 
         with self.connection() as con:
             if isinstance(sql, str):
                 sql = [sql]
             for q in list(sql):
-                con.execute(q)
+                con.execute(text(q))
  
     def __exit__(self):
         if not self.cnx is None:
             self.cnx.close()
 
 
     def to_sql(self,
```

### Comparing `pfstools-0.2.2/.gitignore` & `pfstools-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.2/LICENSE` & `pfstools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.2/pyproject.toml` & `pfstools-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pfstools"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Jake Bridge", email="bridge.jake@gmail.com" },
 ]
 description = "Tools for my regular use. Particular to my work environment: SQL Server with Windows authentication"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pfstools-0.2.2/PKG-INFO` & `pfstools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfstools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tools for my regular use. Particular to my work environment: SQL Server with Windows authentication
 Project-URL: Homepage, https://github.com/jakeb/pfs-data-tools
 Project-URL: Bug Tracker, https://github.com/jakeb/pfs-data-tools/issues
 Author-email: Jake Bridge <bridge.jake@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

