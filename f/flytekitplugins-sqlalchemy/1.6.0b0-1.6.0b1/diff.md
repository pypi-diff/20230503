# Comparing `tmp/flytekitplugins-sqlalchemy-1.6.0b0.tar.gz` & `tmp/flytekitplugins-sqlalchemy-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-sqlalchemy-1.6.0b0.tar", last modified: Wed Apr 19 20:54:35 2023, max compression
+gzip compressed data, was "flytekitplugins-sqlalchemy-1.6.0b1.tar", last modified: Wed May  3 04:48:13 2023, max compression
```

## Comparing `flytekitplugins-sqlalchemy-1.6.0b0.tar` & `flytekitplugins-sqlalchemy-1.6.0b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.875169 flytekitplugins-sqlalchemy-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-19 20:54:35.875169 flytekitplugins-sqlalchemy-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 20:54:06.000000 flytekitplugins-sqlalchemy-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.871169 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.875169 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 20:54:06.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-19 20:54:06.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins/sqlalchemy/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.875169 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:35.875169 flytekitplugins-sqlalchemy-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-19 20:54:25.000000 flytekitplugins-sqlalchemy-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.336323 flytekitplugins-sqlalchemy-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 04:48:13.336323 flytekitplugins-sqlalchemy-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 04:47:44.000000 flytekitplugins-sqlalchemy-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.332323 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.332323 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 04:47:44.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-03 04:47:44.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins/sqlalchemy/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.332323 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:13.000000 flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:13.336323 flytekitplugins-sqlalchemy-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-03 04:48:03.000000 flytekitplugins-sqlalchemy-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b0/PKG-INFO` & `flytekitplugins-sqlalchemy-1.6.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b0/README.md` & `flytekitplugins-sqlalchemy-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins/sqlalchemy/task.py` & `flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins/sqlalchemy/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-sqlalchemy-1.6.0b0/flytekitplugins_sqlalchemy.egg-info/PKG-INFO` & `flytekitplugins-sqlalchemy-1.6.0b1/flytekitplugins_sqlalchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b0/setup.py` & `flytekitplugins-sqlalchemy-1.6.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "sqlalchemy"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "sqlalchemy>=1.4.7"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="dolthub",
     author_email="max@dolthub.com",
     description="SQLAlchemy plugin for flytekit",
```

