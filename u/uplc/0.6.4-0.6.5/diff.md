# Comparing `tmp/uplc-0.6.4.tar.gz` & `tmp/uplc-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplc-0.6.4.tar", last modified: Mon Apr 24 17:44:30 2023, max compression
+gzip compressed data, was "uplc-0.6.5.tar", max compression
```

## Comparing `uplc-0.6.4.tar` & `uplc-0.6.5.tar`

### file list

```diff
@@ -1,37 +1,24 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.313256 uplc-0.6.4/
--rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-04-24 17:34:06.000000 uplc-0.6.4/LICENSE.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-24 17:44:30.313256 uplc-0.6.4/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     2034 2023-04-24 17:34:06.000000 uplc-0.6.4/README.md
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-24 17:44:30.313256 uplc-0.6.4/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     2056 2023-04-24 17:34:06.000000 uplc-0.6.4/setup.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.305256 uplc-0.6.4/uplc/
--rw-r--r--   0 travis    (1000) travis    (1000)      555 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4935 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    28464 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9066 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/flat_decoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10052 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/flat_encoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1202 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/lexer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3357 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/machine.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc/optimizer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/optimizer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      630 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/optimizer/pre_evaluation.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10960 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/parser.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3391 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_acceptance.py
--rw-r--r--   0 travis    (1000) travis    (1000)    14584 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_hypothesis.py
--rw-r--r--   0 travis    (1000) travis    (1000)   211128 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_misc.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1998 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tools.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.313256 uplc-0.6.4/uplc/transformer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      784 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/debrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)      938 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/undebrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1947 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/unique_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3009 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      673 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      110 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1077 2023-01-04 11:32:30.433673 uplc-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-03 14:34:13.048895 uplc-0.6.5/README.md
+-rw-r--r--   0        0        0     1347 2023-05-03 14:30:50.424968 uplc-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-05-03 14:30:50.424968 uplc-0.6.5/uplc/__init__.py
+-rw-r--r--   0        0        0     4935 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/__main__.py
+-rw-r--r--   0        0        0    28464 2023-04-24 17:32:55.398635 uplc-0.6.5/uplc/ast.py
+-rw-r--r--   0        0        0     9066 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/flat_decoder.py
+-rw-r--r--   0        0        0    10052 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/flat_encoder.py
+-rw-r--r--   0        0        0     1202 2023-02-14 01:15:57.671994 uplc-0.6.5/uplc/lexer.py
+-rw-r--r--   0        0        0     3357 2023-03-16 14:22:54.137366 uplc-0.6.5/uplc/machine.py
+-rw-r--r--   0        0        0        0 2023-02-09 01:14:10.658495 uplc-0.6.5/uplc/optimizer/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/optimizer/pre_evaluation.py
+-rw-r--r--   0        0        0    10960 2023-03-26 20:25:01.867354 uplc-0.6.5/uplc/parser.py
+-rw-r--r--   0        0        0        0 2023-01-09 21:06:56.197975 uplc-0.6.5/uplc/tests/__init__.py
+-rw-r--r--   0        0        0     3391 2023-02-09 01:14:54.974376 uplc-0.6.5/uplc/tests/test_acceptance.py
+-rw-r--r--   0        0        0    14584 2023-04-24 17:32:55.398635 uplc-0.6.5/uplc/tests/test_hypothesis.py
+-rw-r--r--   0        0        0   211128 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/tests/test_misc.py
+-rw-r--r--   0        0        0     1998 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/tools.py
+-rw-r--r--   0        0        0        0 2023-01-22 02:07:47.763052 uplc-0.6.5/uplc/transformer/__init__.py
+-rw-r--r--   0        0        0      784 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/transformer/debrujin_variables.py
+-rw-r--r--   0        0        0      938 2023-03-26 20:25:01.871354 uplc-0.6.5/uplc/transformer/undebrujin_variables.py
+-rw-r--r--   0        0        0     1947 2023-04-13 20:56:49.628229 uplc-0.6.5/uplc/transformer/unique_variables.py
+-rw-r--r--   0        0        0     3009 2023-04-06 19:16:35.707063 uplc-0.6.5/uplc/util.py
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 uplc-0.6.5/PKG-INFO
```

### Comparing `uplc-0.6.4/LICENSE.txt` & `uplc-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/PKG-INFO` & `uplc-0.6.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: uplc
-Version: 0.6.4
-Summary: Python implementation of untyped plutus language core
-Home-page: https://github.com/opshin/uplc
-Author: nielstron
-Author-email: n.muendler@web.de
-License: MIT
-Keywords: python cardano smart contract blockchain verification haskell
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Assemblers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 Untyped Plutus Language Core 
 ==================================================
 [![Build Status](https://app.travis-ci.com/OpShin/uplc.svg?branch=master)](https://app.travis-ci.com/OpShin/uplc)
  [![PyPI version](https://badge.fury.io/py/uplc.svg)](https://pypi.org/project/uplc/)
  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uplc.svg)
  [![PyPI - Status](https://img.shields.io/pypi/status/uplc.svg)](https://pypi.org/project/uplc/)
 [![Coverage Status](https://coveralls.io/repos/github/OpShin/uplc/badge.svg?branch=master)](https://coveralls.io/github/OpShin/uplc?branch=master)
@@ -60,14 +39,20 @@
 uplc dump examples/fibonacci.uplc --dialect plutus --unique-varnames
 
 # Evaluate a UPLC program on UPLC input
 uplc eval examples/fibonacci.uplc "(con integer 5)"
 
 # Build smart contract artifacts from the UPLC program
 uplc build examples/fibonacci.uplc
+
+# This package can also be used to analyze built contracts (output from any Smart Contract Language)
+uplc dump build/fibonacci/script.cbor --from-cbor
+
+# Show all options
+uplc --help
 ```
 
 
 ## Scope and Contributions
 This is a side product of the development of a pythonic smart contract language for the Cardano blockchain
 and hence much tailored to the needs of that development.
```

### Comparing `uplc-0.6.4/uplc/__main__.py` & `uplc-0.6.5/uplc/__main__.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/ast.py` & `uplc-0.6.5/uplc/ast.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/flat_decoder.py` & `uplc-0.6.5/uplc/flat_decoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/flat_encoder.py` & `uplc-0.6.5/uplc/flat_encoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/lexer.py` & `uplc-0.6.5/uplc/lexer.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/machine.py` & `uplc-0.6.5/uplc/machine.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/optimizer/pre_evaluation.py` & `uplc-0.6.5/uplc/optimizer/pre_evaluation.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/parser.py` & `uplc-0.6.5/uplc/parser.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/tests/test_acceptance.py` & `uplc-0.6.5/uplc/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/tests/test_hypothesis.py` & `uplc-0.6.5/uplc/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/tests/test_misc.py` & `uplc-0.6.5/uplc/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/tools.py` & `uplc-0.6.5/uplc/tools.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/transformer/debrujin_variables.py` & `uplc-0.6.5/uplc/transformer/debrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/transformer/undebrujin_variables.py` & `uplc-0.6.5/uplc/transformer/undebrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/transformer/unique_variables.py` & `uplc-0.6.5/uplc/transformer/unique_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.4/uplc/util.py` & `uplc-0.6.5/uplc/util.py`

 * *Files identical despite different names*

