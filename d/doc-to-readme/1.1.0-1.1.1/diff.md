# Comparing `tmp/doc-to-readme-1.1.0.tar.gz` & `tmp/doc-to-readme-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-to-readme-1.1.0.tar", last modified: Sat Apr 29 10:17:44 2023, max compression
+gzip compressed data, was "doc-to-readme-1.1.1.tar", last modified: Wed May  3 13:26:37 2023, max compression
```

## Comparing `doc-to-readme-1.1.0.tar` & `doc-to-readme-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/update_readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/update_readme_github.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/How_to_setup_the_pipelines.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/bitbucket-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/access_token_info.png
--rw-r--r--   0 runner    (1001) docker     (123)    66748 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/cicd_variables.png
--rw-r--r--   0 runner    (1001) docker     (123)    91432 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/create_project_access_token_medium.png
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/project_access_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    71484 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/repo_variables.png
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/src/doc_to_md/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/src/doc_to_md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_md/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/src/doc_to_md/doc_to_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/templates/.update_readme_gitlab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/classes_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/functions_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.984373 doc-to-readme-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/.github/workflows/update_readme_github.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/How_to_setup_the_pipelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/images/access_token_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66748 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/images/cicd_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91432 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/images/create_project_access_token_medium.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/images/project_access_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71484 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/images/repo_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:26:37.984373 doc-to-readme-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/src/doc_to_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/src/doc_to_md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:26:37.000000 doc-to-readme-1.1.1/src/doc_to_md/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/src/doc_to_md/doc_to_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/src/doc_to_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-03 13:26:37.000000 doc-to-readme-1.1.1/src/doc_to_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 13:26:37.000000 doc-to-readme-1.1.1/src/doc_to_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:26:37.000000 doc-to-readme-1.1.1/src/doc_to_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:26:37.000000 doc-to-readme-1.1.1/src/doc_to_readme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/templates/.update_readme_gitlab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:26:37.980373 doc-to-readme-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/tests/classes_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/tests/functions_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-03 13:26:26.000000 doc-to-readme-1.1.1/tests/test.py
```

### Comparing `doc-to-readme-1.1.0/.github/workflows/publish.yml` & `doc-to-readme-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/.github/workflows/update_readme.yml` & `doc-to-readme-1.1.1/.github/workflows/update_readme.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/.github/workflows/update_readme_github.yml` & `doc-to-readme-1.1.1/.github/workflows/update_readme_github.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/.gitlab-ci.yml` & `doc-to-readme-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/How_to_setup_the_pipelines.md` & `doc-to-readme-1.1.1/How_to_setup_the_pipelines.md`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/LICENSE` & `doc-to-readme-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/PKG-INFO` & `doc-to-readme-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -77,15 +77,15 @@
 
 - **Command Line**
 ```shell
 python -m doc_to_md.doc_to_md -f "README.md" [-r ROOT_DIR] [-e EXCLUDE_MODULES] [-m SELECTED_MODULES] [--separated]
 
 -r ROOT_DIR             # Directory used as root for searching modules, defaults to folder containing README.md
 -e EXCLUDE_MODULES      # List of modules to be excluded
--s SELECTED_MODULES     # Only these modules will be included
+-m SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
@@ -99,17 +99,17 @@
 
 ## Functions & Classes  
 
 ### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes. |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
-| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
+| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through file, return dict with classes and functions. |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-29
+**Last Update:** 2023-05-03
```

### Comparing `doc-to-readme-1.1.0/README.md` & `doc-to-readme-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 - **Command Line**
 ```shell
 python -m doc_to_md.doc_to_md -f "README.md" [-r ROOT_DIR] [-e EXCLUDE_MODULES] [-m SELECTED_MODULES] [--separated]
 
 -r ROOT_DIR             # Directory used as root for searching modules, defaults to folder containing README.md
 -e EXCLUDE_MODULES      # List of modules to be excluded
--s SELECTED_MODULES     # Only these modules will be included
+-m SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
@@ -63,17 +63,17 @@
 
 ## Functions & Classes  
 
 ### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes. |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
-| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
+| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through file, return dict with classes and functions. |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-29
+**Last Update:** 2023-05-03
```

### Comparing `doc-to-readme-1.1.0/bitbucket-pipelines.yml` & `doc-to-readme-1.1.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/images/access_token_info.png` & `doc-to-readme-1.1.1/images/access_token_info.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/images/cicd_variables.png` & `doc-to-readme-1.1.1/images/cicd_variables.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/images/create_project_access_token_medium.png` & `doc-to-readme-1.1.1/images/create_project_access_token_medium.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/images/project_access_token.png` & `doc-to-readme-1.1.1/images/project_access_token.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/images/repo_variables.png` & `doc-to-readme-1.1.1/images/repo_variables.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/pyproject.toml` & `doc-to-readme-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/src/doc_to_md/doc_to_md.py` & `doc-to-readme-1.1.1/src/doc_to_md/doc_to_md.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def loop_through_repo(
         file: str,
         root_dir: str = None,
         exclude_modules: Optional[Tuple[str, ...]] = None,
         specified_modules: Optional[Tuple[str, ...]] = None
 ) -> None:
-    """Collect documentation from functions & classes
+    """Collect documentation from functions & classes.
 
     Loop through all .py modules in the root directory of this repo and add
     function & class info to a dictionary ('summary').
     To exclude modules, add their name to argument 'exclude_modules'.
 
     :param file: Path to markdown file
     :param root_dir: Path to root directory
@@ -148,15 +148,15 @@
         root_dir=root_dir,
         exclude_modules=exclude_modules,
         specified_modules=specified_modules)
     add_summary_to_md(summary, file, separate=separate)
 
 
 def parse_through_file(file: str) -> Dict[str, Dict[str, str]]:
-    """Parse through module and gather info on classes and functions
+    """Parse through file, return dict with classes and functions.
 
     :param file: Module path
     :returns: Dictionary containing information on classes and functions
     """
 
     with open(file) as fd:
         tree = ast.parse(fd.read())
@@ -167,30 +167,33 @@
         class_definitions = [node for node in tree.body if isinstance(node, ast.ClassDef)]
         method_names = {node.name: class_def.name for class_def in class_definitions
                         for node in class_def.body if isinstance(node, ast.FunctionDef)}
 
     with open(file, 'r') as f:
         functions = {}
         end = True
+        wrong_docu = (":", "Args:", "Returns:")
         for line in f.readlines():
             rm_blanks = line.strip()
             if rm_blanks.startswith("def "):
                 function_name = rm_blanks.split("def ")[1].split("(")[0]
                 if function_name.startswith("__"): continue
+                docu = func_docs.get(function_name)
                 functions[function_name] = {"fn": None,
-                                            "doc": func_docs.get(function_name),
+                                            "doc": docu if docu and not docu.startswith(wrong_docu) else None,
                                             "type": "method" if function_name in method_names else "function",
                                             "parent_class": method_names.get(function_name)}
                 functions[function_name]["fn"] = rm_blanks.split("def ")[1]
                 end = rm_blanks.endswith(":")
             elif rm_blanks.startswith("class "):
                 function_name = rm_blanks.split("class ")[1].split("(")[0].rstrip(":")
                 if function_name.startswith("__"): continue
+                docu = func_docs.get(function_name)
                 functions[function_name] = {"fn": None,
-                                            "doc": func_docs.get(function_name),
+                                            "doc": docu if docu and not docu.startswith(wrong_docu) else None,
                                             "type": "class",
                                             "parent_class": method_names.get(function_name)}
                 end = rm_blanks.endswith(":")
             elif not end:
                 rm_blanks = rm_blanks.split('"""')[0]
                 end = rm_blanks.endswith(":")
                 functions[function_name]["fn"] += rm_blanks
```

### Comparing `doc-to-readme-1.1.0/src/doc_to_readme.egg-info/PKG-INFO` & `doc-to-readme-1.1.1/src/doc_to_readme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -77,15 +77,15 @@
 
 - **Command Line**
 ```shell
 python -m doc_to_md.doc_to_md -f "README.md" [-r ROOT_DIR] [-e EXCLUDE_MODULES] [-m SELECTED_MODULES] [--separated]
 
 -r ROOT_DIR             # Directory used as root for searching modules, defaults to folder containing README.md
 -e EXCLUDE_MODULES      # List of modules to be excluded
--s SELECTED_MODULES     # Only these modules will be included
+-m SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
@@ -99,17 +99,17 @@
 
 ## Functions & Classes  
 
 ### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes. |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
-| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
+| function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through file, return dict with classes and functions. |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-29
+**Last Update:** 2023-05-03
```

### Comparing `doc-to-readme-1.1.0/src/doc_to_readme.egg-info/SOURCES.txt` & `doc-to-readme-1.1.1/src/doc_to_readme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/templates/.update_readme_gitlab.yml` & `doc-to-readme-1.1.1/templates/.update_readme_gitlab.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,24 @@
   SELECTED_MODULES: ""
   SEPARATED: "true"
 
 .push: &push |
   git status
   lines=$(git status -s | wc -l)
   if [ $lines -gt 0 ];then
-    git config --global user.name "${BOT_NAME}"
-    git config --global user.email "${BOT_EMAIL}"
     git add $PATH_TO_README
     git commit -m "${COMMIT_MESSAGE}"
-    git push -o ci.skip "https://${BOT_NAME}:${GIT_PUSH_TOKEN}@${CI_REPOSITORY_URL#*@}" $CI_COMMIT_BRANCH
   fi
+  git push -o ci.skip "https://${BOT_NAME}:${GIT_PUSH_TOKEN}@${CI_REPOSITORY_URL#*@}" $CI_COMMIT_BRANCH
 
 .exec: &exec |
   cmd="doc_to_md.py -f $PATH_TO_README"
-  if [[ ! -z $EXCLUDED_MODULES ]]; then
+  if [[ ! -z "$EXCLUDED_MODULES" ]]; then
     cmd="$cmd -e $EXCLUDED_MODULES"
-  elif [[ ! -z $SELECTED_MODULES ]]; then
+  elif [[ ! -z "$SELECTED_MODULES" ]]; then
     cmd="$cmd -m $SELECTED_MODULES"
   fi
   if [ ! -z $ROOT_DIR ]; then
     cmd="$cmd -r $ROOT_DIR"
   fi
   if [ $SEPARATED = "true" ]; then
     cmd="$cmd --separated"
@@ -37,16 +35,17 @@
   rm doc_to_md.py
 
 update_docu:
   image: alpine:latest
   before_script:
     - apk add bash git
     - apk add --no-cache python3
-    - git clone 'https://github.com/ziselsberger/doc_to_readme.git'
-    - git config --global pull.rebase false
+    - git config --global user.name "${BOT_NAME}"
+    - git config --global user.email "${BOT_EMAIL}"
     - git checkout $CI_COMMIT_BRANCH
-    - git pull
+    - git pull --ff
+    - git clone 'https://github.com/ziselsberger/doc_to_readme.git'
     - cp ./doc_to_readme/src/doc_to_md/doc_to_md.py .
     - rm -rf doc_to_readme
   script:
     - *exec
     - *push
```

### Comparing `doc-to-readme-1.1.0/tests/classes_for_testing.py` & `doc-to-readme-1.1.1/tests/classes_for_testing.py`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/tests/functions_for_testing.py` & `doc-to-readme-1.1.1/tests/functions_for_testing.py`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.1.0/tests/test.py` & `doc-to-readme-1.1.1/tests/test.py`

 * *Files identical despite different names*

