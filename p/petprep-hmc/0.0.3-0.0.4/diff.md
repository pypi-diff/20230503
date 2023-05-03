# Comparing `tmp/petprep_hmc-0.0.3.tar.gz` & `tmp/petprep_hmc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petprep_hmc-0.0.3.tar", last modified: Thu Apr 27 11:15:43 2023, max compression
+gzip compressed data, was "petprep_hmc-0.0.4.tar", last modified: Wed May  3 20:46:33 2023, max compression
```

## Comparing `petprep_hmc-0.0.3.tar` & `petprep_hmc-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.322815 petprep_hmc-0.0.3/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.3/LICENSE
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-27 11:15:43.322628 petprep_hmc-0.0.3/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     4023 2023-04-27 11:08:27.000000 petprep_hmc-0.0.3/README.md
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.321621 petprep_hmc-0.0.3/petprep_hmc/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.3/petprep_hmc/__init__.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.322405 petprep_hmc-0.0.3/petprep_hmc.egg-info/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      224 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/SOURCES.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/dependency_links.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      403 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/requires.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/top_level.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-04-27 11:15:43.322865 petprep_hmc-0.0.3/setup.cfg
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1554 2023-04-27 11:15:38.000000 petprep_hmc-0.0.3/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.631157 petprep_hmc-0.0.4/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.4/LICENSE
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-03 20:46:33.630957 petprep_hmc-0.0.4/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-05-03 20:44:42.000000 petprep_hmc-0.0.4/README.md
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.629747 petprep_hmc-0.0.4/petprep_hmc/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.4/petprep_hmc/__init__.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.630449 petprep_hmc-0.0.4/petprep_hmc.egg-info/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      242 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/SOURCES.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/dependency_links.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      403 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/requires.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/top_level.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-05-03 20:46:33.631324 petprep_hmc-0.0.4/setup.cfg
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1554 2023-05-03 20:44:10.000000 petprep_hmc-0.0.4/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.630581 petprep_hmc-0.0.4/tests/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.4/tests/test_cli.py
```

### Comparing `petprep_hmc-0.0.3/LICENSE` & `petprep_hmc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.3/PKG-INFO` & `petprep_hmc-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep_hmc
-Version: 0.0.3
+Version: 0.0.4
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.3/README.md` & `petprep_hmc-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI](https://img.shields.io/pypi/v/petprep-hmc)](https://pypi.org/project/petprep-hmc/0.0.1/) [![Docker Hub](https://img.shields.io/docker/automated/martinnoergaard/petprep_hmc)](https://hub.docker.com/r/martinnoergaard/petprep_hmc) [![DOI](https://zenodo.org/badge/629392424.svg)](https://zenodo.org/badge/latestdoi/629392424)
+[![PyPI](https://img.shields.io/pypi/v/petprep-hmc)](https://pypi.org/project/petprep-hmc/0.0.4/) [![Docker Hub](https://img.shields.io/docker/automated/martinnoergaard/petprep_hmc)](https://hub.docker.com/r/martinnoergaard/petprep_hmc) [![DOI](https://zenodo.org/badge/629392424.svg)](https://zenodo.org/badge/latestdoi/629392424)
 
 
 # PETPrep Head Motion Correction workflow (BIDS App)
 This BIDS App provides a pipeline for preprocessing and head motion correction of Positron Emission Tomography (PET) data following the Brain Imaging Data Structure (BIDS) standard.
 
 ## Features
 
@@ -29,28 +29,32 @@
 cd petprep_hmc
 pip install -e .
 </pre>
 
 The package is also pip installable and can be installed using the following command
 
 <pre>
-pip install petprep-hmc==0.0.1
+pip install petprep-hmc==0.0.4
 </pre>
 
 ## Usage
 
 To run the PETPrep Head Motion Correction BIDS App, use the following command:
 
 `python3 run.py --bids_dir /path/to/bids_input --output_dir /path/to/bids_output --analysis_level participant [--participant_label PARTICIPANT_LABEL]`
 
 - `--bids_dir`: Path to the input BIDS dataset
 - `--output_dir`: Path to the output directory for preprocessed data
 - `--analysis_level`: Level of the analysis that will be performed. Multiple participant level analyses can be run independently (in parallel) using the same output_dir.
 - `--participant_label`: (Optional) A single participant label or a space-separated list of participant labels to process. If not provided, all participants in the dataset will be processed.
-- `--n_procs`: (Optional) number of processors allocated to be used when running the workflow
+- `--mc_start_time`: (Optional) Start time for when to perform motion correction (subsequent frame will be chosen) in seconds (default = 120 seconds).
+- `--mc_fwhm`: (Optional) FWHM for smoothing of frames prior to estimating motion (default = 10mm).
+- `--mc_thresh`: (Optional) Threshold below the following percentage (0-100) of framewise ROBUST RANGE prior to estimating motion correction (default = 20).
+- `--n_procs`: (Optional) Number of processors allocated to be used when running the workflow.
+- `--no_resample`: (Optional) Whether or not to resample the motion corrected PET data to lowest x/y/z dim in original data (default = False). 
 - `--skip_bids_validator`: (Optional) Whether or not to perform BIDS dataset validation.
 
 For example, to process participant `sub-01`, use the following command:
 
 `python3 run.py --bids_dir /data/bids_input --output_dir /data/bids_output --participant_label 01`
 
 ## Output
```

### Comparing `petprep_hmc-0.0.3/petprep_hmc.egg-info/PKG-INFO` & `petprep_hmc-0.0.4/petprep_hmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep-hmc
-Version: 0.0.3
+Version: 0.0.4
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.3/setup.py` & `petprep_hmc-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petprep_hmc",
-    version="0.0.3",
+    version="0.0.4",
     description='PETPrep Head Motion Correction Workflow',
     author='Martin Norgaard',
     author_email='martin.noergaard@di.ku.dk',
     url='https://github.com/mnoergaard/petprep_hmc',
     packages=find_packages(),
     install_requires=[
         "click==8.1.3",
```

