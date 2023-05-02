# Comparing `tmp/alacorder-80.1.3.tar.gz` & `tmp/alacorder-80.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.3.tar", max compression
+gzip compressed data, was "alacorder-80.1.4.tar", max compression
```

## Comparing `alacorder-80.1.3.tar` & `alacorder-80.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.3/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.3/README.md
--rw-r--r--   0        0        0      697 2023-05-02 17:22:11.238178 alacorder-80.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.3/src/alacorder/__init__.py
--rw-r--r--   0        0        0   213086 2023-05-02 17:21:47.228463 alacorder-80.1.3/src/alacorder/__main__.py
--rw-r--r--   0        0        0   213086 2023-05-02 17:21:55.202860 alacorder-80.1.3/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.4/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.4/README.md
+-rw-r--r--   0        0        0      697 2023-05-02 23:40:15.727335 alacorder-80.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-02 23:39:22.186699 alacorder-80.1.4/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.4/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214420 2023-05-02 23:39:52.536356 alacorder-80.1.4/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214420 2023-05-02 23:39:58.640242 alacorder-80.1.4/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.4/PKG-INFO
```

### Comparing `alacorder-80.1.3/LICENSE` & `alacorder-80.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.3/README.md` & `alacorder-80.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.3/pyproject.toml` & `alacorder-80.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.3"
+version = "80.1.4"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.3/src/alacorder/__main__.py` & `alacorder-80.1.4/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.3"
+version = "80.1.4"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -127,15 +127,15 @@
 
 
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
-    plog("Extracting case info...", cf=cf)
+    print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
     ch = split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
     fs = split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
     fh = explode_split_financial_history(df, debug=cf["DEBUG"])
@@ -187,14 +187,15 @@
         "sentences": sent,
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
+    print("Completed table export.", cf=cf)
     return out
 
 
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
@@ -1577,28 +1578,28 @@
     cases = df.with_columns(
         [
             pl.col("AllPagesText")
             .str.extract(
                 r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                 group_index=1,
             )
-            .str.replace_all("Case Number:", "", literal=True)
+            .str.replace("Case Number:", "", literal=True)
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesTextNoNewLine")
             .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
-            .str.replace_all(r"[^\d/]", "")
+            .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1606,36 +1607,38 @@
                     pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
                 ]
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
-            .str.replace_all(r"(.{3}0000000)", "")
+            .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
             pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").alias("Race"),
             pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
-            .str.replace_all(r"[A-Z].+", "")
+            .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
+            .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
+            .str.strip()
             .alias("State"),
             pl.col("AllPagesText")
             .str.extract_all(
                 r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
             )
             .alias("RE_Charges"),
             pl.col("AllPagesText")
@@ -1695,19 +1698,19 @@
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
-            .str.strip()
             .alias("JuryDemand"),
-            pl.col("AllPagesText")
-            .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(
+                r"Inpatient Treatment Ordered: ([YES|NO]?)"
+            )
+            # .str.strip()
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
             .alias("TrialType"),
             pl.col("AllPagesText")
@@ -1721,25 +1724,31 @@
             .alias("Judge"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office \#: ([0-9\-]+)")
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
+            .str.replace(r"\n", "")
+            .str.replace(r"\s+", " ")
             .str.strip()
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
-            .str.replace(r"\n", "")
+            .str.replace(r"^\-.+", "")
+            .str.replace(r"County\:", "")
+            .str.replace(r"Defendant Status\:", "")
+            .str.replace(r"Judge\:", "")
+            .str.replace(r"Trial Type\:", "")
+            .str.replace(r"Probation Office \#\:", "")
             .str.strip()
             .alias("ArrestingAgencyType"),
             pl.col("AllPagesText")
             .str.extract(r"Arresting Officer: ([A-Z\s]+)")
-            .str.rstrip("S")
-            .str.rstrip("P")
+            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.strip()
             .alias("ArrestingOfficer"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office Name: ([A-Z0-9]+)")
             .alias("ProbationOfficeName"),
             pl.col("AllPagesText")
             .str.extract(r"Traffic Citation \#: ([A-Z0-9]+)")
@@ -1752,24 +1761,24 @@
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.strip()
             .alias("CaseInitiationType"),
             pl.col("AllPagesText")
             .str.extract(r"Domestic Violence: ([YES|NO])")
-            .str.strip()
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
+            .str.replace(r"\n", "")
+            .str.replace(r"\s+", " ")
             .str.strip()
             .alias("AgencyORI"),
             pl.col("AllPagesText")
             .str.extract(r"Driver License N°: ([A-Z0-9]+)")
-            .str.strip()
             .alias("DLRAW"),
             pl.col("AllPagesText")
             .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
             .alias("SSN"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z0-9]{11}?) State ID:")
             .alias("SIDRAW"),
@@ -1796,96 +1805,97 @@
             .str.strip()
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Issuance Status: (\w)")
+            .str.extract(r"Warrant Issuance Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantIssuanceStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Action Status: (\w)")
+            .str.extract(r"Warrant Action Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantActionStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Location Status: (\w)")
+            .str.extract(r"Warrant Location Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantLocationStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
             .str.strip()
             .alias("NumberOfWarrants"),
             pl.col("AllPagesText")
-            .str.extract(r"Bond Type: (\w)")
+            .str.extract(r"Bond Type: (\w+)")  # +
+            .str.replace(r"Bond", "")
             .str.strip()
             .alias("BondType"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
             .str.strip()
             .alias("BondTypeDesc"),
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
-            .str.replace_all(r"[^0-9\.\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
-            .str.strip()
+            # .str.strip()
             .alias("BondCompany"),
-            pl.col("AllPagesText")
-            .str.extract(r"Surety Code: ([A-Z0-9]{4})")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
+            # .str.strip()
             .alias("SuretyCode"),
-            pl.col("AllPagesText")
-            .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            # .str.strip()
             .alias("BondReleaseDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(
+                r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
+            )
+            # .str.strip()
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
             pl.col("AllPagesText")
             .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
             .str.strip()
             .alias("BondsmanProcessReturn"),
             pl.col("AllPagesText")
             .str.extract(r"([\n\s/\d]*?) Appeal Court:")
-            .str.replace_all(r"[\n\s]", "")
             .str.strip()
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
             .alias("AppealCourt"),
             pl.col("AllPagesText")
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
-            .str.rstrip("D")
-            .str.rstrip("T")
+            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
+            .str.rstrip(r"O", "")
             .str.strip()
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
             .str.strip()
             .alias("AppealStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Appeal To: (\w?) Appeal")
+            .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("LowerCourtAppealDate"),
@@ -1920,51 +1930,105 @@
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
+            .str.replace(r"Financial", "")
             .str.strip()
             .alias("TBNV2"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Date\: (\d\d/\d\d/\d\d\d\d)').alias("TurnOverDate"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("TurnOverAmt"),
-            pl.col("AllPagesText").str.extract(r'Frequency Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("FrequencyAmt"),
-            pl.col("AllPagesText").str.extract(r'Due Date\: (\d\d/\d\d/\d\d\d\d)').alias("DueDate"),
-            pl.col("AllPagesText").str.extract(r'Last Paid Date\: (\d\d/\d\d/\d\d\d\d)').alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r'Payor\: ([A-Z0-9]{4})').alias("Payor"),
-            pl.col("AllPagesText").str.extract(r'Enforcement Status\: ([A-Z\:,\s]+)').str.replace_all(r'\s+',' ').str.replace(r' F$','').str.strip().alias("EnforcementStatus"),
-            pl.col("AllPagesText").str.extract(r'Frequency\: (.+)').str.replace(r'Cost Paid By\:','').str.strip().alias("Frequency"),
-            pl.col("AllPagesText").str.extract(r'Placement Status\: (.+)').str.strip().alias("PlacementStatus"),
-            pl.col("AllPagesText").str.extract(r'Comments\: (.+)').str.strip().alias("Comments"),
-            pl.col("AllPagesText").str.extract(r'Over/Under Paid\: \$(\d+\.\d\d)').alias("OverUnderPaid"),
-            pl.col("AllPagesText").str.extract(r'PreTrial\: (YES|NO)').alias("PreTrial"),
-            pl.col("AllPagesText").str.extract(r'PreTrail Date\: (.+)PreTrial').str.strip().alias("PreTrialDate"),
-            pl.col("AllPagesText").str.extract(r'PreTrial Terms\: (YES|NO)').alias("PreTrialTerms"),
-            pl.col("AllPagesText").str.extract(r'Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)').alias("PreTermsDate"),
-            pl.col("AllPagesText").str.extract(r'Delinquent\: (YES|NO)').alias("Delinquent"),
-            pl.col("AllPagesText").str.extract(r'Delinquent Date\: (\d\d/\d\d/\d\d\d\d)').alias("DelinquentDate"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer\: (YES|NO)').alias("DAMailer"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("DAMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer\: (YES|NO)').alias("WarrantMailer"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("WarrantMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Last Update\: (\d\d/\d\d/\d\d\d\d)').alias("EnforcementLastUpdate"),
-            pl.col("AllPagesText").str.extract(r'Updated By\: ([A-Z]{3})').alias("EnforcementUpdatedBy")
+            pl.col("AllPagesText")
+            .str.extract(r"TurnOver Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("TurnOverDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
+            .cast(pl.Float64, strict=False)
+            .alias("TurnOverAmt"),
+            pl.col("AllPagesText")
+            .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
+            .cast(pl.Float64, strict=False)
+            .alias("FrequencyAmt"),
+            pl.col("AllPagesText")
+            .str.extract(r"Due Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DueDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Last Paid Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("LastPaidDate"),
+            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").alias("Payor"),
+            pl.col("AllPagesText")
+            .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
+            .str.replace_all(r"\s+", " ")
+            .str.replace(r" F$", "")
+            .str.strip()
+            .alias("EnforcementStatus"),
+            pl.col("AllPagesText")
+            .str.extract(r"Frequency\: ([W|M])")
+            .str.replace(r"Cost Paid By\:", "")
+            .str.strip()
+            .alias("Frequency"),
+            pl.col("AllPagesText")
+            .str.extract(r"Placement Status\: (.+)")
+            .str.strip()
+            .alias("PlacementStatus"),
+            pl.col("AllPagesText")
+            .str.extract(r"Comments\: (.+)")
+            .str.strip()
+            .alias("Comments"),
+            pl.col("AllPagesText")
+            .str.extract(r"Over/Under Paid\: \$(\d+\.\d\d)")
+            .alias("OverUnderPaid"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrial\: (YES|NO)")
+            .alias("PreTrial"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrail Date\: (.+)PreTrial")
+            .str.strip()
+            .alias("PreTrialDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrial Terms\: (YES|NO)")
+            .alias("PreTrialTerms"),
+            pl.col("AllPagesText")
+            .str.extract(r"Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("PreTermsDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Delinquent\: (YES|NO)")
+            .alias("Delinquent"),
+            pl.col("AllPagesText")
+            .str.extract(r"Delinquent Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DelinquentDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"DA Mailer\: (YES|NO)")
+            .alias("DAMailer"),
+            pl.col("AllPagesText")
+            .str.extract(r"DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DAMailerDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Warrant Mailer\: (YES|NO)")
+            .alias("WarrantMailer"),
+            pl.col("AllPagesText")
+            .str.extract(r"Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("WarrantMailerDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Last Update\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("EnforcementLastUpdate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Updated By\: ([A-Z]{3})")
+            .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
         [
             pl.when(pl.col("D999RAW").is_null())
             .then(pl.lit(0))
             .otherwise(pl.col("D999RAW"))
             .alias("D999")
         ]
     )
 
-
     dlog(cases.columns, cases.shape, "cases raw regex", cf=debug)
 
     # clean columns, unnest totals
     cases = cases.with_columns(
         pl.col("RE_Phone")
         .str.replace_all(r"[^0-9]|2050000000", "")
         .alias("CLEAN_Phone"),
@@ -2160,37 +2224,37 @@
         "NumberOfSubpoenas",
         "AdminUpdatedBy",
         "TransferDesc",
         "TBNV1",
         "TBNV2",
         "DriverLicenseNo",
         "StateID",
-        'TurnOverDate',
-        'TurnOverAmt',
-        'FrequencyAmt',
-        'DueDate',
-        'LastPaidDate',
-        'Payor',
-        'EnforcementStatus',
-        'Frequency',
-        'PlacementStatus',
-        'Comments',
-        'OverUnderPaid',
-        'PreTrial',
-        'PreTrialDate',
-        'PreTrialTerms',
-        'PreTermsDate',
-        'Delinquent',
-        'DelinquentDate',
-        'DAMailer',
-        'DAMailerDate',
-        'WarrantMailer',
-        'WarrantMailerDate',
-        'EnforcementLastUpdate',
-        'EnforcementUpdatedBy'
+        "TurnOverDate",
+        "TurnOverAmt",
+        "FrequencyAmt",
+        "DueDate",
+        "LastPaidDate",
+        "Payor",
+        "EnforcementStatus",
+        "Frequency",
+        "PlacementStatus",
+        "Comments",
+        "OverUnderPaid",
+        "PreTrial",
+        "PreTrialDate",
+        "PreTrialTerms",
+        "PreTermsDate",
+        "Delinquent",
+        "DelinquentDate",
+        "DAMailer",
+        "DAMailerDate",
+        "WarrantMailer",
+        "WarrantMailerDate",
+        "EnforcementLastUpdate",
+        "EnforcementUpdatedBy",
     )
     return cases, all_charges, all_fees
 
 
 def explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
@@ -3983,15 +4047,14 @@
         ],
         [
             sg.Radio("All Charges", "TABLE", key="TB-CHARGES", default=False),
             sg.Radio(
                 "Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False
             ),
             sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
-
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
@@ -4176,15 +4239,15 @@
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
                     archive=False,
                     window=window,
-                )                
+                )
                 thread = threading.Thread(target=init, args=[cf], daemon=True).start()
                 window["TB"].update(disabled=True)
                 continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
@@ -4208,16 +4271,22 @@
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
-            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (".parquet", ".json", ".csv"):
-                thread = threading.Thread(target=archive, args=[cf], daemon=True).start()
+            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (
+                ".parquet",
+                ".json",
+                ".csv",
+            ):
+                thread = threading.Thread(
+                    target=archive, args=[cf], daemon=True
+                ).start()
                 window["MA"].update(disabled=True)
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
@@ -4360,19 +4429,16 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
-    "--criminal-only",
-    "-criminal",
-    is_flag=True,
-    help="Only search criminal cases"
-    )
+    "--criminal-only", "-criminal", is_flag=True, help="Only search criminal cases"
+)
 @click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
```

### Comparing `alacorder-80.1.3/src/alacorder/alac.py` & `alacorder-80.1.4/src/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.3"
+version = "80.1.4"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -127,15 +127,15 @@
 
 
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
-    plog("Extracting case info...", cf=cf)
+    print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
     ch = split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
     fs = split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
     fh = explode_split_financial_history(df, debug=cf["DEBUG"])
@@ -187,14 +187,15 @@
         "sentences": sent,
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
+    print("Completed table export.", cf=cf)
     return out
 
 
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
@@ -1577,28 +1578,28 @@
     cases = df.with_columns(
         [
             pl.col("AllPagesText")
             .str.extract(
                 r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                 group_index=1,
             )
-            .str.replace_all("Case Number:", "", literal=True)
+            .str.replace("Case Number:", "", literal=True)
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesTextNoNewLine")
             .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
-            .str.replace_all(r"[^\d/]", "")
+            .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1606,36 +1607,38 @@
                     pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
                 ]
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
-            .str.replace_all(r"(.{3}0000000)", "")
+            .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
             pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").alias("Race"),
             pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
-            .str.replace_all(r"[A-Z].+", "")
+            .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
+            .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
+            .str.strip()
             .alias("State"),
             pl.col("AllPagesText")
             .str.extract_all(
                 r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
             )
             .alias("RE_Charges"),
             pl.col("AllPagesText")
@@ -1695,19 +1698,19 @@
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
-            .str.strip()
             .alias("JuryDemand"),
-            pl.col("AllPagesText")
-            .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(
+                r"Inpatient Treatment Ordered: ([YES|NO]?)"
+            )
+            # .str.strip()
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
             .alias("TrialType"),
             pl.col("AllPagesText")
@@ -1721,25 +1724,31 @@
             .alias("Judge"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office \#: ([0-9\-]+)")
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
+            .str.replace(r"\n", "")
+            .str.replace(r"\s+", " ")
             .str.strip()
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
-            .str.replace(r"\n", "")
+            .str.replace(r"^\-.+", "")
+            .str.replace(r"County\:", "")
+            .str.replace(r"Defendant Status\:", "")
+            .str.replace(r"Judge\:", "")
+            .str.replace(r"Trial Type\:", "")
+            .str.replace(r"Probation Office \#\:", "")
             .str.strip()
             .alias("ArrestingAgencyType"),
             pl.col("AllPagesText")
             .str.extract(r"Arresting Officer: ([A-Z\s]+)")
-            .str.rstrip("S")
-            .str.rstrip("P")
+            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.strip()
             .alias("ArrestingOfficer"),
             pl.col("AllPagesText")
             .str.extract(r"Probation Office Name: ([A-Z0-9]+)")
             .alias("ProbationOfficeName"),
             pl.col("AllPagesText")
             .str.extract(r"Traffic Citation \#: ([A-Z0-9]+)")
@@ -1752,24 +1761,24 @@
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.strip()
             .alias("CaseInitiationType"),
             pl.col("AllPagesText")
             .str.extract(r"Domestic Violence: ([YES|NO])")
-            .str.strip()
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
+            .str.replace(r"\n", "")
+            .str.replace(r"\s+", " ")
             .str.strip()
             .alias("AgencyORI"),
             pl.col("AllPagesText")
             .str.extract(r"Driver License N°: ([A-Z0-9]+)")
-            .str.strip()
             .alias("DLRAW"),
             pl.col("AllPagesText")
             .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
             .alias("SSN"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z0-9]{11}?) State ID:")
             .alias("SIDRAW"),
@@ -1796,96 +1805,97 @@
             .str.strip()
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Issuance Status: (\w)")
+            .str.extract(r"Warrant Issuance Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantIssuanceStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Action Status: (\w)")
+            .str.extract(r"Warrant Action Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantActionStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Location Status: (\w)")
+            .str.extract(r"Warrant Location Status: (\w+)")
+            .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantLocationStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
             .str.strip()
             .alias("NumberOfWarrants"),
             pl.col("AllPagesText")
-            .str.extract(r"Bond Type: (\w)")
+            .str.extract(r"Bond Type: (\w+)")  # +
+            .str.replace(r"Bond", "")
             .str.strip()
             .alias("BondType"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
             .str.strip()
             .alias("BondTypeDesc"),
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
-            .str.replace_all(r"[^0-9\.\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
-            .str.strip()
+            # .str.strip()
             .alias("BondCompany"),
-            pl.col("AllPagesText")
-            .str.extract(r"Surety Code: ([A-Z0-9]{4})")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
+            # .str.strip()
             .alias("SuretyCode"),
-            pl.col("AllPagesText")
-            .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            # .str.strip()
             .alias("BondReleaseDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
+            pl.col("AllPagesText").str.extract(
+                r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
+            )
+            # .str.strip()
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
             pl.col("AllPagesText")
             .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
             .str.strip()
             .alias("BondsmanProcessReturn"),
             pl.col("AllPagesText")
             .str.extract(r"([\n\s/\d]*?) Appeal Court:")
-            .str.replace_all(r"[\n\s]", "")
             .str.strip()
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
             .alias("AppealCourt"),
             pl.col("AllPagesText")
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
-            .str.rstrip("D")
-            .str.rstrip("T")
+            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
+            .str.rstrip(r"O", "")
             .str.strip()
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
             .str.strip()
             .alias("AppealStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Appeal To: (\w?) Appeal")
+            .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("LowerCourtAppealDate"),
@@ -1920,51 +1930,105 @@
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
+            .str.replace(r"Financial", "")
             .str.strip()
             .alias("TBNV2"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Date\: (\d\d/\d\d/\d\d\d\d)').alias("TurnOverDate"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("TurnOverAmt"),
-            pl.col("AllPagesText").str.extract(r'Frequency Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("FrequencyAmt"),
-            pl.col("AllPagesText").str.extract(r'Due Date\: (\d\d/\d\d/\d\d\d\d)').alias("DueDate"),
-            pl.col("AllPagesText").str.extract(r'Last Paid Date\: (\d\d/\d\d/\d\d\d\d)').alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r'Payor\: ([A-Z0-9]{4})').alias("Payor"),
-            pl.col("AllPagesText").str.extract(r'Enforcement Status\: ([A-Z\:,\s]+)').str.replace_all(r'\s+',' ').str.replace(r' F$','').str.strip().alias("EnforcementStatus"),
-            pl.col("AllPagesText").str.extract(r'Frequency\: (.+)').str.replace(r'Cost Paid By\:','').str.strip().alias("Frequency"),
-            pl.col("AllPagesText").str.extract(r'Placement Status\: (.+)').str.strip().alias("PlacementStatus"),
-            pl.col("AllPagesText").str.extract(r'Comments\: (.+)').str.strip().alias("Comments"),
-            pl.col("AllPagesText").str.extract(r'Over/Under Paid\: \$(\d+\.\d\d)').alias("OverUnderPaid"),
-            pl.col("AllPagesText").str.extract(r'PreTrial\: (YES|NO)').alias("PreTrial"),
-            pl.col("AllPagesText").str.extract(r'PreTrail Date\: (.+)PreTrial').str.strip().alias("PreTrialDate"),
-            pl.col("AllPagesText").str.extract(r'PreTrial Terms\: (YES|NO)').alias("PreTrialTerms"),
-            pl.col("AllPagesText").str.extract(r'Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)').alias("PreTermsDate"),
-            pl.col("AllPagesText").str.extract(r'Delinquent\: (YES|NO)').alias("Delinquent"),
-            pl.col("AllPagesText").str.extract(r'Delinquent Date\: (\d\d/\d\d/\d\d\d\d)').alias("DelinquentDate"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer\: (YES|NO)').alias("DAMailer"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("DAMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer\: (YES|NO)').alias("WarrantMailer"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("WarrantMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Last Update\: (\d\d/\d\d/\d\d\d\d)').alias("EnforcementLastUpdate"),
-            pl.col("AllPagesText").str.extract(r'Updated By\: ([A-Z]{3})').alias("EnforcementUpdatedBy")
+            pl.col("AllPagesText")
+            .str.extract(r"TurnOver Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("TurnOverDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
+            .cast(pl.Float64, strict=False)
+            .alias("TurnOverAmt"),
+            pl.col("AllPagesText")
+            .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
+            .cast(pl.Float64, strict=False)
+            .alias("FrequencyAmt"),
+            pl.col("AllPagesText")
+            .str.extract(r"Due Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DueDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Last Paid Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("LastPaidDate"),
+            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").alias("Payor"),
+            pl.col("AllPagesText")
+            .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
+            .str.replace_all(r"\s+", " ")
+            .str.replace(r" F$", "")
+            .str.strip()
+            .alias("EnforcementStatus"),
+            pl.col("AllPagesText")
+            .str.extract(r"Frequency\: ([W|M])")
+            .str.replace(r"Cost Paid By\:", "")
+            .str.strip()
+            .alias("Frequency"),
+            pl.col("AllPagesText")
+            .str.extract(r"Placement Status\: (.+)")
+            .str.strip()
+            .alias("PlacementStatus"),
+            pl.col("AllPagesText")
+            .str.extract(r"Comments\: (.+)")
+            .str.strip()
+            .alias("Comments"),
+            pl.col("AllPagesText")
+            .str.extract(r"Over/Under Paid\: \$(\d+\.\d\d)")
+            .alias("OverUnderPaid"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrial\: (YES|NO)")
+            .alias("PreTrial"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrail Date\: (.+)PreTrial")
+            .str.strip()
+            .alias("PreTrialDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"PreTrial Terms\: (YES|NO)")
+            .alias("PreTrialTerms"),
+            pl.col("AllPagesText")
+            .str.extract(r"Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("PreTermsDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Delinquent\: (YES|NO)")
+            .alias("Delinquent"),
+            pl.col("AllPagesText")
+            .str.extract(r"Delinquent Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DelinquentDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"DA Mailer\: (YES|NO)")
+            .alias("DAMailer"),
+            pl.col("AllPagesText")
+            .str.extract(r"DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("DAMailerDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Warrant Mailer\: (YES|NO)")
+            .alias("WarrantMailer"),
+            pl.col("AllPagesText")
+            .str.extract(r"Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("WarrantMailerDate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Last Update\: (\d\d/\d\d/\d\d\d\d)")
+            .alias("EnforcementLastUpdate"),
+            pl.col("AllPagesText")
+            .str.extract(r"Updated By\: ([A-Z]{3})")
+            .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
         [
             pl.when(pl.col("D999RAW").is_null())
             .then(pl.lit(0))
             .otherwise(pl.col("D999RAW"))
             .alias("D999")
         ]
     )
 
-
     dlog(cases.columns, cases.shape, "cases raw regex", cf=debug)
 
     # clean columns, unnest totals
     cases = cases.with_columns(
         pl.col("RE_Phone")
         .str.replace_all(r"[^0-9]|2050000000", "")
         .alias("CLEAN_Phone"),
@@ -2160,37 +2224,37 @@
         "NumberOfSubpoenas",
         "AdminUpdatedBy",
         "TransferDesc",
         "TBNV1",
         "TBNV2",
         "DriverLicenseNo",
         "StateID",
-        'TurnOverDate',
-        'TurnOverAmt',
-        'FrequencyAmt',
-        'DueDate',
-        'LastPaidDate',
-        'Payor',
-        'EnforcementStatus',
-        'Frequency',
-        'PlacementStatus',
-        'Comments',
-        'OverUnderPaid',
-        'PreTrial',
-        'PreTrialDate',
-        'PreTrialTerms',
-        'PreTermsDate',
-        'Delinquent',
-        'DelinquentDate',
-        'DAMailer',
-        'DAMailerDate',
-        'WarrantMailer',
-        'WarrantMailerDate',
-        'EnforcementLastUpdate',
-        'EnforcementUpdatedBy'
+        "TurnOverDate",
+        "TurnOverAmt",
+        "FrequencyAmt",
+        "DueDate",
+        "LastPaidDate",
+        "Payor",
+        "EnforcementStatus",
+        "Frequency",
+        "PlacementStatus",
+        "Comments",
+        "OverUnderPaid",
+        "PreTrial",
+        "PreTrialDate",
+        "PreTrialTerms",
+        "PreTermsDate",
+        "Delinquent",
+        "DelinquentDate",
+        "DAMailer",
+        "DAMailerDate",
+        "WarrantMailer",
+        "WarrantMailerDate",
+        "EnforcementLastUpdate",
+        "EnforcementUpdatedBy",
     )
     return cases, all_charges, all_fees
 
 
 def explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
@@ -3983,15 +4047,14 @@
         ],
         [
             sg.Radio("All Charges", "TABLE", key="TB-CHARGES", default=False),
             sg.Radio(
                 "Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False
             ),
             sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
-
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
@@ -4176,15 +4239,15 @@
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
                     archive=False,
                     window=window,
-                )                
+                )
                 thread = threading.Thread(target=init, args=[cf], daemon=True).start()
                 window["TB"].update(disabled=True)
                 continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
@@ -4208,16 +4271,22 @@
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
-            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (".parquet", ".json", ".csv"):
-                thread = threading.Thread(target=archive, args=[cf], daemon=True).start()
+            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (
+                ".parquet",
+                ".json",
+                ".csv",
+            ):
+                thread = threading.Thread(
+                    target=archive, args=[cf], daemon=True
+                ).start()
                 window["MA"].update(disabled=True)
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
@@ -4360,19 +4429,16 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
-    "--criminal-only",
-    "-criminal",
-    is_flag=True,
-    help="Only search criminal cases"
-    )
+    "--criminal-only", "-criminal", is_flag=True, help="Only search criminal cases"
+)
 @click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
```

### Comparing `alacorder-80.1.3/PKG-INFO` & `alacorder-80.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.3
+Version: 80.1.4
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

