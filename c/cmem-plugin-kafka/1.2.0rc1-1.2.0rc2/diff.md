# Comparing `tmp/cmem_plugin_kafka-1.2.0rc1.tar.gz` & `tmp/cmem_plugin_kafka-1.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.2.0rc1.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.2.0rc2.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.2.0rc1.tar` & `cmem_plugin_kafka-1.2.0rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/LICENSE
--rw-r--r--   0        0        0     3733 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/README-public.md
--rw-r--r--   0        0        0        0 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     3485 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14685 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    11073 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    10682 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     8722 2023-04-05 06:58:07.779233 cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2206 2023-04-05 06:58:35.151939 cmem_plugin_kafka-1.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-03 07:18:55.574411 cmem_plugin_kafka-1.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     3733 2023-05-03 07:18:55.574411 cmem_plugin_kafka-1.2.0rc2/README-public.md
+-rw-r--r--   0        0        0        0 2023-05-03 07:18:55.574411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     3485 2023-05-03 07:18:55.574411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14685 2023-05-03 07:18:55.578411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    11073 2023-05-03 07:18:55.578411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:18:55.578411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    10682 2023-05-03 07:18:55.578411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     8722 2023-05-03 07:18:55.578411 cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2206 2023-05-03 07:19:24.338569 cmem_plugin_kafka-1.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.2.0rc2/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.2.0rc1/LICENSE` & `cmem_plugin_kafka-1.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/README-public.md` & `cmem_plugin_kafka-1.2.0rc2/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/constants.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/kafka_handlers.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/workflow/consumer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.2.0rc2/cmem_plugin_kafka/workflow/producer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc1/pyproject.toml` & `cmem_plugin_kafka-1.2.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.2.0rc1"
+version = "1.2.0rc2"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -16,33 +16,33 @@
     "eccenca Corporate Memory", "plugin", "kafka", "kafka-producer", "kafka-consumer",
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-kafka"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-cmem-plugin-base = "^3.0.0"
+cmem-plugin-base = "^3.1.0"
 confluent-kafka = [
     { version = "1.9.2" },
     # before you publish, comment out this next line
     # { markers = "sys_platform == 'darwin'", url = "https://files.pythonhosted.org/packages/fb/16/d04dded73439266a3dbcd585f1128483dcf509e039bacd93642ac5de97d4/confluent-kafka-1.8.2.tar.gz"}
 ]
 defusedxml = "^0.7.1"
 json-stream = "2.3.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
-black = "^23.1.0"
-coverage = "^7.2.1"
+black = "^23.3.0"
+coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
 genbadge = "^1.1.0"
-mypy = "^1.1.1"
+mypy = "^1.2.0"
 pylint-junit = "^0.3.2"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.4.0"
 safety = "^1.10.3"
 typed-ast = "^1.5.4"
 wheel = "^0.38.4"
 cmem-plugin-examples = "*"
 types-requests = "*"
```

### Comparing `cmem_plugin_kafka-1.2.0rc1/PKG-INFO` & `cmem_plugin_kafka-1.2.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.2.0rc1
+Version: 1.2.0rc2
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=3.0.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
 Requires-Dist: confluent-kafka (==1.9.2)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: json-stream (==2.3.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-kafka
```

