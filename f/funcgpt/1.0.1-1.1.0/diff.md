# Comparing `tmp/funcgpt-1.0.1.tar.gz` & `tmp/funcgpt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcgpt-1.0.1.tar", last modified: Mon Apr 24 03:34:55 2023, max compression
+gzip compressed data, was "funcgpt-1.1.0.tar", last modified: Wed May  3 19:32:07 2023, max compression
```

## Comparing `funcgpt-1.0.1.tar` & `funcgpt-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 03:34:55.395568 funcgpt-1.0.1/
--rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 funcgpt-1.0.1/LICENSE
--rw-r--r--   0 leandro    (501) staff       (20)     3213 2023-04-24 03:34:55.395463 funcgpt-1.0.1/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     2360 2023-04-24 02:18:53.000000 funcgpt-1.0.1/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 03:34:55.394814 funcgpt-1.0.1/funcgpt/
--rw-r--r--   0 leandro    (501) staff       (20)       83 2023-04-23 17:46:42.000000 funcgpt-1.0.1/funcgpt/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)      227 2023-04-23 17:02:29.000000 funcgpt-1.0.1/funcgpt/credentials.py
--rw-r--r--   0 leandro    (501) staff       (20)      699 2023-04-24 01:58:32.000000 funcgpt-1.0.1/funcgpt/decorators.py
--rw-r--r--   0 leandro    (501) staff       (20)     5570 2023-04-24 01:58:32.000000 funcgpt-1.0.1/funcgpt/gpt.py
--rw-r--r--   0 leandro    (501) staff       (20)      236 2023-04-23 20:57:38.000000 funcgpt-1.0.1/funcgpt/protocols.py
--rw-r--r--   0 leandro    (501) staff       (20)     3185 2023-04-24 01:58:32.000000 funcgpt-1.0.1/funcgpt/wrapper.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-04-24 03:34:55.395338 funcgpt-1.0.1/funcgpt.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)     3213 2023-04-24 03:34:55.000000 funcgpt-1.0.1/funcgpt.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      276 2023-04-24 03:34:55.000000 funcgpt-1.0.1/funcgpt.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-04-24 03:34:55.000000 funcgpt-1.0.1/funcgpt.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)        8 2023-04-24 03:34:55.000000 funcgpt-1.0.1/funcgpt.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      965 2023-04-24 03:34:50.000000 funcgpt-1.0.1/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-04-24 03:34:55.395597 funcgpt-1.0.1/setup.cfg
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 19:32:07.821697 funcgpt-1.1.0/
+-rw-r--r--   0 leandro    (501) staff       (20)     1127 2023-04-24 02:15:44.000000 funcgpt-1.1.0/LICENSE
+-rw-r--r--   0 leandro    (501) staff       (20)     3213 2023-05-03 19:32:07.821569 funcgpt-1.1.0/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     2360 2023-04-24 02:18:53.000000 funcgpt-1.1.0/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 19:32:07.819445 funcgpt-1.1.0/funcgpt/
+-rw-r--r--   0 leandro    (501) staff       (20)       83 2023-04-23 17:46:42.000000 funcgpt-1.1.0/funcgpt/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)      227 2023-04-23 17:02:29.000000 funcgpt-1.1.0/funcgpt/credentials.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 19:32:07.820263 funcgpt-1.1.0/funcgpt/data/
+-rw-r--r--   0 leandro    (501) staff       (20)   611817 2023-05-03 19:16:20.000000 funcgpt-1.1.0/funcgpt/data/cl100k_base.tiktoken.bz2
+-rw-r--r--   0 leandro    (501) staff       (20)      699 2023-04-24 01:58:32.000000 funcgpt-1.1.0/funcgpt/decorators.py
+-rw-r--r--   0 leandro    (501) staff       (20)     5523 2023-05-03 18:48:37.000000 funcgpt-1.1.0/funcgpt/gpt.py
+-rw-r--r--   0 leandro    (501) staff       (20)      370 2023-05-03 15:47:27.000000 funcgpt-1.1.0/funcgpt/message.py
+-rw-r--r--   0 leandro    (501) staff       (20)      236 2023-04-23 20:57:38.000000 funcgpt-1.1.0/funcgpt/protocols.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4441 2023-05-03 19:29:56.000000 funcgpt-1.1.0/funcgpt/tokentools.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4193 2023-05-03 18:35:03.000000 funcgpt-1.1.0/funcgpt/wrapper.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 19:32:07.820152 funcgpt-1.1.0/funcgpt.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)     3213 2023-05-03 19:32:07.000000 funcgpt-1.1.0/funcgpt.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      385 2023-05-03 19:32:07.000000 funcgpt-1.1.0/funcgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-03 19:32:07.000000 funcgpt-1.1.0/funcgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       16 2023-05-03 19:32:07.000000 funcgpt-1.1.0/funcgpt.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        8 2023-05-03 19:32:07.000000 funcgpt-1.1.0/funcgpt.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)     1058 2023-05-03 18:53:33.000000 funcgpt-1.1.0/pyproject.toml
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-03 19:32:07.821728 funcgpt-1.1.0/setup.cfg
```

### Comparing `funcgpt-1.0.1/LICENSE` & `funcgpt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcgpt-1.0.1/PKG-INFO` & `funcgpt-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcgpt
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library to easily create functions based on OpenAI's GPT
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/funcgpt
 Project-URL: Bug Tracker, https://github.com/leandropls/funcgpt/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `funcgpt-1.0.1/README.md` & `funcgpt-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `funcgpt-1.0.1/funcgpt/decorators.py` & `funcgpt-1.1.0/funcgpt/decorators.py`

 * *Files identical despite different names*

### Comparing `funcgpt-1.0.1/funcgpt/gpt.py` & `funcgpt-1.1.0/funcgpt/gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from codecs import getreader
 from json import dumps, loads
-from typing import IO, Iterator, Literal, TypedDict, cast
+from typing import IO, Iterator, Literal, cast
 from urllib.request import Request, urlopen
 
 from funcgpt.credentials import OPENAI_API_KEY, OPENAI_ORG_ID
+from funcgpt.message import Message
 
 DEFAULT_COMPLETIONS_URL = "https://api.openai.com/v1/chat/completions"
 
 BASE_HEADERS = {
     "Content-Type": "application/json",
     "Authorization": f"Bearer {OPENAI_API_KEY}",
 }
@@ -19,27 +20,14 @@
 match_data = re.compile(r"^data: (.*)(?:\r\n|\r|\n)$").match
 
 match_empty_line = re.compile(r"^(?:\r\n|\r|\n)$").match
 
 utf8reader = getreader("utf-8")
 
 
-class Message(TypedDict):
-    """
-    A message sent or received by the assistant.
-
-    :param role: The role of the message sender or receiver. Can be "system",
-                 "user" or "assistant".
-    :param content: The text content of the message.
-    """
-
-    role: Literal["system", "user", "assistant"]
-    content: str
-
-
 def stream(
     model: Literal["gpt-3.5-turbo", "gpt-4"],
     messages: list[Message],
     temperature: int = 0,
     stop: str | list[str] | None = None,
     chat_completions_url: str = DEFAULT_COMPLETIONS_URL,
 ) -> Iterator[str]:
@@ -130,14 +118,15 @@
     :param temperature: Controls randomness in the model's response. Higher values (e.g., 1) will
                         generate more random answers, while lower values (e.g., 0) make the model
                         more deterministic. Default is 0.
     :param stop: A string or list of strings to specify sequence(s) at which the API will stop
                  generating further tokens. Default is None.
     :param chat_completions_url: The URL endpoint for fetching chat completions. The default value
                                  is DEFAULT_COMPLETIONS_URL.
+    :raises OverflowError: Raised if the model's response exceeds the maximum length.
     :return: The assistant's generated response as a string.
     """
     # Prepare request payload with model, messages, and temperature
     requestArguments = {
         "model": model,
         "messages": messages,
         "temperature": temperature,
@@ -156,9 +145,15 @@
 
     # Send the request to OpenAI's chat completions API
     response = urlopen(request)
 
     # Parse the response JSON
     body = loads(response.read())
 
+    # Get the first choice
+    choice = body["choices"][0]
+
+    if choice["finish_reason"] == "length":
+        raise OverflowError("The model's response exceeded the maximum length.")
+
     # Extract and return the assistant's response
-    return body["choices"][0]["message"]["content"]
+    return choice["message"]["content"]
```

### Comparing `funcgpt-1.0.1/funcgpt.egg-info/PKG-INFO` & `funcgpt-1.1.0/funcgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcgpt
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library to easily create functions based on OpenAI's GPT
 Author-email: Leandro Pereira de Lima e Silva <leandro@lls-software.com>
 Project-URL: Homepage, https://github.com/leandropls/funcgpt
 Project-URL: Bug Tracker, https://github.com/leandropls/funcgpt/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `funcgpt-1.0.1/pyproject.toml` & `funcgpt-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funcgpt"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Leandro Pereira de Lima e Silva", email="leandro@lls-software.com" },
 ]
 description = "A library to easily create functions based on OpenAI's GPT"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,18 +18,24 @@
   "Programming Language :: Python :: 3 :: Only",
   "Operating System :: OS Independent",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Utilities",
 ]
+dependencies = [
+  "tiktoken>=0.3.3",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/leandropls/funcgpt"
 "Bug Tracker" = "https://github.com/leandropls/funcgpt/issues"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 100
+
+[tool.setuptools.package-data]
+funcgpt = ["data/*"]
```

