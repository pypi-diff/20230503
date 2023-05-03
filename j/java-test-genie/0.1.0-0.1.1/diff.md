# Comparing `tmp/java-test-genie-0.1.0.tar.gz` & `tmp/java-test-genie-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java-test-genie-0.1.0.tar", last modified: Thu Apr 27 12:08:13 2023, max compression
+gzip compressed data, was "java-test-genie-0.1.1.tar", last modified: Wed May  3 18:04:19 2023, max compression
```

## Comparing `java-test-genie-0.1.0.tar` & `java-test-genie-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,69 @@
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.085343 java-test-genie-0.1.0/
--rw-r--r--   0 boraelci   (501) staff       (20)     1066 2023-04-16 01:51:44.000000 java-test-genie-0.1.0/LICENSE
--rw-r--r--   0 boraelci   (501) staff       (20)      350 2023-04-16 01:55:32.000000 java-test-genie-0.1.0/MANIFEST.in
--rw-r--r--   0 boraelci   (501) staff       (20)     2560 2023-04-27 11:25:30.000000 java-test-genie-0.1.0/Makefile
--rw-r--r--   0 boraelci   (501) staff       (20)      285 2023-04-27 12:08:13.085168 java-test-genie-0.1.0/PKG-INFO
--rw-r--r--   0 boraelci   (501) staff       (20)     2125 2023-04-27 12:06:30.000000 java-test-genie-0.1.0/README.md
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.076716 java-test-genie-0.1.0/genie/
--rw-r--r--   0 boraelci   (501) staff       (20)       22 2023-04-27 05:28:04.000000 java-test-genie-0.1.0/genie/__init__.py
--rw-r--r--   0 boraelci   (501) staff       (20)     5140 2023-04-27 12:00:47.000000 java-test-genie-0.1.0/genie/main.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.077774 java-test-genie-0.1.0/genie/parsers/
--rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-04-27 12:00:47.000000 java-test-genie-0.1.0/genie/parsers/ClassParser.py
--rw-r--r--   0 boraelci   (501) staff       (20)     1688 2023-04-27 07:01:34.000000 java-test-genie-0.1.0/genie/parsers/ConfigParser.py
--rw-r--r--   0 boraelci   (501) staff       (20)    11237 2023-04-27 05:28:04.000000 java-test-genie-0.1.0/genie/parsers/TestParser.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.082180 java-test-genie-0.1.0/genie/resources/
--rw-r--r--   0 boraelci   (501) staff       (20)     7356 2023-04-27 07:30:28.000000 java-test-genie-0.1.0/genie/resources/gpt_response_for_parsed.json
--rw-r--r--   0 boraelci   (501) staff       (20)     3642 2023-04-27 07:49:35.000000 java-test-genie-0.1.0/genie/resources/gpt_response_for_parsed_broken.json
--rw-r--r--   0 boraelci   (501) staff       (20)     4493 2023-04-27 10:49:22.000000 java-test-genie-0.1.0/genie/resources/gpt_response_for_raw.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      870 2023-04-27 07:15:06.000000 java-test-genie-0.1.0/genie/resources/gpt_system_prompt_parsed.txt
--rw-r--r--   0 boraelci   (501) staff       (20)      442 2023-04-27 09:55:59.000000 java-test-genie-0.1.0/genie/resources/gpt_system_prompt_raw.txt
--rwxr-xr-x   0 boraelci   (501) staff       (20)   322200 2023-04-01 00:09:20.000000 java-test-genie-0.1.0/genie/resources/java-grammar.so
--rwxr-xr-x   0 boraelci   (501) staff       (20)   496550 2023-04-20 17:59:44.000000 java-test-genie-0.1.0/genie/resources/libtree-sitter-java.dylib
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.083735 java-test-genie-0.1.0/genie/wrappers/
--rw-r--r--   0 boraelci   (501) staff       (20)      989 2023-04-27 12:00:47.000000 java-test-genie-0.1.0/genie/wrappers/GptWrapper.py
-drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-04-27 12:08:13.084888 java-test-genie-0.1.0/java_test_genie.egg-info/
--rw-r--r--   0 boraelci   (501) staff       (20)      285 2023-04-27 12:08:13.000000 java-test-genie-0.1.0/java_test_genie.egg-info/PKG-INFO
--rw-r--r--   0 boraelci   (501) staff       (20)      707 2023-04-27 12:08:13.000000 java-test-genie-0.1.0/java_test_genie.egg-info/SOURCES.txt
--rw-r--r--   0 boraelci   (501) staff       (20)        1 2023-04-27 12:08:13.000000 java-test-genie-0.1.0/java_test_genie.egg-info/dependency_links.txt
--rw-r--r--   0 boraelci   (501) staff       (20)       43 2023-04-27 12:08:13.000000 java-test-genie-0.1.0/java_test_genie.egg-info/entry_points.txt
--rw-r--r--   0 boraelci   (501) staff       (20)        6 2023-04-27 12:08:13.000000 java-test-genie-0.1.0/java_test_genie.egg-info/top_level.txt
--rw-r--r--   0 boraelci   (501) staff       (20)     2214 2023-04-27 11:39:55.000000 java-test-genie-0.1.0/pyproject.toml
--rw-r--r--   0 boraelci   (501) staff       (20)       38 2023-04-27 12:08:13.085408 java-test-genie-0.1.0/setup.cfg
--rw-r--r--   0 boraelci   (501) staff       (20)      450 2023-04-27 11:39:06.000000 java-test-genie-0.1.0/setup.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.642155 java-test-genie-0.1.1/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1066 2023-04-16 01:51:44.000000 java-test-genie-0.1.1/LICENSE
+-rw-r--r--   0 boraelci   (501) staff       (20)      350 2023-04-16 01:55:32.000000 java-test-genie-0.1.1/MANIFEST.in
+-rw-r--r--   0 boraelci   (501) staff       (20)     2560 2023-04-27 11:25:30.000000 java-test-genie-0.1.1/Makefile
+-rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-05-03 18:04:19.641988 java-test-genie-0.1.1/PKG-INFO
+-rw-r--r--   0 boraelci   (501) staff       (20)     2327 2023-05-03 17:50:35.000000 java-test-genie-0.1.1/README.md
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.619947 java-test-genie-0.1.1/evaluation/
+-rw-r--r--   0 boraelci   (501) staff       (20)     4105 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/evaluation/evaluate.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.621007 java-test-genie-0.1.1/evaluation/resources/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1123 2023-04-30 10:32:29.000000 java-test-genie-0.1.1/evaluation/resources/gpt_pred.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      466 2023-04-30 11:22:22.000000 java-test-genie-0.1.1/evaluation/resources/gpt_system_prompt_evaluation.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.618079 java-test-genie-0.1.1/evaluation/results/
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.622048 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2044 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1987 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 13:08:30.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    54823 2023-04-30 13:03:15.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.623427 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2041 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1985 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 13:08:59.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    51477 2023-04-30 13:03:49.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t0.5/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.624739 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2034 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:38:13.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    54938 2023-04-30 12:37:20.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s100-t1/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.626348 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/
+-rw-r--r--   0 boraelci   (501) staff       (20)    20266 2023-04-30 17:42:13.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    19805 2023-04-30 17:31:33.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      119 2023-04-30 17:41:54.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)   426119 2023-04-30 17:31:33.000000 java-test-genie-0.1.1/evaluation/results/gpt3.5-s1000-t0/tests.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.629129 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2049 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/bleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     1979 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/codebleus.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      120 2023-04-30 12:53:55.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/summary.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)    55264 2023-04-30 12:51:30.000000 java-test-genie-0.1.1/evaluation/results/gpt4-s100-t1/tests.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)   158769 2023-04-30 18:28:38.000000 java-test-genie-0.1.1/evaluation/visualizations.ipynb
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.629665 java-test-genie-0.1.1/genie/
+-rw-r--r--   0 boraelci   (501) staff       (20)       22 2023-05-03 17:51:18.000000 java-test-genie-0.1.1/genie/__init__.py
+-rw-r--r--   0 boraelci   (501) staff       (20)     5766 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/main.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.630438 java-test-genie-0.1.1/genie/parsers/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-04-27 12:00:47.000000 java-test-genie-0.1.1/genie/parsers/ClassParser.py
+-rw-r--r--   0 boraelci   (501) staff       (20)     2299 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/parsers/ConfigParser.py
+-rw-r--r--   0 boraelci   (501) staff       (20)    11237 2023-04-27 05:28:04.000000 java-test-genie-0.1.1/genie/parsers/TestParser.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.633582 java-test-genie-0.1.1/genie/resources/
+-rw-r--r--   0 boraelci   (501) staff       (20)     7356 2023-04-27 07:30:28.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed.json
+-rw-r--r--   0 boraelci   (501) staff       (20)     3642 2023-04-27 07:49:35.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed_broken.json
+-rw-r--r--   0 boraelci   (501) staff       (20)     4493 2023-05-03 17:40:57.000000 java-test-genie-0.1.1/genie/resources/gpt_response_for_raw.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      870 2023-04-27 07:15:06.000000 java-test-genie-0.1.1/genie/resources/gpt_system_prompt_parsed.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)      493 2023-05-03 17:26:50.000000 java-test-genie-0.1.1/genie/resources/gpt_system_prompt_raw.txt
+-rwxr-xr-x   0 boraelci   (501) staff       (20)   322200 2023-04-01 00:09:20.000000 java-test-genie-0.1.1/genie/resources/java-grammar.so
+-rwxr-xr-x   0 boraelci   (501) staff       (20)   496550 2023-04-20 17:59:44.000000 java-test-genie-0.1.1/genie/resources/libtree-sitter-java.dylib
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.634897 java-test-genie-0.1.1/genie/wrappers/
+-rw-r--r--   0 boraelci   (501) staff       (20)     1138 2023-05-03 17:42:55.000000 java-test-genie-0.1.1/genie/wrappers/GptWrapper.py
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.635968 java-test-genie-0.1.1/java_test_genie.egg-info/
+-rw-r--r--   0 boraelci   (501) staff       (20)     2645 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/PKG-INFO
+-rw-r--r--   0 boraelci   (501) staff       (20)     1934 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/SOURCES.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)        1 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/dependency_links.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)       43 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/entry_points.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)        6 2023-05-03 18:04:19.000000 java-test-genie-0.1.1/java_test_genie.egg-info/top_level.txt
+drwxr-xr-x   0 boraelci   (501) staff       (20)        0 2023-05-03 18:04:19.641635 java-test-genie-0.1.1/milestones/
+-rw-r--r--   0 boraelci   (501) staff       (20)  1820165 2023-05-03 17:45:22.000000 java-test-genie-0.1.1/milestones/Final Report - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)    91567 2023-05-01 10:32:57.000000 java-test-genie-0.1.1/milestones/Project Progress Report - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)    97124 2023-05-01 10:33:08.000000 java-test-genie-0.1.1/milestones/Revised Project Proposal - Bora Elci.pdf
+-rw-r--r--   0 boraelci   (501) staff       (20)      100 2023-05-01 10:33:52.000000 java-test-genie-0.1.1/milestones/Slides link.txt
+-rw-r--r--   0 boraelci   (501) staff       (20)     2214 2023-05-03 18:01:02.000000 java-test-genie-0.1.1/pyproject.toml
+-rw-r--r--   0 boraelci   (501) staff       (20)       38 2023-05-03 18:04:19.642205 java-test-genie-0.1.1/setup.cfg
+-rw-r--r--   0 boraelci   (501) staff       (20)      659 2023-05-03 18:01:43.000000 java-test-genie-0.1.1/setup.py
```

### Comparing `java-test-genie-0.1.0/LICENSE` & `java-test-genie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/Makefile` & `java-test-genie-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/README.md` & `java-test-genie-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+Metadata-Version: 2.1
+Name: java-test-genie
+Version: 0.1.1
+Summary: AI-Driven Unit Test Generation for Java
+Home-page: https://github.com/boraelci/java-test-genie
+Author: Bora Elci
+Author-email: bora.elci@columbia.edu
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JavaTestGenie
+![MIT License](https://img.shields.io/github/license/boraelci/review-master)
+[![PyPI](https://img.shields.io/pypi/v/java-test-genie)](https://pypi.org/project/java-test-genie/)
 
 ## Installation
 
 ```bash
-pip3 install java-test-genie
+pip install java-test-genie
 ```
 
 ## Usage
 
-Set your OpenAI API key with `export OPENAI_API_KEY=<API-KEY-HERE>`. You can obtain it at https://platform.openai.com/account/api-keys
+Before running `genie`, set your OpenAI API key with `export OPENAI_API_KEY=<API-KEY-HERE>`. You can obtain it at https://platform.openai.com/account/api-keys
 
 Ensure that you are in a at the same level with `src/` when running the tool.
 
 You need to create a config file named `.genie.json` within your java repository. This file should be at the same level with `src/` as well as where you will run `genie`. In this file, you can specify which directories & files to include and exclude. The example below includes the `service/` directory but excludes `service/interface`. Similarly, you can specify file names.
 
 ```json
 {
@@ -47,19 +61,21 @@
 
 `git clone https://github.com/boraelci/kaiserschmarrn.git`
 
 ## Grammar
 
 Parsing Java files with the Tree-sitter library requires grammar files. They were obtained in the following way for this tool.
 
-### For Mac
+### For macOS
 
 ```bash
 git clone https://github.com/tree-sitter/tree-sitter-java.git
 cd tree-sitter-java
 tree-sitter generate
 gcc -shared -o libtree-sitter-java.dylib -Isrc src/parser.c
 ```
 
 ### For Windows
 
 Used the one provided as [`java-grammar.so`](https://github.com/microsoft/methods2test/blob/main/scripts/java-grammar.so)
+
+
```

### Comparing `java-test-genie-0.1.0/genie/main.py` & `java-test-genie-0.1.1/genie/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 #!/usr/bin/env python
 
 import argparse
 import json
-import platform
 import os
+import platform
+import re
 import sys
 
 from genie.parsers.ClassParser import ClassParser
 from genie.parsers.ConfigParser import ConfigParser
 from genie.wrappers.GptWrapper import GptWrapper
 
 SINGLE_FILE = False
 SINGLE_FILE_NAME = "AssetService.java"
-LOCAL_RESPONSE = False
+LOCAL_RESPONSE = True
 
 
 def save_test(repo_test_path, test_content):
     repo_test_dir = os.path.dirname(repo_test_path)
     os.makedirs(repo_test_dir, exist_ok=True)
     with open(repo_test_path, "w") as f:
         f.write(test_content)
-    print(f"Saved")
+    print(f"Saved tests to {repo_test_path}")
 
 
 def gpt_raw_classes(genie_dir, repo_dir, selected_class_paths):
     gpt_system_prompt_path = f"{genie_dir}/resources/gpt_system_prompt_raw.txt"
     gpt = GptWrapper(gpt_system_prompt_path)
     for class_path in selected_class_paths:
         class_name_java = class_path.split("/")[-1]
         class_name = class_name_java.replace(".java", "")
         if SINGLE_FILE is True and class_name_java != SINGLE_FILE_NAME:
             continue
 
-        print(f"Generating tests for {class_name_java}")
+        print(f"\nGenerating tests for {class_name_java}...")
         if LOCAL_RESPONSE is True:
             with open(f"{genie_dir}/resources/gpt_response_for_raw.txt", "r") as f:
                 response = f.read()
         else:
             with open(class_path, "r") as f:
                 content = f.read()
-            response = gpt.query(content)
+            try:
+                response = gpt.query(content)
+                print(f"Succesfully generated tests for {class_name_java}")
+            except Exception as e:
+                print(e)
+                print(f"Failed to generate tests for {class_name_java}")
+                continue
 
+        response = re.sub(r"^```$\n?", "", response, flags=re.MULTILINE)
         test_name = class_name + "Test"
         test_path = class_path.replace('src/main', 'src/test')
         test_path = test_path.replace(f"{class_name}.java", f"{test_name}.java")
         repo_test_path = f"{repo_dir}/{test_path}"
 
         test_content = response
         # print(test_content)
@@ -53,16 +61,14 @@
             if user_input.lower() == "y":
                 save_test(repo_test_path, test_content)
             else:
                 print(f"Discarded")
         else:
             save_test(repo_test_path, test_content)
 
-        break
-
 
 def gpt_parsed_classes(genie_dir, repo_dir, tmp_repo_out_dir):
     gpt_system_prompt_path = f"{genie_dir}/resources/gpt_system_prompt_parsed.txt"
     gpt = GptWrapper(gpt_system_prompt_path)
     os.chdir(tmp_repo_out_dir)
     for filename in os.listdir():
         if SINGLE_FILE is True and filename != SINGLE_FILE_NAME:
@@ -98,33 +104,40 @@
             if user_input.lower() == "y":
                 save_test(repo_test_path, test_content)
             else:
                 print(f"Discarded")
         else:
             save_test(repo_test_path, test_content)
 
-        # print(response)
-        break
-
 
 def main():
     # args = parse_args()
     repo_dir = os.getcwd()
     repo_name = repo_dir.split("/")[-1]
     if repo_name == "java-test-genie":  # For quick local testing during early development
         repo_dir = "/Users/boraelci/Desktop/ASE/kaiserschmarrn"
         repo_name = repo_dir.split("/")[-1]
         os.chdir(repo_dir)
     config_path = f"{repo_dir}/.genie.json"
+
+    # Check config file exists
+    if not os.path.exists(config_path):
+        print(
+            f"Error: .genie.json file cannot be found at {config_path}; follow instructions in our README to create one"
+        )
+        sys.exit(1)
     config_parser = ConfigParser(config_path)
+
+    # Check directory is correct
     if "src" not in os.listdir():
         print("Error: src folder cannot be found in the current directory")
         sys.exit(1)
     genie_dir = os.path.dirname(os.path.realpath(__file__))
 
+    # Select grammar file depending on OS
     os_system = platform.system()
     if os_system == "Darwin":
         grammar_file = f"{genie_dir}/resources/libtree-sitter-java.dylib"
     else:
         grammar_file = f"{genie_dir}/resources/java-grammar.so"
 
     tmp_repo_out_dir = f"tmp/output/{repo_name}"
```

### Comparing `java-test-genie-0.1.0/genie/parsers/ClassParser.py` & `java-test-genie-0.1.1/genie/parsers/ClassParser.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/parsers/ConfigParser.py` & `java-test-genie-0.1.1/genie/parsers/ConfigParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import os
 
 
 class ConfigParser:
     def __init__(self, config_path):
         # Load the JSON file
         with open(config_path) as f:
             self.config = json.load(f)
@@ -14,34 +15,45 @@
             parent_dir = item['parent_dir']
 
             # Check for matching files in file_names
             for file_name in item['file_names']:
                 file_path = f"{parent_dir}/{file_name}"
                 if file_path in focals:
                     filtered_files.append(file_path)
+                else:
+                    print(f"Error: file to include cannot be found at {file_path}")
+                    continue
 
             # Check for matching files in dir_names
             for dir_name in item['dir_names']:
                 dir_path = f"{parent_dir}/{dir_name}"
+                if not os.path.exists(dir_path):
+                    print(f"Error: directory to include cannot be found at {dir_path}")
+                    continue
                 for focal in focals:
                     if focal.startswith(dir_path):
                         filtered_files.append(focal)
 
         # Exclude files and directories specified in the exclude section
         for item in self.config['exclude']:
             parent_dir = item['parent_dir']
 
             # Exclude files in file_names
             for file_name in item['file_names']:
                 file_path = f"{parent_dir}/{file_name}"
                 if file_path in filtered_files:
                     filtered_files.remove(file_path)
+                else:
+                    print(f"Error: file to exclude cannot be found at {file_path}")
+                    continue
 
             # Exclude files in dir_names
             for dir_name in item['dir_names']:
                 dir_path = f"{parent_dir}/{dir_name}"
+                if not os.path.exists(dir_path):
+                    print(f"Error: directory to include cannot be found at {dir_path}")
+                    continue
                 filtered_files = [focal for focal in filtered_files if not focal.startswith(dir_path)]
 
         # Remove duplicates
         filtered_files = list(set(filtered_files))
-
         return filtered_files
```

### Comparing `java-test-genie-0.1.0/genie/parsers/TestParser.py` & `java-test-genie-0.1.1/genie/parsers/TestParser.py`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/gpt_response_for_parsed.json` & `java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed.json`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/gpt_response_for_parsed_broken.json` & `java-test-genie-0.1.1/genie/resources/gpt_response_for_parsed_broken.json`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/gpt_response_for_raw.txt` & `java-test-genie-0.1.1/genie/resources/gpt_response_for_raw.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/gpt_system_prompt_parsed.txt` & `java-test-genie-0.1.1/genie/resources/gpt_system_prompt_parsed.txt`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/java-grammar.so` & `java-test-genie-0.1.1/genie/resources/java-grammar.so`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/resources/libtree-sitter-java.dylib` & `java-test-genie-0.1.1/genie/resources/libtree-sitter-java.dylib`

 * *Files identical despite different names*

### Comparing `java-test-genie-0.1.0/genie/wrappers/GptWrapper.py` & `java-test-genie-0.1.1/genie/wrappers/GptWrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 class GptWrapper:
     def __init__(self, system_prompt_path):
         with open(system_prompt_path, "r") as f:
             self.system_prompt = f.read()
 
     def query(self, message):
         openai.api_key = os.environ["OPENAI_API_KEY"]
-        # model = "gpt-4-0314"
-        model = "gpt-3.5-turbo-0301"
+        # model = "gpt-4"
+        model = "gpt-3.5-turbo"
+        temperature = 0
         input_token_count = self.get_input_token_count(model, message)
+        if input_token_count > 3900:
+            raise Exception("Error: this file is too large")
         max_tokens = min(2048, 3900 - input_token_count)
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "system", "content": self.system_prompt},
                 {"role": "user", "content": message},
             ],
             max_tokens=max_tokens,
+            temperature=temperature,
         )
         content = response["choices"][0]["message"]["content"]
         return content
 
     def get_input_token_count(self, model, input):
         encoding = tiktoken.encoding_for_model(model)
         return len(encoding.encode(input))
```

### Comparing `java-test-genie-0.1.0/pyproject.toml` & `java-test-genie-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "java-test-genie"
 authors = [{name = "Bora Elci", email = "bora.elci@columbia.edu"}]
 description="AI-Driven Unit Test Generation for Java"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "openai",
     "tiktoken",
     "tree-sitter"
 ]
```

