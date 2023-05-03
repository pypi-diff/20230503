# Comparing `tmp/flytekitplugins-spark-1.6.0b0.tar.gz` & `tmp/flytekitplugins-spark-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-spark-1.6.0b0.tar", last modified: Wed Apr 19 20:54:35 2023, max compression
+gzip compressed data, was "flytekitplugins-spark-1.6.0b1.tar", last modified: Wed May  3 04:48:12 2023, max compression
```

## Comparing `flytekitplugins-spark-1.6.0b0.tar` & `flytekitplugins-spark-1.6.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/pyspark_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/sd_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-19 20:54:06.000000 flytekitplugins-spark-1.6.0b0/scripts/flytekit_install_spark3.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:35.503163 flytekitplugins-spark-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-19 20:54:25.000000 flytekitplugins-spark-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.976322 flytekitplugins-spark-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/pyspark_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/sd_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:12.000000 flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-03 04:47:44.000000 flytekitplugins-spark-1.6.0b1/scripts/flytekit_install_spark3.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:12.980322 flytekitplugins-spark-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 04:48:03.000000 flytekitplugins-spark-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-spark-1.6.0b0/PKG-INFO` & `flytekitplugins-spark-1.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b0/README.md` & `flytekitplugins-spark-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/__init__.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/models.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/pyspark_transformers.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/pyspark_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/schema.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/sd_transformers.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins/spark/task.py` & `flytekitplugins-spark-1.6.0b1/flytekitplugins/spark/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/PKG-INFO` & `flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b0/flytekitplugins_spark.egg-info/SOURCES.txt` & `flytekitplugins-spark-1.6.0b1/flytekitplugins_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/scripts/flytekit_install_spark3.sh` & `flytekitplugins-spark-1.6.0b1/scripts/flytekit_install_spark3.sh`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b0/setup.py` & `flytekitplugins-spark-1.6.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "spark"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pyspark>=3.0.0"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Spark 3 plugin for flytekit",
```
