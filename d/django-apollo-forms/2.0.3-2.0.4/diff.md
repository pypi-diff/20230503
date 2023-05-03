# Comparing `tmp/django-apollo-forms-2.0.3.tar.gz` & `tmp/django-apollo-forms-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-apollo-forms-2.0.3.tar", last modified: Mon Feb 13 14:39:08 2023, max compression
+gzip compressed data, was "django-apollo-forms-2.0.4.tar", last modified: Wed May  3 14:00:33 2023, max compression
```

## Comparing `django-apollo-forms-2.0.3.tar` & `django-apollo-forms-2.0.4.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.678503 django-apollo-forms-2.0.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-02-13 14:39:08.678503 django-apollo-forms-2.0.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6387 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/v1/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6983 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/v1/api_views.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/v1/permissions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6086 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/v1/serializers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/api/v1/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1116 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/factories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/forms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/lib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/lib/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/lib/emails.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/lib/recaptcha.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7912 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/0002_auto_20180214_2053.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/0003_externalwebhook_service.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/0004_auto_20220816_2013.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2286 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/migrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16418 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.674503 django-apollo-forms-2.0.3/apollo/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.674503 django-apollo-forms-2.0.3/apollo/static/build/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2688748 2023-02-13 14:38:51.000000 django-apollo-forms-2.0.3/apollo/static/build/app.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.674503 django-apollo-forms-2.0.3/apollo/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/images/grid-cell-bg.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4635 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/images/logo.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   799937 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/static/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.670503 django-apollo-forms-2.0.3/apollo/static/src/js/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.674503 django-apollo-forms-2.0.3/apollo/static/src/js/vendor/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86659 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/src/js/vendor/jquery-3.2.1.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/static/webpack.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.674503 django-apollo-forms-2.0.3/apollo/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/templates/forms_manager.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1271 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/templates/noscript.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.678503 django-apollo-forms-2.0.3/apollo/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25799 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/test_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/test_forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/test_lib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15470 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/test_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1790 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/tests/test_signals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3471 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/apollo/views.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-13 14:39:08.678503 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-02-13 14:39:08.000000 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1401 2023-02-13 14:39:08.000000 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-13 14:39:08.000000 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-02-13 14:39:08.000000 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-02-13 14:39:08.000000 django-apollo-forms-2.0.3/django_apollo_forms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-02-13 14:39:08.678503 django-apollo-forms-2.0.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-02-13 14:38:06.000000 django-apollo-forms-2.0.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6387 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6983 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/api_views.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/permissions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6130 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/serializers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/api/v1/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1116 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/factories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/forms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/lib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/emails.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/lib/recaptcha.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7912 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0002_auto_20180214_2053.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0003_externalwebhook_service.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0004_auto_20220816_2013.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2286 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/0006_formfield_validation_message_and_more.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/signals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.095440 django-apollo-forms-2.0.4/apollo/static/build/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2688857 2023-05-03 13:59:54.000000 django-apollo-forms-2.0.4/apollo/static/build/app.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/images/grid-cell-bg.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4635 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/images/logo.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   799937 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.091440 django-apollo-forms-2.0.4/apollo/static/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.091440 django-apollo-forms-2.0.4/apollo/static/src/js/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/static/src/js/vendor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86659 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/src/js/vendor/jquery-3.2.1.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/static/webpack.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/templates/forms_manager.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1271 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/templates/noscript.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/apollo/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25799 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_lib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15470 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1790 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/tests/test_signals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3471 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/apollo/views.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 14:00:33.099440 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8303 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-03 14:00:33.000000 django-apollo-forms-2.0.4/django_apollo_forms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-03 14:00:33.103440 django-apollo-forms-2.0.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-05-03 13:59:14.000000 django-apollo-forms-2.0.4/setup.py
```

### Comparing `django-apollo-forms-2.0.3/PKG-INFO` & `django-apollo-forms-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apollo-forms
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple CMS for forms
 Home-page: https://morgan-and-morgan.github.io/apollo/
 Author: Morgan & Morgan Developers
 Author-email: developers@forthepeople.com
 License: BSD License
 Description: ### What Apollo Is
         At [Morgan & Morgan](https://www.forthepeople.com/), the development team builds lots of forms. A lot. While most of the
```

### Comparing `django-apollo-forms-2.0.3/README.md` & `django-apollo-forms-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/api/v1/api_views.py` & `django-apollo-forms-2.0.4/apollo/api/v1/api_views.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/api/v1/permissions.py` & `django-apollo-forms-2.0.4/apollo/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/api/v1/serializers.py` & `django-apollo-forms-2.0.4/apollo/api/v1/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         fields = ['id', 'name', 'max_width', 'blocks']
 
 
 class FormFieldTemplateSerializer(serializers.ModelSerializer):
     class Meta:
         model = FormFieldTemplate
         fields = ['id', 'name', 'input_type', 'is_visible', 'label', 'label_position', 'placeholder', 'default_value',
-                  'value_choices', 'validation_rule', 'is_submission_label']
+                  'value_choices', 'validation_rule', 'validation_message', 'is_submission_label']
 
 
 class FieldOptionsSerializer(serializers.Serializer):
     widget_types = serializers.ListField(child=serializers.CharField())
     validation_rules = serializers.ListField(child=serializers.CharField())
     label_positions = serializers.ListField(child=serializers.CharField())
 
@@ -65,15 +65,15 @@
         [validated_data.pop(f) for f in template_fields]
 
         return super(FormFieldSerializer, self).update(instance, validated_data)
 
     class Meta:
         model = FormField
         fields = ['id', 'name', 'input_type', 'is_visible', 'label', 'label_position', 'placeholder', 'default_value',
-                  'value_choices', 'validation_rule', 'is_submission_label', 'index']
+                  'value_choices', 'validation_rule', 'validation_message', 'is_submission_label', 'index']
 
 
 class FormSerializer(serializers.ModelSerializer):
     fields = FormFieldSerializer(many=True)
 
     def create(self, validated_data):
         fields = validated_data.pop('fields')
```

### Comparing `django-apollo-forms-2.0.3/apollo/api/v1/urls.py` & `django-apollo-forms-2.0.4/apollo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/factories.py` & `django-apollo-forms-2.0.4/apollo/factories.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/forms.py` & `django-apollo-forms-2.0.4/apollo/forms.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/lib/emails.py` & `django-apollo-forms-2.0.4/apollo/lib/emails.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/lib/recaptcha.py` & `django-apollo-forms-2.0.4/apollo/lib/recaptcha.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/migrations/0001_initial.py` & `django-apollo-forms-2.0.4/apollo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/migrations/0002_auto_20180214_2053.py` & `django-apollo-forms-2.0.4/apollo/migrations/0002_auto_20180214_2053.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/migrations/0003_externalwebhook_service.py` & `django-apollo-forms-2.0.4/apollo/migrations/0003_externalwebhook_service.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/migrations/0004_auto_20220816_2013.py` & `django-apollo-forms-2.0.4/apollo/migrations/0004_auto_20220816_2013.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py` & `django-apollo-forms-2.0.4/apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/models.py` & `django-apollo-forms-2.0.4/apollo/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     value_choices = ArrayField(
         ArrayField(models.CharField(max_length=100), size=2),
         null=True,
         blank=True,
         default=None
     )
     validation_rule = models.CharField(max_length=50, null=True, blank=True, default=RULE_REQUIRED, choices=VALIDATION_RULES)
+    validation_message = models.CharField(max_length=255, null=True, blank=True, default=None)
 
     def __str__(self):
         return """%s // %s (%s)""" % (self.name, self.input_type, self.id)
 
 
 class FormField(models.Model):
     """ a form field is a concrete instance of a field on a form. It must be separate from a FormFieldTemplate
@@ -255,14 +256,15 @@
     value_choices = ArrayField(
         ArrayField(models.CharField(max_length=100), size=2),
         null=True,
         blank=True,
         default=None
     )
     validation_rule = models.CharField(max_length=50, null=True, blank=True, default=FormFieldTemplate.RULE_REQUIRED, choices=FormFieldTemplate.VALIDATION_RULES)
+    validation_message = models.CharField(max_length=255, null=True, blank=True, default=None)
 
     @property
     def name(self):
         return self.template.name
 
     @property
     def input_type(self):
```

### Comparing `django-apollo-forms-2.0.3/apollo/settings.py` & `django-apollo-forms-2.0.4/apollo/settings.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/signals.py` & `django-apollo-forms-2.0.4/apollo/signals.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/build/app.js` & `django-apollo-forms-2.0.4/apollo/static/build/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25155,14 +25155,17 @@
                 }, {
                     'setting': 'value_choices',
                     'widget': 'optionsCreator'
                 }, {
                     'setting': 'validation_rule',
                     'widget': 'select',
                     'options': this.state.validation_rules
+                }, {
+                    'setting': 'validation_message',
+                    'widget': 'text'
                 }];
 
                 // for select fields, if they have no value set then default them to the first of their options
                 fieldSettingOptions.forEach(fo => {
                     if (fo.widget === 'select' && !this.props.field[fo.setting] && fo.options.length > 0) {
                         this.onChangeHandler(fo.setting, 'select')(null, 0, fo.options[0]);
                     }
@@ -76563,15 +76566,15 @@
                                 modal: false,
                                 autoScrollBodyContent: true,
                                 onRequestClose: this.stopEditingField.bind(this)
                             },
                             __WEBPACK_IMPORTED_MODULE_0_react___default.a.createElement(__WEBPACK_IMPORTED_MODULE_9_js_fields_components_FieldCreator__["a" /* default */ ], {
                                 field: this.state.editingField,
                                 api: this.props.api,
-                                editableFields: ['label', 'label_position', 'placeholder', 'default_value', 'value_choices', 'validation_rule'],
+                                editableFields: ['label', 'label_position', 'placeholder', 'default_value', 'value_choices', 'validation_rule', 'validation_message'],
                                 onFieldChanged: this.handleFieldSettingChange.bind(this)
                             })
                         )
                     );
                 }
             }
```

### Comparing `django-apollo-forms-2.0.3/apollo/static/images/grid-cell-bg.png` & `django-apollo-forms-2.0.4/apollo/static/images/grid-cell-bg.png`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/images/logo.png` & `django-apollo-forms-2.0.4/apollo/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/package-lock.json` & `django-apollo-forms-2.0.4/apollo/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/package.json` & `django-apollo-forms-2.0.4/apollo/static/package.json`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/src/js/vendor/jquery-3.2.1.min.js` & `django-apollo-forms-2.0.4/apollo/static/src/js/vendor/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/static/webpack.config.js` & `django-apollo-forms-2.0.4/apollo/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/templates/forms_manager.html` & `django-apollo-forms-2.0.4/apollo/templates/forms_manager.html`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/templates/noscript.html` & `django-apollo-forms-2.0.4/apollo/templates/noscript.html`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/tests/test_api.py` & `django-apollo-forms-2.0.4/apollo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/tests/test_forms.py` & `django-apollo-forms-2.0.4/apollo/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/tests/test_lib.py` & `django-apollo-forms-2.0.4/apollo/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/tests/test_models.py` & `django-apollo-forms-2.0.4/apollo/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/tests/test_signals.py` & `django-apollo-forms-2.0.4/apollo/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/urls.py` & `django-apollo-forms-2.0.4/apollo/urls.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/apollo/views.py` & `django-apollo-forms-2.0.4/apollo/views.py`

 * *Files identical despite different names*

### Comparing `django-apollo-forms-2.0.3/django_apollo_forms.egg-info/PKG-INFO` & `django-apollo-forms-2.0.4/django_apollo_forms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apollo-forms
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple CMS for forms
 Home-page: https://morgan-and-morgan.github.io/apollo/
 Author: Morgan & Morgan Developers
 Author-email: developers@forthepeople.com
 License: BSD License
 Description: ### What Apollo Is
         At [Morgan & Morgan](https://www.forthepeople.com/), the development team builds lots of forms. A lot. While most of the
```

### Comparing `django-apollo-forms-2.0.3/django_apollo_forms.egg-info/SOURCES.txt` & `django-apollo-forms-2.0.4/django_apollo_forms.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 apollo/lib/emails.py
 apollo/lib/recaptcha.py
 apollo/migrations/0001_initial.py
 apollo/migrations/0002_auto_20180214_2053.py
 apollo/migrations/0003_externalwebhook_service.py
 apollo/migrations/0004_auto_20220816_2013.py
 apollo/migrations/0005_alter_apiuser_id_alter_externalwebhook_id_and_more.py
+apollo/migrations/0006_formfield_validation_message_and_more.py
 apollo/migrations/__init__.py
 apollo/static/package-lock.json
 apollo/static/package.json
 apollo/static/webpack.config.js
 apollo/static/build/app.js
 apollo/static/images/grid-cell-bg.png
 apollo/static/images/logo.png
```

### Comparing `django-apollo-forms-2.0.3/setup.py` & `django-apollo-forms-2.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_packages(package):
     """
     Return root package and all sub-packages.
     """
     return [dirpath for dirpath, dirnames, filenames in os.walk(package) if os.path.exists(os.path.join(dirpath, '__init__.py'))]
 
 
-version = '2.0.3'
+version = '2.0.4'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-apollo-forms',
     version=version,
```

