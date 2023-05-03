# Comparing `tmp/dreamai_pdf-0.0.5.tar.gz` & `tmp/dreamai_pdf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.5.tar", last modified: Tue May  2 22:45:30 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.6.tar", last modified: Wed May  3 19:30:23 2023, max compression
```

## Comparing `dreamai_pdf-0.0.5.tar` & `dreamai_pdf-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.5/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 22:45:02.000000 dreamai_pdf-0.0.5/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5299 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.5/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/parse.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2101 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1683 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2368 2023-05-02 22:45:02.000000 dreamai_pdf-0.0.5/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.6/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.6/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1683 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2368 2023-05-03 19:29:46.000000 dreamai_pdf-0.0.6/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/setup.py
```

### Comparing `dreamai_pdf-0.0.5/LICENSE` & `dreamai_pdf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.5/PKG-INFO` & `dreamai_pdf-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf/_modidx.py` & `dreamai_pdf-0.0.6/dreamai_pdf/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,10 +39,12 @@
                                    'dreamai_pdf.parse.pdf_to_batch': ('parse.html#pdf_to_batch', 'dreamai_pdf/parse.py'),
                                    'dreamai_pdf.parse.pdf_to_cols': ('parse.html#pdf_to_cols', 'dreamai_pdf/parse.py'),
                                    'dreamai_pdf.parse.pdf_to_text': ('parse.html#pdf_to_text', 'dreamai_pdf/parse.py'),
                                    'dreamai_pdf.parse.pred_cols': ('parse.html#pred_cols', 'dreamai_pdf/parse.py')},
             'dreamai_pdf.segment': { 'dreamai_pdf.segment.get_contact_dict': ('segment.html#get_contact_dict', 'dreamai_pdf/segment.py'),
                                      'dreamai_pdf.segment.get_edu_dicts': ('segment.html#get_edu_dicts', 'dreamai_pdf/segment.py'),
                                      'dreamai_pdf.segment.get_job_dicts': ('segment.html#get_job_dicts', 'dreamai_pdf/segment.py'),
+                                     'dreamai_pdf.segment.load_ner_model': ('segment.html#load_ner_model', 'dreamai_pdf/segment.py'),
+                                     'dreamai_pdf.segment.load_segs_model': ('segment.html#load_segs_model', 'dreamai_pdf/segment.py'),
                                      'dreamai_pdf.segment.ners_to_dicts': ('segment.html#ners_to_dicts', 'dreamai_pdf/segment.py'),
                                      'dreamai_pdf.segment.segment_to_ners': ('segment.html#segment_to_ners', 'dreamai_pdf/segment.py'),
                                      'dreamai_pdf.segment.text_to_segments': ('segment.html#text_to_segments', 'dreamai_pdf/segment.py')}}}
```

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf/core.py` & `dreamai_pdf-0.0.6/dreamai_pdf/core.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf/parse.py` & `dreamai_pdf-0.0.6/dreamai_pdf/parse.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf/segment.py` & `dreamai_pdf-0.0.6/dreamai_pdf/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_segment.ipynb.
 
 # %% auto 0
-__all__ = ['text_to_segments', 'segment_to_ners', 'ners_to_dicts', 'get_edu_dicts', 'get_job_dicts', 'get_contact_dict']
+__all__ = ['text_to_segments', 'segment_to_ners', 'ners_to_dicts', 'get_edu_dicts', 'get_job_dicts', 'get_contact_dict',
+           'load_segs_model', 'load_ner_model']
 
 # %% ../nbs/02_segment.ipynb 3
 from .core import *
 from .parse import *
 from .imports import *
 
 
@@ -56,7 +57,12 @@
     if is_list(text): text = ' '.join(text)
     mail_regex = re.compile(r'[\w.+-]+@[\w-]+\.[\w.-]+')
     phone_regex = re.compile(r'[\d]{3}[\s-]?[\d]{3}[\s-]?[\d]{4}')
     emails = re.findall(mail_regex, text.lower())
     phones = re.findall(phone_regex, text.lower())
     return {'EMAIL':emails, 'PHONE':phones}
 
+def load_segs_model():
+    return Labels("roberta-large-mnli")
+
+def load_ner_model():
+    return Classifier.load('ner-ontonotes-large')
```

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.6/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.5/dreamai_pdf.egg-info/requires.txt` & `dreamai_pdf-0.0.6/dreamai_pdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.5/settings.ini` & `dreamai_pdf-0.0.6/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_pdf
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_pdf
 nbs_path = nbs
 recursive = True
```

### Comparing `dreamai_pdf-0.0.5/setup.py` & `dreamai_pdf-0.0.6/setup.py`

 * *Files identical despite different names*

