# Comparing `tmp/sparkmeasure-0.21.1.tar.gz` & `tmp/sparkmeasure-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkmeasure-0.21.1.tar", last modified: Mon Aug 22 08:41:43 2022, max compression
+gzip compressed data, was "sparkmeasure-0.23.0.tar", last modified: Wed May  3 09:25:32 2023, max compression
```

## Comparing `sparkmeasure-0.21.1.tar` & `sparkmeasure-0.23.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-08-22 08:41:43.995915 sparkmeasure-0.21.1/
--rw-r--r--   0 luca      (1000) luca      (1000)     1225 2022-08-22 08:41:43.995915 sparkmeasure-0.21.1/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)       67 2022-08-22 08:41:43.995915 sparkmeasure-0.21.1/setup.cfg
--rw-r--r--   0 luca      (1000) luca      (1000)     1508 2022-08-22 08:34:15.000000 sparkmeasure-0.21.1/setup.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-08-22 08:41:43.994915 sparkmeasure-0.21.1/sparkmeasure/
--rw-r--r--   0 luca      (1000) luca      (1000)      123 2022-08-05 09:02:21.000000 sparkmeasure-0.21.1/sparkmeasure/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     2042 2022-08-16 13:05:45.000000 sparkmeasure-0.21.1/sparkmeasure/stagemetrics.py
--rw-r--r--   0 luca      (1000) luca      (1000)     1954 2022-08-22 08:33:48.000000 sparkmeasure-0.21.1/sparkmeasure/taskmetrics.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-08-22 08:41:43.995915 sparkmeasure-0.21.1/sparkmeasure.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1000)     1225 2022-08-22 08:41:43.000000 sparkmeasure-0.21.1/sparkmeasure.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)      279 2022-08-22 08:41:43.000000 sparkmeasure-0.21.1/sparkmeasure.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2022-08-22 08:41:43.000000 sparkmeasure-0.21.1/sparkmeasure.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2022-08-22 08:41:43.000000 sparkmeasure-0.21.1/sparkmeasure.egg-info/not-zip-safe
--rw-r--r--   0 luca      (1000) luca      (1000)       13 2022-08-22 08:41:43.000000 sparkmeasure-0.21.1/sparkmeasure.egg-info/top_level.txt
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 09:25:32.623582 sparkmeasure-0.23.0/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1150 2023-05-03 09:25:32.623582 sparkmeasure-0.23.0/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)       67 2023-05-03 09:25:32.624582 sparkmeasure-0.23.0/setup.cfg
+-rw-r--r--   0 luca      (1000) luca      (1000)     1457 2023-05-03 09:10:32.000000 sparkmeasure-0.23.0/setup.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 09:25:32.622582 sparkmeasure-0.23.0/sparkmeasure/
+-rw-r--r--   0 luca      (1000) luca      (1000)      123 2022-08-05 09:02:21.000000 sparkmeasure-0.23.0/sparkmeasure/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     2942 2023-05-03 09:10:32.000000 sparkmeasure-0.23.0/sparkmeasure/stagemetrics.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     2677 2023-05-03 09:10:32.000000 sparkmeasure-0.23.0/sparkmeasure/taskmetrics.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     1486 2023-05-03 09:10:32.000000 sparkmeasure-0.23.0/sparkmeasure/test_stagemetrics.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     1469 2023-05-03 09:10:32.000000 sparkmeasure-0.23.0/sparkmeasure/test_taskmetrics.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 09:25:32.623582 sparkmeasure-0.23.0/sparkmeasure.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1150 2023-05-03 09:25:32.000000 sparkmeasure-0.23.0/sparkmeasure.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)      346 2023-05-03 09:25:32.000000 sparkmeasure-0.23.0/sparkmeasure.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2023-05-03 09:25:32.000000 sparkmeasure-0.23.0/sparkmeasure.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2023-05-03 09:25:32.000000 sparkmeasure-0.23.0/sparkmeasure.egg-info/not-zip-safe
+-rw-r--r--   0 luca      (1000) luca      (1000)       13 2023-05-03 09:25:32.000000 sparkmeasure-0.23.0/sparkmeasure.egg-info/top_level.txt
```

### Comparing `sparkmeasure-0.21.1/PKG-INFO` & `sparkmeasure-0.23.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: sparkmeasure
-Version: 0.21.1
-Summary: Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads
+Version: 0.23.0
+Summary: Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads.
 Home-page: https://github.com/lucacanali/sparkMeasure
 Author: Luca Canali
 Author-email: luca.canali@cern.ch
 License: Apache License, Version 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 SparkMeasure is a tool for performance troubleshooting of Apache Spark workloads.  
 It simplifies the collection and analysis of Spark performance metrics. The bulk of sparkMeasure is written in Scala.
 This package contains the Python API for sparkMeasure and is intended to work in conjunction with PySpark.
-Use from python command line or in Jupyter notebook environments, or as a tool to instrument Python code running Spark workloads.  
+Use from PySpark, or in Jupyter notebook environments, or in general as a tool to instrument Spark jobs in your Python code.
 **[Link to sparkMeasure GitHub page and documentation](https://github.com/lucacanali/sparkMeasure)**
-
```

### Comparing `sparkmeasure-0.21.1/setup.py` & `sparkmeasure-0.23.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
-description = 'Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads'
+description = 'Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads.'
 
 long_description = """SparkMeasure is a tool for performance troubleshooting of Apache Spark workloads.  
 It simplifies the collection and analysis of Spark performance metrics. The bulk of sparkMeasure is written in Scala.
 This package contains the Python API for sparkMeasure and is intended to work in conjunction with PySpark.
-Use from python command line or in Jupyter notebook environments, or as a tool to instrument Python code running Spark workloads.  
+Use from PySpark, or in Jupyter notebook environments, or in general as a tool to instrument Spark jobs in your Python code.
 **[Link to sparkMeasure GitHub page and documentation](https://github.com/lucacanali/sparkMeasure)**"""
 
 setup(name='sparkmeasure',
-    version='0.21.1',
+    version='0.23.0',
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luca Canali',
     author_email='luca.canali@cern.ch',
     url='https://github.com/lucacanali/sparkMeasure',
     license='Apache License, Version 2.0',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
-    python_requires='>=2.7',
+    python_requires='>=3.6',
     install_requires=[],
     classifiers=[
-    'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: Apache Software License',
     'Intended Audience :: Developers',
     'Development Status :: 4 - Beta',
     ]
     )
```

### Comparing `sparkmeasure-0.21.1/sparkmeasure/stagemetrics.py` & `sparkmeasure-0.23.0/sparkmeasure/stagemetrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 """sparkmeasure is a tool for performance troubleshooting of Apache Spark workloads.
 It simplifies the collection and analysis of Spark task metrics data.
 See details at https://github.com/LucaCanali/sparkMeasure
 """
 
-from __future__ import print_function
-
-"""StageMetrics class provides the API to collect and process task metrics data aggregated by execution stage.
-This is a Python wrapper class to the corresponding Scala class of sparkMeasure.
-"""
 class StageMetrics:
+    """StageMetrics class provides the API to collect and process task metrics data aggregated by execution stage.
+       This is a Python wrapper class to the corresponding Scala class of sparkMeasure."""
     def __init__(self, sparksession):
         self.sparksession = sparksession
         self.sc = self.sparksession.sparkContext
         self.stagemetrics = self.sc._jvm.ch.cern.sparkmeasure.StageMetrics(self.sparksession._jsparkSession)
 
     def begin(self):
+        """Begin collecting stage metrics data."""
         self.stagemetrics.begin()
 
     def end(self):
+        """End collecting stage metrics data."""
         self.stagemetrics.end()
 
     def report(self):
+        """Return a report of the collected stage metrics data."""
         return self.stagemetrics.report()
 
+    def aggregate_stagemetrics(self):
+        """Return a dictionary of the aggregated stage metrics data."""
+        return self.stagemetrics.aggregateStageMetricsJavaMap()
+
     def print_report(self):
+        """Print a report of the collected stage metrics data."""
         print(self.report())
 
     def report_memory(self):
+        """Return the collected stage metrics data for memory usage."""
         return self.stagemetrics.reportMemory()
 
     def print_memory_report(self):
+        """Print a report of the collected stage metrics data for memory usage."""
         print(self.report_memory())
 
     def runandmeasure(self, env, codetorun):
+        """Run a Python code snippet and collect stage metrics data."""
         self.begin()
         exec(codetorun, env)
         self.end()
         self.print_report()
 
     def create_stagemetrics_DF(self, viewname="PerfStageMetrics"):
+        """Create a Spark Dataframe from the collected stage metrics data."""
         df = self.stagemetrics.createStageMetricsDF(viewname)
         # convert the returned Java object to a Python Dataframe
         from pyspark.sql.dataframe import DataFrame
         return DataFrame(df, self.sparksession)
 
     def aggregate_stagemetrics_DF(self, viewname="PerfStageMetrics"):
+        """Create a Spark Dataframe from the aggregated stage metrics data."""
         df = self.stagemetrics.aggregateStageMetrics(viewname)
         # convert the returned Java object to a Python Dataframe
         from pyspark.sql.dataframe import DataFrame
         return DataFrame(df, self.sparksession)
 
     def save_data(self, df, filepathandname, fileformat="json"):
+        """Save the collected stage metrics data to a file."""
         df.repartition(1).write.format(fileformat).save(filepathandname)
 
     def remove_listener(self):
+        """Remove the Spark listener that collects stage metrics data."""
         self.stagemetrics.removeListener()
```

### Comparing `sparkmeasure-0.21.1/sparkmeasure/taskmetrics.py` & `sparkmeasure-0.23.0/sparkmeasure/taskmetrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 """sparkmeasure is a tool for performance troubleshooting of Apache Spark workloads.
 It simplifies the collection and analysis of Spark task metrics data.
 See details at https://github.com/LucaCanali/sparkMeasure
 """
 
-from __future__ import print_function
-
-"""TaskMetrics class provides the API to collect and process task metrics data aggregated by task execution
-This is a finer granularity than StageMetrics and potentially collects much more data.
-This is a Python wrapper class to the corresponding Scala class of sparkMeasure.
-"""
 class TaskMetrics:
+    """TaskMetrics class provides the API to collect and process task metrics data aggregated by task execution
+       This is a finer granularity than StageMetrics and potentially collects much more data.
+       This is a Python wrapper class to the corresponding Scala class of sparkMeasure."""
     def __init__(self, sparksession):
         self.sparksession = sparksession
         self.sc = self.sparksession.sparkContext
         self.taskmetrics = self.sc._jvm.ch.cern.sparkmeasure.TaskMetrics(self.sparksession._jsparkSession)
 
     def begin(self):
+        """Begin collecting task metrics data."""
         self.taskmetrics.begin()
 
     def end(self):
+        """End collecting task metrics data."""
         self.taskmetrics.end()
 
     def report(self):
+        """Return a report of the collected task metrics data."""
         return self.taskmetrics.report()
 
+    def aggregate_taskmetrics(self):
+        """Return a dictionary of the aggregated task metrics data."""
+        return self.taskmetrics.aggregateTaskMetricsJavaMap()
+
     def print_report(self):
+        """Print a report of the collected task metrics data."""
         print(self.report())
 
     def runandmeasure(self, env, codetorun):
+        """Run a Python code snippet and collect task metrics data."""
         self.begin()
         exec(codetorun, env)
         self.end()
         self.print_report()
 
     def create_taskmetrics_DF(self, viewname="PerfTaskMetrics"):
+        """Create a Spark Dataframe from the collected task metrics data."""
         df = self.taskmetrics.createTaskMetricsDF(viewname)
         # convert the returned Java object to a Python Dataframe
         from pyspark.sql.dataframe import DataFrame
         return DataFrame(df, self.sparksession)
 
     def aggregate_taskmetrics_DF(self, viewname="PerfTaskMetrics"):
+        """Create a Spark Dataframe from the aggregated task metrics data."""
         df = self.taskmetrics.aggregateTaskMetrics(viewname)
         # convert the returned Java object to a Python Dataframe
         from pyspark.sql.dataframe import DataFrame
         return DataFrame(df, self.sparksession)
 
     def save_data(self, df, filepathandname, fileformat):
+        """Save the collected task metrics data to a file."""
         df.repartition(1).write.format(fileformat).save(filepathandname)
 
     def remove_listener(self):
+        """Remove the listener from the SparkContext."""
         self.taskmetrics.removeListener()
```

### Comparing `sparkmeasure-0.21.1/sparkmeasure.egg-info/PKG-INFO` & `sparkmeasure-0.23.0/sparkmeasure.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: sparkmeasure
-Version: 0.21.1
-Summary: Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads
+Version: 0.23.0
+Summary: Python API for sparkMeasure, a tool for performance troubleshooting of Apache Spark workloads.
 Home-page: https://github.com/lucacanali/sparkMeasure
 Author: Luca Canali
 Author-email: luca.canali@cern.ch
 License: Apache License, Version 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 SparkMeasure is a tool for performance troubleshooting of Apache Spark workloads.  
 It simplifies the collection and analysis of Spark performance metrics. The bulk of sparkMeasure is written in Scala.
 This package contains the Python API for sparkMeasure and is intended to work in conjunction with PySpark.
-Use from python command line or in Jupyter notebook environments, or as a tool to instrument Python code running Spark workloads.  
+Use from PySpark, or in Jupyter notebook environments, or in general as a tool to instrument Spark jobs in your Python code.
 **[Link to sparkMeasure GitHub page and documentation](https://github.com/lucacanali/sparkMeasure)**
-
```

