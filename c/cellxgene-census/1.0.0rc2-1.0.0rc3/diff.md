# Comparing `tmp/cellxgene_census-1.0.0rc2.tar.gz` & `tmp/cellxgene_census-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.0.0rc2.tar", last modified: Mon May  1 20:53:08 2023, max compression
+gzip compressed data, was "cellxgene_census-1.0.0rc3.tar", last modified: Wed May  3 01:18:11 2023, max compression
```

## Comparing `cellxgene_census-1.0.0rc2.tar` & `cellxgene_census-1.0.0rc3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.640638 cellxgene_census-1.0.0rc2/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 20:53:08.000000 cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:53:08.644638 cellxgene_census-1.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 20:52:56.000000 cellxgene_census-1.0.0rc2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.114545 cellxgene_census-1.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-03 01:18:11.114545 cellxgene_census-1.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.110545 cellxgene_census-1.0.0rc3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:18:11.114545 cellxgene_census-1.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.110545 cellxgene_census-1.0.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.110545 cellxgene_census-1.0.0rc3/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.110545 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-03 01:18:11.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-03 01:18:11.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:18:11.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 01:18:11.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 01:18:11.000000 cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:11.114545 cellxgene_census-1.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-03 01:17:48.000000 cellxgene_census-1.0.0rc3/tests/test_util.py
```

### Comparing `cellxgene_census-1.0.0rc2/LICENSE` & `cellxgene_census-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/PKG-INFO` & `cellxgene_census-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.0.0rc2/README.md` & `cellxgene_census-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/pyproject.toml` & `cellxgene_census-1.0.0rc3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     "numpy>=1.21,<1.24",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs",
     "scipy",
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "certifi",
+    # Temporary fix for https://github.com/single-cell-data/TileDB-SOMA/issues/1322, remove when we update to tiledbsoma>1.2.2
+    "tiledb>=0.21.3",
 ]
 
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
```

### Comparing `cellxgene_census-1.0.0rc2/release_process.md` & `cellxgene_census-1.0.0rc3/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/__init__.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/_open.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.0.0rc3/src/cellxgene_census/_release_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "alias": Optional[str],  # the alias of this entry
     },
 )
 CensusDirectory = Dict[CensusVersionName, Union[CensusVersionName, CensusVersionDescription]]
 
 
 # URL for the default top-level directory of all public data
-CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://census.cellxgene.cziscience.com/cellxgene-census/release.json"
+CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://census.cellxgene.cziscience.com/cell-census/release.json"
 
 
 def get_census_version_description(census_version: str) -> CensusVersionDescription:
     """Get release description for given Census version, from the Census release directory.
 
     Args:
         census_version:
```

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.0.0rc2/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.0.0rc3/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/README.md` & `cellxgene_census-1.0.0rc3/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_acceptance.py` & `cellxgene_census-1.0.0rc3/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_directory.py` & `cellxgene_census-1.0.0rc3/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_get_anndata.py` & `cellxgene_census-1.0.0rc3/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_get_helpers.py` & `cellxgene_census-1.0.0rc3/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_open.py` & `cellxgene_census-1.0.0rc3/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.0.0rc2/tests/test_util.py` & `cellxgene_census-1.0.0rc3/tests/test_util.py`

 * *Files identical despite different names*

