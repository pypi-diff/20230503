# Comparing `tmp/ftw_django_utils-2023.1.1.tar.gz` & `tmp/ftw_django_utils-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftw_django_utils-2023.1.1.tar", max compression
+gzip compressed data, was "ftw_django_utils-2023.2.0.tar", max compression
```

## Comparing `ftw_django_utils-2023.1.1.tar` & `ftw_django_utils-2023.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-04-24 06:47:54.167855 ftw_django_utils-2023.1.1/LICENSE
--rw-r--r--   0        0        0     9176 2023-04-27 09:46:18.265708 ftw_django_utils-2023.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:42.866695 ftw_django_utils-2023.1.1/django_utils/__init__.py
--rw-r--r--   0        0        0      101 2023-04-24 06:47:54.168594 ftw_django_utils-2023.1.1/django_utils/apps.py
--rw-r--r--   0        0        0      931 2023-04-24 06:47:54.168843 ftw_django_utils-2023.1.1/django_utils/authentication/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.168986 ftw_django_utils-2023.1.1/django_utils/db/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169154 ftw_django_utils-2023.1.1/django_utils/db/fields/__init__.py
--rw-r--r--   0        0        0      579 2023-04-24 06:47:54.169320 ftw_django_utils-2023.1.1/django_utils/db/fields/text.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169464 ftw_django_utils-2023.1.1/django_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169619 ftw_django_utils-2023.1.1/django_utils/management/commands/__init__.py
--rw-r--r--   0        0        0      672 2023-04-24 06:47:54.169783 ftw_django_utils-2023.1.1/django_utils/management/commands/sentry_test.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169954 ftw_django_utils-2023.1.1/django_utils/serializer/__init__.py
--rw-r--r--   0        0        0       70 2023-04-24 06:47:54.170297 ftw_django_utils-2023.1.1/django_utils/serializer/fields/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-27 12:17:15.591189 ftw_django_utils-2023.1.1/django_utils/serializer/fields/protected_image_field.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.170724 ftw_django_utils-2023.1.1/django_utils/settings/__init__.py
--rw-r--r--   0        0        0     2229 2023-04-24 06:47:54.170950 ftw_django_utils-2023.1.1/django_utils/settings/logging.py
--rw-r--r--   0        0        0      989 2023-04-24 06:47:54.171110 ftw_django_utils-2023.1.1/django_utils/settings/sentry.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.171273 ftw_django_utils-2023.1.1/django_utils/testing/__init__.py
--rw-r--r--   0        0        0      793 2023-04-24 06:47:54.171507 ftw_django_utils-2023.1.1/django_utils/testing/filestructure.py
--rw-r--r--   0        0        0      358 2023-04-27 12:17:15.591899 ftw_django_utils-2023.1.1/django_utils/testing/urls.py
--rw-r--r--   0        0        0     3701 2023-04-27 12:17:15.592407 ftw_django_utils-2023.1.1/django_utils/testing/views.py
--rw-r--r--   0        0        0       55 2023-04-24 06:47:54.171995 ftw_django_utils-2023.1.1/django_utils/views/__init__.py
--rw-r--r--   0        0        0     1520 2023-04-27 12:17:15.592903 ftw_django_utils-2023.1.1/django_utils/views/file_getter.py
--rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474048 ftw_django_utils-2023.1.1/django_utils/webhooks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474359 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/__init__.py
--rw-r--r--   0        0        0       98 2023-04-25 13:48:47.475387 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/default_delete_hooks.py
--rw-r--r--   0        0        0      214 2023-04-25 13:48:47.476248 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/serializers.py
--rw-r--r--   0        0        0     1158 2023-04-25 13:48:47.476744 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/token_authentication.py
--rw-r--r--   0        0        0      259 2023-04-25 13:48:47.477333 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/urls.py
--rw-r--r--   0        0        0     1837 2023-04-27 12:17:15.593531 ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/views.py
--rw-r--r--   0        0        0     1404 2023-04-28 08:49:17.775722 ftw_django_utils-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0     9874 1970-01-01 00:00:00.000000 ftw_django_utils-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 06:47:54.167855 ftw_django_utils-2023.2.0/LICENSE
+-rw-r--r--   0        0        0    10043 2023-05-03 15:13:01.186342 ftw_django_utils-2023.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 11:53:42.866695 ftw_django_utils-2023.2.0/django_utils/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-24 06:47:54.168594 ftw_django_utils-2023.2.0/django_utils/apps.py
+-rw-r--r--   0        0        0      931 2023-04-24 06:47:54.168843 ftw_django_utils-2023.2.0/django_utils/authentication/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.168986 ftw_django_utils-2023.2.0/django_utils/db/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169154 ftw_django_utils-2023.2.0/django_utils/db/fields/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-24 06:47:54.169320 ftw_django_utils-2023.2.0/django_utils/db/fields/text.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169464 ftw_django_utils-2023.2.0/django_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169619 ftw_django_utils-2023.2.0/django_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0      672 2023-04-24 06:47:54.169783 ftw_django_utils-2023.2.0/django_utils/management/commands/sentry_test.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169954 ftw_django_utils-2023.2.0/django_utils/serializer/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-24 06:47:54.170297 ftw_django_utils-2023.2.0/django_utils/serializer/fields/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-27 12:17:15.591189 ftw_django_utils-2023.2.0/django_utils/serializer/fields/protected_image_field.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.170724 ftw_django_utils-2023.2.0/django_utils/settings/__init__.py
+-rw-r--r--   0        0        0     2229 2023-04-24 06:47:54.170950 ftw_django_utils-2023.2.0/django_utils/settings/logging.py
+-rw-r--r--   0        0        0      989 2023-04-24 06:47:54.171110 ftw_django_utils-2023.2.0/django_utils/settings/sentry.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:47:54.171273 ftw_django_utils-2023.2.0/django_utils/testing/__init__.py
+-rw-r--r--   0        0        0      793 2023-04-24 06:47:54.171507 ftw_django_utils-2023.2.0/django_utils/testing/filestructure.py
+-rw-r--r--   0        0        0      358 2023-04-27 12:17:15.591899 ftw_django_utils-2023.2.0/django_utils/testing/urls.py
+-rw-r--r--   0        0        0     3701 2023-04-27 12:17:15.592407 ftw_django_utils-2023.2.0/django_utils/testing/views.py
+-rw-r--r--   0        0        0       55 2023-04-24 06:47:54.171995 ftw_django_utils-2023.2.0/django_utils/views/__init__.py
+-rw-r--r--   0        0        0     1520 2023-04-27 12:17:15.592903 ftw_django_utils-2023.2.0/django_utils/views/file_getter.py
+-rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474048 ftw_django_utils-2023.2.0/django_utils/webhooks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474359 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-25 13:48:47.475387 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/default_delete_hooks.py
+-rw-r--r--   0        0        0      214 2023-04-25 13:48:47.476248 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/serializers.py
+-rw-r--r--   0        0        0     1158 2023-04-25 13:48:47.476744 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/token_authentication.py
+-rw-r--r--   0        0        0      259 2023-04-25 13:48:47.477333 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/urls.py
+-rw-r--r--   0        0        0     1837 2023-04-27 12:17:15.593531 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/views.py
+-rw-r--r--   0        0        0     1404 2023-05-03 15:15:02.991709 ftw_django_utils-2023.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10741 1970-01-01 00:00:00.000000 ftw_django_utils-2023.2.0/PKG-INFO
```

### Comparing `ftw_django_utils-2023.1.1/LICENSE` & `ftw_django_utils-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/README.md` & `ftw_django_utils-2023.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # django-utils
 A collection of utils used in our Django based web applications
 
-[Changelog](CHANGELOG.rst)
+[Changelog](CHANGELOG.md)
+
+## Development
+
+Installing dependencies, assuming you have poetry installed:
+
+``` bash
+poetry install
+```
+
+## Release
+
+This package uses towncrier to manage the changelog, and to introduce new changes, a file with a concise title and a brief explanation of what the change accomplishes should be created in the `changes` directory, with a suffix indicating whether the change is a feature, bugfix, or other.
+
+To make a release and publish it to PyPI, the following command can be executed:
+
+``` bash
+./bin/release
+```
+
+This script utilizes zest.releaser and towncrier to create the release, build the wheel, and publish it to PyPI.
+
+Before running the release command, it is necessary to configure poetry with an access token for PyPI by executing the following command and inserting the token stored in 1password:
+
+``` bash
+poetry config pypi-token.pypi <token>
+```
 
 ## Settings
 
 ### LogMixin
 
 A mixin containing the logging configuration with default values suited for production.
```

### Comparing `ftw_django_utils-2023.1.1/django_utils/authentication/__init__.py` & `ftw_django_utils-2023.2.0/django_utils/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/db/fields/text.py` & `ftw_django_utils-2023.2.0/django_utils/db/fields/text.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/management/commands/sentry_test.py` & `ftw_django_utils-2023.2.0/django_utils/management/commands/sentry_test.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/serializer/fields/protected_image_field.py` & `ftw_django_utils-2023.2.0/django_utils/serializer/fields/protected_image_field.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/settings/logging.py` & `ftw_django_utils-2023.2.0/django_utils/settings/logging.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/settings/sentry.py` & `ftw_django_utils-2023.2.0/django_utils/settings/sentry.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/testing/filestructure.py` & `ftw_django_utils-2023.2.0/django_utils/testing/filestructure.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/testing/views.py` & `ftw_django_utils-2023.2.0/django_utils/testing/views.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/views/file_getter.py` & `ftw_django_utils-2023.2.0/django_utils/views/file_getter.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/token_authentication.py` & `ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/token_authentication.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/django_utils/webhooks/delete_user/views.py` & `ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/views.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.1.1/pyproject.toml` & `ftw_django_utils-2023.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftw-django-utils"
-version = "2023.1.1"
+version = "2023.2.0"
 description = "A collection of utils used in our Django based web applications."
 authors = ["4teamwork AG"]
 readme = "README.md"
 packages = [{include = "django_utils"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4"
```

### Comparing `ftw_django_utils-2023.1.1/PKG-INFO` & `ftw_django_utils-2023.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw-django-utils
-Version: 2023.1.1
+Version: 2023.2.0
 Summary: A collection of utils used in our Django based web applications.
 Author: 4teamwork AG
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,41 @@
 Requires-Dist: djangorestframework (>=3,<4)
 Requires-Dist: sentry-sdk (>=1.21.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # django-utils
 A collection of utils used in our Django based web applications
 
-[Changelog](CHANGELOG.rst)
+[Changelog](CHANGELOG.md)
+
+## Development
+
+Installing dependencies, assuming you have poetry installed:
+
+``` bash
+poetry install
+```
+
+## Release
+
+This package uses towncrier to manage the changelog, and to introduce new changes, a file with a concise title and a brief explanation of what the change accomplishes should be created in the `changes` directory, with a suffix indicating whether the change is a feature, bugfix, or other.
+
+To make a release and publish it to PyPI, the following command can be executed:
+
+``` bash
+./bin/release
+```
+
+This script utilizes zest.releaser and towncrier to create the release, build the wheel, and publish it to PyPI.
+
+Before running the release command, it is necessary to configure poetry with an access token for PyPI by executing the following command and inserting the token stored in 1password:
+
+``` bash
+poetry config pypi-token.pypi <token>
+```
 
 ## Settings
 
 ### LogMixin
 
 A mixin containing the logging configuration with default values suited for production.
```

