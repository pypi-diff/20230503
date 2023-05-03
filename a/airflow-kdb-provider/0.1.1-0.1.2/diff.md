# Comparing `tmp/airflow-kdb-provider-0.1.1.tar.gz` & `tmp/airflow-kdb-provider-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-kdb-provider-0.1.1.tar", last modified: Wed May  3 06:45:01 2023, max compression
+gzip compressed data, was "dist/airflow-kdb-provider-0.1.2.tar", last modified: Wed May  3 06:53:14 2023, max compression
```

## Comparing `airflow-kdb-provider-0.1.1.tar` & `airflow-kdb-provider-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.745568 airflow-kdb-provider-0.1.1/
--rw-r--r--   0 kabir      (501) staff       (20)    11358 2023-05-03 00:16:45.000000 airflow-kdb-provider-0.1.1/LICENSE
--rw-r--r--   0 kabir      (501) staff       (20)     3140 2023-05-03 06:45:01.745083 airflow-kdb-provider-0.1.1/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)     2185 2023-05-03 00:16:47.000000 airflow-kdb-provider-0.1.1/README.md
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.742706 airflow-kdb-provider-0.1.1/airflow_kdb_provider/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/__init__.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.743768 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/__init__.py
--rw-r--r--   0 kabir      (501) staff       (20)      869 2023-05-03 00:10:53.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/kdb_operator.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:45:01.743475 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/
--rw-r--r--   0 kabir      (501) staff       (20)     3140 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)      368 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/SOURCES.txt
--rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/dependency_links.txt
--rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/requires.txt
--rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-03 06:45:01.000000 airflow-kdb-provider-0.1.1/airflow_kdb_provider.egg-info/top_level.txt
--rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-03 06:45:01.745690 airflow-kdb-provider-0.1.1/setup.cfg
--rw-r--r--   0 kabir      (501) staff       (20)      800 2023-05-03 06:43:42.000000 airflow-kdb-provider-0.1.1/setup.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.474964 airflow-kdb-provider-0.1.2/
+-rw-r--r--   0 kabir      (501) staff       (20)    11358 2023-05-03 00:16:45.000000 airflow-kdb-provider-0.1.2/LICENSE
+-rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-03 06:53:14.474774 airflow-kdb-provider-0.1.2/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)     1634 2023-05-03 06:52:57.000000 airflow-kdb-provider-0.1.2/README.md
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.472732 airflow-kdb-provider-0.1.2/airflow_kdb_provider/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/__init__.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.474185 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/__init__.py
+-rw-r--r--   0 kabir      (501) staff       (20)      869 2023-05-03 00:10:53.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/kdb_operator.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.473813 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/
+-rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)      368 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/requires.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/top_level.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-03 06:53:14.475026 airflow-kdb-provider-0.1.2/setup.cfg
+-rw-r--r--   0 kabir      (501) staff       (20)      800 2023-05-03 06:53:08.000000 airflow-kdb-provider-0.1.2/setup.py
```

### Comparing `airflow-kdb-provider-0.1.1/LICENSE` & `airflow-kdb-provider-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.1/PKG-INFO` & `airflow-kdb-provider-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,53 @@
 Metadata-Version: 2.1
 Name: airflow-kdb-provider
-Version: 0.1.1
+Version: 0.1.2
 Summary: Apache Airflow provider for KDBAirflowOperator
 Home-page: UNKNOWN
 Author: Kabir Jaiswal
 Author-email: kabirjaiswal30@gmail.com
 License: Apache License 2.0
-Description: # KDBAirflowOperator
-        A light weight KDB operator for Apache Airflow
-        KDBAirflowOperator
-        KDBAirflowOperator is a custom Apache Airflow operator that can be used to execute KDB+/q scripts from within Airflow DAGs. KDB+/q is a high-performance, column-oriented database that is popular in the financial industry. This operator allows for seamless integration between Airflow and KDB+/q, making it easier to automate data pipelines that involve KDB+/q.
+Description: # Airflow KDB Provider
         
-        Installation
-        To use this operator, you must first clone the repository from Github:
+        A lightweight KDB provider for Apache Airflow, featuring the `KDBAirflowOperator`. This provider allows for seamless integration between Airflow and KDB+/q, making it easier to automate data pipelines that involve KDB+/q.
         
+        ## Installation
         
-        ```python 
-        git clone https://github.com/kabir12345/KDBAirflowOperator.git 
-        ```
-        Once you have cloned the repository, you can install the operator and its dependencies by running the following command:
+        You can install the Airflow KDB Provider package from PyPI using the following command:
         
-        ```python 
-        pip install -e KDBAirflowOperator
+        ```bash
+        pip install airflow-kdb-provider
         ```
-        
-        This will install the operator in editable mode (-e option), which allows you to make changes to the code and have those changes reflected immediately without the need to reinstall.
-        
-        
-        Usage
+        ## Usage
         To use the KDBAirflowOperator in your Airflow DAG, you must first import it and create an instance of the operator. Here is an example:
-         
-        ```python 
-        from KDBOperator import KDBOperator
+        
+        from airflow_kdb_provider.operators.kdb_operator import KDBOperator
+        ```python
         kdb_operator = KDBOperator(
             task_id='run_kdb_script',
             command='/path/to/kdb_script.q',
             params={'param1': 'value1', 'param2': 'value2'},
             conn_id='kdb_conn',
-            dag=dag) 
-         ```
-        
+            dag=dag)
+        ```
         In this example, we create an instance of the KDBOperator and specify the following parameters:
         
         task_id: the task ID for this operator
         command: the path to the KDB+/q script that we want to execute
         params: a dictionary of parameters that will be passed to the KDB+/q script as command-line arguments
         conn_id: the connection ID for the KDB+/q server that we want to use (this should be defined in Airflow's Connections interface)
         dag: the DAG that this operator belongs to
         Once you have created an instance of the KDBOperator, you can add it to your DAG like any other Airflow operator:
         
-        
-        ```python 
+        ```python
         some_other_operator >> kdb_operator >> some_other_operator2
         ```
         
         In this example, we have added the kdb_operator to our DAG and specified that it should be executed after some_other_operator and before some_other_operator2.
         
         
-        
-        
-        
-        
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `airflow-kdb-provider-0.1.1/README.md` & `airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-# KDBAirflowOperator
-A light weight KDB operator for Apache Airflow
-KDBAirflowOperator
-KDBAirflowOperator is a custom Apache Airflow operator that can be used to execute KDB+/q scripts from within Airflow DAGs. KDB+/q is a high-performance, column-oriented database that is popular in the financial industry. This operator allows for seamless integration between Airflow and KDB+/q, making it easier to automate data pipelines that involve KDB+/q.
-
-Installation
-To use this operator, you must first clone the repository from Github:
-
-
-```python 
-git clone https://github.com/kabir12345/KDBAirflowOperator.git 
-```
-Once you have cloned the repository, you can install the operator and its dependencies by running the following command:
-
-```python 
-pip install -e KDBAirflowOperator
-```
-
-This will install the operator in editable mode (-e option), which allows you to make changes to the code and have those changes reflected immediately without the need to reinstall.
-
-
-Usage
-To use the KDBAirflowOperator in your Airflow DAG, you must first import it and create an instance of the operator. Here is an example:
- 
-```python 
-from KDBOperator import KDBOperator
-kdb_operator = KDBOperator(
-    task_id='run_kdb_script',
-    command='/path/to/kdb_script.q',
-    params={'param1': 'value1', 'param2': 'value2'},
-    conn_id='kdb_conn',
-    dag=dag) 
- ```
-
-In this example, we create an instance of the KDBOperator and specify the following parameters:
-
-task_id: the task ID for this operator
-command: the path to the KDB+/q script that we want to execute
-params: a dictionary of parameters that will be passed to the KDB+/q script as command-line arguments
-conn_id: the connection ID for the KDB+/q server that we want to use (this should be defined in Airflow's Connections interface)
-dag: the DAG that this operator belongs to
-Once you have created an instance of the KDBOperator, you can add it to your DAG like any other Airflow operator:
-
-
-```python 
-some_other_operator >> kdb_operator >> some_other_operator2
-```
-
-In this example, we have added the kdb_operator to our DAG and specified that it should be executed after some_other_operator and before some_other_operator2.
-
-
-
-
-
-
-
-
+Metadata-Version: 2.1
+Name: airflow-kdb-provider
+Version: 0.1.2
+Summary: Apache Airflow provider for KDBAirflowOperator
+Home-page: UNKNOWN
+Author: Kabir Jaiswal
+Author-email: kabirjaiswal30@gmail.com
+License: Apache License 2.0
+Description: # Airflow KDB Provider
+        
+        A lightweight KDB provider for Apache Airflow, featuring the `KDBAirflowOperator`. This provider allows for seamless integration between Airflow and KDB+/q, making it easier to automate data pipelines that involve KDB+/q.
+        
+        ## Installation
+        
+        You can install the Airflow KDB Provider package from PyPI using the following command:
+        
+        ```bash
+        pip install airflow-kdb-provider
+        ```
+        ## Usage
+        To use the KDBAirflowOperator in your Airflow DAG, you must first import it and create an instance of the operator. Here is an example:
+        
+        from airflow_kdb_provider.operators.kdb_operator import KDBOperator
+        ```python
+        kdb_operator = KDBOperator(
+            task_id='run_kdb_script',
+            command='/path/to/kdb_script.q',
+            params={'param1': 'value1', 'param2': 'value2'},
+            conn_id='kdb_conn',
+            dag=dag)
+        ```
+        In this example, we create an instance of the KDBOperator and specify the following parameters:
+        
+        task_id: the task ID for this operator
+        command: the path to the KDB+/q script that we want to execute
+        params: a dictionary of parameters that will be passed to the KDB+/q script as command-line arguments
+        conn_id: the connection ID for the KDB+/q server that we want to use (this should be defined in Airflow's Connections interface)
+        dag: the DAG that this operator belongs to
+        Once you have created an instance of the KDBOperator, you can add it to your DAG like any other Airflow operator:
+        
+        ```python
+        some_other_operator >> kdb_operator >> some_other_operator2
+        ```
+        
+        In this example, we have added the kdb_operator to our DAG and specified that it should be executed after some_other_operator and before some_other_operator2.
+        
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
```

### Comparing `airflow-kdb-provider-0.1.1/airflow_kdb_provider/operators/kdb_operator.py` & `airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/kdb_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.1/setup.py` & `airflow-kdb-provider-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='airflow-kdb-provider',
-    version='0.1.1',
+    version='0.1.2',
     description='Apache Airflow provider for KDBAirflowOperator',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Kabir Jaiswal',
     author_email='kabirjaiswal30@gmail.com',
     license='Apache License 2.0',
     packages=find_packages(),
```

