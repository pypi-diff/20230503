# Comparing `tmp/e-models-1.2.1.2.tar.gz` & `tmp/e-models-1.2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.2.1.2.tar", last modified: Wed May  3 15:34:41 2023, max compression
+gzip compressed data, was "e-models-1.2.1.3.tar", last modified: Wed May  3 15:51:59 2023, max compression
```

## Comparing `e-models-1.2.1.2.tar` & `e-models-1.2.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2.1.2/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:34:41.107950 e-models-1.2.1.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2.1.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:34:41.000000 e-models-1.2.1.2/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-03 15:34:41.000000 e-models-1.2.1.2/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-03 15:34:41.000000 e-models-1.2.1.2/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       16 2023-05-03 15:34:41.000000 e-models-1.2.1.2/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-03 15:34:41.000000 e-models-1.2.1.2/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-05-03 15:33:18.000000 e-models-1.2.1.2/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2.1.2/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34907 2023-05-03 15:21:59.000000 e-models-1.2.1.2/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-03 15:32:59.000000 e-models-1.2.1.2/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2.1.2/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2.1.2/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2.1.2/emodels/html2text/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/emodels/markdown/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2.1.2/emodels/markdown/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8316 2023-05-03 15:09:49.000000 e-models-1.2.1.2/emodels/markdown/tables.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2.1.2/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-03 15:32:59.000000 e-models-1.2.1.2/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2.1.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-03 15:34:41.107950 e-models-1.2.1.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      929 2023-05-03 15:34:12.000000 e-models-1.2.1.2/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:34:41.107950 e-models-1.2.1.2/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4414 2023-05-03 15:32:59.000000 e-models-1.2.1.2/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2.1.2/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.725805 e-models-1.2.1.3/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2.1.3/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:51:59.725805 e-models-1.2.1.3/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2.1.3/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.721805 e-models-1.2.1.3/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 15:51:59.000000 e-models-1.2.1.3/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-03 15:51:59.000000 e-models-1.2.1.3/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-03 15:51:59.000000 e-models-1.2.1.3/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       16 2023-05-03 15:51:59.000000 e-models-1.2.1.3/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-03 15:51:59.000000 e-models-1.2.1.3/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.721805 e-models-1.2.1.3/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-05-03 15:51:17.000000 e-models-1.2.1.3/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2.1.3/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.721805 e-models-1.2.1.3/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35088 2023-05-03 15:43:42.000000 e-models-1.2.1.3/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-03 15:32:59.000000 e-models-1.2.1.3/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2.1.3/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2.1.3/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2.1.3/emodels/html2text/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.725805 e-models-1.2.1.3/emodels/markdown/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2.1.3/emodels/markdown/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8316 2023-05-03 15:09:49.000000 e-models-1.2.1.3/emodels/markdown/tables.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2.1.3/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-03 15:32:59.000000 e-models-1.2.1.3/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2.1.3/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-03 15:51:59.725805 e-models-1.2.1.3/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      929 2023-05-03 15:51:11.000000 e-models-1.2.1.3/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 15:51:59.725805 e-models-1.2.1.3/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4410 2023-05-03 15:49:26.000000 e-models-1.2.1.3/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2.1.3/tests/test_scrapyutils.py
```

### Comparing `e-models-1.2.1.2/LICENSE` & `e-models-1.2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/PKG-INFO` & `e-models-1.2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1.2
+Version: 1.2.1.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1.2/README.md` & `e-models-1.2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/e_models.egg-info/PKG-INFO` & `e-models-1.2.1.3/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1.2
+Version: 1.2.1.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1.2/e_models.egg-info/SOURCES.txt` & `e-models-1.2.1.3/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/emodels/html2text/__init__.py` & `e-models-1.2.1.3/emodels/html2text/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,15 +751,21 @@
                 # It's the end.
                 self.p_p = 0
                 self.out("\n")
                 self.space = False
 
             if self.p_p:
                 if line_break is None:
-                    line_break = "<br>" if self.within_table_row > 0 and self.enable_br_within_table else "\n"
+                    if self.within_table_row:
+                        if self.enable_br_within_table:
+                            line_break = "<br>"
+                        else:
+                            line_break = ""
+                    else:
+                        line_break = "\n"
                 self.out((self.br_toggle + line_break + bq) * self.p_p)
                 self.space = False
                 self.br_toggle = ""
 
             if self.space:
                 if not self.lastWasNL:
                     self.out(" ")
```

### Comparing `e-models-1.2.1.2/emodels/html2text/config.py` & `e-models-1.2.1.3/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/emodels/html2text/utils.py` & `e-models-1.2.1.3/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/emodels/markdown/tables.py` & `e-models-1.2.1.3/emodels/markdown/tables.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/emodels/scrapyutils.py` & `e-models-1.2.1.3/emodels/scrapyutils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.2/setup.py` & `e-models-1.2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.2.1.2',
+    version      = '1.2.1.3',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.2.1.2/tests/test_html2text.py` & `e-models-1.2.1.3/tests/test_html2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,11 @@
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
 <tr><td>Data 7</td><td>Data 8</td></tr>
 </table>
 """
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
-| Data 5| 
-
-Data 6
-
-|
+| Data 5| Data 6|
 | Data 7| Data 8|
 """
         self.assertEqual(response.markdown, expected)
```

### Comparing `e-models-1.2.1.2/tests/test_scrapyutils.py` & `e-models-1.2.1.3/tests/test_scrapyutils.py`

 * *Files identical despite different names*

