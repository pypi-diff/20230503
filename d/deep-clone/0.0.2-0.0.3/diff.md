# Comparing `tmp/deep-clone-0.0.2.tar.gz` & `tmp/deep-clone-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-clone-0.0.2.tar", last modified: Wed May  3 14:23:35 2023, max compression
+gzip compressed data, was "deep-clone-0.0.3.tar", last modified: Wed May  3 17:36:00 2023, max compression
```

## Comparing `deep-clone-0.0.2.tar` & `deep-clone-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 rajan     (1000) rajan     (1000)        0 2023-05-03 14:23:35.318493 deep-clone-0.0.2/
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.2/LICENSE
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)      882 2023-05-03 14:23:35.310488 deep-clone-0.0.2/PKG-INFO
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)      422 2023-05-03 14:08:07.000000 deep-clone-0.0.2/README.md
-drwxrwxrwx   0 rajan     (1000) rajan     (1000)        0 2023-05-03 14:23:35.278464 deep-clone-0.0.2/deep_clone.egg-info/
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)      882 2023-05-03 14:23:34.000000 deep-clone-0.0.2/deep_clone.egg-info/PKG-INFO
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)      199 2023-05-03 14:23:35.000000 deep-clone-0.0.2/deep_clone.egg-info/SOURCES.txt
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)        1 2023-05-03 14:23:34.000000 deep-clone-0.0.2/deep_clone.egg-info/dependency_links.txt
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)       45 2023-05-03 14:23:34.000000 deep-clone-0.0.2/deep_clone.egg-info/entry_points.txt
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)       11 2023-05-03 14:23:34.000000 deep-clone-0.0.2/deep_clone.egg-info/top_level.txt
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)       38 2023-05-03 14:23:35.318493 deep-clone-0.0.2/setup.cfg
--rwxrwxrwx   0 rajan     (1000) rajan     (1000)      731 2023-05-03 14:23:26.000000 deep-clone-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:36:00.808851 deep-clone-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      918 2023-05-03 17:36:00.807851 deep-clone-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-05-03 14:08:07.000000 deep-clone-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 17:36:00.806860 deep-clone-0.0.3/deep_clone.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:36:00.809974 deep-clone-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-05-03 17:23:40.000000 deep-clone-0.0.3/setup.py
```

### Comparing `deep-clone-0.0.2/LICENSE` & `deep-clone-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deep-clone-0.0.2/PKG-INFO` & `deep-clone-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: deep-clone
-Version: 0.0.2
-Summary: Deep clone specific folder from a GitHub repo
-Home-page: https://github.com/rajan-personal/deep-clone
-Author: Rajan Gupta
-Author-email: 96rajangupta@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Deep Clone GitHub Repo - Readme
-
-This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
-
-## Features
-
-- Deep clone a specific folder within a GitHub repository
-- Must specify a specific branch
-- Lightweight cloning, only retrieves the required folder
-
-## Requirements
-
-- Python 3.6 or later
-- Git
-
-## Usage
-
-deep_clone url dir
-
-
-
+Metadata-Version: 2.1
+Name: deep-clone
+Version: 0.0.3
+Summary: Deep clone specific folder from a GitHub repo
+Home-page: https://github.com/rajan-personal/deep-clone
+Author: Rajan Gupta
+Author-email: 96rajangupta@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Deep Clone GitHub Repo - Readme
+
+This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
+
+## Features
+
+- Deep clone a specific folder within a GitHub repository
+- Must specify a specific branch
+- Lightweight cloning, only retrieves the required folder
+
+## Requirements
+
+- Python 3.6 or later
+- Git
+
+## Usage
+
+deep_clone url dir
+
+
+
```

### Comparing `deep-clone-0.0.2/deep_clone.egg-info/PKG-INFO` & `deep-clone-0.0.3/deep_clone.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: deep-clone
-Version: 0.0.2
-Summary: Deep clone specific folder from a GitHub repo
-Home-page: https://github.com/rajan-personal/deep-clone
-Author: Rajan Gupta
-Author-email: 96rajangupta@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Deep Clone GitHub Repo - Readme
-
-This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
-
-## Features
-
-- Deep clone a specific folder within a GitHub repository
-- Must specify a specific branch
-- Lightweight cloning, only retrieves the required folder
-
-## Requirements
-
-- Python 3.6 or later
-- Git
-
-## Usage
-
-deep_clone url dir
-
-
-
+Metadata-Version: 2.1
+Name: deep-clone
+Version: 0.0.3
+Summary: Deep clone specific folder from a GitHub repo
+Home-page: https://github.com/rajan-personal/deep-clone
+Author: Rajan Gupta
+Author-email: 96rajangupta@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Deep Clone GitHub Repo - Readme
+
+This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
+
+## Features
+
+- Deep clone a specific folder within a GitHub repository
+- Must specify a specific branch
+- Lightweight cloning, only retrieves the required folder
+
+## Requirements
+
+- Python 3.6 or later
+- Git
+
+## Usage
+
+deep_clone url dir
+
+
+
```

### Comparing `deep-clone-0.0.2/setup.py` & `deep-clone-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deep-clone",
-    version="0.0.2",
+    version="0.0.3",
     py_modules=["deep_clone"],
     install_requires=[],
     entry_points={
         "console_scripts": [
-            "reverse=deep_clone:main",
+            "deep_clone=deep_clone.main:main",
         ],
     },
     author="Rajan Gupta",
     author_email="96rajangupta@gmail.com",
     description="Deep clone specific folder from a GitHub repo",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

