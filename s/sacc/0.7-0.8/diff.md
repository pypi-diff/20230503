# Comparing `tmp/sacc-0.7.tar.gz` & `tmp/sacc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sacc-0.7.tar", last modified: Wed Dec  7 10:07:35 2022, max compression
+gzip compressed data, was "sacc-0.8.tar", last modified: Wed May  3 09:48:18 2023, max compression
```

## Comparing `sacc-0.7.tar` & `sacc-0.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.330570 sacc-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-07 10:07:30.000000 sacc-0.7/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-07 10:07:30.000000 sacc-0.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.322570 sacc-0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2022-12-07 10:07:30.000000 sacc-0.7/.github/workflows/desc-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-07 10:07:30.000000 sacc-0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-07 10:07:30.000000 sacc-0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-07 10:07:30.000000 sacc-0.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-07 10:07:30.000000 sacc-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-07 10:07:30.000000 sacc-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-07 10:07:35.330570 sacc-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2022-12-07 10:07:30.000000 sacc-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-07 10:07:30.000000 sacc-0.7/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2022-12-07 10:07:30.000000 sacc-0.7/doc/format.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/covariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/data_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/sacc.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/tracers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-07 10:07:30.000000 sacc-0.7/doc/source/windows.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-07 10:07:30.000000 sacc-0.7/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   102753 2022-12-07 10:07:30.000000 sacc-0.7/examples/CMB_LSS_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   120842 2022-12-07 10:07:30.000000 sacc-0.7/examples/CMB_LSS_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2022-12-07 10:07:30.000000 sacc-0.7/examples/Convert_DES_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2022-12-07 10:07:30.000000 sacc-0.7/examples/Convert_KIDS_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50825 2022-12-07 10:07:30.000000 sacc-0.7/examples/Create_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42715 2022-12-07 10:07:30.000000 sacc-0.7/examples/Create_cluster_count_SACC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-07 10:07:30.000000 sacc-0.7/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2022-12-07 10:07:30.000000 sacc-0.7/examples/SACC_for_clusters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   154105 2022-12-07 10:07:30.000000 sacc-0.7/examples/SACC_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2022-12-07 10:07:30.000000 sacc-0.7/examples/SACC_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20744 2022-12-07 10:07:30.000000 sacc-0.7/examples/example-txpipe-sacc1.sacc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-07 10:07:30.000000 sacc-0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/sacc/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-07 10:07:30.000000 sacc-0.7/sacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2022-12-07 10:07:30.000000 sacc-0.7/sacc/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16583 2022-12-07 10:07:30.000000 sacc-0.7/sacc/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    49485 2022-12-07 10:07:30.000000 sacc-0.7/sacc/sacc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2022-12-07 10:07:30.000000 sacc-0.7/sacc/tracers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2022-12-07 10:07:30.000000 sacc-0.7/sacc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2022-12-07 10:07:30.000000 sacc-0.7/sacc/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/sacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-07 10:07:35.000000 sacc-0.7/sacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-12-07 10:07:35.000000 sacc-0.7/sacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 10:07:35.000000 sacc-0.7/sacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-07 10:07:35.000000 sacc-0.7/sacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-07 10:07:35.000000 sacc-0.7/sacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 10:07:35.330570 sacc-0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2022-12-07 10:07:30.000000 sacc-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.326570 sacc-0.7/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 10:07:35.330570 sacc-0.7/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-07 10:07:30.000000 sacc-0.7/test/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-07 10:07:30.000000 sacc-0.7/test/make_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24389 2022-12-07 10:07:30.000000 sacc-0.7/test/test_sacc2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.278178 sacc-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 09:48:07.000000 sacc-0.8/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 09:48:07.000000 sacc-0.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.266177 sacc-0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-03 09:48:07.000000 sacc-0.8/.github/workflows/desc-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 09:48:07.000000 sacc-0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 09:48:07.000000 sacc-0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 09:48:07.000000 sacc-0.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 09:48:07.000000 sacc-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 09:48:07.000000 sacc-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 09:48:18.274178 sacc-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-03 09:48:07.000000 sacc-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 09:48:07.000000 sacc-0.8/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-03 09:48:07.000000 sacc-0.8/doc/format.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/covariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/data_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/sacc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/tracers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/windows.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 09:48:07.000000 sacc-0.8/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   102753 2023-05-03 09:48:07.000000 sacc-0.8/examples/CMB_LSS_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   120842 2023-05-03 09:48:07.000000 sacc-0.8/examples/CMB_LSS_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-03 09:48:07.000000 sacc-0.8/examples/Convert_DES_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-03 09:48:07.000000 sacc-0.8/examples/Convert_KIDS_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-05-03 09:48:07.000000 sacc-0.8/examples/Create_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42715 2023-05-03 09:48:07.000000 sacc-0.8/examples/Create_cluster_count_SACC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 09:48:07.000000 sacc-0.8/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_for_clusters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   154105 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20744 2023-05-03 09:48:07.000000 sacc-0.8/examples/example-txpipe-sacc1.sacc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 09:48:07.000000 sacc-0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/sacc/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 09:48:07.000000 sacc-0.8/sacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-03 09:48:07.000000 sacc-0.8/sacc/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16583 2023-05-03 09:48:07.000000 sacc-0.8/sacc/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-05-03 09:48:07.000000 sacc-0.8/sacc/sacc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-03 09:48:07.000000 sacc-0.8/sacc/tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-03 09:48:07.000000 sacc-0.8/sacc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-03 09:48:07.000000 sacc-0.8/sacc/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/sacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:48:18.278178 sacc-0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-03 09:48:07.000000 sacc-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 09:48:07.000000 sacc-0.8/test/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 09:48:07.000000 sacc-0.8/test/make_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-05-03 09:48:07.000000 sacc-0.8/test/test_sacc2.py
```

### Comparing `sacc-0.7/.github/workflows/desc-ci.yml` & `sacc-0.8/.github/workflows/desc-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 jobs:
   Test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Dependencies
       run: |
         python -m pip install --upgrade numpy pytest
         python -m pip install -r requirements.txt
```

### Comparing `sacc-0.7/.gitignore` & `sacc-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sacc-0.7/LICENSE` & `sacc-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sacc-0.7/PKG-INFO` & `sacc-0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.7
+Version: 0.8
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Sacc
 ====
 
 SACC (Save All Correlations and Covariances) is a format and reference library for general storage
@@ -49,7 +51,9 @@
 
 Citation
 --------
 
 Sacc has been submitted to the [Astrophysics Source Code Library](https://ascl.net/code/v/2277); follow the link that will appear there to NASA ADS to export a bibtex citation.
 
 The core developers of Sacc are Joe Zuntz (maintainer), David Alonso, and Matt Becker.
+
+
```

### Comparing `sacc-0.7/README.md` & `sacc-0.8/README.md`

 * *Files identical despite different names*

### Comparing `sacc-0.7/doc/Makefile` & `sacc-0.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.7/doc/format.md` & `sacc-0.8/doc/format.md`

 * *Files identical despite different names*

### Comparing `sacc-0.7/doc/source/Makefile` & `sacc-0.8/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.7/doc/source/conf.py` & `sacc-0.8/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/doc/source/intro.rst` & `sacc-0.8/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/CMB_LSS_read.ipynb` & `sacc-0.8/examples/CMB_LSS_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/CMB_LSS_write.ipynb` & `sacc-0.8/examples/CMB_LSS_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/Convert_DES_Sacc.ipynb` & `sacc-0.8/examples/Convert_DES_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/Convert_KIDS_Sacc.ipynb` & `sacc-0.8/examples/Convert_KIDS_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/Create_Sacc.ipynb` & `sacc-0.8/examples/Create_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/Create_cluster_count_SACC.ipynb` & `sacc-0.8/examples/Create_cluster_count_SACC.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/SACC_for_clusters.ipynb` & `sacc-0.8/examples/SACC_for_clusters.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/SACC_read.ipynb` & `sacc-0.8/examples/SACC_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/SACC_write.ipynb` & `sacc-0.8/examples/SACC_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.7/examples/example-txpipe-sacc1.sacc` & `sacc-0.8/examples/example-txpipe-sacc1.sacc`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc/covariance.py` & `sacc-0.8/sacc/covariance.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc/data_types.py` & `sacc-0.8/sacc/data_types.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc/sacc.py` & `sacc-0.8/sacc/sacc.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc/tracers.py` & `sacc-0.8/sacc/tracers.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                           "add to the list.")
         self.name = name
         self.quantity = quantity
         self.metadata = kwargs.pop('metadata', {})
 
     def __init_subclass__(cls, tracer_type):
         cls._tracer_classes[tracer_type] = cls
-        cls._tracer_classes[tracer_type.lower()] = cls
         cls.tracer_type = tracer_type
 
     @classmethod
     def make(cls, tracer_type, name, *args, **kwargs):
         """
         Select a Tracer subclass based on tracer_type
         and instantiate in instance of it with the remaining
@@ -100,15 +99,17 @@
         -------
         tables: list
             List of astropy tables
         """
         tables = []
         for name, subcls in cls._tracer_classes.items():
             tracers = [t for t in instance_list if type(t) == subcls]
-            tables += subcls.to_tables(tracers)
+            # If the list is empty, we don't want to append any tables.
+            if tracers:
+                tables += subcls.to_tables(tracers)
         return tables
 
     @classmethod
     def from_tables(cls, table_list):
         """Convert a list of astropy tables into a dictionary of tracers
 
         This is used when loading data from a file.
@@ -643,7 +644,145 @@
                 if key.startswith("META_"):
                     metadata[key[5:]] = value
             tracers[name] = cls(name, z, nz,
                                 quantity=quantity,
                                 extra_columns=extra_columns,
                                 metadata=metadata)
         return tracers
+
+
+class QPNZTracer(BaseTracer, tracer_type='QPNZ'):
+    """
+    A Tracer type for tomographic n(z) data preresented as a `qp.Ensemble`
+
+    Takes a `qp.Ensemble`
+
+    Parameters
+    ----------
+    name: str
+        The name for this specific tracer, e.g. a
+        tomographic bin identifier.
+
+    ensemble: qp.Ensemble
+        The qp.ensemble in questions
+    """
+
+    def __init__(self, name, ens, **kwargs):
+        """
+        Create a tracer corresponding to a distribution in redshift n(z),
+        for example of galaxies.
+
+        Parameters
+        ----------
+        name: str
+            The name for this specific tracer, e.g. a
+            tomographic bin identifier.
+
+        ensemble: qp.Ensemble
+            The qp.ensemble in questions
+
+        Returns
+        -------
+        instance: NZTracer object
+            An instance of this class
+        """
+        super().__init__(name, **kwargs)
+        self.ensemble = ens
+
+    @classmethod
+    def to_tables(cls, instance_list):
+        """Convert a list of NZTracers to a list of astropy tables
+
+        This is used when saving data to a file.
+        Two or three tables are generated per tracer.
+
+        Parameters
+        ----------
+        instance_list: list
+            List of tracer instances
+
+        Returns
+        -------
+        tables: list
+            List of astropy tables
+        """
+        from tables_io.convUtils import convertToApTables
+
+        tables = []
+        
+        for tracer in instance_list:
+            table_dict = tracer.ensemble.build_tables()
+            ap_tables = convertToApTables(table_dict)
+            data_table = ap_tables['data']
+            meta_table = ap_tables['meta']
+            ancil_table = ap_tables.get('ancil', None)
+            meta_table.meta['SACCTYPE'] = 'tracer'
+            meta_table.meta['SACCCLSS'] = cls.tracer_type
+            meta_table.meta['SACCNAME'] = tracer.name
+            meta_table.meta['SACCQTTY'] = tracer.quantity            
+            meta_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:meta'
+
+            data_table.meta['SACCTYPE'] = 'tracer'
+            data_table.meta['SACCCLSS'] = cls.tracer_type
+            data_table.meta['SACCNAME'] = tracer.name
+            data_table.meta['SACCQTTY'] = tracer.quantity            
+            data_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:data'
+
+            for kk, vv in tracer.metadata.items():
+                meta_table.meta['META_'+kk] = vv
+            tables.append(data_table)
+            tables.append(meta_table)
+            if ancil_table:
+                ancil_table.meta['SACCTYPE'] = 'tracer'
+                ancil_table.meta['SACCCLSS'] = cls.tracer_type
+                ancil_table.meta['SACCNAME'] = tracer.name
+                ancil_table.meta['SACCQTTY'] = tracer.quantity            
+                ancil_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:ancil'
+
+                tables.append(ancil_table)
+        return tables
+
+    @classmethod
+    def from_tables(cls, table_list):
+        """Convert an astropy table into a dictionary of tracers
+
+        This is used when loading data from a file.
+        A single tracer object is read from the table.
+
+        Parameters
+        ----------
+        table_list: list[astropy.table.Table]
+            Must contain the appropriate data, for example as saved
+            by to_table.
+
+        Returns
+        -------
+        tracers: dict
+            Dict mapping string names to tracer objects.
+            Only contains one key/value pair for the one tracer.
+        """
+        import qp
+        tracers = {}
+        sorted_dict = {}
+        for table_ in table_list:
+            tokens = table_.meta['EXTNAME'].split(':')
+            table_key = f'{tokens[0]}:{tokens[1]}:{tokens[2]}'
+            table_type = f'{tokens[3]}'
+            if table_key not in sorted_dict:
+                sorted_dict[table_key] = {table_type:table_}
+            else:
+                sorted_dict[table_key][table_type] = table_
+
+        for key, val in sorted_dict.items():
+            meta_table = val['meta']
+            ensemble = qp.from_tables(val)
+            name = meta_table.meta['SACCNAME']
+            quantity = meta_table.meta.get('SACCQTTY', 'generic')
+            ensemble = qp.from_tables(val)
+            metadata = {}
+            for key, value in meta_table.meta.items():
+                if key.startswith("META_"):
+                    metadata[key[5:]] = value
+            tracers[name] = cls(name, ensemble,
+                                quantity=quantity,
+                                metadata=metadata)
+        return tracers
```

### Comparing `sacc-0.7/sacc/utils.py` & `sacc-0.8/sacc/utils.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc/windows.py` & `sacc-0.8/sacc/windows.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/sacc.egg-info/PKG-INFO` & `sacc-0.8/sacc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.7
+Version: 0.8
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Sacc
 ====
 
 SACC (Save All Correlations and Covariances) is a format and reference library for general storage
@@ -49,7 +51,9 @@
 
 Citation
 --------
 
 Sacc has been submitted to the [Astrophysics Source Code Library](https://ascl.net/code/v/2277); follow the link that will appear there to NASA ADS to export a bibtex citation.
 
 The core developers of Sacc are Joe Zuntz (maintainer), David Alonso, and Matt Becker.
+
+
```

### Comparing `sacc-0.7/sacc.egg-info/SOURCES.txt` & `sacc-0.8/sacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sacc-0.7/setup.py` & `sacc-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/test/make_test_data.py` & `sacc-0.8/test/make_test_data.py`

 * *Files identical despite different names*

### Comparing `sacc-0.7/test/test_sacc2.py` & `sacc-0.8/test/test_sacc2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import tempfile
 import sacc
 import sacc.data_types
+import sacc.tracers
 import numpy as np
 import pytest
 import os
 import pathlib
 import urllib
 import time
+import qp
 
 test_dir = pathlib.Path(__file__).resolve().parent
 test_data_dir = test_dir / 'data'
 
 
 # idea based on TreeCorr tests
 def get_from_wiki(url):
@@ -92,22 +94,81 @@
         s.add_data_point('cl_wrong', ('source_0', 'source_0'),
                          0.1, ell=10.)
 
 
 def test_get_data_types():
     s = get_filled_sacc()
     dt1 = [sacc.standard_types.count, sacc.standard_types.galaxy_shear_cl_bb,
-            sacc.standard_types.galaxy_shear_cl_ee]
+           sacc.standard_types.galaxy_shear_cl_ee]
     dt2 = s.get_data_types()
     assert sorted(dt1) == sorted(dt2)
 
     dt2 = s.get_data_types(tracers=('source_0', 'source_1'))
     assert [sacc.standard_types.galaxy_shear_cl_bb] == dt2
 
 
+def test_table_creation_0_instances():
+    """If there are no tracer test_table_creation_0_instances, we should
+    generate no tables."""
+    tables = sacc.tracers.BaseTracer.to_tables([])
+    assert len(tables) == 0
+
+
+def test_table_creation_misc_1_instance():
+    t = sacc.tracers.MiscTracer("source_0")
+    tables = sacc.tracers.BaseTracer.to_tables([t])
+    assert len(tables) == 1
+
+
+def test_table_creation_misc_2_instances():
+    t1 = sacc.tracers.MiscTracer("source_0")
+    t2 = sacc.tracers.MiscTracer("source_1")
+    tables = sacc.tracers.BaseTracer.to_tables([t1, t2])
+    assert len(tables) == 1
+
+
+def test_table_creation_nz_1_instance():
+    t = sacc.tracers.NZTracer("source_0", np.zeros(1), np.zeros(1))
+    tables = sacc.tracers.BaseTracer.to_tables([t])
+    assert len(tables) == 1
+
+
+def test_table_creation_nz_2_instances():
+    t1 = sacc.tracers.NZTracer("source_0", np.zeros(1), np.zeros(1))
+    t2 = sacc.tracers.NZTracer("source_1", np.zeros(1), np.zeros(1))
+    tables = sacc.tracers.BaseTracer.to_tables([t1, t2])
+    assert len(tables) == 2
+
+
+def test_table_creation_map_1_instance():
+    t = sacc.tracers.MapTracer("source_0", 1, [1.5], [10.0])
+    tables = sacc.tracers.BaseTracer.to_tables([t])
+    assert len(tables) == 1
+
+
+def test_table_creation_map_2_instances():
+    t1 = sacc.tracers.MapTracer("source_0", 1, [1.5], [10.0])
+    t2 = sacc.tracers.MapTracer("source_1", 2, [2.5], [15.0])
+    tables = sacc.tracers.BaseTracer.to_tables([t1, t2])
+    assert len(tables) == 2
+
+
+def test_table_creation_numap_1_instance():
+    t = sacc.tracers.NuMapTracer("source_0", 1, [1.5], [10.0], np.zeros(1), np.zeros(1))
+    tables = sacc.tracers.BaseTracer.to_tables([t])
+    assert len(tables) == 2
+
+
+def test_table_creation_numap_2_instances():
+    t1 = sacc.tracers.NuMapTracer("source_0", 1, [1.5], [10.0], np.zeros(1), np.zeros(1))
+    t2 = sacc.tracers.NuMapTracer("source_1", 2, [2.5], [15.0], np.zeros(1), np.zeros(1))
+    tables = sacc.tracers.BaseTracer.to_tables([t1, t2])
+    assert len(tables) == 4
+
+
 def test_construct():
     s = sacc.Sacc()
 
     # Tracer
     z = np.arange(0., 1.0, 0.01)
     nz = (z-0.5)**2/0.1**2
     s.add_tracer('NZ', 'source_0', z, nz,
@@ -426,44 +487,47 @@
     assert (ind == np.arange(20, 40)).all()
 
     # multiple selections
     s2 = s.copy()
     ind = s2.indices(tracers=('source_2', 'source_2'), ell__lt=45)
     assert len(ind) == 5
 
+
 def test_remove_keep_tracers():
     s = get_filled_sacc()
 
     s.remove_tracers(['source_0'])
 
     assert ['source_1', 'source_2'] == list(s.tracers.keys())
     assert [('source_2', 'source_2')] == s.get_tracer_combinations()
 
     s = get_filled_sacc()
     s.keep_tracers(['source_0'])
     assert ['source_0'] == list(s.tracers.keys())
     assert [('source_0',)] == s.get_tracer_combinations()
 
+
 def test_cutting_block_cov():
     covmat = [np.random.uniform(size=(50, 50)),
               np.random.uniform(size=(100, 100)),
               np.random.uniform(size=(150, 150))]
     C = sacc.covariance.BaseCovariance.make(covmat)
     ind = list(range(50))
     C2 = C.keeping_indices(np.arange(50))
     assert C2.size == len(ind)
     assert np.allclose(C2.get_block(ind), covmat[0])
 
+
 def test_cutting_block_cov2():
     covmat = [np.random.uniform(size=(50, 50)),
               np.random.uniform(size=(100, 100)),
               np.random.uniform(size=(150, 150))]
     C = sacc.covariance.BaseCovariance.make(covmat)
-    ind = list(range(50,150))
-    C2 = C.keeping_indices(np.arange(50,150))
+    ind = list(range(50, 150))
+    C2 = C.keeping_indices(np.arange(50, 150))
     assert C2.size == len(ind)
     assert np.allclose(C2.get_block(range(100)), covmat[1])
 
 
 def test_cutting_full_cov():
     covmat = np.random.uniform(size=(100, 100))
     C = sacc.covariance.BaseCovariance.make(covmat)
@@ -750,18 +814,58 @@
     assert np.all(s.mean == s2.mean)
     assert np.all(s.indices(tracers=('src_0', 'source_1')) ==
                   s2.indices(tracers=('src_0', 'source_1')))
     assert np.all(s.indices(tracers=('source_1', 'source_1', 'src_0')) ==
                   s2.indices(tracers=('source_1', 'source_1', 'src_0')))
 
 
-@pytest.mark.parametrize("vv,ncl,ntr",
-                         [('0.2.0', 2, 2),
-                          ('0.3.0', 3, 2),
-                          ('0.4.2', 6, 5)])
-def test_legacy_format(vv, ncl, ntr):
-    print(vv, ncl, ntr)
-    local_file_name = get_from_wiki(
-        f'https://github.com/LSSTDESC/sacc/wiki/legacy_files/dummy_v{vv}.fits')
-    s = sacc.Sacc.load_fits(local_file_name)
-    assert len(s.mean) == ncl * 100
-    assert len(s.tracers) == ntr
+def test_qpnz_tracer():
+    md1 = {'potato': 'if_necessary', 'answer': 42, 'height': 1.83}
+    md2 = {'potato': 'never'}
+    z = np.linspace(0., 1., 101)
+
+    nz_qp_interp = qp.Ensemble(qp.interp, data=dict(xvals=z, yvals=np.ones(shape=(1, 101))))
+    nz_qp_hist = qp.Ensemble(qp.hist, data=dict(bins=z, pdfs=np.ones(shape=(1, 100))))
+
+    T1 = sacc.BaseTracer.make('QPNZ', 'tracer1', nz_qp_interp,
+                              quantity='galaxy_density',
+                              metadata=md1)
+    T2 = sacc.BaseTracer.make('QPNZ', 'tracer2', nz_qp_hist,
+                              quantity='galaxy_shear',
+                              metadata=md2)
+    assert T1.metadata == md1
+    assert T2.metadata == md2
+
+    tables = sacc.BaseTracer.to_tables([T1, T2])
+    D = sacc.BaseTracer.from_tables(tables)
+
+    T1a = D['tracer1']
+    T2a = D['tracer2']
+    assert T1a.metadata == md1
+    assert T2a.metadata == md2
+
+
+def test_io_qp():
+    s = sacc.Sacc()
+
+    # Tracer
+    z = np.linspace(0., 1.0, 101)
+    nz = np.expand_dims((z-0.5)**2/0.1**2, 0)
+    ens = qp.Ensemble(qp.interp, data=dict(xvals=z, yvals=nz))
+    ens.set_ancil(dict(modes = ens.mode(z)))
+    s.add_tracer('QPNZ', 'source_0', ens)
+
+    for i in range(20):
+        ee = 0.1 * i
+        tracers = ('source_0', 'source_0')
+        s.add_data_point(sacc.standard_types.galaxy_shear_cl_ee,
+                         tracers, ee, ell=10.0*i)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        filename = os.path.join(tmpdir, 'test.sacc')
+        s.save_fits(filename)
+        s2 = sacc.Sacc.load_fits(filename)
+
+    assert len(s2) == 20
+    mu = s2.get_mean(sacc.standard_types.galaxy_shear_cl_ee)
+    for i in range(20):
+        assert mu[i] == 0.1 * i
```

