# Comparing `tmp/spei-0.3.3.tar.gz` & `tmp/spei-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei-0.3.3.tar", last modified: Wed Mar  8 13:10:21 2023, max compression
+gzip compressed data, was "spei-0.3.4.tar", last modified: Wed May  3 08:41:56 2023, max compression
```

## Comparing `spei-0.3.3.tar` & `spei-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:10:21.314235 spei-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-08 13:10:03.000000 spei-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-03-08 13:10:21.314235 spei-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-03-08 13:10:03.000000 spei-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-08 13:10:03.000000 spei-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 13:10:21.314235 spei-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:10:21.310235 spei-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:10:21.314235 spei-0.3.3/src/spei/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/si.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-08 13:10:03.000000 spei-0.3.3/src/spei/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:10:21.314235 spei-0.3.3/src/spei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-03-08 13:10:21.000000 spei-0.3.3/src/spei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-08 13:10:21.000000 spei-0.3.3/src/spei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:10:21.000000 spei-0.3.3/src/spei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-08 13:10:21.000000 spei-0.3.3/src/spei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-08 13:10:21.000000 spei-0.3.3/src/spei.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:10:21.314235 spei-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-08 13:10:03.000000 spei-0.3.3/tests/test_dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-08 13:10:03.000000 spei-0.3.3/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-08 13:10:03.000000 spei-0.3.3/tests/test_si.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-08 13:10:03.000000 spei-0.3.3/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:41:56.605783 spei-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 08:41:35.000000 spei-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-03 08:41:56.605783 spei-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-03 08:41:35.000000 spei-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-03 08:41:35.000000 spei-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:41:56.605783 spei-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:41:56.597783 spei-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:41:56.601783 spei-0.3.4/src/spei/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/si.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-03 08:41:35.000000 spei-0.3.4/src/spei/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:41:56.601783 spei-0.3.4/src/spei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-03 08:41:56.000000 spei-0.3.4/src/spei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 08:41:56.000000 spei-0.3.4/src/spei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:41:56.000000 spei-0.3.4/src/spei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 08:41:56.000000 spei-0.3.4/src/spei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 08:41:56.000000 spei-0.3.4/src/spei.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:41:56.601783 spei-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 08:41:35.000000 spei-0.3.4/tests/test_dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-03 08:41:35.000000 spei-0.3.4/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 08:41:35.000000 spei-0.3.4/tests/test_si.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-03 08:41:35.000000 spei-0.3.4/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-03 08:41:35.000000 spei-0.3.4/tests/test_version.py
```

### Comparing `spei-0.3.3/LICENSE` & `spei-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spei-0.3.3/PKG-INFO` & `spei-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple Python package to calculate drought indices for time series such as the SPI, SPEI and SGI.
 Author-email: Martin Vonk <vonk.mart@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin Vonk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: formatting
 Provides-Extra: typing
 Provides-Extra: pytesting
 Provides-Extra: coveraging
```

### Comparing `spei-0.3.3/README.md` & `spei-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `spei-0.3.3/pyproject.toml` & `spei-0.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Hydrology',
         'Intended Audience :: Science/Research',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Typing :: Typed",
 ]
 
 [project.urls]
 homepage = "https://github.com/martinvonk/spei"
 repository = "https://github.com/martinvonk/spei"
 
 [project.optional-dependencies]
```

### Comparing `spei-0.3.3/src/spei/plot.py` & `spei-0.3.4/src/spei/plot.py`

 * *Files identical despite different names*

### Comparing `spei-0.3.3/src/spei/si.py` & `spei-0.3.4/src/spei/si.py`

 * *Files identical despite different names*

### Comparing `spei-0.3.3/src/spei/utils.py` & `spei-0.3.4/src/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei-0.3.3/src/spei.egg-info/PKG-INFO` & `spei-0.3.4/src/spei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple Python package to calculate drought indices for time series such as the SPI, SPEI and SGI.
 Author-email: Martin Vonk <vonk.mart@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin Vonk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: formatting
 Provides-Extra: typing
 Provides-Extra: pytesting
 Provides-Extra: coveraging
```

### Comparing `spei-0.3.3/tests/test_plots.py` & `spei-0.3.4/tests/test_plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import matplotlib as mpl
 from pandas import Series
 from scipy.stats import pearson3
 
 from spei.plot import dist, monthly_density
 from spei.plot import si as plot_si
 
-from .fixtures import prec, si
-
 mpl.use("Agg")  # prevent _tkinter.TclError: Can't find a usable tk.tcl error
 
 
 def test_plot_si(si: Series) -> None:
     _ = plot_si(si)
```

### Comparing `spei-0.3.3/tests/test_validate.py` & `spei-0.3.4/tests/test_validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pytest
 import logging
+
+import pytest
 from pandas import DataFrame, Series, to_datetime
 
 from spei.utils import validate_index, validate_series
 
 
 def test_validate_index(caplog) -> None:
     caplog.set_level(logging.INFO)
```

