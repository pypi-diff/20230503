# Comparing `tmp/trubrics-1.3.5.tar.gz` & `tmp/trubrics-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.3.5.tar", last modified: Tue Apr 25 12:42:39 2023, max compression
+gzip compressed data, was "trubrics-1.3.6.tar", last modified: Wed May  3 06:41:48 2023, max compression
```

## Comparing `trubrics-1.3.5.tar` & `trubrics-1.3.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-25 12:42:28.000000 trubrics-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-25 12:42:39.696141 trubrics-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-25 12:42:28.000000 trubrics-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 12:42:28.000000 trubrics-1.3.5/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-25 12:42:28.000000 trubrics-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 12:42:28.000000 trubrics-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-25 12:42:39.696141 trubrics-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-25 12:42:28.000000 trubrics-1.3.5/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/feedback/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.692141 trubrics-1.3.5/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/ui/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.696141 trubrics-1.3.5/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-25 12:42:28.000000 trubrics-1.3.5/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:42:39.688141 trubrics-1.3.5/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 12:42:39.000000 trubrics-1.3.5/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.977897 trubrics-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-03 06:41:38.000000 trubrics-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 06:41:48.977897 trubrics-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-03 06:41:38.000000 trubrics-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/examples/classification_titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/custom_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 06:41:38.000000 trubrics-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 06:41:38.000000 trubrics-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-03 06:41:48.977897 trubrics-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 06:41:38.000000 trubrics-1.3.6/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.977897 trubrics-1.3.6/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.3.5/LICENSE` & `trubrics-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/README.md` & `trubrics-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/examples/classification_titanic/custom_validator.py` & `trubrics-1.3.6/examples/classification_titanic/custom_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/setup.cfg` & `trubrics-1.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.3.5
+version = 1.3.6
 description = Combine data science knowledge with business user feedback to validate machine learning.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `trubrics-1.3.5/tests/test_context.py` & `trubrics-1.3.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/cli/main.py` & `trubrics-1.3.6/trubrics/cli/main.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/cli/run.py` & `trubrics-1.3.6/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/context.py` & `trubrics-1.3.6/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/example/app_titanic_streamlit.py` & `trubrics-1.3.6/trubrics/example/app_titanic_streamlit.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/example/my_first_trubric.json` & `trubrics-1.3.6/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/example/titanic.py` & `trubrics-1.3.6/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/example/titanic_data.csv` & `trubrics-1.3.6/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/example/trubric_run.py` & `trubrics-1.3.6/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/exceptions.py` & `trubrics-1.3.6/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/feedback/config.py` & `trubrics-1.3.6/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/feedback/dataclass.py` & `trubrics-1.3.6/trubrics/feedback/dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from git import InvalidGitRepositoryError
 from git.repo import Repo
 from loguru import logger
 from pydantic import BaseModel, validator
 
-from trubrics.ui.auth import get_trubrics_auth_token
+from trubrics.ui.auth import expire_after_n_seconds, get_trubrics_auth_token
 from trubrics.ui.firestore import add_document_to_project_subcollection
 from trubrics.ui.trubrics_config import load_trubrics_config
 
 
 class Feedback(BaseModel):
     """
     Dataclass for feedback given by a user from a UI component.
@@ -64,15 +64,17 @@
         trubrics_config = load_trubrics_config()
         self._set_fields_on_save()
 
         if email is None and password is None:
             email = trubrics_config.email
             password = trubrics_config.password.get_secret_value()
 
-        auth = get_trubrics_auth_token(trubrics_config.firebase_auth_api_url, email, password)
+        auth = get_trubrics_auth_token(
+            trubrics_config.firebase_auth_api_url, email, password, rerun=expire_after_n_seconds()
+        )
         if "error" in auth:
             error_msg = f"Error in pushing feedback issue with email '{email}' to the Trubrics UI: {auth['error']}"
             logger.error(error_msg)
             raise Exception(error_msg)
         else:
             self.created_by = {"email": auth["email"], "displayName": auth["displayName"]}
             self.collaborators.append(auth["displayName"])
```

### Comparing `trubrics-1.3.5/trubrics/integrations/dash/collect.py` & `trubrics-1.3.6/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/integrations/gradio/collect.py` & `trubrics-1.3.6/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.3.6/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/integrations/streamlit/collect.py` & `trubrics-1.3.6/trubrics/integrations/streamlit/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import streamlit as st
 
 from trubrics.feedback import config
 from trubrics.feedback.dataclass import Feedback
-from trubrics.ui.auth import get_trubrics_auth_token
+from trubrics.ui.auth import expire_after_n_seconds, get_trubrics_auth_token
 from trubrics.ui.trubrics_config import load_trubrics_config
 
 
 class FeedbackCollector:
     def __init__(
         self,
         data: Optional[str] = None,
@@ -69,15 +69,17 @@
                     label_visibility="collapsed",
                     key="password",
                     type="password",
                 )
                 submitted = st.form_submit_button("Sign In")
                 if submitted:
                     # check auth
-                    auth = get_trubrics_auth_token(trubrics_config.firebase_auth_api_url, self.email, self.password)
+                    auth = get_trubrics_auth_token(
+                        trubrics_config.firebase_auth_api_url, self.email, self.password, rerun=expire_after_n_seconds()
+                    )
                     if "error" in auth:
                         st.error(f"Error authenticating user {self.email}. Try again or contact your admin team.")
                     else:
                         st.success(f"{self.email} successfully signed in.")
                         self.authenticated = True
 
     def st_feedback(
```

### Comparing `trubrics-1.3.5/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.3.6/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/ui/auth.py` & `trubrics-1.3.6/trubrics/ui/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import json
+import time
 from functools import lru_cache
 from typing import Dict
 
 import requests  # type: ignore
 
 
 def get_trubrics_firebase_auth_api_url(firebase_api_key):
     return f"https://identitytoolkit.googleapis.com/v1/accounts:signInWithPassword?key={firebase_api_key}"
 
 
+def expire_after_n_seconds(seconds=600):
+    """Return the same value within `seconds` time period."""
+    return round(time.time() / seconds)
+
+
 @lru_cache(maxsize=32)
-def get_trubrics_auth_token(firebase_auth_api_url, email, password) -> Dict[str, str]:
+def get_trubrics_auth_token(firebase_auth_api_url, email, password, rerun=None) -> Dict[str, str]:
+    del rerun  # this variable is just used to force a refresh of lru_cache
     try:
         r = requests.post(
             firebase_auth_api_url,
             headers={"Content-Type": "application/json"},
             data=json.dumps({"email": email, "password": password, "returnSecureToken": True}),
             timeout=5000,
         )
```

### Comparing `trubrics-1.3.5/trubrics/ui/firestore.py` & `trubrics-1.3.6/trubrics/ui/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/ui/trubrics_config.py` & `trubrics-1.3.6/trubrics/ui/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/validations/dataclass.py` & `trubrics-1.3.6/trubrics/validations/dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from git import InvalidGitRepositoryError
 from git.repo import Repo
 from loguru import logger
 from pydantic import BaseModel, validator
 
 from trubrics.exceptions import TrubricValidationError
-from trubrics.ui.auth import get_trubrics_auth_token
+from trubrics.ui.auth import expire_after_n_seconds, get_trubrics_auth_token
 from trubrics.ui.firestore import add_document_to_project_subcollection
 from trubrics.ui.trubrics_config import load_trubrics_config
 
 
 def _validation_context_example():
     return {
         "example": {
@@ -121,15 +121,18 @@
 
         if raise_on_failure:
             self.raise_trubric_failure()
 
     def save_ui(self, raise_on_failure: bool = False):
         trubrics_config = load_trubrics_config()
         auth = get_trubrics_auth_token(
-            trubrics_config.firebase_auth_api_url, trubrics_config.email, trubrics_config.password.get_secret_value()
+            trubrics_config.firebase_auth_api_url,
+            trubrics_config.email,
+            trubrics_config.password.get_secret_value(),
+            rerun=expire_after_n_seconds(),
         )
 
         self.run_by = {"email": trubrics_config.email, "displayName": trubrics_config.username}
         self.set_dynamic_fields()
 
         res = add_document_to_project_subcollection(
             auth,
```

### Comparing `trubrics-1.3.5/trubrics/validations/model/base.py` & `trubrics-1.3.6/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/validations/run.py` & `trubrics-1.3.6/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics/validations/validation_output.py` & `trubrics-1.3.6/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.5/trubrics.egg-info/SOURCES.txt` & `trubrics-1.3.6/trubrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

