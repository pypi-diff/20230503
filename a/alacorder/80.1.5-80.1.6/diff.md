# Comparing `tmp/alacorder-80.1.5.tar.gz` & `tmp/alacorder-80.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.5.tar", max compression
+gzip compressed data, was "alacorder-80.1.6.tar", max compression
```

## Comparing `alacorder-80.1.5.tar` & `alacorder-80.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.5/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.5/README.md
--rw-r--r--   0        0        0      697 2023-05-03 02:43:24.840859 alacorder-80.1.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-02 23:39:22.186699 alacorder-80.1.5/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.5/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214501 2023-05-03 02:42:37.901150 alacorder-80.1.5/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214501 2023-05-03 02:42:32.417498 alacorder-80.1.5/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.6/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.6/README.md
+-rw-r--r--   0        0        0      697 2023-05-03 14:11:18.248192 alacorder-80.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.6/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214407 2023-05-03 14:10:42.761920 alacorder-80.1.6/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214407 2023-05-03 14:10:37.561100 alacorder-80.1.6/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.6/PKG-INFO
```

### Comparing `alacorder-80.1.5/LICENSE` & `alacorder-80.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.5/README.md` & `alacorder-80.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.5/pyproject.toml` & `alacorder-80.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.5"
+version = "80.1.6"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.5/src/alacorder/__main__.py` & `alacorder-80.1.6/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.5"
+version = "80.1.6"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1840,26 +1840,22 @@
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
-            # .str.strip()
             .alias("BondCompany"),
             pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
-            # .str.strip()
             .alias("SuretyCode"),
             pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            # .str.strip()
             .alias("BondReleaseDate"),
             pl.col("AllPagesText").str.extract(
                 r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
             )
-            # .str.strip()
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
@@ -2276,15 +2272,15 @@
             .alias("FinancialHistory"),
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
-            .str.extract(r"(\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2332,15 +2328,15 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("Charges").str.slice(0, 3).alias("Num"),
             pl.col("Charges").str.slice(4, 4).alias("Code"),
             pl.col("Charges").str.slice(9, 1).alias("Sort"),
             pl.col("Charges")
-            .str.extract(r"(\d\d/\d\d/\d\d\d\d)", group_index=1)
+            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)", group_index=1)
             .alias("CourtActionDate"),
             pl.col("Charges")
             .str.extract(
                 r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
                 group_index=0,
             )
             .alias("RAWCITE"),
@@ -2864,18 +2860,18 @@
         [
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s(\d\d/\d\d/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
+            .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
             .alias("LastUpdate"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s\d\d/\d\d/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
+            .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
@@ -2889,21 +2885,21 @@
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
-            .str.extract(r"Sentence Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("SentenceDate"),
             pl.col("Sentence")
-            .str.extract(r"Sentence Start Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("StartDate"),
             pl.col("Sentence")
-            .str.extract(r"Sentence End Date\: .{0,40}? (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\: (.+?) Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
```

### Comparing `alacorder-80.1.5/src/alacorder/alac.py` & `alacorder-80.1.6/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.5"
+version = "80.1.6"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1840,26 +1840,22 @@
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
-            # .str.strip()
             .alias("BondCompany"),
             pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
-            # .str.strip()
             .alias("SuretyCode"),
             pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            # .str.strip()
             .alias("BondReleaseDate"),
             pl.col("AllPagesText").str.extract(
                 r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
             )
-            # .str.strip()
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
@@ -2276,15 +2272,15 @@
             .alias("FinancialHistory"),
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
-            .str.extract(r"(\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2332,15 +2328,15 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("Charges").str.slice(0, 3).alias("Num"),
             pl.col("Charges").str.slice(4, 4).alias("Code"),
             pl.col("Charges").str.slice(9, 1).alias("Sort"),
             pl.col("Charges")
-            .str.extract(r"(\d\d/\d\d/\d\d\d\d)", group_index=1)
+            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)", group_index=1)
             .alias("CourtActionDate"),
             pl.col("Charges")
             .str.extract(
                 r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
                 group_index=0,
             )
             .alias("RAWCITE"),
@@ -2864,18 +2860,18 @@
         [
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s(\d\d/\d\d/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
+            .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
             .alias("LastUpdate"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s\d\d/\d\d/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
+            .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
@@ -2889,21 +2885,21 @@
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
-            .str.extract(r"Sentence Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("SentenceDate"),
             pl.col("Sentence")
-            .str.extract(r"Sentence Start Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("StartDate"),
             pl.col("Sentence")
-            .str.extract(r"Sentence End Date\: .{0,40}? (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\: (.+?) Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
```

### Comparing `alacorder-80.1.5/PKG-INFO` & `alacorder-80.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.5
+Version: 80.1.6
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

