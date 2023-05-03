# Comparing `tmp/gpyt-0.2.0.tar.gz` & `tmp/gpyt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.0.tar", max compression
+gzip compressed data, was "gpyt-0.2.1.tar", max compression
```

## Comparing `gpyt-0.2.0.tar` & `gpyt-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      709 2023-05-03 03:53:32.417304 gpyt-0.2.0/README.md
--rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.0/gpyt/__main__.py
--rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/_app.py
--rw-r--r--   0        0        0     4150 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/app.py
--rw-r--r--   0        0        0     2012 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/assistant.py
--rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.0/gpyt/debug.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.0/gpyt/exception.py
--rw-r--r--   0        0        0      736 2023-05-03 03:53:32.417304 gpyt-0.2.0/gpyt/styles.cssx
--rw-r--r--   0        0        0      427 2023-05-03 03:53:32.417304 gpyt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 gpyt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      787 2023-05-03 03:56:16.807304 gpyt-0.2.1/README.md
+-rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.1/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.1/gpyt/__main__.py
+-rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.1/gpyt/_app.py
+-rw-r--r--   0        0        0     4150 2023-05-03 03:53:32.417304 gpyt-0.2.1/gpyt/app.py
+-rw-r--r--   0        0        0     2012 2023-05-03 03:53:32.417304 gpyt-0.2.1/gpyt/assistant.py
+-rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.1/gpyt/debug.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.1/gpyt/exception.py
+-rw-r--r--   0        0        0      736 2023-05-03 03:53:32.417304 gpyt-0.2.1/gpyt/styles.cssx
+-rw-r--r--   0        0        0      427 2023-05-03 03:56:52.777304 gpyt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 gpyt-0.2.1/PKG-INFO
```

### Comparing `gpyt-0.2.0/README.md` & `gpyt-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # gpyt
 
 Interact with GPT on the command line.
 
-
 > WIP
 
+Uses [Textual](https://textual.textualize.io).
+
+
 ### How to run:
 ```sh
 $ pip install gpyt
 
 add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
 $ python -m gpyt
 ```
 
 ### Desired Features
+
 * `copy` to copy GPT's response to clipboard
-* color coded responses
 * add gpt jailbreaks (DAN-esque)
 * `new` to start a new chat (clear all history and console window)
 * store chat logs somewhere.
 * add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
   (informal) or -f (for file input) or --dan (for jailbreak)
 * scrolling text (adjustable speed, or disable all together)
 * use streams api?
 * model select CLI
-* loading wheel
-* textual !!!
+* add API_KEY from CLI
+
+
+### Completed Features
+
+[x] loading wheel
+[x] textual !!!
```

### Comparing `gpyt-0.2.0/gpyt/__init__.py` & `gpyt-0.2.1/gpyt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.0/gpyt/_app.py` & `gpyt-0.2.1/gpyt/_app.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.0/gpyt/app.py` & `gpyt-0.2.1/gpyt/app.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.0/gpyt/assistant.py` & `gpyt-0.2.1/gpyt/assistant.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.0/gpyt/styles.cssx` & `gpyt-0.2.1/gpyt/styles.cssx`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.0/PKG-INFO` & `gpyt-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.0
+Version: 0.2.1
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
@@ -14,33 +14,40 @@
 Requires-Dist: textual[dev] (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
 Interact with GPT on the command line.
 
-
 > WIP
 
+Uses [Textual](https://textual.textualize.io).
+
+
 ### How to run:
 ```sh
 $ pip install gpyt
 
 add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
 $ python -m gpyt
 ```
 
 ### Desired Features
+
 * `copy` to copy GPT's response to clipboard
-* color coded responses
 * add gpt jailbreaks (DAN-esque)
 * `new` to start a new chat (clear all history and console window)
 * store chat logs somewhere.
 * add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
   (informal) or -f (for file input) or --dan (for jailbreak)
 * scrolling text (adjustable speed, or disable all together)
 * use streams api?
 * model select CLI
-* loading wheel
-* textual !!!
+* add API_KEY from CLI
+
+
+### Completed Features
+
+[x] loading wheel
+[x] textual !!!
```

