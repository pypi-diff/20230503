# Comparing `tmp/unstructured_api_tools-0.9.3.tar.gz` & `tmp/unstructured_api_tools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_api_tools-0.9.3.tar", last modified: Mon Apr 10 17:39:08 2023, max compression
+gzip compressed data, was "unstructured_api_tools-0.9.4.tar", last modified: Thu Apr 13 17:45:52 2023, max compression
```

## Comparing `unstructured_api_tools-0.9.3.tar` & `unstructured_api_tools-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:39:08.857967 unstructured_api_tools-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.849966 unstructured_api_tools-0.9.3/unstructured_api_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/api_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_app.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:52.544789 unstructured_api_tools-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 17:45:52.544789 unstructured_api_tools-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 17:45:52.544789 unstructured_api_tools-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:52.540789 unstructured_api_tools-0.9.4/unstructured_api_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:52.540789 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/api_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:52.544789 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/templates/pipeline_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 17:45:43.000000 unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/templates/pipeline_app.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:45:52.540789 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 17:45:52.000000 unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/top_level.txt
```

### Comparing `unstructured_api_tools-0.9.3/LICENSE.md` & `unstructured_api_tools-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/PKG-INFO` & `unstructured_api_tools-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_api_tools
-Version: 0.9.3
+Version: 0.9.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured-api-tools
 Author: Unstructured Technologies
 Author-email: mrobinson@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_api_tools-0.9.3/README.md` & `unstructured_api_tools-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/setup.py` & `unstructured_api_tools-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/cli.py` & `unstructured_api_tools-0.9.4/unstructured_api_tools/cli.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/api_conventions.py` & `unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/api_conventions.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/convert.py` & `unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/convert.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/lint.py` & `unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/lint.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_api.txt` & `unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/templates/pipeline_api.txt`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_app.txt` & `unstructured_api_tools-0.9.4/unstructured_api_tools/pipelines/templates/pipeline_app.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .{{ module }} import router as {{module}}_router
 {% endfor %}
 
 app = FastAPI(
   title="{{ title }}",
   description="""{{ description }}""",
   version="{{ version or '1.0.0' }}",
-  docs_url="{{ '/' ~ version_name ~ '/docs' if version_name else '/docs' }}"
+  docs_url="{{ '/' ~ version_name ~ '/docs' if version_name else '/docs' }}",
+  openapi_url="{{ '/' ~ version_name ~ '/openapi.json' if version_name else '/openapi.json' }}"
 )
 
 {% for module in module_names -%}
 app.include_router({{ module }}_router)
 {% endfor %}
 
 @app.get("/healthcheck", status_code=status.HTTP_200_OK, include_in_schema=False)
```

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/PKG-INFO` & `unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-api-tools
-Version: 0.9.3
+Version: 0.9.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured-api-tools
 Author: Unstructured Technologies
 Author-email: mrobinson@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/SOURCES.txt` & `unstructured_api_tools-0.9.4/unstructured_api_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

