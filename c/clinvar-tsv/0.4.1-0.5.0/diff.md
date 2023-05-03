# Comparing `tmp/clinvar-tsv-0.4.1.tar.gz` & `tmp/clinvar-tsv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinvar-tsv-0.4.1.tar", last modified: Fri Sep  9 08:35:24 2022, max compression
+gzip compressed data, was "clinvar-tsv-0.5.0.tar", last modified: Wed May  3 10:52:53 2023, max compression
```

## Comparing `clinvar-tsv-0.4.1.tar` & `clinvar-tsv-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      784 2022-09-09 08:34:51.000000 clinvar-tsv-0.4.1/HISTORY.rst
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     1107 2021-10-20 06:32:02.000000 clinvar-tsv-0.4.1/LICENSE
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      392 2021-10-20 06:32:02.000000 clinvar-tsv-0.4.1/MANIFEST.in
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     3527 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/PKG-INFO
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     2052 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/README.rst
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/clinvar_tsv/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     3701 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/Snakefile
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)       93 2021-10-20 06:32:02.000000 clinvar-tsv-0.4.1/clinvar_tsv/__init__.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     6220 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/__main__.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      497 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/clinvar_tsv/_version.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    21252 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/common.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      351 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/exceptions.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    10666 2022-09-09 08:34:35.000000 clinvar-tsv-0.4.1/clinvar_tsv/merge_tsvs.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     7646 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/normalize.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     4970 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/clinvar_tsv/parse_clinvar_xml.py
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.901051 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     3527 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/PKG-INFO
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     1003 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/SOURCES.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        1 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/dependency_links.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)       58 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/entry_points.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        1 2022-08-26 14:57:02.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/not-zip-safe
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      103 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/requires.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)       12 2022-09-09 08:35:24.000000 clinvar-tsv-0.4.1/clinvar_tsv.egg-info/top_level.txt
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.901051 clinvar-tsv-0.4.1/requirements/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      370 2022-08-29 08:46:18.000000 clinvar-tsv-0.4.1/requirements/base.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      163 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/requirements/dev.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      331 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/requirements/test.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)       25 2021-10-20 06:32:02.000000 clinvar-tsv-0.4.1/requirements.txt
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      805 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/setup.cfg
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     2133 2022-08-29 08:36:05.000000 clinvar-tsv-0.4.1/setup.py
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.901051 clinvar-tsv-0.4.1/tests/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     2006 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/conftest.py
-drwxr-xr-x   0 holtgrem_c (100131) hpc-ag-cubi (1005272)        0 2022-09-09 08:35:24.905051 clinvar-tsv-0.4.1/tests/data/
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)      413 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/data/README.md
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    12893 2022-08-29 06:42:40.000000 clinvar-tsv-0.4.1/tests/data/clinvar-74722873.xml
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)  1054250 2022-08-29 07:56:38.000000 clinvar-tsv-0.4.1/tests/data/clinvar-in-context-74722873.xml
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    23586 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/data/clinvar-spta1.xml
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     4968 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/data/parsed-74722873.37.tsv
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)   319422 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/data/parsed-in-context-74722873.37.tsv
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)   267731 2022-09-07 09:18:20.000000 clinvar-tsv-0.4.1/tests/data/parsed-in-context-74722873.37.tsv~
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     8733 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/data/parsed-spta1.37.tsv
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    20050 2022-09-09 08:34:35.000000 clinvar-tsv-0.4.1/tests/test_merge_tsvs.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    20003 2022-09-08 12:47:04.000000 clinvar-tsv-0.4.1/tests/test_merge_tsvs.py~
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)     5771 2022-09-08 13:09:14.000000 clinvar-tsv-0.4.1/tests/test_parse_xml.py
--rw-r--r--   0 holtgrem_c (100131) hpc-ag-cubi (1005272)    68448 2021-10-20 06:32:02.000000 clinvar-tsv-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/clinvar_tsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/clinvar_tsv/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/clinvar_tsv/parse_clinvar_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 10:52:53.000000 clinvar-tsv-0.5.0/clinvar_tsv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.919907 clinvar-tsv-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:52:53.923907 clinvar-tsv-0.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-92148661.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1054250 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-in-context-74722873.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/clinvar-spta1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319422 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-in-context-74722873.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/data/parsed-spta1.37.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_merge_tsvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_parse_xml_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/tests/test_parse_xml_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-05-03 10:52:49.000000 clinvar-tsv-0.5.0/versioneer.py
```

### Comparing `clinvar-tsv-0.4.1/LICENSE` & `clinvar-tsv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/README.rst` & `clinvar-tsv-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,43 @@
-.. image:: https://coveralls.io/repos/github/bihealth/clinvar-tsv/badge.svg?branch=main
-   :target: https://coveralls.io/github/bihealth/clinvar-tsv?branch=main
+[![CI](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml/badge.svg)](https://github.com/bihealth/clinvar-tsv/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/bihealth/clinvar-tsv/branch/main/graph/badge.svg?token=287XB5P11T)](https://codecov.io/gh/bihealth/clinvar-tsv)
 
-===========
-Clinvar-TSV
-===========
+# Clinvar-TSV
 
 The code in this repository allows to first download,t hen convert ClinVar XML files into TSV files (one for b37 and b38).
-The TSV files will contain one entry for each ClinVar ``<ReferenceClinVarAssertion>`` entry with important information extracted from ClinVar.
-The code is used by `bihealth/varfish-db-downloader <https://github.com/bihealth/varfish-db-downloader/>`_.
+The TSV files will contain one entry for each ClinVar `<ReferenceClinVarAssertion>` entry with important information extracted from ClinVar.
+The code is used by [bihealth/varfish-db-downloader](https://github.com/bihealth/varfish-db-downloader).
 
-- `clinvar-tsv on PyPi <https://pypi.org/project/clinvar-tsv/>`__
-- `clinvar-tsv on bioconda <http://bioconda.github.io/recipes/clinvar-tsv/README.html>`__
+- [clinvar-tsv on PyPi](https://pypi.org/project/clinvar-tsv/)
+- [clinvar-tsv on bioconda](http://bioconda.github.io/recipes/clinvar-tsv/README.html)
 
---------
-Overview
---------
+## Overview
 
-Users usually run the tool by calling ``clinvar_tsv main``.
-
-::
-
-    clinvar_tsv main \
-        --cores 2 \
-        --b37-path hs37d5.fa \
-        --b38-path hs38.fa
+Users usually run the tool by calling `clinvar_tsv main`.
+
+```
+$ clinvar_tsv main \
+    --cores 2 \
+    --b37-path hs37d5.fa \
+    --b38-path hs38.fa
+```
 
 This will call a Snakemake workflow that will in turn do the following
 
-1. Download the latest ClinVar XML file to the ``downloads/`` directory using ``wget``.
-2. Parse the XML file and convert it into a "raw" TSV file in ``parsed`` for each the 37 and 38 release with ``clinvar_tsv parse_xml``.
+1. Download the latest ClinVar XML file to the `downloads/` directory using `wget`.
+2. Parse the XML file and convert it into a "raw" TSV file in `parsed` for each the 37 and 38 release with `clinvar_tsv parse_xml`.
    This file contains one record for each ClinVar VCV record.
-3. Sort this file by coordinate and VCV ID using Unix ``sort``, and finally...
+3. Sort this file by coordinate and VCV ID using Unix `sort`, and finally...
 4. Merge the lines in the resulting TSV file (for each genome build) by VCV ID and produce aggregate summaries for each VCV.
 
 There are two summaries:
 
-- ``summary_clinvar_*`` -- which merges record which attempts to imitate the `approach taken by ClinVar <https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/>`__
-- ``summary_paranoid_*`` -- which considers all assessment as equally important, whether the reporter provided assessment criteria or not
+- `summary_clinvar_*` -- which merges record which attempts to imitate the [approach taken by ClinVar](https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/)
+- `summary_paranoid_*` -- which considers all assessment as equally important, whether the reporter provided assessment criteria or not
 
-----------
-References
-----------
+## References
 
 Documentation in ClinVar:
 
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/review_status/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/help/
 - https://www.ncbi.nlm.nih.gov/clinvar/docs/variation_report/
```

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv/Snakefile` & `clinvar-tsv-0.5.0/clinvar_tsv/Snakefile`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     'b38': config.get('b38_path', '/dev/null'),
 }
 
 
 rule default:
     input:
         expand(
-            "output/clinvar.{build}.tsv{ext}",
+            "output/clinvar_{size}.{build}.tsv{ext}",
+            size=("small", "sv"),
             build=("b37", "b38"),
             ext=(".gz", ".gz.tbi", ".gz.md5", ".gz.tbi.md5"),
         )
 
 
 rule download_xml:
     output: "downloads/ClinVarFullRelease_00-latest.xml.gz"
@@ -35,35 +36,39 @@
 
 
 rule parse_clinvar:
     input:
         release_xml="downloads/ClinVarFullRelease_00-latest.xml.gz",
         summary="downloads/variant_summary.txt.gz",
     output:
-        b37=temp("parsed/clinvar_table_raw.b37.tsv"),
-        b38=temp("parsed/clinvar_table_raw.b38.tsv"),
+        b37_small="parsed/clinvar_table_raw.b37.tsv",
+        b37_sv="parsed/clinvar_sv.b37.tsv",
+        b38_small="parsed/clinvar_table_raw.b38.tsv",
+        b38_sv="parsed/clinvar_sv.b38.tsv",
     shell:
         r"""
         set -euo pipefail
 
         clinvar_tsv parse_xml \
             --clinvar-xml {input.release_xml} \
-            --output-b37 {output.b37} \
-            --output-b38 {output.b38} \
+            --output-b37-small {output.b37_small} \
+            --output-b37-sv {output.b37_sv} \
+            --output-b38-small {output.b38_small} \
+            --output-b38-sv {output.b38_sv} \
             $(if [[ {config[debug]} == "True" ]]; then
-                echo "--max-rcvs 100"
+                echo "--max-rcvs 1000"
             fi)
         """
 
 
 rule normalize_clinvar:
     input:
         tsv="parsed/clinvar_table_raw.{genome_build}.tsv",
         reference=lambda wildcards: REF[wildcards.genome_build],
-    output: temp("normalized/clinvar_table_normalized.{genome_build}.tsv.gz"),
+    output: "normalized/clinvar_table_normalized.{genome_build}.tsv.gz",
     shell:
         r"""
         set -euo pipefail
 
         clinvar_tsv normalize_tsv \
             --input-tsv {input.tsv} \
             --reference {input.reference} \
@@ -73,18 +78,18 @@
         > {output}
         """
 
 
 rule sort_tabix_clinvar:
     input: "normalized/clinvar_table_normalized.{genome_build}.tsv.gz",
     output:
-        tsv="unmerged/clinvar.{genome_build}.tsv.gz",
-        tbi="unmerged/clinvar.{genome_build}.tsv.gz.tbi",
-        tsv_md5="unmerged/clinvar.{genome_build}.tsv.gz.md5",
-        tbi_md5="unmerged/clinvar.{genome_build}.tsv.gz.tbi.md5",
+        tsv="unmerged/clinvar_small.{genome_build}.tsv.gz",
+        tbi="unmerged/clinvar_small.{genome_build}.tsv.gz.tbi",
+        tsv_md5="unmerged/clinvar_small.{genome_build}.tsv.gz.md5",
+        tbi_md5="unmerged/clinvar_small.{genome_build}.tsv.gz.tbi.md5",
     shell:
         r"""
         set -euo pipefail
 
         cat \
             <(zcat {input} | head -n 1) \
             <(zcat {input} | tail -n +2 | sort -k2,2V -k3,3n -k4,4n -k11,11) \
@@ -93,21 +98,46 @@
         tabix -S 1 -s 2 -b 3 -e 4 -f {output.tsv}
 
         cd $(dirname {output.tsv})
         md5sum $(basename {output.tsv}) >$(basename {output.tsv}).md5
         md5sum $(basename {output.tbi}) >$(basename {output.tbi}).md5
         """
 
+rule sort_svs:
+    input: "parsed/clinvar_sv.{genome_build}.tsv",
+    output:
+        tsv="unmerged/clinvar_sv.{genome_build}.tsv.gz",
+        tbi="unmerged/clinvar_sv.{genome_build}.tsv.gz.tbi",
+        tsv_md5="unmerged/clinvar_sv.{genome_build}.tsv.gz.md5",
+        tbi_md5="unmerged/clinvar_sv.{genome_build}.tsv.gz.tbi.md5",
+    params:
+        clinvar_version=config.get("clinvar_version", ".")
+    shell:
+        r"""
+        set -euo pipefail
+
+        cat \
+            <(cat {input} | head -n 1) \
+            <(cat {input} | tail -n +2 | sort -k2,2V -k3,3n -k4,4n -k11,11) \
+        | bgzip -c \
+        > {output.tsv}
+        tabix -S 1 -s 2 -b 3 -e 4 -f {output.tsv}
+
+        cd $(dirname {output.tsv})
+        md5sum $(basename {output.tsv}) >$(basename {output.tsv}).md5
+        md5sum $(basename {output.tbi}) >$(basename {output.tbi}).md5
+        """
+
 rule merge_clinvar:
-    input: "unmerged/clinvar.{genome_build}.tsv.gz",
+    input: "unmerged/clinvar_{size}.{genome_build}.tsv.gz",
     output:
-        tsv="output/clinvar.{genome_build}.tsv.gz",
-        tbi="output/clinvar.{genome_build}.tsv.gz.tbi",
-        tsv_md5="output/clinvar.{genome_build}.tsv.gz.md5",
-        tbi_md5="output/clinvar.{genome_build}.tsv.gz.tbi.md5",
+        tsv="output/clinvar_{size}.{genome_build}.tsv.gz",
+        tbi="output/clinvar_{size}.{genome_build}.tsv.gz.tbi",
+        tsv_md5="output/clinvar_{size}.{genome_build}.tsv.gz.md5",
+        tbi_md5="output/clinvar_{size}.{genome_build}.tsv.gz.tbi.md5",
     params:
         clinvar_version=config.get("clinvar_version", ".")
     shell:
         r"""
         set -euo pipefail
 
         zcat {input} \
```

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv/__main__.py` & `clinvar-tsv-0.5.0/clinvar_tsv/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 def run_inspect(args):
     kwargs = {
         "snakefile": os.path.join(os.path.dirname(__file__), "Snakefile"),
         "workdir": args.work_dir,
         "summary": True,
         "verbose": True,
     }
+    print(f"Running snakemake {kwargs}")
     snakemake.snakemake(**kwargs)
 
 
 def run_main(args):
     """Entry point for the main program."""
     kwargs = {
         "snakefile": os.path.join(os.path.dirname(__file__), "Snakefile"),
@@ -36,35 +37,42 @@
             "clinvar_version": args.clinvar_version,
         },
         "printshellcmds": True,
         "verbose": True,
         "force_incomplete": True,
         "cores": 8,
     }
+    print(f"Running snakemake {kwargs}")
     return not snakemake.snakemake(**kwargs)
 
 
 def open_maybe_gzip(path, mode):
     if path.endswith(".gz"):
         return gzip.open(path, mode)
     else:
         return open(path, mode)
 
 
 def run_parse_xml(args):
     """Parse XML file."""
-    with open(args.output_b37, "wt") as output_b37:
-        with open(args.output_b38, "wt") as output_b38:
-            parser = parse_clinvar_xml.ClinvarParser(
-                input_file=open_maybe_gzip(args.clinvar_xml, "rb"),
-                out_b37=output_b37,
-                out_b38=output_b38,
-                max_rcvs=args.max_rcvs,
-            )
-            parser.run()
+    with (
+        open(args.output_b37_small, "wt") as output_b37_small,
+        open(args.output_b37_sv, "wt") as output_b37_sv,
+        open(args.output_b38_small, "wt") as output_b38_small,
+        open(args.output_b38_sv, "wt") as output_b38_sv,
+    ):
+        parser = parse_clinvar_xml.ClinvarParser(
+            input_file=open_maybe_gzip(args.clinvar_xml, "rb"),
+            out_b37_small=output_b37_small,
+            out_b37_sv=output_b37_sv,
+            out_b38_small=output_b38_small,
+            out_b38_sv=output_b38_sv,
+            max_rcvs=args.max_rcvs,
+        )
+        parser.run()
 
 
 def run_normalize_tsv(args):
     with open(args.input_tsv, "rt") as input_tsv:
         with open(args.output_tsv, "wt") as output_tsv:
             normalize.normalize_tab_delimited_file(input_tsv, output_tsv, args.reference)
 
@@ -125,18 +133,24 @@
     # -----------------------------------------------------------------------
     # Command: parse_xml
     # -----------------------------------------------------------------------
 
     parser_parse_xml = subparsers.add_parser("parse_xml", help="Parse the Clinvar XML")
     parser_parse_xml.add_argument("--clinvar-xml", required=True, help="Path to Clinvar XML file.")
     parser_parse_xml.add_argument(
-        "--output-b37", required=True, help="Output path for GRCh37 file."
+        "--output-b37-small", required=True, help="Output path for small vars GRCh37 file."
     )
     parser_parse_xml.add_argument(
-        "--output-b38", required=True, help="Output path for GRCh38 file."
+        "--output-b37-sv", required=True, help="Output path for SV GRCh37 file."
+    )
+    parser_parse_xml.add_argument(
+        "--output-b38-small", required=True, help="Output path for small vars GRCh38 file."
+    )
+    parser_parse_xml.add_argument(
+        "--output-b38-sv", required=True, help="Output path for SV GRCh38 file."
     )
     parser_parse_xml.add_argument(
         "--max-rcvs", required=False, type=int, help="Maximal number of RCV records to process."
     )
     parser_parse_xml.set_defaults(func=run_parse_xml)
 
     # -----------------------------------------------------------------------
```

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv/common.py` & `clinvar-tsv-0.5.0/clinvar_tsv/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,21 +202,23 @@
 
     @classmethod
     def from_element(cls, element: ET.Element):
         symbols = [
             elem.text for elem in element.findall('.//Symbol/ElementValue[@Type="Preferred"]')
         ]
         hgnc_ids = [elem.attrib.get("ID") for elem in element.findall('.//XRef[@DB="HGNC"]')]
+        n = element.findall("./SequenceLocation")
+        m = element.findall(".//SequenceLocation")
         return Measure(
             measure_type=element.attrib.get("Type"),
             symbols=tuple(sorted(set(symbols))),
             hgnc_ids=tuple(sorted(set(hgnc_ids))),
             sequence_locations={
                 elem.attrib.get("Assembly"): SequenceLocation.from_element(elem)
-                for elem in element.findall("./SequenceLocation")
+                for elem in (n or m)
             },
             comments=tuple(
                 elem.text
                 for elem in chain(
                     element.findall("./MeasureRelationship/Comment"), element.findall("./Comment")
                 )
             ),
@@ -535,32 +537,31 @@
         "probably not pathogenic",
         "protective",
         "suspected benign",
     ),
     0: (
         "uncertain significance",
         # below: other
-        "affects",
         "association",
         "association not found",
         "cancer",
         "confers sensitivity",
         "drug response",
-        "drug response",
         "drug-response",
         "histocompatibility",
         "not provided",
         "other",
         "protective",
         "risk factor",
         "uncertain",
         "unknown",
         "untested",
         "variant of unknown significance",
         "associated with leiomyomas",
+        "conflicting data from submitters",
     ),
     1: (
         "likely pathogenic",
         # below: other
         "affects",
         "association",
         "confers sensitivity",
@@ -609,15 +610,19 @@
         return cls.UNCERTAIN
 
     def label(self):
         return _PATHOGENICITY_LABELS[self.value][0]
 
 
 _REVIEW_STATUS_LABELS = {
-    1: ("conflicting interpretations", "conflicting interpretations of pathogenicity"),
+    1: (
+        "conflicting interpretations",
+        "conflicting interpretations of pathogenicity",
+        "conflicting data from submitters",
+    ),
     2: ("criteria provided",),
     3: ("multiple submitters",),
     4: ("no assertion criteria provided",),
     5: ("no assertion provided",),
     6: ("no conflicts",),
     7: ("practice guideline",),
     8: ("reviewed by expert panel",),
```

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv/merge_tsvs.py` & `clinvar-tsv-0.5.0/clinvar_tsv/merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv/normalize.py` & `clinvar-tsv-0.5.0/clinvar_tsv/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     header = infile.readline()  # get header of input file
     columns = header.strip("\n").split("\t")  # parse col names
     outfile.write("\t".join(columns) + "\n")  # write header line plus the CpG col to be generated
     counter = 0
     ref_equals_alt = 0
     wrong_ref = 0
     invalid_nucleotide = 0
+    unknown_contig = 0
     for line in infile.readlines():
         data = dict(zip(columns, line.strip("\n").split("\t")))
         # fill the data with blanks for any missing data
         for column in columns:
             if column not in data.keys():
                 data[column] = ""
         pos = int(data.get("position", data["start"]))
@@ -172,14 +173,18 @@
         # Perform normalization
         try:
             _, pos, data["reference"], data["alternative"] = normalize(
                 pysam_fasta, chrom, pos, data["reference"], data["alternative"]
             )
             if data["chromosome"].startswith("chr"):
                 data["chromosome"] = data["chromosome"][3:]
+        except KeyError as e:
+            sys.stderr.write("\n" + str(e) + "\n")
+            unknown_contig += 1
+            continue
         except RefEqualsAltError as e:
             sys.stderr.write("\n" + str(e) + "\n")
             ref_equals_alt += 1
             continue
         except WrongRefError as e:
             sys.stderr.write("\n" + str(e) + "\n")
             wrong_ref += 1
@@ -196,10 +201,10 @@
         outfile.write("\t".join([data[column] for column in columns]) + "\n")
         counter += 1
         if verbose and counter % 1000 == 0:
             sys.stderr.write("\r%s records processed\n" % (counter))
     outfile.write("\n\n")
     if verbose:
         sys.stderr.write(
-            "Final counts of variants discarded:\nREF == ALT: %s\nWrong REF: %s\nInvalid nucleotide: %s\n"
-            % (ref_equals_alt, wrong_ref, invalid_nucleotide)
+            "Final counts of variants discarded:\nREF == ALT: %s\nWrong REF: %s\nInvalid nucleotide: %s\nUnknown contig: %s\n"
+            % (ref_equals_alt, wrong_ref, invalid_nucleotide, unknown_contig)
         )
```

### Comparing `clinvar-tsv-0.4.1/clinvar_tsv.egg-info/SOURCES.txt` & `clinvar-tsv-0.5.0/clinvar_tsv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-HISTORY.rst
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 clinvar_tsv/Snakefile
 clinvar_tsv/__init__.py
 clinvar_tsv/__main__.py
@@ -23,17 +22,17 @@
 clinvar_tsv.egg-info/requires.txt
 clinvar_tsv.egg-info/top_level.txt
 requirements/base.txt
 requirements/dev.txt
 requirements/test.txt
 tests/conftest.py
 tests/test_merge_tsvs.py
-tests/test_merge_tsvs.py~
-tests/test_parse_xml.py
+tests/test_parse_xml_small.py
+tests/test_parse_xml_sv.py
 tests/data/README.md
 tests/data/clinvar-74722873.xml
+tests/data/clinvar-92148661.xml
 tests/data/clinvar-in-context-74722873.xml
 tests/data/clinvar-spta1.xml
 tests/data/parsed-74722873.37.tsv
 tests/data/parsed-in-context-74722873.37.tsv
-tests/data/parsed-in-context-74722873.37.tsv~
 tests/data/parsed-spta1.37.tsv
```

### Comparing `clinvar-tsv-0.4.1/setup.cfg` & `clinvar-tsv-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/setup.py` & `clinvar-tsv-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,40 +21,38 @@
                 inner_path = os.path.join(os.path.dirname(path), fname)
                 requirements += parse_requirements(inner_path)
             elif line != "" and not line.startswith("#"):
                 requirements.append(line)
     return requirements
 
 
-with open("README.rst") as readme_file:
+with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
+with open("CHANGELOG.md") as history_file:
     history = history_file.read()
 
-requirements = parse_requirements("requirements.txt")
-
-test_requirements = [
-    # TODO: put package test requirements here
-]
+test_requirements = parse_requirements("requirements/test.txt")
+install_requirements = parse_requirements("requirements/base.txt")
 
 setup(
     name="clinvar-tsv",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description=("Python 3 library for accessing and managing BioMedical sheets"),
     long_description=readme + "\n\n" + history,
+    long_description_content_type="text/markdown",
     author="Manuel Holtgrewe",
     author_email="manuel.holtgrewe@bihealth.de",
     url="https://github.com/bihealth/clinvar-tsv",
     packages=find_packages(),
     package_dir={"clinvar_tsv": "clinvar_tsv"},
     entry_points={"console_scripts": ["clinvar_tsv = clinvar_tsv.__main__:main"]},
     include_package_data=True,
-    install_requires=requirements,
+    install_requires=install_requirements,
     license="MIT license",
     zip_safe=False,
     keywords="clinvar",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `clinvar-tsv-0.4.1/tests/conftest.py` & `clinvar-tsv-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/clinvar-74722873.xml` & `clinvar-tsv-0.5.0/tests/data/clinvar-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/clinvar-in-context-74722873.xml` & `clinvar-tsv-0.5.0/tests/data/clinvar-in-context-74722873.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/clinvar-spta1.xml` & `clinvar-tsv-0.5.0/tests/data/clinvar-spta1.xml`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/parsed-74722873.37.tsv` & `clinvar-tsv-0.5.0/tests/data/parsed-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/parsed-in-context-74722873.37.tsv` & `clinvar-tsv-0.5.0/tests/data/parsed-in-context-74722873.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/data/parsed-spta1.37.tsv` & `clinvar-tsv-0.5.0/tests/data/parsed-spta1.37.tsv`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/test_merge_tsvs.py` & `clinvar-tsv-0.5.0/tests/test_merge_tsvs.py`

 * *Files identical despite different names*

### Comparing `clinvar-tsv-0.4.1/tests/test_parse_xml.py` & `clinvar-tsv-0.5.0/tests/test_parse_xml_small.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from clinvar_tsv.parse_clinvar_xml import ClinvarParser
 
 
 def test_parse_74722873(tmpdir):
     """Test with record seen as problematic before"""
     with contextlib.ExitStack() as stack:
         inputf = stack.push(open("tests/data/clinvar-74722873.xml", "rt"))
-        out37 = stack.push((tmpdir / "out37.tsv").open("wt"))
-        out38 = stack.push((tmpdir / "out38.tsv").open("wt"))
-        parser = ClinvarParser(inputf, out37, out38)
+        out37_small = stack.push((tmpdir / "out37.small.tsv").open("wt"))
+        out37_sv = stack.push((tmpdir / "out37.sv.tsv").open("wt"))
+        out38_small = stack.push((tmpdir / "out38.small.tsv").open("wt"))
+        out38_sv = stack.push((tmpdir / "out38.sv.tsv").open("wt"))
+        parser = ClinvarParser(inputf, out37_small, out37_sv, out38_small, out38_sv)
         parser.run()
 
-    with (tmpdir / "out37.tsv").open("rt") as input37:
+    with (tmpdir / "out37.small.tsv").open("rt") as input37:
         lines = input37.readlines()
         assert len(lines) == 2
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh37",
             "9",
             "13150558",
@@ -29,15 +31,15 @@
             "snv",
             '{"MPDZ"}',
             '{"HGNC:7208"}',
             "VCV000376860",
             "RCV000430591",
         ]
 
-    with (tmpdir / "out38.tsv").open("rt") as input38:
+    with (tmpdir / "out38.small.tsv").open("rt") as input38:
         lines = input38.readlines()
         assert len(lines) == 2
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh38",
             "9",
             "13150559",
@@ -53,20 +55,22 @@
         ]
 
 
 def test_parse_74722873_in_context(tmpdir):
     """Test with record seen as problematic before, this time in contet"""
     with contextlib.ExitStack() as stack:
         inputf = stack.push(open("tests/data/clinvar-in-context-74722873.xml", "rt"))
-        out37 = stack.push((tmpdir / "out37.tsv").open("wt"))
-        out38 = stack.push((tmpdir / "out38.tsv").open("wt"))
-        parser = ClinvarParser(inputf, out37, out38)
+        out37_small = stack.push((tmpdir / "out37.small.tsv").open("wt"))
+        out37_sv = stack.push((tmpdir / "out37.sv.tsv").open("wt"))
+        out38_small = stack.push((tmpdir / "out38.small.tsv").open("wt"))
+        out38_sv = stack.push((tmpdir / "out38.sv.tsv").open("wt"))
+        parser = ClinvarParser(inputf, out37_small, out37_sv, out38_small, out38_sv)
         parser.run()
 
-    with (tmpdir / "out37.tsv").open("rt") as input37:
+    with (tmpdir / "out37.small.tsv").open("rt") as input37:
         lines = input37.readlines()
         assert len(lines) == 71
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh37",
             "14",
             "105246551",
@@ -91,15 +95,15 @@
             "snv",
             '{"BRCA1"}',
             '{"HGNC:1100"}',
             "VCV000054401",
             "RCV000430192",
         ]
 
-    with (tmpdir / "out38.tsv").open("rt") as input38:
+    with (tmpdir / "out38.small.tsv").open("rt") as input38:
         lines = input38.readlines()
         assert len(lines) == 71
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh38",
             "14",
             "104780214",
@@ -129,20 +133,22 @@
         ]
 
 
 def test_parse_spta1(tmpdir):
     """Test with record seen as problematic before"""
     with contextlib.ExitStack() as stack:
         inputf = stack.push(open("tests/data/clinvar-spta1.xml", "rt"))
-        out37 = stack.push((tmpdir / "out37.tsv").open("wt"))
-        out38 = stack.push((tmpdir / "out38.tsv").open("wt"))
-        parser = ClinvarParser(inputf, out37, out38)
+        out37_small = stack.push((tmpdir / "out37.small.tsv").open("wt"))
+        out37_sv = stack.push((tmpdir / "out37.sv.tsv").open("wt"))
+        out38_small = stack.push((tmpdir / "out38.small.tsv").open("wt"))
+        out38_sv = stack.push((tmpdir / "out38.sv.tsv").open("wt"))
+        parser = ClinvarParser(inputf, out37_small, out37_sv, out38_small, out38_sv)
         parser.run()
 
-    with (tmpdir / "out37.tsv").open("rt") as input37:
+    with (tmpdir / "out37.small.tsv").open("rt") as input37:
         lines = input37.readlines()
         assert len(lines) == 3
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh37",
             "1",
             "158624528",
@@ -167,15 +173,15 @@
             "snv",
             '{"SPTA1"}',
             '{"HGNC:11272"}',
             "VCV000012846",
             "RCV000251633",
         ]
 
-    with (tmpdir / "out38.tsv").open("rt") as input38:
+    with (tmpdir / "out38.small.tsv").open("rt") as input38:
         lines = input38.readlines()
         assert len(lines) == 3
         assert lines[0].split("\t")[:2] == ["release", "chromosome"]
         assert lines[1].split("\t")[:12] == [
             "GRCh38",
             "1",
             "158654738",
```

### Comparing `clinvar-tsv-0.4.1/versioneer.py` & `clinvar-tsv-0.5.0/versioneer.py`

 * *Files identical despite different names*

