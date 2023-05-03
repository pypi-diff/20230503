# Comparing `tmp/ausbildungsnachweise_utils-0.0.6.tar.gz` & `tmp/ausbildungsnachweise_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ausbildungsnachweise_utils-0.0.6.tar", last modified: Wed May  3 07:30:52 2023, max compression
+gzip compressed data, was "ausbildungsnachweise_utils-0.0.7.tar", last modified: Wed May  3 10:51:06 2023, max compression
```

## Comparing `ausbildungsnachweise_utils-0.0.6.tar` & `ausbildungsnachweise_utils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3085 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/processor.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2204 2023-05-03 07:23:35.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/starter.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.439607 ausbildungsnachweise_utils-0.0.7/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3281 2023-05-03 10:37:49.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/processor.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2204 2023-05-03 10:35:16.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/starter.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-03 10:51:06.439607 ausbildungsnachweise_utils-0.0.7/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/setup.py
```

### Comparing `ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/processor.py` & `ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 import subprocess
 import xml.etree.ElementTree as ET
 
 from pathlib import Path
 from docx import Document
 
 
-FILE_DIR = Path(__file__).parent
+# FILE_DIR = Path(__file__).parent
+FILE_DIR = Path().absolute()
 
 LIBREOFFICE_BINARY = "libreoffice"
 
-DEFAULT_SIGNATURE_FILE_PATH = FILE_DIR / "../resources/default_signature.png"
-DEFAULT_TEMPLATE_FILE_PATH = FILE_DIR / "../resources/template_ausbildungsnachweis.docx"
+# DEFAULT_SIGNATURE_FILE_PATH = FILE_DIR / "../resources/default_signature.png"
+# DEFAULT_TEMPLATE_FILE_PATH = FILE_DIR / "../resources/template_ausbildungsnachweis.docx"
+DEFAULT_SIGNATURE_FILE_PATH = FILE_DIR / "resources/default_signature.png"
+DEFAULT_TEMPLATE_FILE_PATH = FILE_DIR / "resources/template_ausbildungsnachweis.docx"
 
 
 def sign_pdf(input_file_path: Path, output_file_path: Path, signature_img_file_path: Path = DEFAULT_SIGNATURE_FILE_PATH) -> None:
     doc = fitz.open(input_file_path)
 
     for page in doc:
         # Find
```

### Comparing `ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/starter.py` & `ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/starter.py`

 * *Files identical despite different names*

### Comparing `ausbildungsnachweise_utils-0.0.6/setup.py` & `ausbildungsnachweise_utils-0.0.7/setup.py`

 * *Files identical despite different names*

