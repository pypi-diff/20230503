# Comparing `tmp/Flask-First-0.9.3.tar.gz` & `tmp/Flask-First-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-First-0.9.3.tar", last modified: Thu Jan  6 18:01:19 2022, max compression
+gzip compressed data, was "Flask-First-0.9.4.tar", last modified: Fri Mar  4 14:59:16 2022, max compression
```

## Comparing `Flask-First-0.9.3.tar` & `Flask-First-0.9.4.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.483800 Flask-First-0.9.3/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1084 2021-11-22 15:21:11.000000 Flask-First-0.9.3/LICENSE
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       84 2021-12-01 14:03:35.000000 Flask-First-0.9.3/MANIFEST.in
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2834 2022-01-06 18:01:19.483800 Flask-First-0.9.3/PKG-INFO
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2205 2021-12-24 15:45:21.000000 Flask-First-0.9.3/README.md
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.475800 Flask-First-0.9.3/examples/
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/examples/minimum_app/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      423 2021-12-08 16:51:20.000000 Flask-First-0.9.3/examples/minimum_app/main.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      525 2021-11-22 15:21:11.000000 Flask-First-0.9.3/examples/minimum_app/openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       94 2021-12-01 08:06:00.000000 Flask-First-0.9.3/pyproject.toml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      776 2022-01-06 18:01:19.483800 Flask-First-0.9.3/setup.cfg
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      265 2021-12-18 22:02:57.000000 Flask-First-0.9.3/setup.py
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.475800 Flask-First-0.9.3/src/
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/src/Flask_First.egg-info/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2834 2022-01-06 18:01:19.000000 Flask-First-0.9.3/src/Flask_First.egg-info/PKG-INFO
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1494 2022-01-06 18:01:19.000000 Flask-First-0.9.3/src/Flask_First.egg-info/SOURCES.txt
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)        1 2022-01-06 18:01:19.000000 Flask-First-0.9.3/src/Flask_First.egg-info/dependency_links.txt
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       63 2022-01-06 18:01:19.000000 Flask-First-0.9.3/src/Flask_First.egg-info/requires.txt
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       12 2022-01-06 18:01:19.000000 Flask-First-0.9.3/src/Flask_First.egg-info/top_level.txt
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/src/flask_first/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)    11067 2022-01-06 17:54:33.000000 Flask-First-0.9.3/src/flask_first/__init__.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1967 2021-12-19 18:42:31.000000 Flask-First-0.9.3/src/flask_first/exceptions.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2575 2021-12-24 15:24:26.000000 Flask-First-0.9.3/src/flask_first/schema_maker.py
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.475800 Flask-First-0.9.3/src/flask_first/static/
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/src/flask_first/static/swagger_ui/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      665 2021-11-30 13:35:51.000000 Flask-First-0.9.3/src/flask_first/static/swagger_ui/favicon-16x16.png
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      628 2021-11-30 13:35:51.000000 Flask-First-0.9.3/src/flask_first/static/swagger_ui/favicon-32x32.png
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)  1081656 2021-11-30 13:45:22.000000 Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui-bundle.js
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)   321259 2021-11-30 13:45:22.000000 Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)   143859 2021-11-30 13:45:22.000000 Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui.css
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.475800 Flask-First-0.9.3/src/flask_first/templates/
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/src/flask_first/templates/swagger_ui/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1638 2021-11-30 19:46:37.000000 Flask-First-0.9.3/src/flask_first/templates/swagger_ui/index.html
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/tests/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)        0 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/__init__.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      781 2021-11-30 19:50:00.000000 Flask-First-0.9.3/tests/conftest.py
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.479800 Flask-First-0.9.3/tests/specs/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       62 2021-12-19 07:26:18.000000 Flask-First-0.9.3/tests/specs/bad.openapi.yaml
-drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-01-06 18:01:19.483800 Flask-First-0.9.3/tests/specs/v3.0/
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      868 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/additional_properties.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      952 2021-12-24 07:10:22.000000 Flask-First-0.9.3/tests/specs/v3.0/all_of.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      699 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/any_of.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1091 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/callback.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      550 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/examples.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     3546 2021-12-08 16:20:56.000000 Flask-First-0.9.3/tests/specs/v3.0/full.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      573 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/headers.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      755 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/links.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      393 2021-12-04 09:07:36.000000 Flask-First-0.9.3/tests/specs/v3.0/mini.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      413 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/not_registered_endpoint.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      663 2021-12-05 11:35:33.000000 Flask-First-0.9.3/tests/specs/v3.0/nullable.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      910 2021-12-13 16:40:13.000000 Flask-First-0.9.3/tests/specs/v3.0/object.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      699 2021-11-22 15:21:11.000000 Flask-First-0.9.3/tests/specs/v3.0/one_of.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     8145 2021-12-17 13:11:12.000000 Flask-First-0.9.3/tests/specs/v3.0/openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1253 2021-12-24 15:33:53.000000 Flask-First-0.9.3/tests/specs/v3.0/parameters.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1109 2021-12-23 14:50:32.000000 Flask-First-0.9.3/tests/specs/v3.0/ref.openapi.yaml
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)    11084 2021-12-24 15:37:11.000000 Flask-First-0.9.3/tests/test_flask_first.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      308 2021-11-30 19:50:00.000000 Flask-First-0.9.3/tests/test_init_ext.py
--rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2008 2021-12-19 18:31:12.000000 Flask-First-0.9.3/tests/test_specification.py
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.693215 Flask-First-0.9.4/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1084 2021-11-22 15:21:11.000000 Flask-First-0.9.4/LICENSE
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       84 2021-12-01 14:03:35.000000 Flask-First-0.9.4/MANIFEST.in
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2834 2022-03-04 14:59:16.693215 Flask-First-0.9.4/PKG-INFO
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2205 2021-12-24 15:45:21.000000 Flask-First-0.9.4/README.md
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.681215 Flask-First-0.9.4/examples/
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.685215 Flask-First-0.9.4/examples/minimum_app/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      423 2021-12-08 16:51:20.000000 Flask-First-0.9.4/examples/minimum_app/main.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      525 2021-11-22 15:21:11.000000 Flask-First-0.9.4/examples/minimum_app/openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       94 2021-12-01 08:06:00.000000 Flask-First-0.9.4/pyproject.toml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      776 2022-03-04 14:59:16.693215 Flask-First-0.9.4/setup.cfg
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      265 2021-12-18 22:02:57.000000 Flask-First-0.9.4/setup.py
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.685215 Flask-First-0.9.4/src/
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/src/Flask_First.egg-info/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2834 2022-03-04 14:59:16.000000 Flask-First-0.9.4/src/Flask_First.egg-info/PKG-INFO
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1538 2022-03-04 14:59:16.000000 Flask-First-0.9.4/src/Flask_First.egg-info/SOURCES.txt
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)        1 2022-03-04 14:59:16.000000 Flask-First-0.9.4/src/Flask_First.egg-info/dependency_links.txt
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       63 2022-03-04 14:59:16.000000 Flask-First-0.9.4/src/Flask_First.egg-info/requires.txt
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       12 2022-03-04 14:59:16.000000 Flask-First-0.9.4/src/Flask_First.egg-info/top_level.txt
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/src/flask_first/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)    11278 2022-03-04 14:58:24.000000 Flask-First-0.9.4/src/flask_first/__init__.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1967 2021-12-19 18:42:31.000000 Flask-First-0.9.4/src/flask_first/exceptions.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2793 2022-03-04 14:58:24.000000 Flask-First-0.9.4/src/flask_first/schema_maker.py
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.685215 Flask-First-0.9.4/src/flask_first/static/
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/src/flask_first/static/swagger_ui/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      665 2021-11-30 13:35:51.000000 Flask-First-0.9.4/src/flask_first/static/swagger_ui/favicon-16x16.png
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      628 2021-11-30 13:35:51.000000 Flask-First-0.9.4/src/flask_first/static/swagger_ui/favicon-32x32.png
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)  1081656 2021-11-30 13:45:22.000000 Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui-bundle.js
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)   321259 2021-11-30 13:45:22.000000 Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)   143859 2021-11-30 13:45:22.000000 Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui.css
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.685215 Flask-First-0.9.4/src/flask_first/templates/
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/src/flask_first/templates/swagger_ui/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1638 2021-11-30 19:46:37.000000 Flask-First-0.9.4/src/flask_first/templates/swagger_ui/index.html
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/tests/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)        0 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/__init__.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      798 2022-03-04 14:58:24.000000 Flask-First-0.9.4/tests/conftest.py
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.689215 Flask-First-0.9.4/tests/specs/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)       62 2021-12-19 07:26:18.000000 Flask-First-0.9.4/tests/specs/bad.openapi.yaml
+drwxrwxr-x   0 konstantin  (1000) konstantin  (1000)        0 2022-03-04 14:59:16.693215 Flask-First-0.9.4/tests/specs/v3.0/
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      868 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/additional_properties.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      952 2021-12-24 07:10:22.000000 Flask-First-0.9.4/tests/specs/v3.0/all_of.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      699 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/any_of.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1091 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/callback.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      550 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/examples.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     3546 2021-12-08 16:20:56.000000 Flask-First-0.9.4/tests/specs/v3.0/full.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      573 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/headers.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      755 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/links.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      393 2021-12-04 09:07:36.000000 Flask-First-0.9.4/tests/specs/v3.0/mini.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      413 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/not_registered_endpoint.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      663 2021-12-05 11:35:33.000000 Flask-First-0.9.4/tests/specs/v3.0/nullable.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      910 2021-12-13 16:40:13.000000 Flask-First-0.9.4/tests/specs/v3.0/object.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      699 2021-11-22 15:21:11.000000 Flask-First-0.9.4/tests/specs/v3.0/one_of.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     8145 2021-12-17 13:11:12.000000 Flask-First-0.9.4/tests/specs/v3.0/openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      711 2022-03-04 14:58:24.000000 Flask-First-0.9.4/tests/specs/v3.0/param_as_list.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1253 2021-12-24 15:33:53.000000 Flask-First-0.9.4/tests/specs/v3.0/parameters.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     1109 2021-12-23 14:50:32.000000 Flask-First-0.9.4/tests/specs/v3.0/ref.openapi.yaml
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)    12168 2022-03-04 14:58:24.000000 Flask-First-0.9.4/tests/test_flask_first.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)      308 2021-11-30 19:50:00.000000 Flask-First-0.9.4/tests/test_init_ext.py
+-rw-rw-r--   0 konstantin  (1000) konstantin  (1000)     2071 2022-03-04 14:58:24.000000 Flask-First-0.9.4/tests/test_specification.py
```

### Comparing `Flask-First-0.9.3/LICENSE` & `Flask-First-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/PKG-INFO` & `Flask-First-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-First
-Version: 0.9.3
+Version: 0.9.4
 Summary: Flask extension for using "specification first" principle via OpenAPI specification.
 Home-page: https://github.com/flask-pro/flask-first
 Author: Konstantin Fadeev
 Author-email: fadeev@stantis.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/flask-pro/flask-first/issues
 Platform: UNKNOWN
```

### Comparing `Flask-First-0.9.3/README.md` & `Flask-First-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/examples/minimum_app/openapi.yaml` & `Flask-First-0.9.4/examples/minimum_app/openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/setup.cfg` & `Flask-First-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/Flask_First.egg-info/PKG-INFO` & `Flask-First-0.9.4/src/Flask_First.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-First
-Version: 0.9.3
+Version: 0.9.4
 Summary: Flask extension for using "specification first" principle via OpenAPI specification.
 Home-page: https://github.com/flask-pro/flask-first
 Author: Konstantin Fadeev
 Author-email: fadeev@stantis.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/flask-pro/flask-first/issues
 Platform: UNKNOWN
```

### Comparing `Flask-First-0.9.3/src/Flask_First.egg-info/SOURCES.txt` & `Flask-First-0.9.4/src/Flask_First.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,10 @@
 tests/specs/v3.0/links.openapi.yaml
 tests/specs/v3.0/mini.openapi.yaml
 tests/specs/v3.0/not_registered_endpoint.openapi.yaml
 tests/specs/v3.0/nullable.openapi.yaml
 tests/specs/v3.0/object.openapi.yaml
 tests/specs/v3.0/one_of.openapi.yaml
 tests/specs/v3.0/openapi.yaml
+tests/specs/v3.0/param_as_list.openapi.yaml
 tests/specs/v3.0/parameters.openapi.yaml
 tests/specs/v3.0/ref.openapi.yaml
```

### Comparing `Flask-First-0.9.3/src/flask_first/__init__.py` & `Flask-First-0.9.4/src/flask_first/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from .exceptions import FirstRequestArgsValidation
 from .exceptions import FirstRequestJSONValidation
 from .exceptions import FirstRequestPathParamValidation
 from .exceptions import FirstResponseJSONValidation
 from .exceptions import register_errors
 from .schema_maker import make_marshmallow_schema
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 
 class First:
     """This class is used to generation routes from OpenAPI specification."""
 
     def __init__(
         self,
@@ -183,18 +183,22 @@
         if isinstance(payload, MultiDict):
             serialized_payload = {}
 
             # payload.to_dict(flat=False) serializing all arguments as list for correct receipt of
             # arguments of same name:
             # {'first_arg': ['1'], 'second_arg': ['10'], 'args_list': ['1', '2']}
             for key, value in payload.to_dict(flat=False).items():
-                if len(value) == 1:
-                    serialized_payload[key] = value[0]
-                if len(value) > 1:
+                if key not in schema['properties']:
+                    serialized_payload[key] = value
+                elif schema['properties'][key]['type'] == 'array':
                     serialized_payload[key] = value
+                elif len(value) > 1:
+                    serialized_payload[key] = value
+                else:
+                    serialized_payload[key] = value[0]
         else:
             serialized_payload = payload
 
         marshmallow_schema = make_marshmallow_schema(schema)
         return marshmallow_schema().load(serialized_payload)
 
     def _registration_swagger_ui_blueprint(self, swagger_ui_path: Union[str, Path]) -> None:
```

### Comparing `Flask-First-0.9.3/src/flask_first/exceptions.py` & `Flask-First-0.9.4/src/flask_first/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/schema_maker.py` & `Flask-First-0.9.4/src/flask_first/schema_maker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List
 from typing import Union
 
 from marshmallow import fields
 from marshmallow import Schema
 from marshmallow import validate
 
+
 FIELDS_VIA_TYPES = {
     'boolean': fields.Boolean(),
     'number': fields.Float(),
     'string': fields.String(),
     'integer': fields.Integer(),
 }
 
@@ -39,20 +40,25 @@
     if as_nested:
         return fields.Nested(schema_object)
     else:
         return schema_object
 
 
 def _make_array_field(schema: dict) -> fields.Field:
-    if schema['items']['type'] == 'object':
+    data_type = schema['items']['type']
+    data_format = schema['items'].get('format')
+    if data_type == 'object':
         nested_field = _make_field_for_schema(schema['items'])
         nested_field.many = True
         field = nested_field
+    elif data_format and data_format in FIELDS_VIA_FORMATS:
+        nested_field = FIELDS_VIA_FORMATS[data_format]
+        field = fields.List(nested_field)
     else:
-        nested_field = FIELDS_VIA_TYPES[schema['items']['type']]
+        nested_field = FIELDS_VIA_TYPES[data_type]
         field = fields.List(nested_field)
 
     return field
 
 
 def _make_field_validators(schema: dict) -> List[validate.Validator]:
     validators = []
```

### Comparing `Flask-First-0.9.3/src/flask_first/static/swagger_ui/favicon-16x16.png` & `Flask-First-0.9.4/src/flask_first/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/static/swagger_ui/favicon-32x32.png` & `Flask-First-0.9.4/src/flask_first/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui-bundle.js` & `Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui-standalone-preset.js` & `Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/static/swagger_ui/swagger-ui.css` & `Flask-First-0.9.4/src/flask_first/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/src/flask_first/templates/swagger_ui/index.html` & `Flask-First-0.9.4/src/flask_first/templates/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/conftest.py` & `Flask-First-0.9.4/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
+from pathlib import Path
 
 import pytest
 from flask import Flask
 from flask.testing import FlaskClient
 
 from src.flask_first import First
 
-basedir = os.path.abspath(os.path.dirname(__file__))
+BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 @pytest.fixture()
 def fx_config():
     class Config:
-        PATH_TO_SPEC = os.path.join(basedir, "specs/v3.0/openapi.yaml")
+        PATH_TO_SPEC = Path(BASEDIR, 'specs/v3.0/openapi.yaml')
 
     return Config
 
 
 @pytest.fixture()
 def fx_app(fx_config):
-    app = Flask("testing_app")
+    app = Flask('testing_app')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
     First(fx_config.PATH_TO_SPEC, app)
 
     app_context = app.app_context()
     app_context.push()
```

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/additional_properties.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/additional_properties.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/all_of.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/all_of.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/any_of.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/any_of.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/callback.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/callback.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/examples.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/examples.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/full.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/full.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/headers.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/headers.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/links.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/links.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/nullable.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/nullable.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/object.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/object.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/one_of.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/one_of.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/parameters.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/parameters.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/specs/v3.0/ref.openapi.yaml` & `Flask-First-0.9.4/tests/specs/v3.0/ref.openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-First-0.9.3/tests/test_flask_first.py` & `Flask-First-0.9.4/tests/test_flask_first.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 from flask import Flask
 from flask import jsonify
 from flask import request
 from flask import Response
 
+from .conftest import BASEDIR
 from src.flask_first import First
 
 ITEM = {
     'uuid': '789d995f-3aa0-4bf8-a37b-2f2f2086d503',
     'name': 'test_item',
     'description': 'Item from tests.',
 }
@@ -126,15 +127,15 @@
 
 
 def test_specification__all_of():
     app = Flask('testing_all_of')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/all_of.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/all_of.openapi.yaml')
     first = First(full_spec, app)
 
     def all_of_endpoint() -> dict:
         return {'id': 1, 'name': 'Test_name'}
 
     first.add_view_func(all_of_endpoint)
 
@@ -146,15 +147,15 @@
 
 
 def test_specification__one_of():
     app = Flask('testing_one_of')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/one_of.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/one_of.openapi.yaml')
     first = First(full_spec, app)
 
     def one_of_endpoint() -> dict:
         return {'name': 'Test_name'}
 
     first.add_view_func(one_of_endpoint)
 
@@ -163,15 +164,15 @@
 
 
 def test_specification__any_of():
     app = Flask('testing_any_of')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/any_of.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/any_of.openapi.yaml')
     first = First(full_spec, app)
 
     def any_of_endpoint() -> dict:
         return {'id': 1}
 
     first.add_view_func(any_of_endpoint)
 
@@ -180,15 +181,15 @@
 
 
 def test_specification__not_registered_endpoint():
     app = Flask('not_registered_endpoint')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/not_registered_endpoint.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/not_registered_endpoint.openapi.yaml')
     First(full_spec, app)
 
     @app.route('/index')
     def index() -> str:
         return 'OK'
 
     with app.test_client() as test_client:
@@ -198,15 +199,15 @@
 
 
 def test_specification__headers():
     app = Flask('endpoint_with_header')
     app.debug = 1
     app.testing = 1
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/headers.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/headers.openapi.yaml')
     first = First(full_spec, app)
 
     def endpoint_with_header() -> dict:
         return {'message': request.headers['Name']}
 
     first.add_view_func(endpoint_with_header)
 
@@ -216,15 +217,15 @@
         assert r.json['message'] == 'test_header'
 
 
 def test_specification__factory_app():
     def mini_endpoint() -> dict:
         return {'message': 'test_factory_app'}
 
-    first = First(Path('specs/v3.0/mini.openapi.yaml'))
+    first = First(Path(BASEDIR, 'specs/v3.0/mini.openapi.yaml'))
 
     def create_app():
         app = Flask('factory_app')
         app.debug = 1
         app.testing = 1
         app.config['FIRST_RESPONSE_VALIDATION'] = True
         first.init_app(app)
@@ -239,15 +240,15 @@
         assert r.json['message'] == 'test_factory_app'
 
 
 def test_specification__registration_function():
     def mini_endpoint() -> dict:
         return {'message': 'test_factory_app'}
 
-    first = First(Path('specs/v3.0/mini.openapi.yaml'))
+    first = First(Path(BASEDIR, 'specs/v3.0/mini.openapi.yaml'))
 
     def create_app():
         app = Flask('factory_app')
         app.debug = 1
         app.testing = 1
         app.config['FIRST_RESPONSE_VALIDATION'] = True
         first.init_app(app)
@@ -262,15 +263,15 @@
         assert r.json['message'] == 'test_factory_app'
 
 
 def test_specification__response_obj():
     def mini_endpoint() -> dict:
         return {'one': {'one_message': 'message'}, 'list': [{'list_message': 'message'}]}
 
-    first = First(Path('specs/v3.0/object.openapi.yaml'))
+    first = First(Path(BASEDIR, 'specs/v3.0/object.openapi.yaml'))
 
     def create_app():
         app = Flask('object_app')
         app.debug = 1
         app.testing = 1
         app.config['FIRST_RESPONSE_VALIDATION'] = True
         first.init_app(app)
@@ -285,15 +286,15 @@
         assert r.json == {'one': {'one_message': 'message'}, 'list': [{'list_message': 'message'}]}
 
 
 def test_specification__resolving_references():
     def mini_endpoint(uuid: str) -> dict:
         return {'one': {'one_message': uuid}, 'list': [{'list_message': uuid}]}
 
-    first = First(Path('specs/v3.0/ref.openapi.yaml'))
+    first = First(Path(BASEDIR, 'specs/v3.0/ref.openapi.yaml'))
 
     def create_app():
         app = Flask('object_app')
         app.debug = 1
         app.testing = 1
         app.config['FIRST_RESPONSE_VALIDATION'] = True
         first.init_app(app)
@@ -321,15 +322,15 @@
 
         return {
             'uuid_from_path': uuid_from_path,
             'uuid_from_query': str(uuid_from_query),
             'datetime_from_query': str(datetime_from_query).replace(' ', 'T'),
         }
 
-    first = First(Path('specs/v3.0/parameters.openapi.yaml'))
+    first = First(Path(BASEDIR, 'specs/v3.0/parameters.openapi.yaml'))
 
     def create_app():
         app = Flask('params__format')
         app.debug = 1
         app.testing = 1
         app.config['FIRST_RESPONSE_VALIDATION'] = True
         first.init_app(app)
@@ -347,7 +348,40 @@
         )
         assert r.status_code == 200
         assert r.json == {
             'uuid_from_path': test_uuid,
             'uuid_from_query': test_uuid,
             'datetime_from_query': test_datetime,
         }
+
+
+def test_specification__param_as_list():
+    def mini_endpoint() -> dict:
+        args = request.first_args
+        param_as_list = args['param_as_list']
+
+        assert isinstance(param_as_list, list)
+        assert isinstance(param_as_list[0], uuid.UUID)
+
+        return {'param_as_list': param_as_list}
+
+    first = First(Path(BASEDIR, 'specs/v3.0/param_as_list.openapi.yaml'))
+
+    def create_app():
+        app = Flask('param_as_list')
+        app.debug = 1
+        app.testing = 1
+        app.config['FIRST_RESPONSE_VALIDATION'] = True
+        first.init_app(app)
+        first.add_view_func(mini_endpoint)
+        return app
+
+    app = create_app()
+
+    with app.test_client() as test_client:
+        test_uuid = str(uuid.uuid4())
+        r = test_client.get(
+            '/parameters_endpoint',
+            query_string={'param_as_list': [test_uuid]},
+        )
+        assert r.status_code == 200
+        assert r.json == {'param_as_list': [test_uuid]}
```

### Comparing `Flask-First-0.9.3/tests/test_specification.py` & `Flask-First-0.9.4/tests/test_specification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 from pathlib import Path
 
 import pytest
 from flask import Flask
 from flask import request
 
+from .conftest import BASEDIR
 from src.flask_first import First
 from src.flask_first.exceptions import FirstOpenAPIValidation
 
 
 def test_specification__bad_response(fx_app, fx_client):
     def bad_response() -> dict:
         return {'message': 'OK', 'non_exist_field': 'BAD'}
@@ -20,47 +20,47 @@
 
     assert fx_client.get('/bad_response').status_code == 500
 
 
 def test_specification__full_field_openapi():
     app = Flask('testing_app')
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/full.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/full.openapi.yaml')
     First(full_spec, app)
 
 
 def test_specification__bad_openapi():
     app = Flask('bad_api')
     app.debug = True
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/bad.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/bad.openapi.yaml')
     try:
         assert not First(full_spec, app)
     except FirstOpenAPIValidation:
         assert True
 
 
-@pytest.mark.parametrize('spec', os.listdir('specs/v3.0'))
+@pytest.mark.parametrize('spec', Path(BASEDIR, 'specs/v3.0').iterdir())
 def test_specification__check_v30_specs(spec):
     specs_dir = 'specs/v3.0'
     app = Flask('check_v30_specs')
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path(f'{specs_dir}/{spec}')
+    full_spec = Path(BASEDIR, specs_dir, spec)
     First(full_spec, app=app, swagger_ui_path='/docs')
 
     r = app.test_client().get('/docs', follow_redirects=True)
     assert r.status_code == 200
     assert '/docs/openapi.yaml' in r.data.decode()
 
 
 def test_specification__nullable_parameter():
     app = Flask('testing_app')
     app.debug = True
     app.config['FIRST_RESPONSE_VALIDATION'] = True
-    full_spec = Path('specs/v3.0/nullable.openapi.yaml')
+    full_spec = Path(BASEDIR, 'specs/v3.0/nullable.openapi.yaml')
     first = First(full_spec, app)
 
     def nullable_endpoint() -> dict:
         return {'message': request.json['message']}
 
     first.add_view_func(nullable_endpoint)
```

