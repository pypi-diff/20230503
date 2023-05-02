# Comparing `tmp/linumpy-0.1.tar.gz` & `tmp/linumpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linumpy-0.1.tar", last modified: Tue May  2 23:20:27 2023, max compression
+gzip compressed data, was "linumpy-0.1.1.tar", last modified: Tue May  2 23:33:03 2023, max compression
```

## Comparing `linumpy-0.1.tar` & `linumpy-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:27.716075 linumpy-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 23:20:07.000000 linumpy-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-02 23:20:27.716075 linumpy-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 23:20:07.000000 linumpy-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:27.716075 linumpy-0.1/linumpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:07.000000 linumpy-0.1/linumpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:27.716075 linumpy-0.1/linumpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:07.000000 linumpy-0.1/linumpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 23:20:07.000000 linumpy-0.1/linumpy/io/allen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:27.716075 linumpy-0.1/linumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-02 23:20:27.000000 linumpy-0.1/linumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 23:20:27.000000 linumpy-0.1/linumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:20:27.000000 linumpy-0.1/linumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 23:20:27.000000 linumpy-0.1/linumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 23:20:27.000000 linumpy-0.1/linumpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:20:27.716075 linumpy-0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-02 23:20:07.000000 linumpy-0.1/scripts/linum_download_allen.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:20:27.716075 linumpy-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 23:20:07.000000 linumpy-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:33:03.966382 linumpy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 23:32:48.000000 linumpy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-02 23:33:03.966382 linumpy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 23:32:48.000000 linumpy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:33:03.966382 linumpy-0.1.1/linumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:32:48.000000 linumpy-0.1.1/linumpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:33:03.966382 linumpy-0.1.1/linumpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:32:48.000000 linumpy-0.1.1/linumpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 23:32:48.000000 linumpy-0.1.1/linumpy/io/allen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:33:03.966382 linumpy-0.1.1/linumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-02 23:33:03.000000 linumpy-0.1.1/linumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 23:33:03.000000 linumpy-0.1.1/linumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:33:03.000000 linumpy-0.1.1/linumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 23:33:03.000000 linumpy-0.1.1/linumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 23:33:03.000000 linumpy-0.1.1/linumpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:33:03.966382 linumpy-0.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-02 23:32:48.000000 linumpy-0.1.1/scripts/linum_download_allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:33:03.966382 linumpy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-02 23:32:48.000000 linumpy-0.1.1/setup.py
```

### Comparing `linumpy-0.1/LICENSE` & `linumpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linumpy-0.1/PKG-INFO` & `linumpy-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: linumpy
-Version: 0.1
+Version: 0.1.1
 Summary: linumpy: microscopy tools and utilities
 Home-page: https://github.com/linum-uqam/linumpy
 Download-URL: 
 Author: The LINUM developers
 Author-email: 
 Maintainer: Joël Lefebvre
 Maintainer-email: lefebvre.joel@uqam.ca
+License: GPLv3+
 Platform: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linumpy
 
 **Linumpy** is the main library supporting research and development at the *Laboratoire d'Imagerie Numérique, Neurophotonique et Microscopie* ([LINUM]).
```

### Comparing `linumpy-0.1/README.md` & `linumpy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `linumpy-0.1/linumpy/io/allen.py` & `linumpy-0.1.1/linumpy/io/allen.py`

 * *Files identical despite different names*

### Comparing `linumpy-0.1/linumpy.egg-info/PKG-INFO` & `linumpy-0.1.1/linumpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: linumpy
-Version: 0.1
+Version: 0.1.1
 Summary: linumpy: microscopy tools and utilities
 Home-page: https://github.com/linum-uqam/linumpy
 Download-URL: 
 Author: The LINUM developers
 Author-email: 
 Maintainer: Joël Lefebvre
 Maintainer-email: lefebvre.joel@uqam.ca
+License: GPLv3+
 Platform: OS Independent
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linumpy
 
 **Linumpy** is the main library supporting research and development at the *Laboratoire d'Imagerie Numérique, Neurophotonique et Microscopie* ([LINUM]).
```

### Comparing `linumpy-0.1/scripts/linum_download_allen.py` & `linumpy-0.1.1/scripts/linum_download_allen.py`

 * *Files identical despite different names*

### Comparing `linumpy-0.1/setup.py` & `linumpy-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import glob
 
 from setuptools import setup, find_packages
 
 # Versions
 _version_major = 0
 _version_minor = 1
-_version_micro = ''
+_version_micro = 1
 _version_extra = ''
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
     _ver.append(_version_micro)
 if _version_extra:
@@ -47,14 +47,17 @@
 opts = dict(name="linumpy",
             maintainer="Joël Lefebvre",
             maintainer_email="lefebvre.joel@uqam.ca",
             description="linumpy: microscopy tools and utilities",
             long_description=long_description,
             long_description_content_type="text/markdown",
             url="https://github.com/linum-uqam/linumpy",
+            license="GPLv3+",
+            license_files=["LICENSE"],
+            python_requires=">=3.10",
             download_url="",
             classifiers=CLASSIFIERS,
             author="The LINUM developers",
             author_email="",
             platforms="OS Independent",
             version=__version__,
             packages=find_packages(),
```

