# Comparing `tmp/e-models-1.2.1.tar.gz` & `tmp/e-models-1.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.2.1.tar", last modified: Wed May  3 15:01:21 2023, max compression
+gzip compressed data, was "e-models-1.2.1.1.tar", last modified: Wed May  3 15:11:31 2023, max compression
```

## Comparing `e-models-1.2.1.tar` & `e-models-1.2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.959453 e-models-1.2.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-03 15:01:21.959453 e-models-1.2.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.955453 e-models-1.2.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-03 15:01:21.000000 e-models-1.2.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-03 15:01:21.000000 e-models-1.2.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-03 15:01:21.000000 e-models-1.2.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       16 2023-05-03 15:01:21.000000 e-models-1.2.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-03 15:01:21.000000 e-models-1.2.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.955453 e-models-1.2.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-05-03 15:00:53.000000 e-models-1.2.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.955453 e-models-1.2.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34921 2023-05-03 14:53:27.000000 e-models-1.2.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.2.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2.1/emodels/html2text/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.955453 e-models-1.2.1/emodels/markdown/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2.1/emodels/markdown/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8316 2023-05-03 14:56:38.000000 e-models-1.2.1/emodels/markdown/tables.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2.1/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-02 19:24:43.000000 e-models-1.2.1/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-03 15:01:21.959453 e-models-1.2.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      927 2023-05-03 15:00:45.000000 e-models-1.2.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:01:21.955453 e-models-1.2.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3699 2023-05-03 14:51:03.000000 e-models-1.2.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2.1.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:11:31.735538 e-models-1.2.1.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2.1.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:11:31.000000 e-models-1.2.1.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-03 15:11:31.000000 e-models-1.2.1.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-03 15:11:31.000000 e-models-1.2.1.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       16 2023-05-03 15:11:31.000000 e-models-1.2.1.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-03 15:11:31.000000 e-models-1.2.1.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-05-03 15:11:08.000000 e-models-1.2.1.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2.1.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34807 2023-05-03 15:09:49.000000 e-models-1.2.1.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.2.1.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2.1.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2.1.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2.1.1/emodels/html2text/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/emodels/markdown/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2.1.1/emodels/markdown/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8316 2023-05-03 15:09:49.000000 e-models-1.2.1.1/emodels/markdown/tables.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2.1.1/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-02 19:24:43.000000 e-models-1.2.1.1/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2.1.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-03 15:11:31.735538 e-models-1.2.1.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      929 2023-05-03 15:11:01.000000 e-models-1.2.1.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:11:31.735538 e-models-1.2.1.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3699 2023-05-03 14:51:03.000000 e-models-1.2.1.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2.1.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.2.1/LICENSE` & `e-models-1.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/PKG-INFO` & `e-models-1.2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1
+Version: 1.2.1.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1/README.md` & `e-models-1.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/e_models.egg-info/PKG-INFO` & `e-models-1.2.1.1/e_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1
+Version: 1.2.1.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1/e_models.egg-info/SOURCES.txt` & `e-models-1.2.1.1/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/emodels/html2text/__init__.py` & `e-models-1.2.1.1/emodels/html2text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -643,15 +643,14 @@
 
                 if tag == "tr" and start:
                     self.within_table_row += 1
                     self.td_count = 0
                     self.o("| ", line_break="\n")
                 if tag == "tr" and not start:
                     self.split_next_td = False
-                    print("HUHU end", self.within_table_row)
                     self.o("|")
                     if self.within_table_row > 0:
                         self.within_table_row -= 1
                     self.pbr()
                 if tag == "tr" and not start and self.table_header:
                     # Underline table header
                     self.o("| " + "|".join(["---"] * self.td_count) + "|")
@@ -750,15 +749,14 @@
             if force == "end":
                 # It's the end.
                 self.p_p = 0
                 self.out("\n")
                 self.space = False
 
             if self.p_p:
-                print("MEME", self.within_table_row)
                 if line_break is None:
                     line_break = "<br>" if self.within_table_row > 0 else "\n"
                 self.out((self.br_toggle + line_break + bq) * self.p_p)
                 self.space = False
                 self.br_toggle = ""
 
             if self.space:
```

### Comparing `e-models-1.2.1/emodels/html2text/config.py` & `e-models-1.2.1.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/emodels/html2text/utils.py` & `e-models-1.2.1.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/emodels/markdown/tables.py` & `e-models-1.2.1.1/emodels/markdown/tables.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/emodels/scrapyutils.py` & `e-models-1.2.1.1/emodels/scrapyutils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/setup.py` & `e-models-1.2.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.2.1',
+    version      = '1.2.1.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.2.1/tests/test_html2text.py` & `e-models-1.2.1.1/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1/tests/test_scrapyutils.py` & `e-models-1.2.1.1/tests/test_scrapyutils.py`

 * *Files identical despite different names*

