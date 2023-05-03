# Comparing `tmp/yellowdog-python-examples-5.0.5.tar.gz` & `tmp/yellowdog-python-examples-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.5.tar", last modified: Tue Apr 18 12:14:44 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-5.0.6.tar", last modified: Wed May  3 10:28:18 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.5.tar` & `yellowdog-python-examples-5.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.358337 yellowdog-python-examples-5.0.5/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.5/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-18 12:14:44.358406 yellowdog-python-examples-5.0.5/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.5/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109332 2023-04-18 11:54:44.000000 yellowdog-python-examples-5.0.5/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.5/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.5/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-18 12:14:44.358706 yellowdog-python-examples-5.0.5/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.357434 yellowdog-python-examples-5.0.5/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-18 12:14:05.000000 yellowdog-python-examples-5.0.5/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.5/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.5/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.5/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.5/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.5/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.5/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.5/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.5/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.5/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40102 2023-04-18 12:14:05.000000 yellowdog-python-examples-5.0.5/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.5/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.5/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.5/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.5/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.5/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.5/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.5/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.5/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.358233 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.927729 yellowdog-python-examples-5.0.6/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.6/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-03 10:28:18.927791 yellowdog-python-examples-5.0.6/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.6/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109989 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.6/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.6/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-05-03 10:28:18.928081 yellowdog-python-examples-5.0.6/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.926862 yellowdog-python-examples-5.0.6/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.6/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.6/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.6/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18351 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5544 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3749 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.6/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40102 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.6/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.6/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.927618 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.5/LICENSE` & `yellowdog-python-examples-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/PKG-INFO` & `yellowdog-python-examples-5.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.5
+Version: 5.0.6
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.5/PYPI_README.md` & `yellowdog-python-examples-5.0.6/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/README.md` & `yellowdog-python-examples-5.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,20 @@
 
 <!--te-->
 
 # Overview
 
 This repository contains a set of example Python scripts for interacting with the YellowDog Platform. The scripts use the **[YellowDog Python SDK](https://docs.yellowdog.co/api/python/index.html)**, the code for which can be found [on GitHub](https://github.com/yellowdog/yellowdog-sdk-python-public).
 
+
+*(Note: these scripts are intended to be a helpful starting point for experimenting with the YellowDog Platform. They are not assured to be of production quality nor do they represent a standard or recommended method for using YellowDog.)*
+
 This documentation should be read in conjunction with the main **[YellowDog Documentation](https://docs.yellowdog.co)**, which provides a comprehensive description of the concepts and operation of the YellowDog Platform.
 
-The scripts are intended to be helpful starting points for experimenting with the YellowDog Platform. They are not assured to be of production quality nor to represent a standard or recommended method for using YellowDog.
+Template solutions for experimenting with these scripts can be found in the **[python-examples-templates](https://github.com/yellowdog/python-examples-templates)** repository.
 
 The scripts provide the following capabilities:
 
 - **Provisioning** Worker Pools with the **`yd-provision`** command
 - **Submitting** Work Requirements with the **`yd-submit`** command
 - **Uploading** files to the YellowDog Object Store with the **`yd-upload`** command
 - **Instantiating** Compute Requirements with the **`yd-instantiate`** command
@@ -744,41 +747,44 @@
 
 ## Variable Substitutions in Work Requirement Properties
 
 Variable substitutions can be used within any property value in TOML configuration files or Work Requirement JSON files. See the description [above](#variable-substitutions) for more details on variable substitutions. This is a powerful feature that allows Work Requirements to be parameterised by supplying values on the command line, via environment variables or via the TOML file.
 
 ### Task and Task Group Name Substitution
 
-The following numbering and naming substitutions are available for use in Task and Task Group naming, i.e., they can be used in the `name` properties for Tasks and Task Groups respectively in JSON Work Requirements. Note that Task Group names cannot use the `{{task_number}}` directive.
+The following numbering and naming substitutions are available for use in Task and Task Group naming, only when the Work Requirement is specified as  JSON document, i.e., they can be used in the `name` properties for Tasks and Task Groups in JSON specifications.
 
-**Tasks** can also use any of the substitutions in any of their properties.
+The following table defines the context(s) in which each variable can be used:
 
 | Directive               | Description                                       | Task | Task Group |
 |:------------------------|:--------------------------------------------------|:-----|:-----------|
 | `{{task_number}}`       | The current Task number                           | Yes  |            |
 | `{{task_name}}`         | The current Task name                             | Yes  |            |
 | `{{task_group_name}}`   | The current Task Group name                       | Yes  |            |
 | `{{task_count}}`        | The number of Tasks in the current Task Group     | Yes  | Yes        |
 | `{{task_group_number}}` | The current Task Group number                     | Yes  | Yes        |
 | `{{task_group_count}}`  | The number of Task Groups in the Work Requirement | Yes  | Yes        |
 
-Numbers are zero-padded for neat formatting and sorting, e.g., Task number 37 of 1000 Tasks would be substituted as `0037`.
+In addition, **Tasks** defined in JSON documents can use any of the substitutions above in any of their properties, not just `name`.
+
+Numbers are zero-padded for neat formatting and sorting, e.g., Task number `37` of `1000` Tasks would be substituted as `0037`.
 
 As an example, the following JSON Work Requirement:
 
 ```json
 {
   "taskGroups": [
     {
       "name": "my_task_group_{{task_group_number}}_a1",
       "executable": "ex1.sh",
       "taskCount": 2,
       "tasks": [
         {
-          "name": "my_task_{{task_number}}-of-{{task_count}}"
+          "name": "my_task_{{task_number}}-of-{{task_count}}",
+          "environment": {"TASK_NUMBER": "{{task_number}}"}
         }
       ]
     },
     {
       "name": "my_task_group_{{task_group_number}}_b1",
       "executable": "ex2.sh",
       "taskCount": 2,
@@ -1306,14 +1312,15 @@
 | `nodeBootTimeLimit`        | The time in minutes allowed for a node to boot and register with the platform before it is terminated.                          | `10.0`    |
 | `nodeIdleGracePeriod`      | The time in minutes after a node registers during which the idle check is not applied.                                          | `2.0`     |
 | `nodeIdleTimeLimit`        | The time in minutes for which a node can be idle before it can be shut down by auto-scaling.                                    | `5.0`     |
 | `targetInstanceCount`      | The initial number of nodes to create for the Worker Pool.                                                                      | `1`       |
 | `templateId`               | The YellowDog Compute Template ID to use for provisioning.                                                                      |           |
 | `userData`                 | User Data to be supplied to instances on boot.                                                                                  |           |
 | `userDataFile`             | As above, but read the User Data from the filename supplied in this property.                                                   |           |
+| `userDataFiles`            | As above, but create the User Data by concatenating the contents of a list of filenames supplied in this property.              |           |
 | `workersPerVCPU`           | The number of Workers to establish per vCPU on each node in the Worker Pool. (Overrides `workersPerNode`.)                      |           |
 | `workersPerNode`           | The number of Workers to establish on each node in the Worker Pool.                                                             | `1`       |
 | `workerPoolData`           | The name of a file containing a JSON document defining a Worker Pool.                                                           |           |
 | `workerTag`                | The Worker Tag to publish for the all of the Workers.                                                                           |           |
 
 ## Automatic Properties
 
@@ -1338,17 +1345,18 @@
     minNodes = 1
     name = "my-worker-pool"
     nodeBootTimeLimit = 5
     nodeIdleGracePeriod = 5
     nodeIdleTimeLimit = 3
     targetInstanceCount = 1
     templateId = "ydid:crt:D9C548:465a107c-7cea-46e3-9fdd-15116cb92c40"
-    # Note: only one of 'userData'/'userDataFile' should be set
+    # Note: only one of 'userData'/'userDataFile'/'userDataFiles' should be set
     userData = ""
     userDataFile = "myuserdata.txt"
+    userDataFiles = ["myuserdata1.txt", "myuserdata2.txt"]
     workerTag = "tag-{{username}}"
     workersPerNode = 1
 #   workerPoolData = "worker_pool.json"
 ```
 
 ## Worker Pool Specification Using JSON Documents
 
@@ -1497,14 +1505,16 @@
 - `instanceTags`
 - `requirementName`: derived from the `name` property in the `TOML` configuration. (The name will be generated automatically if not supplied in either the TOML file or the JSON specification.)
 - `requirementNamespace`: derived from the `namespace` property in the `TOML` configuration
 - `requirementTag`: : derived from the `tag` property in the `TOML` configuration
 - `targetInstanceCount`
 - `templateId`
 - `userData`
+- `userDataFile`
+- `userDataFiles`
 
 **Properties Inherited within the `provisionedProperties` Property**
 
 - `autoShutdown`
 - `autoShutdownConditions`: derived from the `autoShutdownDelay`, `ascAllNodesInactive`, `ascAllWorkersReleased`, `ascNodeActionFailed`, `ascUnclaimedAfterStartup` and `ascNoRegisteredWorkers` properties in the `TOML` configuration
 - `nodeBootTimeLimit`
 - `nodeIdleGracePeriod`
```

### Comparing `yellowdog-python-examples-5.0.5/pyproject.toml` & `yellowdog-python-examples-5.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/setup.cfg` & `yellowdog-python-examples-5.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/abort.py` & `yellowdog-python-examples-5.0.6/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/admin.py` & `yellowdog-python-examples-5.0.6/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/args.py` & `yellowdog-python-examples-5.0.6/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/cancel.py` & `yellowdog-python-examples-5.0.6/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/check_imports.py` & `yellowdog-python-examples-5.0.6/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/compact_json.py` & `yellowdog-python-examples-5.0.6/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/config.py` & `yellowdog-python-examples-5.0.6/yd_commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     node_boot_time_limit: float = 10
     node_idle_grace_period: float = 2
     node_idle_time_limit: float = 5
     target_instance_count: int = 0
     template_id: Optional[str] = None
     user_data: Optional[str] = None
     user_data_file: Optional[str] = None
+    user_data_files: Optional[List[str]] = None
     worker_pool_data_file: Optional[str] = None
     worker_tag: Optional[str] = None
     workers_per_vcpu: Optional[int] = None
     workers_per_node: int = 1
 
 
 # CLI > YD_CONF > 'config.toml'
@@ -405,14 +406,15 @@
             node_idle_time_limit=wp_section.get(
                 NODE_IDLE_TIME_LIMIT, wp_section.get(AUTO_SCALING_IDLE_DELAY, 5)
             ),
             target_instance_count=wp_section.get(TARGET_INSTANCE_COUNT, 1),
             template_id=wp_section.get(TEMPLATE_ID, None),
             user_data=wp_section.get(USERDATA, None),
             user_data_file=wp_section.get(USERDATAFILE, None),
+            user_data_files=wp_section.get(USERDATAFILES, None),
             worker_pool_data_file=worker_pool_data_file,
             worker_tag=worker_tag,
             workers_per_vcpu=wp_section.get(WORKERS_PER_VCPU, None),
             workers_per_node=wp_section.get(WORKERS_PER_NODE, 1),
         )
 
     except KeyError as e:
```

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/config_keys.py` & `yellowdog-python-examples-5.0.6/yd_commands/config_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 TEMPLATE_ID = "templateId"  # String
 UPLOAD_FILES = "uploadFiles"  # List of Dicts
 LOCAL_PATH = "localPath"  # String
 UPLOAD_PATH = "uploadPath"  # String
 URL = "url"  # String
 USERDATA = "userData"  # String
 USERDATAFILE = "userDataFile"  # String
+USERDATAFILES = "userDataFiles"  # List of Strings
 VARIABLES = "variables"  # Dictionary
 VCPUS = "vcpus"  # List of two Floats
 VERIFY_AT_START = "verifyAtStart"  # List of Strings
 VERIFY_WAIT = "verifyWait"  # List of Strings
 WORKERS_PER_VCPU = "workersPerVCPU"  # Integer
 WORKERS_PER_NODE = "workersPerNode"  # Integer
 WORKER_POOL_SECTION = "workerPool"  # No value
@@ -161,14 +162,15 @@
     TEMPLATE_ID,
     UPLOAD_FILES,
     LOCAL_PATH,
     UPLOAD_PATH,
     URL,
     USERDATA,
     USERDATAFILE,
+    USERDATAFILES,
     VARIABLES,
     VCPUS,
     VERIFY_AT_START,
     VERIFY_WAIT,
     WORKERS_PER_VCPU,
     WORKERS_PER_NODE,
     WORKER_POOL_SECTION,
```

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/csv_data.py` & `yellowdog-python-examples-5.0.6/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/delete.py` & `yellowdog-python-examples-5.0.6/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/download.py` & `yellowdog-python-examples-5.0.6/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/instantiate.py` & `yellowdog-python-examples-5.0.6/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/interactive.py` & `yellowdog-python-examples-5.0.6/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-5.0.6/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/list.py` & `yellowdog-python-examples-5.0.6/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/object_utilities.py` & `yellowdog-python-examples-5.0.6/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/printing.py` & `yellowdog-python-examples-5.0.6/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/provision.py` & `yellowdog-python-examples-5.0.6/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/reformat_json.py` & `yellowdog-python-examples-5.0.6/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/shutdown.py` & `yellowdog-python-examples-5.0.6/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/submit.py` & `yellowdog-python-examples-5.0.6/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/submit_utils.py` & `yellowdog-python-examples-5.0.6/yd_commands/submit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,9 +179,9 @@
     Format a string to be consistent with YellowDog naming requirements.
     """
     # Make obvious substitutions
     yd_name = yd_name.replace("/", "-").replace(" ", "_").lower()
     # Enforce acceptable regex and name length
     yd_name = re.sub("[^a-z0-9_-]", "", yd_name)
     if not yd_name[0].isalpha():
-        yd_name = f"z_{yd_name}"
+        yd_name = f"yd_{yd_name}"
     return yd_name[:60]
```

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/terminate.py` & `yellowdog-python-examples-5.0.6/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/type_check.py` & `yellowdog-python-examples-5.0.6/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/upload.py` & `yellowdog-python-examples-5.0.6/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/upload_utils.py` & `yellowdog-python-examples-5.0.6/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/validate_properties.py` & `yellowdog-python-examples-5.0.6/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/variables.py` & `yellowdog-python-examples-5.0.6/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/version.py` & `yellowdog-python-examples-5.0.6/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yd_commands/wrapper.py` & `yellowdog-python-examples-5.0.6/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.5
+Version: 5.0.6
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

