# Comparing `tmp/extism_func_gen-0.3.0.tar.gz` & `tmp/extism_func_gen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extism_func_gen-0.3.0.tar", max compression
+gzip compressed data, was "extism_func_gen-0.4.0.tar", max compression
```

## Comparing `extism_func_gen-0.3.0.tar` & `extism_func_gen-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      741 2023-04-28 22:36:50.998017 extism_func_gen-0.3.0/README.md
--rw-r--r--   0        0        0     4079 2023-04-30 20:58:00.513758 extism_func_gen-0.3.0/func_gen/__init__.py
--rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.3.0/func_gen/eval.wasm
--rw-r--r--   0        0        0      437 2023-04-30 20:59:31.487403 extism_func_gen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 extism_func_gen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      859 2023-05-03 17:28:02.212729 extism_func_gen-0.4.0/README.md
+-rw-r--r--   0        0        0     4401 2023-05-03 17:36:28.650342 extism_func_gen-0.4.0/func_gen/__init__.py
+-rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.4.0/func_gen/eval.wasm
+-rw-r--r--   0        0        0      437 2023-05-03 17:37:19.122329 extism_func_gen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 extism_func_gen-0.4.0/PKG-INFO
```

### Comparing `extism_func_gen-0.3.0/README.md` & `extism_func_gen-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 func-gen can be used to generate unix text processing utilities from English text.
 It uses [langchain](https://python.langchain.com/en/latest/index.html) to create javascript functions
 to process text, and it uses [Extism](https://extism.org/) and the [JavaScript PDK](https://extism.org/docs/write-a-plugin/js-pdk)
 to safely execute the code in a Wasm sandbox.
 
 ## Install
 
-```
+> **Note**: First you need to [install Extism](https://extism.org/docs/install) on your machine if you have not:
+
+```bash
 pip install --upgrade extism-func-gen
 ```
 
 ## Run
 
 ```bash
 # Need to set the OpenAI API key
```

### Comparing `extism_func_gen-0.3.0/func_gen/__init__.py` & `extism_func_gen-0.4.0/func_gen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,31 @@
         SystemMessage(content="Your goal is to write a Javascript function."),
         SystemMessage(content="You must export the function as the default export, using the CommonJS module syntax."),
         SystemMessage(content="You should not import or require any code."),
         SystemMessage(content="""
 This JavaScript environment has a global object for making http request called "Http". On that object is a function
 "request" which is a synchronous, blocking funciton and has the following jsdoc:
 
-@param {Object} request - The HTTP request object
-@param {string} request.url - The url for the request
-@param {string} request.method - The HTTP method for the request
-@param {Object} request.headers - Key-Value pairs to be assigned to the headers of the response
-@param {string} body - The request HTTP body. This parameter is required. Use null if the body is not needed.
+@param {Object} request - Required: The HTTP request object
+@param {string} request.url - Required: The url for the request
+@param {string} request.method - Required: The HTTP method for the request
+@param {Object} request.headers - Optional: Key-Value pairs to be assigned to the headers of the response
+@param {string} body - Required: The request HTTP body. This parameter is required. Use null if the body is not needed.
 @return {HttpResponse} - the HTTP response
 
 It returns an HttpResponse which has two properties, a "body" containing the HTTP response body as a string
 and "status_code" which contains the integer Http status code.
 
 You are to use this function to make http requests
                       """.strip()),
+        SystemMessage(content="""
+An example of making a GET HTTP request would look like:
+
+let response = Http.request({ url: "https://example.com", method: "GET", headers: {} }, null)
+                      """.strip()),
         SystemMessage(content="You must not include any comments, explanations, or markdown. The response should be JavaScript only."),
         HumanMessage(content=description),
     ]
 
     response = chat(messages)
     code = response.content
     match = MARKDOWN_RE.match(code)
@@ -103,12 +108,13 @@
 
     if not os.path.exists(target):
         print(f"Could not find function {args.func_name} in {HOME_DIR}")
         print("To define it use the -d parameter with an English description. Example:")
         print(f"  func-gen {args.func_name} -d 'Write a function that counts the number of vowels in a string'")
         exit(1)
 
+    inpt = sys.stdin.read() if not sys.stdin.isatty() else ""
     with open(target, 'r') as file:
-        result = execute_code(file.read(), sys.stdin.read())
+        result = execute_code(file.read(), inpt)
         print(result.decode('utf-8'))
```

### Comparing `extism_func_gen-0.3.0/func_gen/eval.wasm` & `extism_func_gen-0.4.0/func_gen/eval.wasm`

 * *Files identical despite different names*

### Comparing `extism_func_gen-0.3.0/PKG-INFO` & `extism_func_gen-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extism-func-gen
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: The Extism Authors
 Author-email: oss@extism.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,17 @@
 func-gen can be used to generate unix text processing utilities from English text.
 It uses [langchain](https://python.langchain.com/en/latest/index.html) to create javascript functions
 to process text, and it uses [Extism](https://extism.org/) and the [JavaScript PDK](https://extism.org/docs/write-a-plugin/js-pdk)
 to safely execute the code in a Wasm sandbox.
 
 ## Install
 
-```
+> **Note**: First you need to [install Extism](https://extism.org/docs/install) on your machine if you have not:
+
+```bash
 pip install --upgrade extism-func-gen
 ```
 
 ## Run
 
 ```bash
 # Need to set the OpenAI API key
```

