# Comparing `tmp/gpyt-0.2.4.tar.gz` & `tmp/gpyt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.4.tar", max compression
+gzip compressed data, was "gpyt-0.2.5.tar", max compression
```

## Comparing `gpyt-0.2.4.tar` & `gpyt-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      892 2023-05-03 06:35:37.777304 gpyt-0.2.4/README.md
--rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.4/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.4/gpyt/__main__.py
--rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.4/gpyt/_app.py
--rw-r--r--   0        0        0     4667 2023-05-03 20:36:50.527304 gpyt-0.2.4/gpyt/app.py
--rw-r--r--   0        0        0     2044 2023-05-03 06:34:17.987304 gpyt-0.2.4/gpyt/assistant.py
--rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.4/gpyt/debug.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.4/gpyt/exception.py
--rw-r--r--   0        0        0      780 2023-05-03 06:34:17.987304 gpyt-0.2.4/gpyt/styles.cssx
--rw-r--r--   0        0        0      427 2023-05-03 20:36:58.707304 gpyt-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 gpyt-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-05-03 06:35:37.777304 gpyt-0.2.5/README.md
+-rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.5/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.5/gpyt/__main__.py
+-rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.5/gpyt/_app.py
+-rw-r--r--   0        0        0     4660 2023-05-03 20:39:43.137304 gpyt-0.2.5/gpyt/app.py
+-rw-r--r--   0        0        0     2044 2023-05-03 06:34:17.987304 gpyt-0.2.5/gpyt/assistant.py
+-rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.5/gpyt/debug.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.5/gpyt/exception.py
+-rw-r--r--   0        0        0      780 2023-05-03 06:34:17.987304 gpyt-0.2.5/gpyt/styles.cssx
+-rw-r--r--   0        0        0      427 2023-05-03 20:39:50.347304 gpyt-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 gpyt-0.2.5/PKG-INFO
```

### Comparing `gpyt-0.2.4/README.md` & `gpyt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.4/gpyt/__init__.py` & `gpyt-0.2.5/gpyt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.4/gpyt/_app.py` & `gpyt-0.2.5/gpyt/_app.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.4/gpyt/app.py` & `gpyt-0.2.5/gpyt/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     """Used strictly for the purposes of renaming the Header widget."""
 
     def __init__(self, assistant: Assistant):
         super().__init__(assistant=assistant)
 
 
 def main():
-    gpt = Assistant(api_key=API_KEY or "", model=MODEL, prompt=PROMPT)
-    app = gpyt(assistant=gpt)
     app.run()
 
 
+gpt = Assistant(api_key=API_KEY or "", model=MODEL, prompt=PROMPT)
+app = gpyt(assistant=gpt)
+
 if __name__ == "__main__":
     main()
```

### Comparing `gpyt-0.2.4/gpyt/assistant.py` & `gpyt-0.2.5/gpyt/assistant.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.4/gpyt/styles.cssx` & `gpyt-0.2.5/gpyt/styles.cssx`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.4/PKG-INFO` & `gpyt-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.4
+Version: 0.2.5
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
```

