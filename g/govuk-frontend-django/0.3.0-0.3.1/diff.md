# Comparing `tmp/govuk_frontend_django-0.3.0.tar.gz` & `tmp/govuk_frontend_django-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk_frontend_django-0.3.0.tar", max compression
+gzip compressed data, was "govuk_frontend_django-0.3.1.tar", max compression
```

## Comparing `govuk_frontend_django-0.3.0.tar` & `govuk_frontend_django-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.3.0/LICENSE
--rw-r--r--   0        0        0     1346 2023-04-26 12:03:56.841463 govuk_frontend_django-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.3.0/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.3.0/govuk_frontend_django/components/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-26 12:03:22.552736 govuk_frontend_django-0.3.0/govuk_frontend_django/components/accordion.py
--rw-r--r--   0        0        0      939 2023-04-21 17:53:53.640544 govuk_frontend_django-0.3.0/govuk_frontend_django/components/back_link.py
--rw-r--r--   0        0        0     4249 2023-04-26 11:55:41.152480 govuk_frontend_django-0.3.0/govuk_frontend_django/components/base.py
--rw-r--r--   0        0        0     1170 2023-04-21 17:53:53.647358 govuk_frontend_django-0.3.0/govuk_frontend_django/components/breadcrumbs.py
--rw-r--r--   0        0        0     1221 2023-04-26 12:03:22.554265 govuk_frontend_django-0.3.0/govuk_frontend_django/components/button.py
--rw-r--r--   0        0        0     1838 2023-04-26 12:03:22.552820 govuk_frontend_django-0.3.0/govuk_frontend_django/components/character_count.py
--rw-r--r--   0        0        0     1892 2023-04-26 11:22:44.437285 govuk_frontend_django-0.3.0/govuk_frontend_django/components/checkboxes.py
--rw-r--r--   0        0        0     1723 2023-04-21 17:53:53.661217 govuk_frontend_django-0.3.0/govuk_frontend_django/components/cookie_banner.py
--rw-r--r--   0        0        0     1598 2023-04-21 17:53:53.655825 govuk_frontend_django-0.3.0/govuk_frontend_django/components/date_input.py
--rw-r--r--   0        0        0     1053 2023-04-21 17:53:53.652778 govuk_frontend_django-0.3.0/govuk_frontend_django/components/details.py
--rw-r--r--   0        0        0     1023 2023-04-21 17:53:53.655383 govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_message.py
--rw-r--r--   0        0        0     1349 2023-04-21 17:53:53.658748 govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_summary.py
--rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.657118 govuk_frontend_django-0.3.0/govuk_frontend_django/components/fieldset.py
--rw-r--r--   0        0        0     1251 2023-04-26 12:03:22.554327 govuk_frontend_django-0.3.0/govuk_frontend_django/components/file_upload.py
--rw-r--r--   0        0        0     2007 2023-04-21 17:53:53.671128 govuk_frontend_django-0.3.0/govuk_frontend_django/components/footer.py
--rw-r--r--   0        0        0     1552 2023-04-21 17:53:53.664873 govuk_frontend_django-0.3.0/govuk_frontend_django/components/header.py
--rw-r--r--   0        0        0      927 2023-04-21 17:53:53.661696 govuk_frontend_django-0.3.0/govuk_frontend_django/components/hint.py
--rw-r--r--   0        0        0     1890 2023-04-26 12:03:22.554386 govuk_frontend_django-0.3.0/govuk_frontend_django/components/input.py
--rw-r--r--   0        0        0      960 2023-04-21 17:53:53.665398 govuk_frontend_django-0.3.0/govuk_frontend_django/components/inset_text.py
--rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.666367 govuk_frontend_django-0.3.0/govuk_frontend_django/components/label.py
--rw-r--r--   0        0        0     1241 2023-04-21 17:53:53.667052 govuk_frontend_django-0.3.0/govuk_frontend_django/components/notification_banner.py
--rw-r--r--   0        0        0     1729 2023-04-21 17:53:53.670872 govuk_frontend_django-0.3.0/govuk_frontend_django/components/pagination.py
--rw-r--r--   0        0        0     1015 2023-04-21 17:53:53.675594 govuk_frontend_django-0.3.0/govuk_frontend_django/components/panel.py
--rw-r--r--   0        0        0      980 2023-04-21 17:53:53.668688 govuk_frontend_django-0.3.0/govuk_frontend_django/components/phase_banner.py
--rw-r--r--   0        0        0     1753 2023-04-21 17:53:53.677427 govuk_frontend_django-0.3.0/govuk_frontend_django/components/radios.py
--rw-r--r--   0        0        0     1504 2023-04-26 12:03:22.554441 govuk_frontend_django-0.3.0/govuk_frontend_django/components/select.py
--rw-r--r--   0        0        0      956 2023-04-21 17:53:53.671708 govuk_frontend_django-0.3.0/govuk_frontend_django/components/skip_link.py
--rw-r--r--   0        0        0     1850 2023-04-21 17:53:53.679515 govuk_frontend_django-0.3.0/govuk_frontend_django/components/summary_list.py
--rw-r--r--   0        0        0     1653 2023-04-21 17:53:53.681216 govuk_frontend_django-0.3.0/govuk_frontend_django/components/table.py
--rw-r--r--   0        0        0     1171 2023-04-21 17:53:53.675164 govuk_frontend_django-0.3.0/govuk_frontend_django/components/tabs.py
--rw-r--r--   0        0        0      892 2023-04-21 17:53:53.675735 govuk_frontend_django-0.3.0/govuk_frontend_django/components/tag.py
--rw-r--r--   0        0        0     1344 2023-04-26 12:03:22.554550 govuk_frontend_django-0.3.0/govuk_frontend_django/components/textarea.py
--rw-r--r--   0        0        0      986 2023-04-26 12:03:22.554676 govuk_frontend_django-0.3.0/govuk_frontend_django/components/warning_text.py
--rw-r--r--   0        0        0     2583 2023-04-24 16:19:58.566629 govuk_frontend_django-0.3.0/govuk_frontend_django/templates/govuk_frontend_django/base.html
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/__init__.py
--rw-r--r--   0        0        0    13974 2023-04-26 11:55:41.159321 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-26 11:55:41.160076 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
--rw-r--r--   0        0        0     1207 2023-04-26 11:55:41.160364 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
--rw-r--r--   0        0        0     3291 2023-04-26 11:55:41.160730 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
--rw-r--r--   0        0        0     2198 2023-04-26 11:55:41.161234 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
--rw-r--r--   0        0        0     1532 2023-04-26 11:55:41.162116 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
--rw-r--r--   0        0        0     5243 2023-04-26 11:55:41.162430 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
--rw-r--r--   0        0        0     1600 2023-04-26 11:55:41.162691 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
--rw-r--r--   0        0        0     2209 2023-04-26 11:55:41.162946 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
--rw-r--r--   0        0        0     1388 2023-04-26 11:55:41.163196 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
--rw-r--r--   0        0        0     7121 2023-04-26 11:55:41.163497 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
--rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
--rw-r--r--   0        0        0     1286 2023-04-26 11:55:41.164058 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
--rw-r--r--   0        0        0     1367 2023-04-26 12:04:03.046183 govuk_frontend_django-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 govuk_frontend_django-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1705 2023-05-03 19:45:21.840338 govuk_frontend_django-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.3.1/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.3.1/govuk_frontend_django/components/__init__.py
+-rw-r--r--   0        0        0     1296 2023-05-03 19:45:21.838656 govuk_frontend_django-0.3.1/govuk_frontend_django/components/accordion.py
+-rw-r--r--   0        0        0      939 2023-04-21 17:53:53.640544 govuk_frontend_django-0.3.1/govuk_frontend_django/components/back_link.py
+-rw-r--r--   0        0        0     4249 2023-04-26 11:55:41.152480 govuk_frontend_django-0.3.1/govuk_frontend_django/components/base.py
+-rw-r--r--   0        0        0     1170 2023-04-21 17:53:53.647358 govuk_frontend_django-0.3.1/govuk_frontend_django/components/breadcrumbs.py
+-rw-r--r--   0        0        0     1221 2023-05-03 19:45:21.839102 govuk_frontend_django-0.3.1/govuk_frontend_django/components/button.py
+-rw-r--r--   0        0        0     1838 2023-05-03 19:45:21.837170 govuk_frontend_django-0.3.1/govuk_frontend_django/components/character_count.py
+-rw-r--r--   0        0        0     1892 2023-04-26 11:22:44.437285 govuk_frontend_django-0.3.1/govuk_frontend_django/components/checkboxes.py
+-rw-r--r--   0        0        0     1723 2023-04-21 17:53:53.661217 govuk_frontend_django-0.3.1/govuk_frontend_django/components/cookie_banner.py
+-rw-r--r--   0        0        0     1598 2023-04-21 17:53:53.655825 govuk_frontend_django-0.3.1/govuk_frontend_django/components/date_input.py
+-rw-r--r--   0        0        0     1053 2023-04-21 17:53:53.652778 govuk_frontend_django-0.3.1/govuk_frontend_django/components/details.py
+-rw-r--r--   0        0        0     1023 2023-04-21 17:53:53.655383 govuk_frontend_django-0.3.1/govuk_frontend_django/components/error_message.py
+-rw-r--r--   0        0        0     1349 2023-04-21 17:53:53.658748 govuk_frontend_django-0.3.1/govuk_frontend_django/components/error_summary.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.657118 govuk_frontend_django-0.3.1/govuk_frontend_django/components/fieldset.py
+-rw-r--r--   0        0        0     1251 2023-05-03 19:45:21.838824 govuk_frontend_django-0.3.1/govuk_frontend_django/components/file_upload.py
+-rw-r--r--   0        0        0     2007 2023-04-21 17:53:53.671128 govuk_frontend_django-0.3.1/govuk_frontend_django/components/footer.py
+-rw-r--r--   0        0        0     1552 2023-04-21 17:53:53.664873 govuk_frontend_django-0.3.1/govuk_frontend_django/components/header.py
+-rw-r--r--   0        0        0      927 2023-04-21 17:53:53.661696 govuk_frontend_django-0.3.1/govuk_frontend_django/components/hint.py
+-rw-r--r--   0        0        0     1890 2023-05-03 19:45:21.840088 govuk_frontend_django-0.3.1/govuk_frontend_django/components/input.py
+-rw-r--r--   0        0        0      960 2023-04-21 17:53:53.665398 govuk_frontend_django-0.3.1/govuk_frontend_django/components/inset_text.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.666367 govuk_frontend_django-0.3.1/govuk_frontend_django/components/label.py
+-rw-r--r--   0        0        0     1241 2023-04-21 17:53:53.667052 govuk_frontend_django-0.3.1/govuk_frontend_django/components/notification_banner.py
+-rw-r--r--   0        0        0     1729 2023-04-21 17:53:53.670872 govuk_frontend_django-0.3.1/govuk_frontend_django/components/pagination.py
+-rw-r--r--   0        0        0     1015 2023-04-21 17:53:53.675594 govuk_frontend_django-0.3.1/govuk_frontend_django/components/panel.py
+-rw-r--r--   0        0        0      980 2023-04-21 17:53:53.668688 govuk_frontend_django-0.3.1/govuk_frontend_django/components/phase_banner.py
+-rw-r--r--   0        0        0     1753 2023-04-21 17:53:53.677427 govuk_frontend_django-0.3.1/govuk_frontend_django/components/radios.py
+-rw-r--r--   0        0        0     1504 2023-05-03 19:45:21.838706 govuk_frontend_django-0.3.1/govuk_frontend_django/components/select.py
+-rw-r--r--   0        0        0      956 2023-04-21 17:53:53.671708 govuk_frontend_django-0.3.1/govuk_frontend_django/components/skip_link.py
+-rw-r--r--   0        0        0     1850 2023-04-21 17:53:53.679515 govuk_frontend_django-0.3.1/govuk_frontend_django/components/summary_list.py
+-rw-r--r--   0        0        0     1653 2023-04-21 17:53:53.681216 govuk_frontend_django-0.3.1/govuk_frontend_django/components/table.py
+-rw-r--r--   0        0        0     1171 2023-04-21 17:53:53.675164 govuk_frontend_django-0.3.1/govuk_frontend_django/components/tabs.py
+-rw-r--r--   0        0        0      892 2023-04-21 17:53:53.675735 govuk_frontend_django-0.3.1/govuk_frontend_django/components/tag.py
+-rw-r--r--   0        0        0     1344 2023-05-03 19:45:21.840147 govuk_frontend_django-0.3.1/govuk_frontend_django/components/textarea.py
+-rw-r--r--   0        0        0      986 2023-05-03 19:45:21.840202 govuk_frontend_django-0.3.1/govuk_frontend_django/components/warning_text.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:40:36.710697 govuk_frontend_django-0.3.1/govuk_frontend_django/py.typed
+-rw-r--r--   0        0        0     2583 2023-04-24 16:19:58.566629 govuk_frontend_django-0.3.1/govuk_frontend_django/templates/govuk_frontend_django/base.html
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/__init__.py
+-rw-r--r--   0        0        0    13974 2023-04-26 11:55:41.159321 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0     1518 2023-04-26 11:55:41.160076 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
+-rw-r--r--   0        0        0     1207 2023-04-26 11:55:41.160364 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
+-rw-r--r--   0        0        0     3291 2023-04-26 11:55:41.160730 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
+-rw-r--r--   0        0        0     2198 2023-04-26 11:55:41.161234 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
+-rw-r--r--   0        0        0     1532 2023-04-26 11:55:41.162116 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
+-rw-r--r--   0        0        0     5243 2023-04-26 11:55:41.162430 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
+-rw-r--r--   0        0        0     1600 2023-04-26 11:55:41.162691 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
+-rw-r--r--   0        0        0     2209 2023-04-26 11:55:41.162946 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
+-rw-r--r--   0        0        0     1388 2023-04-26 11:55:41.163196 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
+-rw-r--r--   0        0        0     7121 2023-04-26 11:55:41.163497 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
+-rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
+-rw-r--r--   0        0        0     1286 2023-04-26 11:55:41.164058 govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
+-rw-r--r--   0        0        0     1424 2023-05-03 19:45:21.840303 govuk_frontend_django-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 govuk_frontend_django-0.3.1/PKG-INFO
```

### Comparing `govuk_frontend_django-0.3.0/LICENSE` & `govuk_frontend_django-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/README.md` & `govuk_frontend_django-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,40 @@
 
 
 The `govuk_frontend_django` package contains Django functionality to help when building a GOV.UK website.
 
 The main part of this package is the [template tags](./template-tags/index.md) that it offers for use in your templates. These template tags will reduce the amount of markup that you need to maintain in your project.
 
 This package also contains some helpful [templates](./templates.md) for your project, such as the `govuk_frontend_django/base.html` template which contains the basic structure of a GOV.UK website.
-Packages
+
 ## Getting started
 
 First install the package:
 ```bash
 pip install govuk-frontend-django
-
-# or
-
-poetry add govuk-frontend-django
 ```
 
 In your settings file, add the app to your `INSTALLED_APPS`:
 ```python
 INSTALLED_APPS = [
     ...
     "govuk_frontend_django",
 ]
 ```
 
+Start using the template tags in your templates!
+```django
+{% load govuk_frontend_django %}
+
+{% gds_component "back-link" href="/" %}
+```
+
+[More template tags](./template-tags/index.md)
+
 ## Compatibility table
 
 Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
 
 | Package Version | GOV.UK Frontend Version |
 | --------------- | ----------------------- |
-| 0.2.0           | v4.5.0                  |
-| 0.3.0           | v4.6.0                  |
+| [0.2.1](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.1) | [v4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
+| [0.3.1](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.1) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
```

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/accordion.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/back_link.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/back_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/base.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/base.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/breadcrumbs.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/button.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/button.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/character_count.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/character_count.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/checkboxes.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/cookie_banner.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/date_input.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/date_input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/details.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/details.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_message.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/error_message.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_summary.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/fieldset.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/file_upload.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/file_upload.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/footer.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/header.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/hint.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/hint.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/input.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/inset_text.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/inset_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/label.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/label.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/notification_banner.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/notification_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/pagination.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/panel.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/panel.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/phase_banner.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/radios.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/radios.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/select.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/select.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/skip_link.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/skip_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/summary_list.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/table.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/tabs.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/tag.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/tag.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/textarea.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/textarea.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/components/warning_text.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/components/warning_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templates/govuk_frontend_django/base.html` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templates/govuk_frontend_django/base.html`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py` & `govuk_frontend_django-0.3.1/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.0/pyproject.toml` & `govuk_frontend_django-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "govuk-frontend-django"
-version = "0.3.0"
+version = "0.3.1"
 description = "Django functionality to help when building a GOV.UK website."
 authors = [
     "DBT Live Service Team <live.services@digital.trade.gov.uk>",
     "Cam Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Sam Dudley <samuel.dudley@digital.trade.gov.uk>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://uktrade.github.io/govuk-frontend-django/"
 repository = "https://github.com/uktrade/govuk-frontend-django/"
 documentation = "https://uktrade.github.io/govuk-frontend-django/"
-packages = [{include = "govuk_frontend_django"}]
+packages = [
+    {include = "govuk_frontend_django"},
+    {include = "govuk_frontend_django/py.typed"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^4.1.7"
 jinja2 = "^3.1.2"
 govuk-frontend-jinja = "2.6.0"
```

### Comparing `govuk_frontend_django-0.3.0/PKG-INFO` & `govuk_frontend_django-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-django
-Version: 0.3.0
+Version: 0.3.1
 Summary: Django functionality to help when building a GOV.UK website.
 Home-page: https://uktrade.github.io/govuk-frontend-django/
 License: MIT
 Author: DBT Live Service Team
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,36 +26,41 @@
 
 
 The `govuk_frontend_django` package contains Django functionality to help when building a GOV.UK website.
 
 The main part of this package is the [template tags](./template-tags/index.md) that it offers for use in your templates. These template tags will reduce the amount of markup that you need to maintain in your project.
 
 This package also contains some helpful [templates](./templates.md) for your project, such as the `govuk_frontend_django/base.html` template which contains the basic structure of a GOV.UK website.
-Packages
+
 ## Getting started
 
 First install the package:
 ```bash
 pip install govuk-frontend-django
-
-# or
-
-poetry add govuk-frontend-django
 ```
 
 In your settings file, add the app to your `INSTALLED_APPS`:
 ```python
 INSTALLED_APPS = [
     ...
     "govuk_frontend_django",
 ]
 ```
 
+Start using the template tags in your templates!
+```django
+{% load govuk_frontend_django %}
+
+{% gds_component "back-link" href="/" %}
+```
+
+[More template tags](./template-tags/index.md)
+
 ## Compatibility table
 
 Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
 
 | Package Version | GOV.UK Frontend Version |
 | --------------- | ----------------------- |
-| 0.2.0           | v4.5.0                  |
-| 0.3.0           | v4.6.0                  |
+| [0.2.1](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.1) | [v4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
+| [0.3.1](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.1) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
```

