# Comparing `tmp/anisocado-0.2.2.tar.gz` & `tmp/AnisoCADO-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anisocado-0.2.2.tar", last modified: Wed Feb 15 12:36:44 2023, max compression
+gzip compressed data, was "AnisoCADO-0.2.3.tar", last modified: Wed May  3 08:38:35 2023, max compression
```

## Comparing `anisocado-0.2.2.tar` & `AnisoCADO-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-02-15 12:36:44.333717 anisocado-0.2.2/
--rw-r--r--   0 hugo      (1000) users      (998)      391 2023-02-01 12:08:31.000000 anisocado-0.2.2/LICENSE
--rw-r--r--   0 hugo      (1000) users      (998)       40 2023-02-01 12:08:31.000000 anisocado-0.2.2/MANIFEST.in
--rw-r--r--   0 hugo      (1000) users      (998)     1536 2023-02-15 12:36:44.333717 anisocado-0.2.2/PKG-INFO
--rw-r--r--   0 hugo      (1000) users      (998)      920 2023-02-01 12:08:31.000000 anisocado-0.2.2/README.md
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-02-15 12:36:44.333717 anisocado-0.2.2/anisocado/
--rw-r--r--   0 hugo      (1000) users      (998)      107 2023-02-01 12:08:31.000000 anisocado-0.2.2/anisocado/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    10116 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/_anisocado.py
--rw-r--r--   0 hugo      (1000) users      (998)     6101 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/misc.py
--rw-r--r--   0 hugo      (1000) users      (998)    16782 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/psf.py
--rw-r--r--   0 hugo      (1000) users      (998)    23379 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/psf_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)    36858 2023-02-15 12:36:23.000000 anisocado-0.2.2/anisocado/pupil_utils.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-02-15 12:36:44.333717 anisocado-0.2.2/anisocado/tests/
--rw-r--r--   0 hugo      (1000) users      (998)        1 2023-02-01 12:08:31.000000 anisocado-0.2.2/anisocado/tests/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)     1927 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/tests/test_playing_around.py
--rw-r--r--   0 hugo      (1000) users      (998)     3464 2023-02-01 13:55:41.000000 anisocado-0.2.2/anisocado/tests/test_psf_functions.py
--rw-r--r--   0 hugo      (1000) users      (998)     2467 2023-02-01 12:08:31.000000 anisocado-0.2.2/anisocado/tests/test_scao_psf.py
--rw-r--r--   0 hugo      (1000) users      (998)       54 2023-02-15 12:36:23.000000 anisocado-0.2.2/anisocado/version.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-02-15 12:36:44.333717 anisocado-0.2.2/anisocado.egg-info/
--rw-r--r--   0 hugo      (1000) users      (998)     1536 2023-02-15 12:36:44.000000 anisocado-0.2.2/anisocado.egg-info/PKG-INFO
--rw-r--r--   0 hugo      (1000) users      (998)      500 2023-02-15 12:36:44.000000 anisocado-0.2.2/anisocado.egg-info/SOURCES.txt
--rw-r--r--   0 hugo      (1000) users      (998)        1 2023-02-15 12:36:44.000000 anisocado-0.2.2/anisocado.egg-info/dependency_links.txt
--rw-r--r--   0 hugo      (1000) users      (998)       31 2023-02-15 12:36:44.000000 anisocado-0.2.2/anisocado.egg-info/requires.txt
--rw-r--r--   0 hugo      (1000) users      (998)       10 2023-02-15 12:36:44.000000 anisocado-0.2.2/anisocado.egg-info/top_level.txt
--rw-r--r--   0 hugo      (1000) users      (998)       38 2023-02-15 12:36:44.333717 anisocado-0.2.2/setup.cfg
--rw-r--r--   0 hugo      (1000) users      (998)     1541 2023-02-01 12:08:31.000000 anisocado-0.2.2/setup.py
+drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-05-03 08:38:35.653399 AnisoCADO-0.2.3/
+drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-05-03 08:38:35.653399 AnisoCADO-0.2.3/AnisoCADO.egg-info/
+-rw-r--r--   0 hugo      (1000) users      (998)     1922 2023-05-03 08:38:35.000000 AnisoCADO-0.2.3/AnisoCADO.egg-info/PKG-INFO
+-rw-r--r--   0 hugo      (1000) users      (998)      358 2023-05-03 08:38:35.000000 AnisoCADO-0.2.3/AnisoCADO.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo      (1000) users      (998)        1 2023-05-03 08:38:35.000000 AnisoCADO-0.2.3/AnisoCADO.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo      (1000) users      (998)      146 2023-05-03 08:38:35.000000 AnisoCADO-0.2.3/AnisoCADO.egg-info/requires.txt
+-rw-r--r--   0 hugo      (1000) users      (998)       10 2023-05-03 08:38:35.000000 AnisoCADO-0.2.3/AnisoCADO.egg-info/top_level.txt
+-rw-r--r--   0 hugo      (1000) users      (998)    35149 2023-05-01 09:47:58.000000 AnisoCADO-0.2.3/LICENSE
+-rw-r--r--   0 hugo      (1000) users      (998)       40 2023-05-03 07:45:50.000000 AnisoCADO-0.2.3/MANIFEST.in
+-rw-r--r--   0 hugo      (1000) users      (998)     1922 2023-05-03 08:38:35.653399 AnisoCADO-0.2.3/PKG-INFO
+-rw-r--r--   0 hugo      (1000) users      (998)      920 2023-02-01 12:08:31.000000 AnisoCADO-0.2.3/README.md
+drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-05-03 08:38:35.653399 AnisoCADO-0.2.3/anisocado/
+-rw-r--r--   0 hugo      (1000) users      (998)      107 2023-02-01 12:08:31.000000 AnisoCADO-0.2.3/anisocado/__init__.py
+-rw-r--r--   0 hugo      (1000) users      (998)    10116 2023-02-01 13:55:41.000000 AnisoCADO-0.2.3/anisocado/_anisocado.py
+-rw-r--r--   0 hugo      (1000) users      (998)     6101 2023-02-01 13:55:41.000000 AnisoCADO-0.2.3/anisocado/misc.py
+-rw-r--r--   0 hugo      (1000) users      (998)    16782 2023-02-01 13:55:41.000000 AnisoCADO-0.2.3/anisocado/psf.py
+-rw-r--r--   0 hugo      (1000) users      (998)    23379 2023-02-01 13:55:41.000000 AnisoCADO-0.2.3/anisocado/psf_utils.py
+-rw-r--r--   0 hugo      (1000) users      (998)    36858 2023-02-15 12:36:23.000000 AnisoCADO-0.2.3/anisocado/pupil_utils.py
+-rw-r--r--   0 hugo      (1000) users      (998)      104 2023-05-03 08:30:44.000000 AnisoCADO-0.2.3/anisocado/version.py
+-rw-r--r--   0 hugo      (1000) users      (998)     1427 2023-05-03 08:30:13.000000 AnisoCADO-0.2.3/pyproject.toml
+-rw-r--r--   0 hugo      (1000) users      (998)       38 2023-05-03 08:38:35.653399 AnisoCADO-0.2.3/setup.cfg
```

### Comparing `anisocado-0.2.2/PKG-INFO` & `AnisoCADO-0.2.3/AnisoCADO.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
-Name: anisocado
-Version: 0.2.2
+Name: AnisoCADO
+Version: 0.2.3
 Summary: Generate off-axis SCAO PSFs for the ELT
-Home-page: https://github.com/astronomyk/anisocado
-Author: Eric Gendron, Kieran Leschinski
-Author-email: kieran.leschinski@univie.ac.at
-License: GNU general public license
+Author: Eric Gendron
+Author-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>
+Maintainer-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>, Hugo Buddelmeijer <hugo@buddelmeijer.nl>
+License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Project-URL: Homepage, https://anisocado.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/AstarVienna/AnisoCADO/
+Project-URL: Bug Reports, https://github.com/AstarVienna/AnisoCADO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # AnisoCADO
 
 [![Tests](https://github.com/AstarVienna/AnisoCADO/actions/workflows/tests.yml/badge.svg)](https://github.com/AstarVienna/AnisoCADO/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/anisocado/badge/?version=latest)](https://anisocado.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `anisocado-0.2.2/README.md` & `AnisoCADO-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado/_anisocado.py` & `AnisoCADO-0.2.3/anisocado/_anisocado.py`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado/misc.py` & `AnisoCADO-0.2.3/anisocado/misc.py`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado/psf.py` & `AnisoCADO-0.2.3/anisocado/psf.py`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado/psf_utils.py` & `AnisoCADO-0.2.3/anisocado/psf_utils.py`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado/pupil_utils.py` & `AnisoCADO-0.2.3/anisocado/pupil_utils.py`

 * *Files identical despite different names*

### Comparing `anisocado-0.2.2/anisocado.egg-info/PKG-INFO` & `AnisoCADO-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
-Name: anisocado
-Version: 0.2.2
+Name: AnisoCADO
+Version: 0.2.3
 Summary: Generate off-axis SCAO PSFs for the ELT
-Home-page: https://github.com/astronomyk/anisocado
-Author: Eric Gendron, Kieran Leschinski
-Author-email: kieran.leschinski@univie.ac.at
-License: GNU general public license
+Author: Eric Gendron
+Author-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>
+Maintainer-email: Kieran Leschinski <kieran.leschinski@unive.ac.at>, Hugo Buddelmeijer <hugo@buddelmeijer.nl>
+License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Project-URL: Homepage, https://anisocado.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/AstarVienna/AnisoCADO/
+Project-URL: Bug Reports, https://github.com/AstarVienna/AnisoCADO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # AnisoCADO
 
 [![Tests](https://github.com/AstarVienna/AnisoCADO/actions/workflows/tests.yml/badge.svg)](https://github.com/AstarVienna/AnisoCADO/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/anisocado/badge/?version=latest)](https://anisocado.readthedocs.io/en/latest/?badge=latest)
```

