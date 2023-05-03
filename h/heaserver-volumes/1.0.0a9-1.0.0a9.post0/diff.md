# Comparing `tmp/heaserver-volumes-1.0.0a9.tar.gz` & `tmp/heaserver-volumes-1.0.0a9.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heaserver-volumes-1.0.0a9.tar", last modified: Wed Mar  9 00:24:36 2022, max compression
+gzip compressed data, was "dist\heaserver-volumes-1.0.0a9.post0.tar", last modified: Wed Mar  9 00:38:07 2022, max compression
```

## Comparing `heaserver-volumes-1.0.0a9.tar` & `heaserver-volumes-1.0.0a9.post0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.768460 heaserver-volumes-1.0.0a9/
--rw-rw-rw-   0        0        0    11625 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9/LICENSE
--rw-rw-rw-   0        0        0       39 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9/MANIFEST.in
--rw-rw-rw-   0        0        0     4638 2022-03-09 00:24:36.768460 heaserver-volumes-1.0.0a9/PKG-INFO
--rw-rw-rw-   0        0        0     3388 2021-12-01 18:30:50.000000 heaserver-volumes-1.0.0a9/README.md
--rw-rw-rw-   0        0        0       42 2022-03-09 00:24:36.768460 heaserver-volumes-1.0.0a9/setup.cfg
--rw-rw-rw-   0        0        0     1754 2022-03-09 00:24:10.000000 heaserver-volumes-1.0.0a9/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.538734 heaserver-volumes-1.0.0a9/src/
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.530680 heaserver-volumes-1.0.0a9/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.616632 heaserver-volumes-1.0.0a9/src/heaserver/volume/
--rw-rw-rw-   0        0        0        0 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9/src/heaserver/volume/__init__.py
--rw-rw-rw-   0        0        0    29999 2022-03-08 23:55:16.000000 heaserver-volumes-1.0.0a9/src/heaserver/volume/service.py
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.619636 heaserver-volumes-1.0.0a9/src/heaserver/volume/wstl/
--rw-rw-rw-   0        0        0    12791 2022-02-18 20:36:29.000000 heaserver-volumes-1.0.0a9/src/heaserver/volume/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.712815 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/
--rw-rw-rw-   0        0        0     4638 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-03-09 00:24:36.000000 heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.538734 heaserver-volumes-1.0.0a9/tests/
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.538734 heaserver-volumes-1.0.0a9/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-03-09 00:24:36.766384 heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/
--rw-rw-rw-   0        0        0        0 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/__init__.py
--rw-rw-rw-   0        0        0      907 2022-01-18 21:07:54.000000 heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/test_all.py
--rw-rw-rw-   0        0        0     6522 2022-02-18 20:36:29.000000 heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/testcase.py
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.710898 heaserver-volumes-1.0.0a9.post0/
+-rw-rw-rw-   0        0        0    11625 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9.post0/LICENSE
+-rw-rw-rw-   0        0        0       39 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9.post0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4732 2022-03-09 00:38:07.695260 heaserver-volumes-1.0.0a9.post0/PKG-INFO
+-rw-rw-rw-   0        0        0     3476 2022-03-09 00:36:51.000000 heaserver-volumes-1.0.0a9.post0/README.md
+-rw-rw-rw-   0        0        0       42 2022-03-09 00:38:07.710898 heaserver-volumes-1.0.0a9.post0/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-03-09 00:37:34.000000 heaserver-volumes-1.0.0a9.post0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.532270 heaserver-volumes-1.0.0a9.post0/src/
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.516641 heaserver-volumes-1.0.0a9.post0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.585678 heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/
+-rw-rw-rw-   0        0        0        0 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/__init__.py
+-rw-rw-rw-   0        0        0    29999 2022-03-08 23:55:16.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/service.py
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.616924 heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/wstl/
+-rw-rw-rw-   0        0        0    12791 2022-02-18 20:36:29.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.679617 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/
+-rw-rw-rw-   0        0        0     4732 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-03-09 00:38:07.000000 heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.532270 heaserver-volumes-1.0.0a9.post0/tests/
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.532270 heaserver-volumes-1.0.0a9.post0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-03-09 00:38:07.695260 heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/
+-rw-rw-rw-   0        0        0        0 2021-07-22 04:45:13.000000 heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/__init__.py
+-rw-rw-rw-   0        0        0      907 2022-01-18 21:07:54.000000 heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/test_all.py
+-rw-rw-rw-   0        0        0     6522 2022-02-18 20:36:29.000000 heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/testcase.py
```

### Comparing `heaserver-volumes-1.0.0a9/LICENSE` & `heaserver-volumes-1.0.0a9.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.0a9/PKG-INFO` & `heaserver-volumes-1.0.0a9.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.0.0a9
+Version: 1.0.0a9.post0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
@@ -47,14 +47,15 @@
     * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
     * git, found at https://git-scm.com/download/win.
 * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
 * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
 Python to your environment variables. The install for all users option will help keep you from accidentally installing
 packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
 below.
+* Upgrade pip to version 21.1.2 or greater with `python -m pip install --upgrade pip`.
 * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
 with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
 environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do
 this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
 after you newly configure a project with your virtualenv.**
 * From the project's root directory, and using the activated virtualenv, run `pip install wheel` followed by
   `pip install -r requirements_dev.txt`. **Do NOT run `python setup.py develop`. It will break your environment.**
```

### Comparing `heaserver-volumes-1.0.0a9/README.md` & `heaserver-volumes-1.0.0a9.post0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
     * git, found at https://git-scm.com/download/win.
 * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
 * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
 Python to your environment variables. The install for all users option will help keep you from accidentally installing
 packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
 below.
+* Upgrade pip to version 21.1.2 or greater with `python -m pip install --upgrade pip`.
 * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
 with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
 environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do
 this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
 after you newly configure a project with your virtualenv.**
 * From the project's root directory, and using the activated virtualenv, run `pip install wheel` followed by
   `pip install -r requirements_dev.txt`. **Do NOT run `python setup.py develop`. It will break your environment.**
```

### Comparing `heaserver-volumes-1.0.0a9/setup.py` & `heaserver-volumes-1.0.0a9.post0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-volumes',
-    version='1.0.0a9',
+    version='1.0.0a9.post0',
     description="The HEA volumes service",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.8',
```

### Comparing `heaserver-volumes-1.0.0a9/src/heaserver/volume/service.py` & `heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.0a9/src/heaserver/volume/wstl/all.json` & `heaserver-volumes-1.0.0a9.post0/src/heaserver/volume/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/PKG-INFO` & `heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.0.0a9
+Version: 1.0.0a9.post0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
@@ -47,14 +47,15 @@
     * Build Tools for Visual Studio 2019, found at https://visualstudio.microsoft.com/downloads/. Select the C++ tools.
     * git, found at https://git-scm.com/download/win.
 * On Mac, Xcode or the command line developer tools is required, found in the Apple Store app.
 * Python 3.8: Download and install Python 3.8 from https://www.python.org, and select the options to install for all users and add
 Python to your environment variables. The install for all users option will help keep you from accidentally installing
 packages into your Python installation's site-packages directory instead of to your virtualenv environment, described
 below.
+* Upgrade pip to version 21.1.2 or greater with `python -m pip install --upgrade pip`.
 * Create a virtualenv environment using the `python -m venv <venv_directory>` command, substituting `<venv_directory>`
 with the directory name of your virtual environment. Run `source <venv_directory>/bin/activate` (or `<venv_directory>/Scripts/activate` on Windows) to activate the virtual
 environment. You will need to activate the virtualenv every time before starting work, or your IDE may be able to do
 this for you automatically. **Note that PyCharm will do this for you, but you have to create a new Terminal panel
 after you newly configure a project with your virtualenv.**
 * From the project's root directory, and using the activated virtualenv, run `pip install wheel` followed by
   `pip install -r requirements_dev.txt`. **Do NOT run `python setup.py develop`. It will break your environment.**
```

### Comparing `heaserver-volumes-1.0.0a9/src/heaserver_volumes.egg-info/SOURCES.txt` & `heaserver-volumes-1.0.0a9.post0/src/heaserver_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/test_all.py` & `heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.0.0a9/tests/heaserver/volumetest/testcase.py` & `heaserver-volumes-1.0.0a9.post0/tests/heaserver/volumetest/testcase.py`

 * *Files identical despite different names*

