# Comparing `tmp/mkdocs-snakemake-rule-plugin-0.2.0.tar.gz` & `tmp/mkdocs-snakemake-rule-plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.2.0.tar", last modified: Fri Apr 21 21:37:49 2023, max compression
+gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.2.1.tar", last modified: Wed May  3 08:42:54 2023, max compression
```

## Comparing `mkdocs-snakemake-rule-plugin-0.2.0.tar` & `mkdocs-snakemake-rule-plugin-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    34961 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/LICENSE.md
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1812 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/PKG-INFO
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1068 2023-04-21 21:30:37.000000 mkdocs-snakemake-rule-plugin-0.2.0/README.md
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       73 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/__init__.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      497 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/_version.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    11327 2023-04-21 21:16:40.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/markdown.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      602 2023-04-21 07:59:26.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/plugin.py
-drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1812 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      529 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)        1 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       85 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       14 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       29 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      283 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/setup.cfg
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1301 2023-04-20 07:41:50.000000 mkdocs-snakemake-rule-plugin-0.2.0/setup.py
--rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    83607 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/versioneer.py
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/LICENSE.md` & `mkdocs-snakemake-rule-plugin-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/PKG-INFO` & `mkdocs-snakemake-rule-plugin-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-snakemake-rule-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: MkDocs Plugin used to extrace rule information, to generate code and tables.
 Home-page: https://github.com/smeds/mkdocs-snakemake-rule-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
@@ -67,9 +66,7 @@
 ## Source 
 #SNAKEMAKE_RULE_SOURCE__fastp__fastp_pe#
 
 ## Parameters
 #SNAKEMAKE_RULE_TABLEE__fastp__fastp_pe#
 
 ```
-
-
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/README.md` & `mkdocs-snakemake-rule-plugin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/markdown.py` & `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def extract_snakemake_rule(file_path, rule):
     rule_content = ""
     with open(file_path, 'r') as reader:
         for line in reader:
             if line.startswith('rule') and rule in line:
                 rule_content += line
                 for line in reader:
-                    if not line.startswith("rule") or line.startswith("def") or re.search(r"^[A-Za-z_-]+"):
+                    if not line.startswith("rule") and not line.startswith("def") and not re.search(r"^[A-Za-z_-]+"):
                         rule_content += line
                     else:
                         return rule_content
     return rule_content
 
 
 def markdown_source(code_item):
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/plugin.py` & `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO` & `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-snakemake-rule-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: MkDocs Plugin used to extrace rule information, to generate code and tables.
 Home-page: https://github.com/smeds/mkdocs-snakemake-rule-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
@@ -67,9 +66,7 @@
 ## Source 
 #SNAKEMAKE_RULE_SOURCE__fastp__fastp_pe#
 
 ## Parameters
 #SNAKEMAKE_RULE_TABLEE__fastp__fastp_pe#
 
 ```
-
-
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt` & `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/setup.py` & `mkdocs-snakemake-rule-plugin-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.0/versioneer.py` & `mkdocs-snakemake-rule-plugin-0.2.1/versioneer.py`

 * *Files identical despite different names*

