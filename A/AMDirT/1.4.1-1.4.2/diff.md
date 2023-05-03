# Comparing `tmp/AMDirT-1.4.1.tar.gz` & `tmp/AMDirT-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AMDirT-1.4.1.tar", last modified: Wed May  3 12:46:49 2023, max compression
+gzip compressed data, was "AMDirT-1.4.2.tar", last modified: Wed May  3 13:49:42 2023, max compression
```

## Comparing `AMDirT-1.4.1.tar` & `AMDirT-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.638845 AMDirT-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/autofill/
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/autofill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/core/
--rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/ena.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/merge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/application/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/viewer/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 12:46:44.000000 AMDirT-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 12:46:49.634845 AMDirT-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 12:46:44.000000 AMDirT-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:46:49.638845 AMDirT-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-03 12:46:44.000000 AMDirT-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.650574 AMDirT-1.4.2/AMDirT/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.650574 AMDirT-1.4.2/AMDirT/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/assets/tables.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.650574 AMDirT-1.4.2/AMDirT/autofill/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/autofill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.650574 AMDirT-1.4.2/AMDirT/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/core/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/core/ena.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/merge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/validate/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/validate/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/validate/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/validate/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/validate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.654574 AMDirT-1.4.2/AMDirT/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-03 13:49:39.000000 AMDirT-1.4.2/AMDirT/viewer/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:42.650574 AMDirT-1.4.2/AMDirT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:42.000000 AMDirT-1.4.2/AMDirT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 13:49:39.000000 AMDirT-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 13:49:42.654574 AMDirT-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 13:49:39.000000 AMDirT-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:49:42.654574 AMDirT-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-03 13:49:39.000000 AMDirT-1.4.2/setup.py
```

### Comparing `AMDirT-1.4.1/AMDirT/autofill/__init__.py` & `AMDirT-1.4.2/AMDirT/autofill/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/cli.py` & `AMDirT-1.4.2/AMDirT/cli.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/convert/__init__.py` & `AMDirT-1.4.2/AMDirT/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/core/__init__.py` & `AMDirT-1.4.2/AMDirT/core/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/core/diff.py` & `AMDirT-1.4.2/AMDirT/core/diff.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/core/ena.py` & `AMDirT-1.4.2/AMDirT/core/ena.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/merge/__init__.py` & `AMDirT-1.4.2/AMDirT/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/validate/__init__.py` & `AMDirT-1.4.2/AMDirT/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/validate/application/__init__.py` & `AMDirT-1.4.2/AMDirT/validate/application/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/validate/domain/__init__.py` & `AMDirT-1.4.2/AMDirT/validate/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/validate/exceptions.py` & `AMDirT-1.4.2/AMDirT/validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/viewer/__init__.py` & `AMDirT-1.4.2/AMDirT/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT/viewer/streamlit.py` & `AMDirT-1.4.2/AMDirT/viewer/streamlit.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/AMDirT.egg-info/PKG-INFO` & `AMDirT-1.4.2/AMDirT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4.1
+Version: 1.4.2
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003826.svg)](https://doi.org/10.5281/zenodo.4003826) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
 # AMDirT
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
```

### Comparing `AMDirT-1.4.1/AMDirT.egg-info/SOURCES.txt` & `AMDirT-1.4.2/AMDirT.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 AMDirT.egg-info/PKG-INFO
 AMDirT.egg-info/SOURCES.txt
 AMDirT.egg-info/dependency_links.txt
 AMDirT.egg-info/entry_points.txt
 AMDirT.egg-info/requires.txt
 AMDirT.egg-info/top_level.txt
 AMDirT/assets/__init__.py
+AMDirT/assets/tables.json
 AMDirT/autofill/__init__.py
 AMDirT/convert/__init__.py
 AMDirT/core/__init__.py
 AMDirT/core/diff.py
 AMDirT/core/ena.py
 AMDirT/merge/__init__.py
 AMDirT/validate/__init__.py
```

### Comparing `AMDirT-1.4.1/LICENSE` & `AMDirT-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.1/PKG-INFO` & `AMDirT-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4.1
+Version: 1.4.2
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003826.svg)](https://doi.org/10.5281/zenodo.4003826) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
 # AMDirT
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
```

### Comparing `AMDirT-1.4.1/README.md` & `AMDirT-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003826.svg)](https://doi.org/10.5281/zenodo.4003826) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
 # AMDirT
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
```

### Comparing `AMDirT-1.4.1/setup.py` & `AMDirT-1.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,10 +38,9 @@
         "numpy",
         "requests",
         "colorlog"
     ],
     packages=find_packages(exclude="test"),
     entry_points={"console_scripts": ["AMDirT = AMDirT.cli:cli"]},
     package_dir={"AMDirT": "AMDirT"},
-    include_package_data=True,
     package_data={"AMDirT.assets": ["tables.json"]},
 )
```

