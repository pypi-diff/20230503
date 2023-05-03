# Comparing `tmp/pandasai-0.2.0.tar.gz` & `tmp/pandasai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.0.tar", max compression
+gzip compressed data, was "pandasai-0.2.1.tar", max compression
```

## Comparing `pandasai-0.2.0.tar` & `pandasai-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.0/LICENSE
--rw-r--r--   0        0        0     4396 2023-05-02 22:31:16.282339 pandasai-0.2.0/README.md
--rw-r--r--   0        0        0     5966 2023-05-02 22:04:48.980512 pandasai-0.2.0/pandasai/__init__.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.0/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0      657 2023-05-02 22:33:39.314750 pandasai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 pandasai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4396 2023-05-02 22:59:27.189355 pandasai-0.2.1/README.md
+-rw-r--r--   0        0        0     5966 2023-05-02 23:27:07.273996 pandasai-0.2.1/pandasai/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.1/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      657 2023-05-03 14:50:10.271752 pandasai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 pandasai-0.2.1/PKG-INFO
```

### Comparing `pandasai-0.2.0/LICENSE` & `pandasai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/README.md` & `pandasai-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/__init__.py` & `pandasai-0.2.1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/exceptions.py` & `pandasai-0.2.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/llm/alpaca.py` & `pandasai-0.2.1/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/llm/base.py` & `pandasai-0.2.1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/llm/open_assistant.py` & `pandasai-0.2.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pandasai/llm/openai.py` & `pandasai-0.2.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.0/pyproject.toml` & `pandasai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.0"
+version = "0.2.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.2.0/PKG-INFO` & `pandasai-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

