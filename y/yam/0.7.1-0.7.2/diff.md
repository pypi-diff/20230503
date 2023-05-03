# Comparing `tmp/yam-0.7.1.tar.gz` & `tmp/yam-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yam-0.7.1.tar", last modified: Wed Mar  8 13:36:05 2023, max compression
+gzip compressed data, was "yam-0.7.2.tar", last modified: Wed May  3 19:45:35 2023, max compression
```

## Comparing `yam-0.7.1.tar` & `yam-0.7.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-03-08 13:36:05.000000 yam-0.7.1/
--rw-rw-r--   0 eule      (1000) eule      (1000)       81 2017-08-23 08:53:34.000000 yam-0.7.1/MANIFEST.in
-drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/
--rw-rw-r--   0 eule      (1000) eule      (1000)      654 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/PKG-INFO
--rw-rw-r--   0 eule      (1000) eule      (1000)        1 2017-08-24 16:32:16.000000 yam-0.7.1/yam.egg-info/not-zip-safe
--rw-rw-r--   0 eule      (1000) eule      (1000)      546 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/SOURCES.txt
--rw-rw-r--   0 eule      (1000) eule      (1000)       74 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/requires.txt
--rw-rw-r--   0 eule      (1000) eule      (1000)       75 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/entry_points.txt
--rw-rw-r--   0 eule      (1000) eule      (1000)        4 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/top_level.txt
--rw-rw-r--   0 eule      (1000) eule      (1000)        1 2023-03-08 13:36:05.000000 yam-0.7.1/yam.egg-info/dependency_links.txt
--rw-rw-r--   0 eule      (1000) eule      (1000)     1529 2023-03-07 16:08:32.000000 yam-0.7.1/README.md
--rw-rw-r--   0 eule      (1000) eule      (1000)      654 2023-03-08 13:36:05.000000 yam-0.7.1/PKG-INFO
-drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-03-08 13:36:05.000000 yam-0.7.1/yam/
--rw-rw-r--   0 eule      (1000) eule      (1000)    23814 2020-04-29 15:33:13.000000 yam-0.7.1/yam/commands.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     3034 2020-04-29 15:32:15.000000 yam-0.7.1/yam/stack.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    10500 2023-03-08 13:35:36.000000 yam-0.7.1/yam/__init__.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    27881 2023-03-07 17:19:38.000000 yam-0.7.1/yam/correlate.py
-drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-03-08 13:36:05.000000 yam-0.7.1/yam/tests/
--rw-rw-r--   0 eule      (1000) eule      (1000)      684 2023-03-07 15:02:28.000000 yam-0.7.1/yam/tests/__init__.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     2244 2019-04-10 08:08:50.000000 yam-0.7.1/yam/tests/test_stretch.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    16323 2023-03-07 15:02:28.000000 yam-0.7.1/yam/tests/test_correlate.py
--rw-rw-r--   0 eule      (1000) eule      (1000)       33 2017-08-23 08:53:34.000000 yam-0.7.1/yam/tests/__main__.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    12718 2023-03-08 13:11:12.000000 yam-0.7.1/yam/tests/test_main.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     1393 2018-02-12 16:47:05.000000 yam-0.7.1/yam/_from_msnoise.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    15476 2019-05-02 08:31:26.000000 yam-0.7.1/yam/imaging.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    57924 2018-03-09 13:47:24.000000 yam-0.7.1/yam/_from_miic.py
--rw-rw-r--   0 eule      (1000) eule      (1000)    11276 2023-03-07 16:08:32.000000 yam-0.7.1/yam/util.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     8561 2023-03-08 13:11:12.000000 yam-0.7.1/yam/conf_example.json
--rw-rw-r--   0 eule      (1000) eule      (1000)    16954 2023-03-08 13:11:12.000000 yam-0.7.1/yam/main.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     8273 2019-04-10 08:09:24.000000 yam-0.7.1/yam/stretch.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     4972 2020-03-02 15:28:30.000000 yam-0.7.1/yam/io.py
--rw-rw-r--   0 eule      (1000) eule      (1000)     1084 2019-04-10 07:54:46.000000 yam-0.7.1/LICENSE
--rw-rw-r--   0 eule      (1000) eule      (1000)     3617 2023-03-08 13:11:12.000000 yam-0.7.1/CHANGELOG
--rw-rw-r--   0 eule      (1000) eule      (1000)       38 2023-03-08 13:36:05.000000 yam-0.7.1/setup.cfg
--rw-rw-r--   0 eule      (1000) eule      (1000)     1710 2023-03-07 16:08:32.000000 yam-0.7.1/setup.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-05-03 19:45:35.332691 yam-0.7.2/
+-rw-rw-r--   0 eule      (1000) eule      (1000)     3673 2023-05-03 19:42:55.000000 yam-0.7.2/CHANGELOG
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1085 2023-05-03 19:41:42.000000 yam-0.7.2/LICENSE
+-rw-rw-r--   0 eule      (1000) eule      (1000)       81 2017-08-23 08:53:34.000000 yam-0.7.2/MANIFEST.in
+-rw-rw-r--   0 eule      (1000) eule      (1000)      583 2023-05-03 19:45:35.332691 yam-0.7.2/PKG-INFO
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1826 2023-05-03 19:41:42.000000 yam-0.7.2/README.md
+-rw-rw-r--   0 eule      (1000) eule      (1000)       38 2023-05-03 19:45:35.332691 yam-0.7.2/setup.cfg
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1645 2023-05-03 19:41:42.000000 yam-0.7.2/setup.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-05-03 19:45:35.332691 yam-0.7.2/yam/
+-rw-rw-r--   0 eule      (1000) eule      (1000)    11318 2023-05-03 19:44:47.000000 yam-0.7.2/yam/__init__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    57924 2018-03-09 13:47:24.000000 yam-0.7.2/yam/_from_miic.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1393 2018-02-12 16:47:05.000000 yam-0.7.2/yam/_from_msnoise.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    23820 2023-05-03 19:41:42.000000 yam-0.7.2/yam/commands.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     8561 2023-03-08 13:11:12.000000 yam-0.7.2/yam/conf_example.json
+-rw-rw-r--   0 eule      (1000) eule      (1000)    27881 2023-05-03 19:41:42.000000 yam-0.7.2/yam/correlate.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    15476 2023-05-03 19:41:42.000000 yam-0.7.2/yam/imaging.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     4972 2023-05-03 19:41:42.000000 yam-0.7.2/yam/io.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    16954 2023-05-03 19:41:42.000000 yam-0.7.2/yam/main.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     3034 2023-05-03 19:41:42.000000 yam-0.7.2/yam/stack.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     8273 2023-05-03 19:41:42.000000 yam-0.7.2/yam/stretch.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-05-03 19:45:35.332691 yam-0.7.2/yam/tests/
+-rw-rw-r--   0 eule      (1000) eule      (1000)      685 2023-05-03 19:41:42.000000 yam-0.7.2/yam/tests/__init__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)       33 2017-08-23 08:53:34.000000 yam-0.7.2/yam/tests/__main__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    16323 2023-05-03 19:41:42.000000 yam-0.7.2/yam/tests/test_correlate.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    12846 2023-05-03 19:41:42.000000 yam-0.7.2/yam/tests/test_main.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2244 2023-05-03 19:41:42.000000 yam-0.7.2/yam/tests/test_stretch.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    11276 2023-05-03 19:41:42.000000 yam-0.7.2/yam/util.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2023-05-03 19:45:35.332691 yam-0.7.2/yam.egg-info/
+-rw-rw-r--   0 eule      (1000) eule      (1000)      583 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/PKG-INFO
+-rw-rw-r--   0 eule      (1000) eule      (1000)      546 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/SOURCES.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        1 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/dependency_links.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)       74 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/entry_points.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        1 2017-08-24 16:32:16.000000 yam-0.7.2/yam.egg-info/not-zip-safe
+-rw-rw-r--   0 eule      (1000) eule      (1000)       74 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/requires.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        4 2023-05-03 19:45:35.000000 yam-0.7.2/yam.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yam-0.7.1/yam.egg-info/PKG-INFO` & `yam-0.7.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yam
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yet another monitoring tool using correlations of ambient noise (seismology)
 Home-page: https://github.com/trichter/yam
 Author: Tom Eulenfeld
-Author-email: tom.eulenfeld@gmail.de
 License: MIT
-Description: Please look at the project site for tutorials and information.
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+Please look at the project site for tutorials and information.
```

### Comparing `yam-0.7.1/yam.egg-info/SOURCES.txt` & `yam-0.7.2/yam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yam-0.7.1/README.md` & `yam-0.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 
 [![build status](https://github.com/trichter/yam/workflows/tests/badge.svg)](https://github.com/trichter/yam/actions)
 [![codecov](https://codecov.io/gh/trichter/yam/branch/master/graph/badge.svg)](https://codecov.io/gh/trichter/yam)
 [![pypi version](https://img.shields.io/pypi/v/yam.svg)](https://pypi.python.org/pypi/yam)
 [![python version](https://img.shields.io/pypi/pyversions/yam.svg)](https://python.org)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3953646.svg)](https://doi.org/10.5281/zenodo.3953646)
 
+`yam` is a Python-based command line package for correlating seismic recordings of ambient vibrations and for the monitoring of relative seismic velocity changes.
 
 #### Resources
 
-* [Documentation](http://yam.readthedocs.io)
+* [Documentation](http://yam.readthedocs.io) including installation instructions
 * Example: Inter-station cross-correlations -> [notebook](https://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/yam_xcorr_ipoc/xcorr_ipoc.ipynb)
 * Showcase / advanced tutorial: Monitoring seismic velocity -> [notebook](http://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/yam_velocity_variations_patcx/processing_patcx.ipynb)
 * Yam poster at EGU 2018, doi: [10.6084/m9.figshare.16976017](https://doi.org/10.6084/m9.figshare.16976017)
 * Get help or discuss in the ObsPy forum, please use the [ObsPy Related Projects category](https://discourse.obspy.org/c/obspy-related-projects)
+* You are welcome to contribute code by opening pull requests or report bugs in the issue tracker
 
 
 #### Citation
 
 If you found this package useful, please consider citing it.
 
 Eulenfeld T (2020),
```

### Comparing `yam-0.7.1/PKG-INFO` & `yam-0.7.2/yam.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yam
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yet another monitoring tool using correlations of ambient noise (seismology)
 Home-page: https://github.com/trichter/yam
 Author: Tom Eulenfeld
-Author-email: tom.eulenfeld@gmail.de
 License: MIT
-Description: Please look at the project site for tutorials and information.
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+Please look at the project site for tutorials and information.
```

### Comparing `yam-0.7.1/yam/commands.py` & `yam-0.7.2/yam/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2018 Tom Eulenfeld, GPLv3
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """Commands used by the CLI interface"""
 import functools
 import glob
 import logging
 import multiprocessing
 import os
 import re
```

### Comparing `yam-0.7.1/yam/stack.py` & `yam-0.7.2/yam/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """Stack correlations"""
 import numpy as np
 import obspy
 from obspy import UTCDateTime as UTC
 
 from yam.util import _corr_id, _time2sec, IterTime
```

### Comparing `yam-0.7.1/yam/__init__.py` & `yam-0.7.2/yam/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2018 Tom Eulenfeld, GPLv3
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """
 yam Documentation
 =================
 
 
 Motivation
 ----------
@@ -13,50 +13,52 @@
 and MICC `MIIC <https://github.com/miic-sw/miic>`_.
 *MSNoise* is especially useful for large datasets and continuous monitoring. Configuration and the state of a project
 is managed by sqlite or mysql database. A project can be configured via web interface,
 commands are issued via command line interface. Velocity variations are determined with the
 Moving Window Cross Spectral technique (MWCS).
 *MIIC* is another monitoring library using the time-domain stretching technique.
 
-*Yam*, contrary to MSNoise, is designed for off-line usage, but also includes capabilities to reprocess continuously
-growing data. Yam does not rely onto a database, but rather checks on the fly which results already exist and which
+*Yam*, contrary to MSNoise, is designed to work with completed datasets, but also
+includes capabilities to process new additional data.
+Yam does not rely onto a database, but rather checks on the fly which results already exist and which
 results have still to be calculated.
 Cross-correlations are written to HDF5 files via the ObsPy plugin obspyh5. Thus, correlation data can be easily
 accessed with ObsPy's |read| function after the calculation. It follows a similar processing flow as MSNoise,
 but it uses the stretching similar to MIIC. (It is of course feasible to implement MWCS.)
 One of its strong points is the configuration declared in a simple, but heavily commented JSON file.
 It is possible to declare similar configurations.
 A possible use case is the reprocessing of the whole dataset in a different frequency band.
 Some code was reused from previous project `sito <https://github.com/trichter/sito>`_.
 
 
 Installation
 ------------
 
-Dependencies of yam are ``obspy>=1.1 obspyh5>=0.3 h5py``.
+Dependencies of yam are ``obspy>=1.1 obspyh5>=0.3 h5py tqdm``.
 Optional dependencies are ``IPython`` and ``cartopy``.
 The recommended way to install yam is via `anaconda <https://docs.anaconda.com/anaconda/install.html>`_ and pip::
 
     conda --add channels conda-forge
-    conda create -n yam cartopy h5py IPython matplotlib numpy obspy scipy tqdm
+    conda create -n yam cartopy h5py IPython obspy tqdm
     conda activate yam
     pip install yam
 
 After that, you can run the tests with ``yam-runtests`` and check if everything is installed properly.
 
 
 How to use yam
 --------------
 
 The scripts are started with the command line program ``yam``.
 ``yam -h`` gives an overview over available commands and options. Each command has its own help,
 e.g. ``yam correlate -h`` will print help for the ``correlate`` command.
 
 ``create`` will create an example configuration file in JSON format.
-The processing commands are ``correlate``, ``stack`` and ``stretch``.
+The processing commands ``correlate``, ``stack`` and ``stretch`` support parallelization.
+The number of cores can be specified with the ``--njobs`` flag, by default all available cores are used.
 
 ``info``, ``print``, ``load`` and ``plot`` commands allow to inspect correlations,
 stacks and stretching results as well as preprocessed data and other aspects.
 ``remove`` removes correlations or stretching results (necessary if configuration changed).
 
 Correlations, corresponding stacks and stretching results are saved in HDF5 files.
 The indices inside the HDF5 files are the following (first for correlations, second for stretching results)::
@@ -91,22 +93,29 @@
 
 
 Tutorial
 ********
 
 A small tutorial with an example dataset is included.
 It can be loaded into an empty directory with ``yam create --tutorial``.
-Now you can try out some of the following commands:
+Plots are created in a separate ``plots`` folder and can be
+interactively shown with the ``--show`` flag.
+Please open a console to work through the example command sequence.
+It is recommended to open the configuration file to simultaneously check the
+configuration of the keys used:
 
 .. code:: bash
 
+    mkdir yam_tutorial; cd yam_tutorial  # switch to empty directory
+    yam create --tutorial  # load tutorial dataset and configuration file
+
     yam info               # plot information about project
     yam info stations      # print inventory info
     yam info data          # plot info about data files
-    yam plot stations      # plot station map
+    yam plot stations      # plot station map (needs cartopy)
     yam print data CX.PATCX..BHZ 2010-02-03       # load data for a specific station and day and print information
     yam load data CX.PATCX..BHZ 2010-02-03        # load data for a specific station and day and start an IPython session
     yam plot data CX.PATCX..BHZ 2010-02-03        # plot a day file
     yam plot prepdata CX.PATCX..BHZ 2010-02-03 1  # plot the preprocessed data of the same day
                                                   # (preprocessing defined in corr config 1)
     yam correlate 1        # correlates data with corr configuration 1
     yam correlate 1        # should finish fast, because everything is already calculated
@@ -116,23 +125,28 @@
                                                        # ("wiggle" plot also possible)
     yam stack c1_s1d 3dm1d       # stack 1 day correlations with a moving stack of 3 days
     yam stack cauto 2            # stack auto-correlations with stack configuration 2
 
     yam stretch c1_s1d_s3dm1d 1  # stretch the stacked data with stretch configuration 1
     yam stretch cauto_s2 2       # stretch the stacked auto-correlations with another stretch configuration
     yam info                     # find out about the keys which are already in use
-    yam plot cauto_t2            # plot similarity matrices for the given processing chain
-    yam plot cauto_s2_t2 --plot-options '{"show_line": true}' --show  # plot all similarity matrices for this processing
-                                                                      # chain and display them on screen (zoom etc.)
+    yam plot cauto_s2_t2         # plot similarity matrices for the given processing chain
+    yam plot cauto_s2_t2 --plot-options '{"show_line": true}' --show  # plot similarity matrices and show
+                                                                      # an interactive plot
     yam plot c1_s1d_s3dm1d_t1/CX.PATCX-CX.PB01  # plot similarity matrices, but only for one station combination
                                                 # (restricting the group is also possible for stacking and stretching)
 
 Of course, the plots do not look overwhelmingly for such a small dataset.
 
-The readme in the Github repository links to a further advanced tutorial.
+Two advanced tutorials are available as Jupyter notebooks:
+
+* `Inter-station cross-correlations <https://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/yam_xcorr_ipoc/xcorr_ipoc.ipynb>`_
+* `Monitoring seismic velocity <http://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/yam_velocity_variations_patcx/processing_patcx.ipynb>`_
+
+Further resources are listed in the readme of the Github repository.
 
 
 Use your own data
 *****************
 
 Create the example configuration with ``yam create`` and adapt it to your needs.
 A good start is to change the ``inventory`` and ``data`` parameters.
@@ -190,11 +204,11 @@
 .. |Inventory.plot| replace:: `Inventory.plot() <obspy.core.inventory.inventory.Inventory.plot>`
 .. |Inventory.select| replace:: `Inventory.filter() <obspy.core.inventory.inventory.Inventory.select>`
 .. |Axes.plot| replace:: `Axes.plot() <matplotlib.axes.Axes.plot>`
 
 .. |io| replace:: io configuration dictionary
 """
 
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 from yam.main import run
 from yam.commands import read_dicts
```

### Comparing `yam-0.7.1/yam/correlate.py` & `yam-0.7.2/yam/correlate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """Preprocessing and correlation"""
 import yam.stack
 from yam.util import _filter, IterTime, smooth as smooth_func, _time2sec
 from obspy.signal.cross_correlation import correlate as obscorr
 from functools import partial
 import itertools
 import logging
```

### Comparing `yam-0.7.1/yam/tests/__init__.py` & `yam-0.7.2/yam/tests/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Tests for the rf package.
+Tests for the yam package.
 
 yam-runtests [-h] [-v] [-p] [-d] [--full] [-n num]
 
 -h    short help
 -v    be verbose
 -p    use permanent tempdir
 -d    empty permanent tempdir at start
```

### Comparing `yam-0.7.1/yam/tests/test_stretch.py` & `yam-0.7.2/yam/tests/test_stretch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2019 Tom Eulenfeld, MIT license
+# Copyright 2018-2023 Tom Eulenfeld, MIT license
 
 import os.path
 import tempfile
 import unittest
 
 import numpy as np
 from obspy import Stream, Trace, UTCDateTime as UTC
```

### Comparing `yam-0.7.1/yam/tests/test_correlate.py` & `yam-0.7.2/yam/tests/test_correlate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 import unittest
 import sys
 import warnings
 
 import numpy as np
 from obspy import read, read_inventory, UTCDateTime as UTC
 from obspy.signal.cross_correlation import correlate, xcorr_max
```

### Comparing `yam-0.7.1/yam/tests/test_main.py` & `yam-0.7.2/yam/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 
 import unittest
 import unittest.mock
 from pkg_resources import load_entry_point
 from contextlib import redirect_stderr, redirect_stdout
 import glob
 import io
@@ -164,18 +164,21 @@
         pr2 = self.out('-c conf2.json print data CX.PB06..BHZ 2010-02-05')
         self.assertEqual(pr, pr2)
 
         # check correlation
         t1 = time.time()
         self.out('correlate 1')  # takes long
         t2 = time.time()
+        # should be faster, run 3x to get some statistics
         self.out('correlate 1 -v')
+        self.out('correlate 1')
+        self.out('correlate 1')
         t3 = time.time()
         if not self.permanent_tempdir:
-            self.assertLess(t3 - t2, 0.5 * (t2 - t1))
+            self.assertLess((t3 - t2) / 3, 0.9 * (t2 - t1))
         self.out('correlate auto')  # takes long
         self.out('correlate 1a')  # takes long
         self.out('info', 'c1_s1d: 7 combs')
         self.out('info', 'c1a_s1d: 3 combs')
         self.out('info', 'cauto: 2 combs')
         cauto_info = self.out('info cauto',
                               'CX.PATCX/.BHZ-.BHZ/2010-02/2010-02-05')
```

### Comparing `yam-0.7.1/yam/_from_msnoise.py` & `yam-0.7.2/yam/_from_msnoise.py`

 * *Files identical despite different names*

### Comparing `yam-0.7.1/yam/imaging.py` & `yam-0.7.2/yam/imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """
 Plotting functions
 
 Common arguments in plotting functions are:
 
 :stream: |Stream| object with correlations
 :fname: file name for the plot output
```

### Comparing `yam-0.7.1/yam/_from_miic.py` & `yam-0.7.2/yam/_from_miic.py`

 * *Files identical despite different names*

### Comparing `yam-0.7.1/yam/util.py` & `yam-0.7.2/yam/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """Utility functions"""
 
 from importlib import import_module
 import logging
 import numbers
 import os
 from pkg_resources import resource_filename
```

### Comparing `yam-0.7.1/yam/conf_example.json` & `yam-0.7.2/yam/conf_example.json`

 * *Files identical despite different names*

### Comparing `yam-0.7.1/yam/main.py` & `yam-0.7.2/yam/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """
 Command line interface and main entry point
 """
 
 import argparse
 from argparse import SUPPRESS
 from copy import deepcopy
```

### Comparing `yam-0.7.1/yam/stretch.py` & `yam-0.7.2/yam/stretch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019, Tom Eulenfeld, MIT license
+# Copyright 2017-2023, Tom Eulenfeld, MIT license
 """
 Stretch correlations
 
 The results are returned in a dictionary with the following entries:
 
 :times: strings of starttimes of the traces (1D array, length ``N1``)
 :velchange_values: velocity changes (%) corresponding to the used stretching
```

### Comparing `yam-0.7.1/yam/io.py` & `yam-0.7.2/yam/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2019 Tom Eulenfeld, MIT license
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 """Reading and writing correlations and stretching results"""
 
 import h5py
 
 import obspyh5
 import yam
 import os.path
```

### Comparing `yam-0.7.1/LICENSE` & `yam-0.7.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2017-2019 Tom Eulenfeld
+Copyright (c) 2017-2023 Tom Eulenfeld
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
@@ -13,8 +13,8 @@
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `yam-0.7.1/CHANGELOG` & `yam-0.7.2/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+v0.7.2:
+  * improve the documentation and the tutorials
 v0.7.1:
   * use pyfftw if environment variable YAM_FFTW is set and different from "no" or "false"
     (before pyfftw was used if environment variable was set, regardless of its value)
 v0.7.0:
   * consequently use float16 in the code,
     switching to other dtypes may not be completely supported at this point and
     the possibility to change the dtype may be removed later
```

### Comparing `yam-0.7.1/setup.py` & `yam-0.7.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017-2018 Tom Eulenfeld, GPLv3
+# Copyright 2017-2023 Tom Eulenfeld, MIT license
 import os.path
 import re
 
 from setuptools import find_packages, setup
 
 
 def find_version(*paths):
@@ -28,28 +28,27 @@
 
 REQUIRES = ['h5py', 'matplotlib', 'numpy', 'obspy>=1.1', 'obspyh5>=0.3',
             'scipy>=0.18', 'setuptools', 'tqdm']
 
 CLASSIFIERS = [
     'Environment :: Console',
     'Intended Audience :: Science/Research',
-    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+    'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Physics'
     ]
 
 
 setup(name='yam',
       version=VERSION,
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       url='https://github.com/trichter/yam',
       author='Tom Eulenfeld',
-      author_email='tom.eulenfeld@gmail.de',
       license='MIT',
       packages=find_packages(),
       package_dir={'yam': 'yam'},
       install_requires=REQUIRES,
       entry_points=ENTRY_POINTS,
       include_package_data=True,
       zip_safe=False,
```

