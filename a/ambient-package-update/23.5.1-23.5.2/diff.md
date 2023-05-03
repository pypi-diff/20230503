# Comparing `tmp/ambient-package-update-23.5.1.tar.gz` & `tmp/ambient-package-update-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.1.tar", last modified: Wed May  3 12:48:36 2023, max compression
+gzip compressed data, was "ambient-package-update-23.5.2.tar", last modified: Wed May  3 13:02:39 2023, max compression
```

## Comparing `ambient-package-update-23.5.1.tar` & `ambient-package-update-23.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      454 2023-05-03 12:44:56.853972 ambient-package-update-23.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 08:39:26.832463 ambient-package-update-23.5.1/.gitignore
--rw-r--r--   0        0        0      904 2023-04-28 11:22:25.211332 ambient-package-update-23.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1085 2023-05-02 14:35:16.960409 ambient-package-update-23.5.1/LICENSE.md
--rw-r--r--   0        0        0     1371 2023-05-03 12:44:56.838786 ambient-package-update-23.5.1/README.md
--rw-r--r--   0        0        0       94 2023-05-03 08:28:52.195731 ambient-package-update-23.5.1/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 08:22:28.014681 ambient-package-update-23.5.1/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 08:24:28.642109 ambient-package-update-23.5.1/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      397 2023-05-03 08:45:30.225058 ambient-package-update-23.5.1/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 12:37:34.706813 ambient-package-update-23.5.1/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 12:35:54.896071 ambient-package-update-23.5.1/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 08:24:28.642109 ambient-package-update-23.5.1/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3378 2023-05-03 12:19:39.422790 ambient-package-update-23.5.1/main.py
--rw-r--r--   0        0        0     2481 2023-05-03 12:47:10.018088 ambient-package-update-23.5.1/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-05-03 12:47:33.374386 ambient-package-update-23.5.1/requirements.txt
--rw-r--r--   0        0        0      446 2023-05-03 06:41:19.038389 ambient-package-update-23.5.1/scripts/setup_venv.ps1
--rw-r--r--   0        0        0     1780 2023-05-01 13:36:25.998330 ambient-package-update-23.5.1/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-04-28 11:22:25.211332 ambient-package-update-23.5.1/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      528 2023-05-02 10:23:29.338844 ambient-package-update-23.5.1/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1104 2023-04-27 08:41:13.643600 ambient-package-update-23.5.1/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      133 2023-04-27 09:33:15.754076 ambient-package-update-23.5.1/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     4485 2023-05-03 12:40:38.841955 ambient-package-update-23.5.1/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2020-10-29 08:14:58.247751 ambient-package-update-23.5.1/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 12:20:10.276141 ambient-package-update-23.5.1/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2020-10-29 08:14:58.263559 ambient-package-update-23.5.1/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3580 2023-05-01 13:48:42.803630 ambient-package-update-23.5.1/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       69 2023-03-28 10:15:26.101761 ambient-package-update-23.5.1/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 ambient-package-update-23.5.1/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/LICENSE.md
+-rw-r--r--   0        0        0     1695 2023-05-03 13:01:45.777494 ambient-package-update-23.5.2/README.md
+-rw-r--r--   0        0        0       93 2023-05-03 13:01:45.765213 ambient-package-update-23.5.2/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      396 2023-05-03 13:01:45.749587 ambient-package-update-23.5.2/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.2/main.py
+-rw-r--r--   0        0        0     2481 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/requirements.txt
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/scripts/setup_venv.ps1
+-rw-r--r--   0        0        0     1780 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1104 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     4485 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/Readme.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3580 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 ambient-package-update-23.5.2/PKG-INFO
```

### Comparing `ambient-package-update-23.5.1/.gitignore` & `ambient-package-update-23.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/.pre-commit-config.yaml` & `ambient-package-update-23.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/LICENSE.md` & `ambient-package-update-23.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/README.md` & `ambient-package-update-23.5.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+[![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
+[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
+
 # Ambient Package Update
 
 This repository will help keep all Python packages maintained by 
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
 ## Installation
 
 1. Ensure you have installed Python >=3.10 and the binary is in your system path
 2. Navigate into the project directory
 3. Execute scripts/setup_venv.ps1 (on Windows) or rename the file to "setup_venv.sh" and execute it for macOS and UNIX
 
 ## Versioning
 
-This project follows the CalVer versioning pattern: `YY.0M.[RELEASE]`
+This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
 ## Usage
 
 todo:
 - write usage paragraph
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
@@ -42,9 +45,12 @@
 
   ```
   flit publish --repository testpypi
   ```
 
 ## Changelog
 
-**23.05.1**
+**23.5.2**
+* Templates render a trailing newline (to conform with Python linting)
+
+**23.5.1**
 * Initial release
```

### Comparing `ambient-package-update-23.5.1/ambient_package_update/metadata/package.py` & `ambient-package-update-23.5.2/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/pyproject.toml` & `ambient-package-update-23.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/requirements.txt` & `ambient-package-update-23.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/.github/workflows/ci.yml.tpl` & `ambient-package-update-23.5.2/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/.pre-commit-config.yaml.tpl` & `ambient-package-update-23.5.2/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/LICENSE.md.tpl` & `ambient-package-update-23.5.2/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/Readme.md.tpl` & `ambient-package-update-23.5.2/templates/Readme.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/docs/Makefile.tpl` & `ambient-package-update-23.5.2/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/docs/conf.py.tpl` & `ambient-package-update-23.5.2/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/docs/make.bat.tpl` & `ambient-package-update-23.5.2/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/templates/pyproject.toml.tpl` & `ambient-package-update-23.5.2/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.1/PKG-INFO` & `ambient-package-update-23.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.5.1
+Version: 23.5.2
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,28 +21,31 @@
 Requires-Dist: pre-commit~=3.2
 Requires-Dist: black~=23.3
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
 Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md#Changelog
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
 Project-URL: Maintained by, https://ambient.digital/
 
+[![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
+[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
+
 # Ambient Package Update
 
 This repository will help keep all Python packages maintained by 
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
 ## Installation
 
 1. Ensure you have installed Python >=3.10 and the binary is in your system path
 2. Navigate into the project directory
 3. Execute scripts/setup_venv.ps1 (on Windows) or rename the file to "setup_venv.sh" and execute it for macOS and UNIX
 
 ## Versioning
 
-This project follows the CalVer versioning pattern: `YY.0M.[RELEASE]`
+This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
 ## Usage
 
 todo:
 - write usage paragraph
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
@@ -69,9 +72,12 @@
 
   ```
   flit publish --repository testpypi
   ```
 
 ## Changelog
 
-**23.05.1**
+**23.5.2**
+* Templates render a trailing newline (to conform with Python linting)
+
+**23.5.1**
 * Initial release
```

