# Comparing `tmp/pandasai-0.2.1.tar.gz` & `tmp/pandasai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.1.tar", max compression
+gzip compressed data, was "pandasai-0.2.2.tar", max compression
```

## Comparing `pandasai-0.2.1.tar` & `pandasai-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.1/LICENSE
--rw-r--r--   0        0        0     4396 2023-05-02 22:59:27.189355 pandasai-0.2.1/README.md
--rw-r--r--   0        0        0     5966 2023-05-02 23:27:07.273996 pandasai-0.2.1/pandasai/__init__.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.1/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0      657 2023-05-03 14:50:10.271752 pandasai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 pandasai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4396 2023-05-02 22:59:27.189355 pandasai-0.2.2/README.md
+-rw-r--r--   0        0        0     6249 2023-05-03 14:53:42.378833 pandasai-0.2.2/pandasai/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.2/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      677 2023-05-03 14:55:44.337550 pandasai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5205 1970-01-01 00:00:00.000000 pandasai-0.2.2/PKG-INFO
```

### Comparing `pandasai-0.2.1/LICENSE` & `pandasai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/README.md` & `pandasai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pandasai/__init__.py` & `pandasai-0.2.2/pandasai/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ PandasAI is a wrapper around a LLM to make dataframes convesational """
 import io
 import sys
 import pandas as pd
 from .llm.base import LLM
+from .helpers.notebook import Notebook
 from .exceptions import LLMNotFoundError
 
 
 class PandasAI:
     """PandasAI is a wrapper around a LLM to make dataframes convesational"""
 
     _task_instruction: str = """
@@ -37,14 +38,15 @@
     """
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
     _enforce_privacy: bool = False
     _max_retries: int = 3
     _original_instruction_and_prompt = None
+    _is_notebook: bool = False
     last_code_generated: str = None
     code_output: str = None
 
     def __init__(
         self,
         llm=None,
         conversational=True,
@@ -56,31 +58,35 @@
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
 
+        self.notebook = Notebook()
+        self._in_notebook = self.notebook.in_notebook()
+
     def conversational_answer(self, question: str, code: str, answer: str) -> str:
         """Return the conversational answer"""
         if self._enforce_privacy:
             # we don't want to send potentially sensitive data to the LLM server
             # if the user has set enforce_privacy to True
             return answer
 
         instruction = self._response_instruction.format(
             question=question, code=code, answer=answer
         )
-        return self._llm.call(instruction, answer)
+        return self._llm.call(instruction, "")
 
     def run(
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
+        show_code: bool = False,
     ) -> str:
         """Run the LLM with the given prompt"""
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         rows_to_display = 5
         if self._enforce_privacy:
             rows_to_display = 0
@@ -103,14 +109,16 @@
         self.log(
             f"""
 Code generated:
 ```
 {code}
 ```"""
         )
+        if show_code and self._in_notebook:
+            self.notebook.create_new_cell(code)
 
         answer = self.run_code(code, data_frame, False)
         self.code_output = answer
         self.log(f"Answer: {answer}")
 
         if is_conversational_answer is None:
             is_conversational_answer = self._is_conversational_answer
```

### Comparing `pandasai-0.2.1/pandasai/exceptions.py` & `pandasai-0.2.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pandasai/llm/alpaca.py` & `pandasai-0.2.2/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pandasai/llm/base.py` & `pandasai-0.2.2/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pandasai/llm/open_assistant.py` & `pandasai-0.2.2/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pandasai/llm/openai.py` & `pandasai-0.2.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.1/pyproject.toml` & `pandasai-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.1"
+version = "0.2.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 astor = "^0.8.1"
 openai = "^0.27.5"
+ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
```

### Comparing `pandasai-0.2.1/PKG-INFO` & `pandasai-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
```

