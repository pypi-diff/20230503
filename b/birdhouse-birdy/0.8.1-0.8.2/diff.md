# Comparing `tmp/birdhouse-birdy-0.8.1.tar.gz` & `tmp/birdhouse-birdy-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdhouse-birdy-0.8.1.tar", last modified: Wed Dec  1 12:46:21 2021, max compression
+gzip compressed data, was "birdhouse-birdy-0.8.2.tar", last modified: Wed May  3 12:15:09 2023, max compression
```

## Comparing `birdhouse-birdy-0.8.1.tar` & `birdhouse-birdy-0.8.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.273992 birdhouse-birdy-0.8.1/
--rw-r--r--   0 pingu      (501) staff       (20)      221 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     6127 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/CHANGES.rst
--rw-r--r--   0 pingu      (501) staff       (20)    11358 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/LICENSE.txt
--rw-r--r--   0 pingu      (501) staff       (20)      183 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     9126 2021-12-01 12:46:21.274193 birdhouse-birdy-0.8.1/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1904 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/README.rst
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.259935 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     9126 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1132 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)       45 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/entry_points.txt
--rw-r--r--   0 pingu      (501) staff       (20)      337 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       12 2021-12-01 12:46:21.000000 birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/top_level.txt
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.261672 birdhouse-birdy-0.8.1/birdy/
--rw-r--r--   0 pingu      (501) staff       (20)      192 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/__init__.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.264775 birdhouse-birdy-0.8.1/birdy/cli/
--rw-r--r--   0 pingu      (501) staff       (20)     2729 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/cli/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     4941 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/cli/base.py
--rw-r--r--   0 pingu      (501) staff       (20)     1102 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/cli/misc.py
--rw-r--r--   0 pingu      (501) staff       (20)     2093 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/cli/run.py
--rw-r--r--   0 pingu      (501) staff       (20)      548 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/cli/types.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.267242 birdhouse-birdy-0.8.1/birdy/client/
--rw-r--r--   0 pingu      (501) staff       (20)     4734 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)    15353 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/base.py
--rw-r--r--   0 pingu      (501) staff       (20)    10829 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/converters.py
--rw-r--r--   0 pingu      (501) staff       (20)     9426 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/notebook.py
--rw-r--r--   0 pingu      (501) staff       (20)     2354 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/outputs.py
--rw-r--r--   0 pingu      (501) staff       (20)     9699 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/client/utils.py
--rw-r--r--   0 pingu      (501) staff       (20)      954 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/dependencies.py
--rw-r--r--   0 pingu      (501) staff       (20)      450 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/exceptions.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.268404 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/
--rw-r--r--   0 pingu      (501) staff       (20)     1092 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/README.md
--rw-r--r--   0 pingu      (501) staff       (20)       60 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)    15076 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/base.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.269701 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/
--rw-r--r--   0 pingu      (501) staff       (20)     6036 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
--rw-r--r--   0 pingu      (501) staff       (20)     1837 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
--rw-r--r--   0 pingu      (501) staff       (20)     2910 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.270137 birdhouse-birdy-0.8.1/birdy/templates/
--rw-r--r--   0 pingu      (501) staff       (20)     3173 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/templates/cmd.py.j2
--rw-r--r--   0 pingu      (501) staff       (20)     5856 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/birdy/utils.py
--rw-r--r--   0 pingu      (501) staff       (20)       81 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      249 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/requirements_dev.txt
--rw-r--r--   0 pingu      (501) staff       (20)       82 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/requirements_extra.txt
--rw-r--r--   0 pingu      (501) staff       (20)      852 2021-12-01 12:46:21.275240 birdhouse-birdy-0.8.1/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     2139 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2021-12-01 12:46:21.273645 birdhouse-birdy-0.8.1/tests/
--rw-r--r--   0 pingu      (501) staff       (20)       13 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)      489 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/common.py
--rw-r--r--   0 pingu      (501) staff       (20)     1413 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_cli.py
--rw-r--r--   0 pingu      (501) staff       (20)    12313 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_client.py
--rw-r--r--   0 pingu      (501) staff       (20)     2208 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_converters.py
--rw-r--r--   0 pingu      (501) staff       (20)      180 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_dependencies.py
--rw-r--r--   0 pingu      (501) staff       (20)      162 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_notebook.py
--rw-r--r--   0 pingu      (501) staff       (20)     4521 2021-12-01 12:41:12.000000 birdhouse-birdy-0.8.1/tests/test_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.527940 birdhouse-birdy-0.8.2/
+-rw-r--r--   0 pingu      (501) staff       (20)      221 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     6489 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/CHANGES.rst
+-rw-r--r--   0 pingu      (501) staff       (20)    11358 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/LICENSE.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      183 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     9468 2023-05-03 12:15:09.528091 birdhouse-birdy-0.8.2/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     1904 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/README.rst
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.514851 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     9468 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     1132 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       44 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/entry_points.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      337 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       12 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/top_level.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.517108 birdhouse-birdy-0.8.2/birdy/
+-rw-r--r--   0 pingu      (501) staff       (20)      192 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/__init__.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.519562 birdhouse-birdy-0.8.2/birdy/cli/
+-rw-r--r--   0 pingu      (501) staff       (20)     2729 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     4941 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/base.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1102 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/misc.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2093 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/run.py
+-rw-r--r--   0 pingu      (501) staff       (20)      548 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/types.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.521661 birdhouse-birdy-0.8.2/birdy/client/
+-rw-r--r--   0 pingu      (501) staff       (20)     4734 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)    15876 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/base.py
+-rw-r--r--   0 pingu      (501) staff       (20)    10685 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/converters.py
+-rw-r--r--   0 pingu      (501) staff       (20)     9424 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/notebook.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2354 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/outputs.py
+-rw-r--r--   0 pingu      (501) staff       (20)     9699 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)      954 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/dependencies.py
+-rw-r--r--   0 pingu      (501) staff       (20)      450 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/exceptions.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.522730 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/
+-rw-r--r--   0 pingu      (501) staff       (20)     1092 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/README.md
+-rw-r--r--   0 pingu      (501) staff       (20)       60 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)    15076 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/base.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.524036 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/
+-rw-r--r--   0 pingu      (501) staff       (20)     6092 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
+-rw-r--r--   0 pingu      (501) staff       (20)     1832 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
+-rw-r--r--   0 pingu      (501) staff       (20)     3037 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.524372 birdhouse-birdy-0.8.2/birdy/templates/
+-rw-r--r--   0 pingu      (501) staff       (20)     3173 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/templates/cmd.py.j2
+-rw-r--r--   0 pingu      (501) staff       (20)     5856 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)       81 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      249 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements_dev.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       82 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements_extra.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      852 2023-05-03 12:15:09.528883 birdhouse-birdy-0.8.2/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     2139 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.527662 birdhouse-birdy-0.8.2/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)       13 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)      489 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/common.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1413 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_cli.py
+-rw-r--r--   0 pingu      (501) staff       (20)    11959 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_client.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2208 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_converters.py
+-rw-r--r--   0 pingu      (501) staff       (20)      180 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_dependencies.py
+-rw-r--r--   0 pingu      (501) staff       (20)      162 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_notebook.py
+-rw-r--r--   0 pingu      (501) staff       (20)     4521 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_utils.py
```

### Comparing `birdhouse-birdy-0.8.1/CHANGES.rst` & `birdhouse-birdy-0.8.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Change History
 **************
 
+0.8.2 (2023-04-28)
+==================
+
+Changes:
+
+* Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
+* Remove tests with live 52North WPS server since it seems offline.
+* Remove Python 3.6 from test matrix and add 3.10.
+* Handle the removal of the `verbose` argument in `OWSLib.WebProcessingService` 0.29.0.
+
 0.8.1 (2021-12-01)
 ==================
 
 Changes:
 
 * Before trying to open a netCDF dataset, determine whether link is a valid OPeNDAP endpoint to avoid unnecessarily raising the cryptic ``syntax error, unexpected WORD_WORD, expecting SCAN_ATTR or SCAN_DATASET or SCAN_ERROR``.
```

### Comparing `birdhouse-birdy-0.8.1/LICENSE.txt` & `birdhouse-birdy-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/PKG-INFO` & `birdhouse-birdy-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.1
+Version: 0.8.2
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -53,19 +52,19 @@
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
 .. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.1?filepath=notebooks
+   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
    :alt: Binder Launcher
 
 .. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.1/notebooks/
+   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
    :alt: NBViewer
    :height: 20
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
 
@@ -81,14 +80,24 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.2 (2023-04-28)
+==================
+
+Changes:
+
+* Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
+* Remove tests with live 52North WPS server since it seems offline.
+* Remove Python 3.6 from test matrix and add 3.10.
+* Handle the removal of the `verbose` argument in `OWSLib.WebProcessingService` 0.29.0.
+
 0.8.1 (2021-12-01)
 ==================
 
 Changes:
 
 * Before trying to open a netCDF dataset, determine whether link is a valid OPeNDAP endpoint to avoid unnecessarily raising the cryptic ``syntax error, unexpected WORD_WORD, expecting SCAN_ATTR or SCAN_DATASET or SCAN_ERROR``.
 
@@ -370,9 +379,7 @@
 * allow local file path for complex inputs.
 * send complex data inline with requet to remote wps service.
 
 0.1.0 (2014-12-02)
 ==================
 
 * Initial Release.
-
-
```

### Comparing `birdhouse-birdy-0.8.1/README.rst` & `birdhouse-birdy-0.8.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
 .. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.1?filepath=notebooks
+   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
    :alt: Binder Launcher
 
 .. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.1/notebooks/
+   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
    :alt: NBViewer
    :height: 20
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
```

### Comparing `birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/PKG-INFO` & `birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.1
+Version: 0.8.2
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -53,19 +52,19 @@
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
 .. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.1?filepath=notebooks
+   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
    :alt: Binder Launcher
 
 .. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.1/notebooks/
+   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
    :alt: NBViewer
    :height: 20
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
 
@@ -81,14 +80,24 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.2 (2023-04-28)
+==================
+
+Changes:
+
+* Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
+* Remove tests with live 52North WPS server since it seems offline.
+* Remove Python 3.6 from test matrix and add 3.10.
+* Handle the removal of the `verbose` argument in `OWSLib.WebProcessingService` 0.29.0.
+
 0.8.1 (2021-12-01)
 ==================
 
 Changes:
 
 * Before trying to open a netCDF dataset, determine whether link is a valid OPeNDAP endpoint to avoid unnecessarily raising the cryptic ``syntax error, unexpected WORD_WORD, expecting SCAN_ATTR or SCAN_DATASET or SCAN_ERROR``.
 
@@ -370,9 +379,7 @@
 * allow local file path for complex inputs.
 * send complex data inline with requet to remote wps service.
 
 0.1.0 (2014-12-02)
 ==================
 
 * Initial Release.
-
-
```

### Comparing `birdhouse-birdy-0.8.1/birdhouse_birdy.egg-info/SOURCES.txt` & `birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/cli/__init__.py` & `birdhouse-birdy-0.8.2/birdy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/cli/base.py` & `birdhouse-birdy-0.8.2/birdy/cli/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/cli/misc.py` & `birdhouse-birdy-0.8.2/birdy/cli/misc.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/cli/run.py` & `birdhouse-birdy-0.8.2/birdy/cli/run.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/cli/types.py` & `birdhouse-birdy-0.8.2/birdy/cli/types.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/client/__init__.py` & `birdhouse-birdy-0.8.2/birdy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/client/base.py` & `birdhouse-birdy-0.8.2/birdy/client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from owslib.wps import (
     ASYNC,
     SYNC,
     WPS_DEFAULT_VERSION,
     ComplexData,
     WebProcessingService,
 )
+from warnings import warn
+import packaging.version
 
 from birdy.client import notebook, utils
 from birdy.client.outputs import WPSResult
 from birdy.exceptions import UnauthorizedException
 from birdy.utils import embed, fix_url, guess_type, sanitize
 
 
@@ -42,21 +44,21 @@
         converters=None,
         username=None,
         password=None,
         headers=None,
         auth=None,
         verify=True,
         cert=None,
-        verbose=False,
         progress=False,
         version=WPS_DEFAULT_VERSION,
         caps_xml=None,
         desc_xml=None,
         language=None,
         lineage=False,
+        **kwds,
     ):
         """Initialize WPSClient.
 
         Parameters
         ----------
         url: str
           Link to WPS provider. config (Config): an instance
@@ -73,16 +75,16 @@
         auth: requests.auth.AuthBase
           requests-style auth class to authenticate.
           see https://2.python-requests.org/en/master/user/authentication/
         verify: bool
           passed to :class:`owslib.wps.WebProcessingService`
         cert: str
           passed to :class:`owslib.wps.WebProcessingService`
-        verbose: str
-          passed to :class:`owslib.wps.WebProcessingService`
+        verbose: bool
+          Deprecated. passed to :class:`owslib.wps.WebProcessingService` for owslib < 0.29
         progress: bool
           If True, enable interactive user mode.
         version: str
           WPS version to use.
         language: str
           passed to :class:`owslib.wps.WebProcessingService` (ex: 'fr-CA', 'en_US').
         lineage: bool
@@ -113,25 +115,36 @@
             # We prepare a dummy request, call the auth object with it, and get its headers
             dummy_request = requests.Request("get", "http://localhost")
             r = auth(dummy_request.prepare())
 
             auth_headers = ["Authorization", "Proxy-Authorization", "Cookie"]
             headers.update({h: r.headers[h] for h in auth_headers if h in r.headers})
 
+        if "verbose" in kwds:
+            if packaging.version.parse(owslib.__version__) >= packaging.version.parse(
+                "0.29.0"
+            ):
+                kwds.pop("verbose")
+            warn(
+                "The 'verbose' keyword is deprecated and will be removed in a future version. Starting with owslib "
+                "0.29.0, debugging information is logged instead of printed.",
+                DeprecationWarning,
+            )
+
         self._wps = WebProcessingService(
             url,
             version=version,
             username=username,
             password=password,
-            verbose=verbose,
             headers=headers,
             verify=verify,
             cert=cert,
             skip_caps=True,
             language=language,
+            **kwds,
         )
 
         try:
             self._wps.getcapabilities(xml=caps_xml)
         except ServiceException as e:
             if "AccessForbidden" in str(e):
                 raise UnauthorizedException(
@@ -305,15 +318,14 @@
                 else arg
             )
             supported_mimetypes = [v.mimeType for v in input_param.supportedValues]
 
             for value in values:
                 #  if input_param.dataType == "ComplexData": seems simpler
                 if isinstance(input_param.defaultValue, ComplexData):
-
                     # Guess the mimetype of the input value
                     mimetype, encoding = guess_type(value, supported_mimetypes)
 
                     if encoding is None:
                         encoding = input_param.defaultValue.encoding
 
                     if isinstance(value, ComplexData):
```

### Comparing `birdhouse-birdy-0.8.1/birdy/client/converters.py` & `birdhouse-birdy-0.8.2/birdy/client/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,14 @@
 # TODO: Add test for this.
 class GeotiffRioxarrayConverter(BaseConverter):  # noqa: D101
     mimetypes = ["image/tiff; subtype=geotiff"]
     extensions = ["tiff", "tif"]
     priority = 3
 
     def check_dependencies(self):  # noqa: D102
-        GeotiffRasterioConverter.check_dependencies(self)  # type: ignore
         self._check_import("rioxarray")
 
     def convert(self):  # noqa: D102
         import xarray  # isort: skip
         import rioxarray  # noqa
 
         return xarray.open_rasterio(self.file)
@@ -268,15 +267,14 @@
 # TODO: Add test for this.
 class GeotiffRasterioConverter(BaseConverter):  # noqa: D101
     mimetypes = ["image/tiff; subtype=geotiff"]
     extensions = ["tiff", "tif"]
     priority = 2
 
     def check_dependencies(self):  # noqa: D102
-        GeotiffGdalConverter.check_dependencies(self)  # type: ignore
         self._check_import("rasterio")
 
     def convert(self):  # noqa: D102
         import rasterio  # isort: skip
 
         return rasterio.open(self.file).read()
```

### Comparing `birdhouse-birdy-0.8.1/birdy/client/notebook.py` & `birdhouse-birdy-0.8.2/birdy/client/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         style = {"description_width": "initial"}
         if any(
             [
                 o.dataType == "ComplexData" and len(o.supportedValues) > 1
                 for (key, o) in outputs
             ]
         ):
-            for (key, output) in outputs:
+            for key, output in outputs:
                 if hasattr(output, "supportedValues"):
                     of[key] = widgets.RadioButtons(
                         options=[o.mimeType for o in output.supportedValues],
                         description=output.title,
                         description_tooltip=output.abstract,
                         style=style,
                     )
```

### Comparing `birdhouse-birdy-0.8.1/birdy/client/outputs.py` & `birdhouse-birdy-0.8.2/birdy/client/outputs.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/client/utils.py` & `birdhouse-birdy-0.8.2/birdy/client/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/dependencies.py` & `birdhouse-birdy-0.8.2/birdy/dependencies.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/README.md` & `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/README.md`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/base.py` & `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb` & `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970486111111111%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'url = "*

 * *            '"http://boreas.ouranos.ca/geoserver/wfs"\\n\'), (4, \'version = "2.0.0"\\n\')], '*

 * *            "delete: [4, 3]}}, 5: {'source': "*

 * *            '[\'wfs_connection.build_layer(layer_typename="public:HydroLAKES_poly", '*

 * *            "source_map=demo_map)']}, 9: {'source': "*

 * *            "['wfs_connection.create_feature_property_widget(\\n', '    "*

 * *            'widget_name="Wshd_area", feature_property="Wshd_area", '*

 * *            'widget_position="botto […]*

```diff
@@ -15,16 +15,16 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from birdy import IpyleafletWFS\n",
                 "from ipyleaflet import Map\n",
                 "\n",
-                "url = 'http://boreas.ouranos.ca/geoserver/wfs'\n",
-                "version = '2.0.0'\n",
+                "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
+                "version = \"2.0.0\"\n",
                 "\n",
                 "wfs_connection = IpyleafletWFS(url, version)\n",
                 "\n",
                 "demo_map = Map(center=(46.42, -64.14), zoom=8)\n",
                 "demo_map"
             ]
         },
@@ -53,15 +53,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "wfs_connection.build_layer(layer_typename='public:HydroLAKES_poly', source_map=demo_map)"
+                "wfs_connection.build_layer(layer_typename=\"public:HydroLAKES_poly\", source_map=demo_map)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### The layer created above will have a refresh button, which can be pressed to refresh the WFS layer.\n",
@@ -91,16 +91,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "wfs_connection.create_feature_property_widget(widget_name='Wshd_area', feature_property='Wshd_area', widget_position='bottomleft')\n",
-                "demo_map\n"
+                "wfs_connection.create_feature_property_widget(\n",
+                "    widget_name=\"Wshd_area\", feature_property=\"Wshd_area\", widget_position=\"bottomleft\"\n",
+                ")\n",
+                "demo_map"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### To replace the default property widget, the same function can be used with the 'main_widget' name.\n",
@@ -110,15 +112,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "wfs_connection.create_feature_property_widget(widget_name='main_widget', feature_property='Lake_area')"
+                "wfs_connection.create_feature_property_widget(\n",
+                "    widget_name=\"main_widget\", feature_property=\"Lake_area\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### The geojson data is available. The results are also filtered by what is visible on the map."
@@ -127,25 +131,24 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "gjson = wfs_connection.geojson\n",
-                "gjson['features'][0].keys()"
+                "gjson[\"features\"][0].keys()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "gjson['totalFeatures']\n"
+                "gjson[\"totalFeatures\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### A search by ID for features is also available. Let's set back the main widget to default so we can have access to feature IDs again"
@@ -153,15 +156,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "wfs_connection.create_feature_property_widget(widget_name='main_widget')\n",
+                "wfs_connection.create_feature_property_widget(widget_name=\"main_widget\")\n",
                 "demo_map"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/quickstart-template.ipynb` & `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/quickstart-template.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997125%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'from ipyleaflet import Map\\n'), (4, 'url = "*

 * *            '"http://boreas.ouranos.ca/geoserver/wfs"\\n\'), (5, \'version = "2.0.0"\\n\')], '*

 * *            "delete: [5, 4, 1]}}, 3: {'source': {insert: [(1, "*

 * *            '\'boreas_wfs.build_layer(layer_typename="public:HydroLAKES_poly", source_map=m)\')], '*

 * *            'delete: [2, 1]}}}'}*

```diff
@@ -14,19 +14,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from birdy import IpyleafletWFS\n",
-                "from ipyleaflet  import Map\n",
+                "from ipyleaflet import Map\n",
                 "\n",
                 "# Initialize the connection\n",
-                "url ='http://boreas.ouranos.ca/geoserver/wfs'\n",
-                "version ='2.0.0'\n",
+                "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
+                "version = \"2.0.0\"\n",
                 "\n",
                 "boreas_wfs = IpyleafletWFS(url, version)\n",
                 "\n",
                 "# Create and render map\n",
                 "m = Map(center=(46.42, -64.14), zoom=8)\n",
                 "m"
             ]
@@ -44,16 +44,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Build the WFS layer\n",
-                "boreas_wfs.build_layer(layer_typename='public:HydroLAKES_poly', source_map=m)\n",
-                "\n"
+                "boreas_wfs.build_layer(layer_typename=\"public:HydroLAKES_poly\", source_map=m)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `birdhouse-birdy-0.8.1/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb` & `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971164772727272%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, 'url = "*

 * *            '"http://boreas.ouranos.ca/geoserver/wfs"\\n\'), (5, \'version = "2.0.0"\\n\'), (7, '*

 * *            "'wfs = IpyleafletWFS(url, version)')], delete: [7, 5, 4]}}, 2: {'source': {insert: "*

 * *            "[(2, 'm')], delete: [2]}}, 4: {'source': {insert: [(3, 'basin_style = {\\n'), (4, "*

 * *            '\'    "color": "#d000ff",\\n\'), (5, \'    "opacity": 1,\\n\'), (6, \'    '*

 * *            '"dashArray": "10",\\n\'), (7, \'    "fillOpacity": 0.0,\\n\'), (8, […]*

```diff
@@ -15,29 +15,29 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from birdy import IpyleafletWFS\n",
                 "from ipyleaflet import Map\n",
                 "\n",
                 "# Create connection\n",
-                "url = 'http://boreas.ouranos.ca/geoserver/wfs'\n",
-                "version = '2.0.0'\n",
+                "url = \"http://boreas.ouranos.ca/geoserver/wfs\"\n",
+                "version = \"2.0.0\"\n",
                 "\n",
-                "wfs = IpyleafletWFS(url, version)\n"
+                "wfs = IpyleafletWFS(url, version)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create the map instance\n",
                 "m = Map(center=(47.90, -69.90), zoom=11)\n",
-                "m\n"
+                "m"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -51,19 +51,27 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create wfs layer\n",
                 "# Move and zoom to the desired extent before running this cell\n",
                 "# Do NOT zoom too far out, as large GeoJSON layers can be long to load and even cause crashed\n",
-                "basin_style = { 'color': '#d000ff', 'opacity': 1, 'dashArray': '10', 'fillOpacity': 0.0, 'weight': 3 }\n",
-                "lake_style = { 'color': '#00aeff', 'dashArray': '0', 'fillOpacity': 0.5, 'weight': 0.5 }\n",
+                "basin_style = {\n",
+                "    \"color\": \"#d000ff\",\n",
+                "    \"opacity\": 1,\n",
+                "    \"dashArray\": \"10\",\n",
+                "    \"fillOpacity\": 0.0,\n",
+                "    \"weight\": 3,\n",
+                "}\n",
+                "lake_style = {\"color\": \"#00aeff\", \"dashArray\": \"0\", \"fillOpacity\": 0.5, \"weight\": 0.5}\n",
                 "\n",
-                "lakes = wfs.create_wfsgeojson_layer('public:HydroLAKES_poly', m, layer_style=lake_style)\n",
-                "basins = wfs.create_wfsgeojson_layer('public:wshed_bound_n2', m, layer_style=basin_style)"
+                "lakes = wfs.create_wfsgeojson_layer(\"public:HydroLAKES_poly\", m, layer_style=lake_style)\n",
+                "basins = wfs.create_wfsgeojson_layer(\n",
+                "    \"public:wshed_bound_n2\", m, layer_style=basin_style\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `birdhouse-birdy-0.8.1/birdy/templates/cmd.py.j2` & `birdhouse-birdy-0.8.2/birdy/templates/cmd.py.j2`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/birdy/utils.py` & `birdhouse-birdy-0.8.2/birdy/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/setup.cfg` & `birdhouse-birdy-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.1
+current_version = 0.8.2
 commit = True
 tag = True
 
 [metadata]
 description-file = README.rst
 
 [bumpversion:file:birdy/__init__.py]
```

### Comparing `birdhouse-birdy-0.8.1/setup.py` & `birdhouse-birdy-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/tests/test_cli.py` & `birdhouse-birdy-0.8.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/tests/test_client.py` & `birdhouse-birdy-0.8.2/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,36 +57,14 @@
     assert wps.language == "fr-CA"
     p = wps._processes["translation"]
     assert p.title == "Processus traduit"
     resp = wps.translation(10)
     assert resp.processOutputs[0].title == "Sortie #1"
 
 
-@pytest.mark.online
-@pytest.mark.xfail(reason="A wps process has invalid defaultValue Inf")
-def test_52north():
-    """Test for the 52North conventions for WPS.
-
-    This WPS server has process and input ids with dots and dashes.
-    """
-    WPSClient(url_52n)
-
-
-@pytest.mark.online
-def test_52north_simple():
-    """Check only a few 52north processes."""
-    WPSClient(
-        url_52n,
-        processes=[
-            "org.n52.wps.server.algorithm.r.AnnotationValidation",
-            "org.n52.wps.server.r.uncertweb.make-realizations",
-        ],
-    )
-
-
 def test_52north_offline():
     """Check offline 52north processes."""
     WPSClient(
         url_52n,
         caps_xml=open(resource_file("wps_52n_caps.xml"), "rb").read(),
         desc_xml=open(resource_file("wps_52n_desc.xml"), "rb").read(),
     )
@@ -427,7 +405,14 @@
     def test_local_uri(self):  # noqa: D102
         assert is_embedded_in_request(self.remote, self.uri)
         assert not is_embedded_in_request(self.local, self.uri)
 
     def test_url(self):  # noqa: D102
         assert not is_embedded_in_request(self.remote, self.url)
         assert not is_embedded_in_request(self.local, self.url)
+
+
+def test_verbose_deprecation():  # noqa: D103
+    with pytest.warns(DeprecationWarning):
+        WPSClient(
+            url=URL_EMU, caps_xml=EMU_CAPS_XML, desc_xml=EMU_DESC_XML, verbose=True
+        )
```

### Comparing `birdhouse-birdy-0.8.1/tests/test_converters.py` & `birdhouse-birdy-0.8.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.1/tests/test_utils.py` & `birdhouse-birdy-0.8.2/tests/test_utils.py`

 * *Files identical despite different names*

