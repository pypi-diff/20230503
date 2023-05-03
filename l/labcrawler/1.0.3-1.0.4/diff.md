# Comparing `tmp/labcrawler-1.0.3.tar.gz` & `tmp/labcrawler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-1.0.3.tar", last modified: Mon May  1 22:18:46 2023, max compression
+gzip compressed data, was "labcrawler-1.0.4.tar", last modified: Wed May  3 14:49:58 2023, max compression
```

## Comparing `labcrawler-1.0.3.tar` & `labcrawler-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.958523 labcrawler-1.0.3/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.3/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.3/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)    14416 2023-05-01 22:18:46.957861 labcrawler-1.0.3/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    14134 2023-05-01 22:16:55.000000 labcrawler-1.0.3/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.613164 labcrawler-1.0.3/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.3/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3710 2023-05-01 22:16:55.000000 labcrawler-1.0.3/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5431 2023-05-01 22:16:55.000000 labcrawler-1.0.3/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.3/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-05-01 22:16:51.000000 labcrawler-1.0.3/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.3/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.951966 labcrawler-1.0.3/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.903715 labcrawler-1.0.3/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    14416 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       80 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      714 2023-05-01 22:16:55.000000 labcrawler-1.0.3/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-05-01 22:18:46.958665 labcrawler-1.0.3/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.956537 labcrawler-1.0.3/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.3/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-05-01 22:18:21.000000 labcrawler-1.0.3/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.519645 labcrawler-1.0.4/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.4/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.4/MANIFEST.in
+-rw-r--r--   0 francispotter   (501) staff       (20)    14373 2023-05-03 14:49:58.518974 labcrawler-1.0.4/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    14091 2023-05-03 14:49:29.000000 labcrawler-1.0.4/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.492976 labcrawler-1.0.4/labcrawler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.4/labcrawler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/_legacy.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3710 2023-05-03 14:49:24.000000 labcrawler-1.0.4/labcrawler/analysis.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5582 2023-05-03 14:49:29.000000 labcrawler-1.0.4/labcrawler/cli.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.4/labcrawler/gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-05-03 14:49:24.000000 labcrawler-1.0.4/labcrawler/gitlab_ci_data_loader.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.4/labcrawler/gitlab_repository_files_extractor.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/project_data_file.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.516083 labcrawler-1.0.4/labcrawler/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/labcrawler.json.template
+-rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.505751 labcrawler-1.0.4/labcrawler.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    14373 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       80 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      714 2023-05-01 22:16:55.000000 labcrawler-1.0.4/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-05-03 14:49:58.519785 labcrawler-1.0.4/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.517933 labcrawler-1.0.4/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.4/test/test_gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-05-03 14:49:43.000000 labcrawler-1.0.4/version
```

### Comparing `labcrawler-1.0.3/LICENSE` & `labcrawler-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/PKG-INFO` & `labcrawler-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -193,19 +193,15 @@
 ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
 ci_config_committers[['committer_name','project_name']]
 
 ```
 
-If you want to see all of the rows when performing queries, rather than just a sample, try:
-
-``` python
-pandas.set_option('display.max_rows', None)
-```
+LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
 >>> neat(projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
```

### Comparing `labcrawler-1.0.3/README.md` & `labcrawler-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -183,19 +183,15 @@
 ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
 ci_config_committers[['committer_name','project_name']]
 
 ```
 
-If you want to see all of the rows when performing queries, rather than just a sample, try:
-
-``` python
-pandas.set_option('display.max_rows', None)
-```
+LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
 >>> neat(projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
```

### Comparing `labcrawler-1.0.3/labcrawler/_legacy.py` & `labcrawler-1.0.4/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler/analysis.py` & `labcrawler-1.0.4/labcrawler/analysis.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler/cli.py` & `labcrawler-1.0.4/labcrawler/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from platform import python_version
 import logging
 import sys
 import os
 
 from platformdirs import user_data_dir
 from platformdirs import user_documents_dir
+import pandas
 
 from labcrawler.analysis import RawDataSet
 from labcrawler.analysis import AssembledDataSet
 from labcrawler.analysis import DATATYPES
 from labcrawler.gitlab_ci_data_loader import GitLabCIDataLoader
 from labcrawler.analysis import output_neat
 
@@ -142,12 +143,15 @@
         loader.load_files()
         loader.load_blames()
 
     def analyze(self):
         raw = RawDataSet(self.config['output_dir'])
         assembled = AssembledDataSet(raw)
         values = vars(assembled)
-        banner = "\n".join([f"{len(values[t].index)} {t}" for t in values])
+        banner = "Available: raw, neat, pandas\n"
+        banner += "\n".join([f"{len(values[t].index)} {t}" for t in values])
         banner = f"LabCrawler analysis\n{banner}\nPython {python_version()}"
         values['raw'] = raw
         values['neat'] = output_neat
+        values['pandas'] = pandas
+        pandas.set_option('display.max_rows', None)
         interact(local=values, banner=banner)
```

### Comparing `labcrawler-1.0.3/labcrawler/gitlab_ci_config.py` & `labcrawler-1.0.4/labcrawler/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.4/labcrawler/gitlab_ci_data_loader.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-1.0.4/labcrawler/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler/templates/meltano.yml` & `labcrawler-1.0.4/labcrawler/templates/meltano.yml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.4/labcrawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -193,19 +193,15 @@
 ci_config_paths.query("local_include.notnull()")[['project_name','local_include']]
 
 # Who has edited the main CI configuration file
 ci_config_committers[['committer_name','project_name']]
 
 ```
 
-If you want to see all of the rows when performing queries, rather than just a sample, try:
-
-``` python
-pandas.set_option('display.max_rows', None)
-```
+LabCrawler sets the `max_rows` attribute to `None` so you will see all the rows in default DataFrame output.
 
 For prettier output, we've added a `neat()` function.
 
 ```python
 >>> neat(projects[['name_with_namespace','merge_method']])
 name_with_namespace                                          merge_method
 -----------------------------------------------------------  --------------
```

### Comparing `labcrawler-1.0.3/labcrawler.egg-info/SOURCES.txt` & `labcrawler-1.0.4/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/pyproject.toml` & `labcrawler-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.3/test/test_gitlab_ci_config.py` & `labcrawler-1.0.4/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*

