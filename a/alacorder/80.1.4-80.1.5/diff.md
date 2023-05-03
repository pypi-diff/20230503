# Comparing `tmp/alacorder-80.1.4.tar.gz` & `tmp/alacorder-80.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.4.tar", max compression
+gzip compressed data, was "alacorder-80.1.5.tar", max compression
```

## Comparing `alacorder-80.1.4.tar` & `alacorder-80.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.4/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.4/README.md
--rw-r--r--   0        0        0      697 2023-05-02 23:40:15.727335 alacorder-80.1.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-02 23:39:22.186699 alacorder-80.1.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214420 2023-05-02 23:39:52.536356 alacorder-80.1.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214420 2023-05-02 23:39:58.640242 alacorder-80.1.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.5/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.5/README.md
+-rw-r--r--   0        0        0      697 2023-05-03 02:43:24.840859 alacorder-80.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-02 23:39:22.186699 alacorder-80.1.5/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214501 2023-05-03 02:42:37.901150 alacorder-80.1.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214501 2023-05-03 02:42:32.417498 alacorder-80.1.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.5/PKG-INFO
```

### Comparing `alacorder-80.1.4/LICENSE` & `alacorder-80.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.4/README.md` & `alacorder-80.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.4/pyproject.toml` & `alacorder-80.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.4"
+version = "80.1.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.4/src/alacorder/.DS_Store` & `alacorder-80.1.5/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.4/src/alacorder/__main__.py` & `alacorder-80.1.5/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.4"
+version = "80.1.5"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1622,14 +1622,15 @@
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
+            .str.replace(r'[A-Za-z\:\s]+','')
             .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
@@ -1724,15 +1725,15 @@
             .alias("Judge"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office \#: ([0-9\-]+)")
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
-            .str.replace(r"\n", "")
+            .str.replace(r"\n", " ")
             .str.replace(r"\s+", " ")
             .str.strip()
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
             .str.replace(r"^\-.+", "")
             .str.replace(r"County\:", "")
@@ -1878,20 +1879,21 @@
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
-            .str.rstrip(r"O", "")
+            .str.rstrip("O")
             .str.strip()
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
+            .str.replace_all(r'\n','')
             .str.strip()
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .alias("AppealTo"),
             pl.col("AllPagesText")
```

### Comparing `alacorder-80.1.4/src/alacorder/alac.py` & `alacorder-80.1.5/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.4"
+version = "80.1.5"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1622,14 +1622,15 @@
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
+            .str.replace(r'[A-Za-z\:\s]+','')
             .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
@@ -1724,15 +1725,15 @@
             .alias("Judge"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office \#: ([0-9\-]+)")
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
-            .str.replace(r"\n", "")
+            .str.replace(r"\n", " ")
             .str.replace(r"\s+", " ")
             .str.strip()
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
             .str.replace(r"^\-.+", "")
             .str.replace(r"County\:", "")
@@ -1878,20 +1879,21 @@
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
-            .str.rstrip(r"O", "")
+            .str.rstrip("O")
             .str.strip()
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
+            .str.replace_all(r'\n','')
             .str.strip()
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .alias("AppealTo"),
             pl.col("AllPagesText")
```

### Comparing `alacorder-80.1.4/PKG-INFO` & `alacorder-80.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.4
+Version: 80.1.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

