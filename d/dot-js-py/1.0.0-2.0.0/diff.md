# Comparing `tmp/dot-js-py-1.0.0.tar.gz` & `tmp/dot_js_py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dot-js-py-1.0.0.tar", max compression
+gzip compressed data, was "dot_js_py-2.0.0.tar", max compression
```

## Comparing `dot-js-py-1.0.0.tar` & `dot_js_py-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,22 @@
--rw-r--r--   0        0        0     1067 2022-10-26 13:15:27.675700 dot-js-py-1.0.0/LICENSE
--rw-r--r--   0        0        0     1976 2022-10-26 15:44:50.902461 dot-js-py-1.0.0/README.md
--rw-r--r--   0        0        0      515 2022-10-26 15:45:38.799597 dot-js-py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4583 2022-10-26 15:44:50.903303 dot-js-py-1.0.0/src/doT/__init__.py
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 dot-js-py-1.0.0/setup.py
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 dot-js-py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 08:37:04.028294 dot_js_py-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1976 2023-05-03 08:37:04.028383 dot_js_py-2.0.0/README.md
+-rw-r--r--   0        0        0      659 2023-05-03 16:27:45.542724 dot_js_py-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5649 2023-05-03 16:27:43.338519 dot_js_py-2.0.0/src/doT/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:14:40.230150 dot_js_py-2.0.0/src/doT/tests/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-03 16:27:43.338883 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[arrays.tmpl].json
+-rw-r--r--   0        0        0      272 2023-05-03 16:27:43.339155 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[conditionals.tmpl].json
+-rw-r--r--   0        0        0       68 2023-05-03 16:27:43.339334 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[encode.tmpl].json
+-rw-r--r--   0        0        0      117 2023-05-03 16:27:43.339580 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[evaluation.tmpl].json
+-rw-r--r--   0        0        0      109 2023-05-03 16:27:43.339824 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[interpolation.tmpl].json
+-rw-r--r--   0        0        0      177 2023-05-03 16:27:43.339994 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[issue_4.tmpl].json
+-rw-r--r--   0        0        0      137 2023-05-03 16:27:43.340157 dot_js_py-2.0.0/src/doT/tests/__snapshots__/test_dot/test_template[partials.tmpl].json
+-rw-r--r--   0        0        0      175 2023-05-03 16:27:43.340406 dot_js_py-2.0.0/src/doT/tests/conftest.py
+-rw-r--r--   0        0        0       55 2023-05-03 15:56:14.098606 dot_js_py-2.0.0/src/doT/tests/test_dot/arrays.tmpl
+-rw-r--r--   0        0        0      182 2023-05-03 15:56:09.639840 dot_js_py-2.0.0/src/doT/tests/test_dot/conditionals.tmpl
+-rw-r--r--   0        0        0       17 2023-05-03 15:56:18.492870 dot_js_py-2.0.0/src/doT/tests/test_dot/encode.tmpl
+-rw-r--r--   0        0        0       56 2023-05-03 16:27:43.340955 dot_js_py-2.0.0/src/doT/tests/test_dot/evaluation.tmpl
+-rw-r--r--   0        0        0       56 2023-05-03 16:27:43.341202 dot_js_py-2.0.0/src/doT/tests/test_dot/interpolation.tmpl
+-rw-r--r--   0        0        0       96 2023-05-03 12:49:57.759451 dot_js_py-2.0.0/src/doT/tests/test_dot/issue_4.tmpl
+-rw-r--r--   0        0        0       75 2023-05-03 15:56:04.990327 dot_js_py-2.0.0/src/doT/tests/test_dot/partials.tmpl
+-rw-r--r--   0        0        0      608 2023-05-03 16:27:43.340710 dot_js_py-2.0.0/src/doT/tests/test_dot.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 dot_js_py-2.0.0/PKG-INFO
```

### Comparing `dot-js-py-1.0.0/LICENSE` & `dot_js_py-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dot-js-py-1.0.0/README.md` & `dot_js_py-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dot-js-py-1.0.0/pyproject.toml` & `dot_js_py-2.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 [tool.poetry]
 name = "dot-js-py"
-version = "1.0.0"
+version = "2.0.0"
 description = "A python implementation of the famous js template engine. doT.js."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "doT", from = "src" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=2.7"
+python = ">=3.8.1,<4.0.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+syrupy = "<4.0.0"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `dot-js-py-1.0.0/PKG-INFO` & `dot_js_py-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: dot-js-py
-Version: 1.0.0
+Version: 2.0.0
 Summary: A python implementation of the famous js template engine. doT.js.
 License: MIT
 Author: lucemia
 Author-email: lucemia@gmail.com
-Requires-Python: >=2.7
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 doT.py
 ======
 
 A python implementation of the famous js template engine. doT.js. http://olado.github.io/doT/index.html.
 It do excetly the same thing as doT.js except written in python. Thus, it can be used in python web framework.
```

#### html2text {}

```diff
@@ -1,20 +1,16 @@
-Metadata-Version: 2.1 Name: dot-js-py Version: 1.0.0 Summary: A python
+Metadata-Version: 2.1 Name: dot-js-py Version: 2.0.0 Summary: A python
 implementation of the famous js template engine. doT.js. License: MIT Author:
-lucemia Author-email: lucemia@gmail.com Requires-Python: >=2.7 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Description-Content-Type: text/markdown doT.py ====== A python
-implementation of the famous js template engine. doT.js. http://
-olado.github.io/doT/index.html. It do excetly the same thing as doT.js except
+lucemia Author-email: lucemia@gmail.com Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Description-Content-Type: text/markdown doT.py
+====== A python implementation of the famous js template engine. doT.js. http:/
+/olado.github.io/doT/index.html. It do excetly the same thing as doT.js except
 written in python. Thus, it can be used in python web framework. doT.py compile
 the template to a pure javascript function in server side; therefore client
 side can evaluate the template later without any dependency. Which means it
 saves the time for client to load template engine and to load template file. In
 short, doT.py allows using client side template tech without include a template
 engine in client side. ## Installation `pip install doT-js-py` ### Here is an
 example: #### Use client side template ```html
```

