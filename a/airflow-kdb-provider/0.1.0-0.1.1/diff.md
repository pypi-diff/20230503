# Comparing `tmp/airflow-kdb-provider-0.1.0.tar.gz` & `tmp/airflow-kdb-provider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-kdb-provider-0.1.0.tar", last modified: Wed May  3 06:22:38 2023, max compression
+gzip compressed data, was "dist/airflow-kdb-provider-0.1.1.tar", last modified: Wed May  3 06:45:01 2023, max compression
```

## Comparing `airflow-kdb-provider-0.1.0.tar` & `airflow-kdb-provider-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:22:38.461564 airflow-kdb-provider-0.1.0/
--rw-r--r--   0 kabir      (501) staff       (20)      466 2023-05-03 06:22:38.461376 airflow-kdb-provider-0.1.0/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)     2185 2023-05-03 00:16:47.000000 airflow-kdb-provider-0.1.0/README.md
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:22:38.459548 airflow-kdb-provider-0.1.0/airflow_kdb_provider/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider/__init__.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:22:38.460781 airflow-kdb-provider-0.1.0/airflow_kdb_provider/operators/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider/operators/__init__.py
--rw-r--r--   0 kabir      (501) staff       (20)      869 2023-05-03 00:10:53.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider/operators/kdb_operator.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:22:38.460435 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/
--rw-r--r--   0 kabir      (501) staff       (20)      466 2023-05-03 06:22:38.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)      360 2023-05-03 06:22:38.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/SOURCES.txt
--rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-03 06:22:38.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/dependency_links.txt
--rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-03 06:22:38.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/requires.txt
--rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-03 06:22:38.000000 airflow-kdb-provider-0.1.0/airflow_kdb_provider.egg-info/top_level.txt
--rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-03 06:22:38.461630 airflow-kdb-provider-0.1.0/setup.cfg
--rw-r--r--   0 kabir      (501) staff       (20)      594 2023-05-03 00:16:51.000000 airflow-kdb-provider-0.1.0/setup.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.745568 airflow-kdb-provider-0.1.1/
+-rw-r--r--   0 kabir      (501) staff       (20)    11358 2023-05-03 00:16:45.000000 airflow-kdb-provider-0.1.1/LICENSE
+-rw-r--r--   0 kabir      (501) staff       (20)     3140 2023-05-03 06:45:01.745083 airflow-kdb-provider-0.1.1/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)     2185 2023-05-03 00:16:47.000000 airflow-kdb-provider-0.1.1/README.md
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.742706 airflow-kdb-provider-0.1.1/airflow_kdb_provider/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/__init__.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.743768 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/__init__.py
+-rw-r--r--   0 kabir      (501) staff       (20)      869 2023-05-03 00:10:53.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/kdb_operator.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.743475 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/
+-rw-r--r--   0 kabir      (501) staff       (20)     3140 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)      368 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/requires.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/top_level.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-03 06:45:01.745690 airflow-kdb-provider-0.1.1/setup.cfg
+-rw-r--r--   0 kabir      (501) staff       (20)      800 2023-05-03 06:43:42.000000 airflow-kdb-provider-0.1.1/setup.py
```

### Comparing `airflow-kdb-provider-0.1.0/README.md` & `airflow-kdb-provider-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.0/airflow_kdb_provider/operators/kdb_operator.py` & `airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/kdb_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.0/setup.py` & `airflow-kdb-provider-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from setuptools import find_packages, setup
 
+# Read the README.md content
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='airflow-kdb-provider',
-    version='0.1.0',
+    version='0.1.1',
     description='Apache Airflow provider for KDBAirflowOperator',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Kabir Jaiswal',
     author_email='kabirjaiswal30@gmail.com',
     license='Apache License 2.0',
     packages=find_packages(),
     install_requires=[
         'apache-airflow>=2.0.0',
     ],
```

