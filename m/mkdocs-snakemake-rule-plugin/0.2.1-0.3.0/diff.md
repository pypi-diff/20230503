# Comparing `tmp/mkdocs-snakemake-rule-plugin-0.2.1.tar.gz` & `tmp/mkdocs-snakemake-rule-plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.2.1.tar", last modified: Wed May  3 08:42:54 2023, max compression
+gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.3.0.tar", last modified: Wed May  3 09:37:32 2023, max compression
```

## Comparing `mkdocs-snakemake-rule-plugin-0.2.1.tar` & `mkdocs-snakemake-rule-plugin-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 08:42:54.000000 mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 08:42:54.948369 mkdocs-snakemake-rule-plugin-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-03 08:42:48.000000 mkdocs-snakemake-rule-plugin-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 09:37:32.000000 mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 09:37:32.688612 mkdocs-snakemake-rule-plugin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-03 09:37:24.000000 mkdocs-snakemake-rule-plugin-0.3.0/versioneer.py
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/LICENSE.md` & `mkdocs-snakemake-rule-plugin-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/PKG-INFO` & `mkdocs-snakemake-rule-plugin-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-snakemake-rule-plugin
-Version: 0.2.1
+Version: 0.3.0
 Summary: MkDocs Plugin used to extrace rule information, to generate code and tables.
 Home-page: https://github.com/smeds/mkdocs-snakemake-rule-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/README.md` & `mkdocs-snakemake-rule-plugin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/markdown.py` & `mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 def extract_snakemake_rule(file_path, rule):
     rule_content = ""
     with open(file_path, 'r') as reader:
         for line in reader:
             if line.startswith('rule') and rule in line:
                 rule_content += line
                 for line in reader:
-                    if not line.startswith("rule") and not line.startswith("def") and not re.search(r"^[A-Za-z_-]+"):
+                    # Stop when new rule, function or variable is found
+                    if not line.startswith("rule") and not line.startswith("def") and not re.search(r"^[A-Za-z_-]+", line):
                         rule_content += line
                     else:
                         return rule_content
     return rule_content
 
 
 def markdown_source(code_item):
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin/plugin.py` & `mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO` & `mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-snakemake-rule-plugin
-Version: 0.2.1
+Version: 0.3.0
 Summary: MkDocs Plugin used to extrace rule information, to generate code and tables.
 Home-page: https://github.com/smeds/mkdocs-snakemake-rule-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt` & `mkdocs-snakemake-rule-plugin-0.3.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/setup.py` & `mkdocs-snakemake-rule-plugin-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.2.1/versioneer.py` & `mkdocs-snakemake-rule-plugin-0.3.0/versioneer.py`

 * *Files identical despite different names*

