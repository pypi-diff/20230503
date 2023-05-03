# Comparing `tmp/django-yubin-2.0.0b2.tar.gz` & `tmp/django-yubin-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-yubin-2.0.0b2.tar", last modified: Wed Apr 12 11:10:22 2023, max compression
+gzip compressed data, was "django-yubin-2.0.0b3.tar", last modified: Wed May  3 14:02:11 2023, max compression
```

## Comparing `django-yubin-2.0.0b2.tar` & `django-yubin-2.0.0b3.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/mailparser_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/create_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/db2file.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/file2db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/sample.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/management/commands/send_test_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/message_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0002_auto_20170405_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0003_auto_20171201_1506.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0004_message_date_sent.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0005_auto_20181128_0407.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0006_auto_20200319_1120.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0007_auto_20200319_1158.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0008_auto_20200320_0407.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0009_auto_20221122_1605.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/0010_message_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/storage_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.154146 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/message/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/admin/django_yubin/message/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/html_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/templates/django_yubin/message_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/django_yubin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.158146 django-yubin-2.0.0b2/django_yubin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 11:10:22.000000 django-yubin-2.0.0b2/django_yubin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/mailviews.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/docs/storages.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 11:10:22.162146 django-yubin-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 11:10:11.000000 django-yubin-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/mailparser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/django_yubin/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/create_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/db2file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/file2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/management/commands/send_test_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/message_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/django_yubin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0002_auto_20170405_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0003_auto_20171201_1506.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0004_message_date_sent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0005_auto_20181128_0407.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0006_auto_20200319_1120.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0007_auto_20200319_1158.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0008_auto_20200320_0407.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0009_auto_20221122_1605.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0010_message_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/storage_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin/templates/admin/django_yubin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/django_yubin/templates/admin/django_yubin/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/templates/admin/django_yubin/message/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/django_yubin/templates/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/templates/django_yubin/html_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/templates/django_yubin/message_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/django_yubin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.350207 django-yubin-2.0.0b3/django_yubin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-03 14:02:11.000000 django-yubin-2.0.0b3/django_yubin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-03 14:02:11.000000 django-yubin-2.0.0b3/django_yubin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:02:11.000000 django-yubin-2.0.0b3/django_yubin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 14:02:11.000000 django-yubin-2.0.0b3/django_yubin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 14:02:11.000000 django-yubin-2.0.0b3/django_yubin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/mailviews.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/docs/storages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 14:02:11.354207 django-yubin-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-03 14:02:02.000000 django-yubin-2.0.0b3/setup.py
```

### Comparing `django-yubin-2.0.0b2/LICENSE` & `django-yubin-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/PKG-INFO` & `django-yubin-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-yubin-2.0.0b2/README.rst` & `django-yubin-2.0.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/__init__.py` & `django-yubin-2.0.0b3/django_yubin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,31 @@
     the signature of the ``EmailMessage.send`` function which it may emulate.
     """
     from . import models, settings
 
     if settings.MAILER_TEST_MODE and settings.MAILER_TEST_EMAIL:
         email_message = _set_message_test_mode(email_message, settings.MAILER_TEST_EMAIL)
 
-    count = 0
-    for to_email in email_message.recipients():
-        message = models.Message.objects.create(
-            to_address=to_email,
-            from_address=email_message.from_email,
-            subject=email_message.subject,
-            message_data=email_message.message().as_string(),
-            storage=settings.MAILER_STORAGE_BACKEND)
-        if message.enqueue('Enqueued from a Backend or django-yubin itself.'):
-            count += 1
-        else:
-            logger.exception('Error enqueuing an email', extra={'email_message': message})
-    return count
+    if not email_message.recipients():
+        return 0
+
+    message = models.Message.objects.create(
+        to_address=','.join(email_message.to),
+        cc_address=','.join(email_message.cc),
+        bcc_address=','.join(email_message.bcc),
+        from_address=email_message.from_email,
+        subject=email_message.subject,
+        message_data=email_message.message().as_string(),
+        storage=settings.MAILER_STORAGE_BACKEND)
+
+    if message.enqueue('Enqueued from a Backend or django-yubin itself.'):
+        return 1
+    else:
+        logger.exception('Error enqueuing an email', extra={'email_message': message})
+        return 0
 
 
 def _set_message_test_mode(email_message, mailer_test_email):
     """
     Sets the headers of the message with test values when
     ``MAILER_TEST_MODE`` setting is ``True``
     """
```

### Comparing `django-yubin-2.0.0b2/django_yubin/admin.py` & `django-yubin-2.0.0b3/django_yubin/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     @admin.display(description=_('Storage'))
     def storage_class(self, instance):
         return mark_safe(instance.storage.split('.')[-1])
 
     list_display = ('from_address', 'to_address', 'subject', 'date_created', 'date_sent',
                     'date_enqueued', 'status', 'storage_class', 'message_link')
     list_filter = ('date_created', 'date_sent', 'date_enqueued', 'status')
-    fields = ('from_address', 'to_address', 'subject', 'message_data', 'storage', 'date_sent',
-              'sent_count', 'date_enqueued', 'enqueued_count', 'status')
-    readonly_fields = ('to_address', 'from_address', 'subject', 'message_data', 'storage',
-                       'date_created')
+    fields = ('from_address', 'to_address', 'cc_address', 'bcc_address', 'subject', 'message_data',
+              'storage', 'date_sent', 'sent_count', 'date_enqueued', 'enqueued_count', 'status')
+    readonly_fields = ('to_address', 'cc_address', 'bcc_address', 'from_address', 'subject', 'message_data',
+                       'storage', 'date_created')
     search_fields = ('to_address', 'subject', 'from_address')
     date_hierarchy = 'date_created'
     ordering = ('-date_created',)
     actions = ['enqueue_action', 'mark_as_sent_action', 'mark_as_created_action']
     inlines = [LogInline]
 
     def enqueue_action(self, request, queryset):
```

### Comparing `django-yubin-2.0.0b2/django_yubin/backends.py` & `django-yubin-2.0.0b3/django_yubin/backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/constants.py` & `django-yubin-2.0.0b3/django_yubin/constants.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/engine.py` & `django-yubin-2.0.0b3/django_yubin/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         msg = "Message is not in queue status, ignoring the email."
         logger.warning(msg)
         message.add_log(msg)
         return False
 
     message.mark_as(models.Message.STATUS_IN_PROCESS, "Trying to send the message.")
 
-    if models.Blacklist.objects.filter(email=message.to_address).exists():
-        msg = "Not sending to blacklisted email: %s" % message.to_address
+    recipients = message.recipients()
+    if models.Blacklist.objects.filter(email__in=recipients).exists():
+        msg = "Not sending due blacklisted email in: %s" % recipients
         logger.info(msg)
         message.mark_as(models.Message.STATUS_BLACKLISTED, msg)
         return False
 
     if settings.PAUSE_SEND:
         msg = "Sending is paused, discarding the email."
         logger.info(msg)
```

### Comparing `django-yubin-2.0.0b2/django_yubin/mailparser_utils.py` & `django-yubin-2.0.0b3/django_yubin/mailparser_utils.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/management/commands/create_mail.py` & `django-yubin-2.0.0b3/django_yubin/management/commands/create_mail.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,25 @@
             default=1,
             help='Number of fake mails to create.',
         )
 
     def handle(self, *args, **options):
         number = int(options['quantity'])
 
-        from_email = 'test@example.com'
-        to = ['recipient@example.com']
+        from_email = 'from@example.com'
+        to = ['to1@example.com', 'to2@example.com']
+        cc = ['cc@example.com']
+        bcc = ['bcc@example.com']
 
         for i in range(1, number + 1):
             subject = 'Subject test %s ✉️ 🙂 àäá' % i
             content = 'Body test <strong>%s</strong> ✉️ 🙂 àäá.' % i
             attachment_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'sample.pdf')
             with open(attachment_path, 'rb') as f:
                 attachment = f.read()
             filename = 'sample.pdf'
             mimetype = 'application/pdf'
             message = BasicHTMLAttachmentEmailMessageView(subject, content, attachment, filename, mimetype)
-            message.send(from_email=from_email, to=to)
+            message.send(from_email=from_email, to=to, cc=cc, bcc=bcc)
 
         # This output is checked in tests.
         self.stdout.write('Created email(s): %d' % number)
```

### Comparing `django-yubin-2.0.0b2/django_yubin/management/commands/file2db.py` & `django-yubin-2.0.0b3/django_yubin/management/commands/file2db.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/management/commands/sample.pdf` & `django-yubin-2.0.0b3/django_yubin/management/commands/sample.pdf`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/management/commands/send_test_mail.py` & `django-yubin-2.0.0b3/django_yubin/management/commands/send_test_mail.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/message_views.py` & `django-yubin-2.0.0b3/django_yubin/message_views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0001_initial.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0002_auto_20170405_1635.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0002_auto_20170405_1635.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0003_auto_20171201_1506.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0003_auto_20171201_1506.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0006_auto_20200319_1120.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0006_auto_20200319_1120.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0007_auto_20200319_1158.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0007_auto_20200319_1158.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/migrations/0009_auto_20221122_1605.py` & `django-yubin-2.0.0b3/django_yubin/migrations/0009_auto_20221122_1605.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/models.py` & `django-yubin-2.0.0b3/django_yubin/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,19 @@
         (STATUS_IN_PROCESS, _('In process')),
         (STATUS_SENT, _('Sent')),
         (STATUS_FAILED, _('Failed')),
         (STATUS_BLACKLISTED, _('Blacklisted')),
         (STATUS_DISCARDED, _('Discarded')),
     )
 
-    # These 3 fields are to easy access, filtering and searching without parsing the email.
-    to_address = models.CharField(_('to address'), max_length=200)
+    to_address = models.TextField(_('to addresses'))
+    cc_address = models.TextField(_('cc addresses'), blank=True, default="")
+    bcc_address = models.TextField(_('bcc addresses'), blank=True, default="")
+
+    # These fields are to easy access, filtering and searching without parsing the email.
     from_address = models.CharField(_('from address'), max_length=200)
     subject = models.CharField(_('subject'), max_length=255)
 
     # This field is for internal use in storage backends. They can use it to save the email
     # like the DatabaseSorageBackend, the file path like the FileStorageBackend, etc.
     # Other users must access this data through the ``message_data`` property.
     _message_data = models.TextField(_('message data'), db_column='message_data')
@@ -95,33 +98,51 @@
 
     def __init__(self, *args, **kwargs):
         if '_message_data' in kwargs:
             raise FieldError("_message_data can not be used for creating instances, use message_data.")
         return super().__init__(*args, **kwargs)
 
     def __str__(self):
-        return '%s: %s' % (self.to_address, self.subject)
+        recipients = self.to_address
+        if self.cc_address:
+            recipients += ', %s' % self.cc_address
+        if self.bcc_address:
+            recipients += ', %s' % self.bcc_address
+        return '%s: %s' % (recipients, self.subject)
+
+    def to(self):
+        return [email.strip() for email in self.to_address.split(",") if email.strip()]
+
+    def cc(self):
+        return [email.strip() for email in self.cc_address.split(",") if email.strip()]
+
+    def bcc(self):
+        return [email.strip() for email in self.bcc_address.split(",") if email.strip()]
+
+    def recipients(self):
+        return self.to() + self.cc() + self.bcc()
 
     def get_message_parser(self):
         return mailparser.parse_from_string(self.message_data)
 
     def get_email_message(self):
         """
         Returns EmailMultiAlternatives or EmailMessage depending on whether the email is multipart or not.
         """
         msg = self.get_message_parser()
+        to = self.to() or mailparser_utils.get_addresses(msg.to)
+        cc = self.cc() or mailparser_utils.get_addresses(msg.cc)
+        bcc = self.bcc() or mailparser_utils.get_addresses(msg.bcc)
 
         Email = EmailMultiAlternatives if msg.text_html else EmailMessage
         email = Email(
             subject=msg.subject,
             body='\n'.join(msg.text_plain),
             from_email=mailparser_utils.get_address(msg.from_),
-            to=mailparser_utils.get_addresses(msg.to),
-            cc=mailparser_utils.get_addresses(msg.cc),
-            bcc=mailparser_utils.get_addresses(msg.bcc),
+            to=to, cc=cc, bcc=bcc,
         )
 
         if msg.text_html:
             email.attach_alternative('<br>'.join(msg.text_html), mimetype='text/html')
 
         for attachment in msg.attachments:
             email.attach(
```

### Comparing `django-yubin-2.0.0b2/django_yubin/settings.py` & `django-yubin-2.0.0b3/django_yubin/settings.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/signals.py` & `django-yubin-2.0.0b3/django_yubin/signals.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/storage_backends.py` & `django-yubin-2.0.0b3/django_yubin/storage_backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/tasks.py` & `django-yubin-2.0.0b3/django_yubin/tasks.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/templates/django_yubin/message_detail.html` & `django-yubin-2.0.0b3/django_yubin/templates/django_yubin/message_detail.html`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin/views.py` & `django-yubin-2.0.0b3/django_yubin/views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/django_yubin.egg-info/PKG-INFO` & `django-yubin-2.0.0b3/django_yubin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-yubin-2.0.0b2/django_yubin.egg-info/SOURCES.txt` & `django-yubin-2.0.0b3/django_yubin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 django_yubin/migrations/0004_message_date_sent.py
 django_yubin/migrations/0005_auto_20181128_0407.py
 django_yubin/migrations/0006_auto_20200319_1120.py
 django_yubin/migrations/0007_auto_20200319_1158.py
 django_yubin/migrations/0008_auto_20200320_0407.py
 django_yubin/migrations/0009_auto_20221122_1605.py
 django_yubin/migrations/0010_message_storage.py
+django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py
 django_yubin/migrations/__init__.py
 django_yubin/templates/admin/django_yubin/message/change_form.html
 django_yubin/templates/django_yubin/html_detail.html
 django_yubin/templates/django_yubin/message_detail.html
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
```

### Comparing `django-yubin-2.0.0b2/docs/Makefile` & `django-yubin-2.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/changelog.rst` & `django-yubin-2.0.0b3/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 --------------------
 
 Changed
 ^^^^^^^
 * Send and queue emails with Celery instead of with Cron.
 * Drop priority headers (useless with queues).
 * Storage backends to save emails in databases, file storages, etc.
+* Cc and Bcc support.
 * Supported versions: Python 3.8~3.11, Django 3.2~4.2, Celery 5.0~5.2.
 * Migrate CI/CD from Travis to Github Actions.
 * Docker Compose for external dependencies in development environment.
 * Get django_yubin version programmatically.
 * Update docs.
```

### Comparing `django-yubin-2.0.0b2/docs/conf.py` & `django-yubin-2.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/contributing.rst` & `django-yubin-2.0.0b3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/index.rst` & `django-yubin-2.0.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/install.rst` & `django-yubin-2.0.0b3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/mailviews.rst` & `django-yubin-2.0.0b3/docs/mailviews.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/queue.rst` & `django-yubin-2.0.0b3/docs/queue.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/settings.rst` & `django-yubin-2.0.0b3/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/docs/storages.rst` & `django-yubin-2.0.0b3/docs/storages.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.0b2/setup.py` & `django-yubin-2.0.0b3/setup.py`

 * *Files identical despite different names*

