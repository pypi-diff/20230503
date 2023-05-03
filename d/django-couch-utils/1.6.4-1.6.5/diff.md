# Comparing `tmp/django-couch-utils-1.6.4.tar.gz` & `tmp/django-couch-utils-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-couch-utils-1.6.4.tar", last modified: Thu Jun 23 13:55:42 2022, max compression
+gzip compressed data, was "django-couch-utils-1.6.5.tar", last modified: Wed May  3 07:45:56 2023, max compression
```

## Comparing `django-couch-utils-1.6.4.tar` & `django-couch-utils-1.6.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/
--rw-r--r--   0 elf       (1000) elf       (1010)      624 2021-02-24 16:06:41.000000 django-couch-utils-1.6.4/.gitignore
--rw-r--r--   0 elf       (1000) elf       (1010)      198 2011-11-03 14:31:32.000000 django-couch-utils-1.6.4/.hgtags
--rw-r--r--   0 elf       (1000) elf       (1010)      114 2013-03-03 12:28:30.000000 django-couch-utils-1.6.4/MANIFEST.in
--rw-r--r--   0 elf       (1000) elf       (1010)      596 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/PKG-INFO
--rw-r--r--   0 elf       (1000) elf       (1010)      182 2011-05-16 13:49:43.000000 django-couch-utils-1.6.4/README
--rw-r--r--   0 elf       (1000) elf       (1010)      905 2013-09-05 19:18:11.000000 django-couch-utils-1.6.4/cluster_test.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/
--rw-r--r--   0 elf       (1000) elf       (1010)     7422 2021-02-24 16:31:03.000000 django-couch-utils-1.6.4/django_couch/__init__.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/
--rw-r--r--   0 elf       (1000) elf       (1010)      930 2022-05-26 12:46:36.000000 django-couch-utils-1.6.4/django_couch/admin/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)     4818 2010-05-08 13:01:15.000000 django-couch-utils-1.6.4/django_couch/admin/deprecated.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1136 2010-11-03 12:31:56.000000 django-couch-utils-1.6.4/django_couch/admin/forms.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/templates/
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/
--rw-r--r--   0 elf       (1000) elf       (1010)      316 2010-07-22 19:48:54.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/app.html
--rw-r--r--   0 elf       (1000) elf       (1010)      339 2010-07-22 19:48:45.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/attachment_delete.html
--rw-r--r--   0 elf       (1000) elf       (1010)      361 2010-07-22 20:24:09.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/base.html
--rw-r--r--   0 elf       (1000) elf       (1010)     2004 2010-07-28 17:41:03.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/document.html
--rw-r--r--   0 elf       (1000) elf       (1010)      287 2010-07-22 19:49:25.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/document_delete.html
--rw-r--r--   0 elf       (1000) elf       (1010)      965 2010-07-28 17:15:22.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/documents.html
--rw-r--r--   0 elf       (1000) elf       (1010)      354 2010-07-22 19:45:56.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/login.html
--rw-r--r--   0 elf       (1000) elf       (1010)      594 2010-09-14 10:02:36.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/root.html
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/snippets/
--rw-r--r--   0 elf       (1000) elf       (1010)      624 2010-07-20 18:36:27.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin/snippets/path.html
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/
--rw-r--r--   0 elf       (1000) elf       (1010)     2931 2010-05-08 12:09:12.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/change_list.html
--rw-r--r--   0 elf       (1000) elf       (1010)      514 2010-05-08 12:12:11.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/change_list_results.html
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/includes/
--rw-r--r--   0 elf       (1000) elf       (1010)      865 2010-05-08 13:07:56.000000 django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/includes/fieldset.html
--rw-r--r--   0 elf       (1000) elf       (1010)     1327 2010-09-14 09:21:28.000000 django-couch-utils-1.6.4/django_couch/admin/urls.py
--rw-r--r--   0 elf       (1000) elf       (1010)     4977 2017-03-29 12:20:48.000000 django-couch-utils-1.6.4/django_couch/admin/views.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/auth/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-18 18:48:13.000000 django-couch-utils-1.6.4/django_couch/auth/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)      197 2010-07-28 19:07:18.000000 django-couch-utils-1.6.4/django_couch/auth/admin.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1423 2017-09-25 11:05:18.000000 django-couch-utils-1.6.4/django_couch/auth/backend.py
--rw-r--r--   0 elf       (1000) elf       (1010)      737 2010-07-28 18:45:05.000000 django-couch-utils-1.6.4/django_couch/auth/forms.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/auth/management/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 13:37:15.000000 django-couch-utils-1.6.4/django_couch/auth/management/__init__.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/auth/management/commands/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 13:37:19.000000 django-couch-utils-1.6.4/django_couch/auth/management/commands/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)     3605 2017-09-25 11:11:27.000000 django-couch-utils-1.6.4/django_couch/auth/models.py
--rw-r--r--   0 elf       (1000) elf       (1010)      855 2012-09-24 08:35:04.000000 django-couch-utils-1.6.4/django_couch/auth/utils.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/cluster/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2013-03-03 09:53:45.000000 django-couch-utils-1.6.4/django_couch/cluster/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)     3807 2013-03-03 12:08:46.000000 django-couch-utils-1.6.4/django_couch/cluster/forms.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/cluster/templatetags/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2013-03-03 10:13:14.000000 django-couch-utils-1.6.4/django_couch/cluster/templatetags/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1096 2013-03-03 10:15:30.000000 django-couch-utils-1.6.4/django_couch/cluster/templatetags/cluster_extras.py
--rw-r--r--   0 elf       (1000) elf       (1010)      414 2013-03-12 09:38:02.000000 django-couch-utils-1.6.4/django_couch/cluster/urls.py
--rw-r--r--   0 elf       (1000) elf       (1010)     7938 2013-05-16 08:56:50.000000 django-couch-utils-1.6.4/django_couch/cluster/views.py
--rw-r--r--   0 elf       (1000) elf       (1010)       89 2011-05-06 20:48:38.000000 django-couch-utils-1.6.4/django_couch/context_processors.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/flatpages/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-18 18:23:03.000000 django-couch-utils-1.6.4/django_couch/flatpages/__init__.py
--rw-r--r--   0 elf       (1000) elf       (1010)      224 2010-07-26 08:04:57.000000 django-couch-utils-1.6.4/django_couch/flatpages/admin.py
--rw-r--r--   0 elf       (1000) elf       (1010)      583 2010-07-21 06:32:39.000000 django-couch-utils-1.6.4/django_couch/flatpages/forms.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1529 2014-09-26 13:20:49.000000 django-couch-utils-1.6.4/django_couch/flatpages/middleware.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1427 2013-08-29 11:17:01.000000 django-couch-utils-1.6.4/django_couch/flatpages/sitemaps.py
--rw-r--r--   0 elf       (1000) elf       (1010)      763 2010-05-31 18:36:03.000000 django-couch-utils-1.6.4/django_couch/generic.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/management/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-02-22 10:02:12.000000 django-couch-utils-1.6.4/django_couch/management/__init__.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/management/commands/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-02-22 10:02:12.000000 django-couch-utils-1.6.4/django_couch/management/commands/__init__.py
--rwxr-xr-x   0 elf       (1000) elf       (1010)    14079 2022-05-26 12:54:08.000000 django-couch-utils-1.6.4/django_couch/management/commands/couch.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1506 2017-03-29 12:21:45.000000 django-couch-utils-1.6.4/django_couch/management/commands/couch_create_admin.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1770 2010-11-16 10:07:12.000000 django-couch-utils-1.6.4/django_couch/management/commands/couch_init.py
--rw-r--r--   0 elf       (1000) elf       (1010)     1272 2011-03-13 12:59:55.000000 django-couch-utils-1.6.4/django_couch/management/commands/couch_munin.py
--rw-r--r--   0 elf       (1000) elf       (1010)     2629 2022-06-23 13:51:17.000000 django-couch-utils-1.6.4/django_couch/management/commands/couch_ping.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/sitemaps/
--rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 19:02:02.000000 django-couch-utils-1.6.4/django_couch/sitemaps/__init__.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/sitemaps/templates/
--rw-r--r--   0 elf       (1000) elf       (1010)      680 2010-07-23 19:12:46.000000 django-couch-utils-1.6.4/django_couch/sitemaps/templates/sitemap.xml
--rw-r--r--   0 elf       (1000) elf       (1010)      386 2010-07-23 19:01:25.000000 django-couch-utils-1.6.4/django_couch/sitemaps/views.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/templates/
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/
--rw-r--r--   0 elf       (1000) elf       (1010)     2266 2013-03-03 11:43:36.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/base.html
--rw-r--r--   0 elf       (1000) elf       (1010)      405 2013-03-03 11:56:49.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/config.html
--rw-r--r--   0 elf       (1000) elf       (1010)     7047 2013-03-03 10:19:20.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/node.html
--rw-r--r--   0 elf       (1000) elf       (1010)      744 2013-03-03 12:09:41.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/node_edit.html
--rw-r--r--   0 elf       (1000) elf       (1010)     1032 2013-03-03 10:05:45.000000 django-couch-utils-1.6.4/django_couch/templates/cluster/nodes.html
--rw-r--r--   0 elf       (1000) elf       (1010)     6094 2011-07-06 08:14:36.000000 django-couch-utils-1.6.4/django_couch/translit.py
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/
--rw-r--r--   0 elf       (1000) elf       (1010)      596 2022-06-23 13:55:41.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/PKG-INFO
--rw-r--r--   0 elf       (1000) elf       (1010)     2706 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt
--rw-r--r--   0 elf       (1000) elf       (1010)     1766 2011-05-18 09:11:46.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt.orig
--rw-r--r--   0 elf       (1000) elf       (1010)     1230 2011-01-20 13:41:56.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt~
--rw-r--r--   0 elf       (1000) elf       (1010)        1 2022-06-23 13:55:41.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/dependency_links.txt
--rw-r--r--   0 elf       (1000) elf       (1010)       20 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/requires.txt
--rw-r--r--   0 elf       (1000) elf       (1010)       13 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/django_couch_utils.egg-info/top_level.txt
-drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/doc/
--rw-r--r--   0 elf       (1000) elf       (1010)     3150 2011-05-09 13:44:15.000000 django-couch-utils-1.6.4/doc/Makefile
--rw-r--r--   0 elf       (1000) elf       (1010)     1063 2011-07-06 08:14:36.000000 django-couch-utils-1.6.4/doc/authentication.rst
--rw-r--r--   0 elf       (1000) elf       (1010)     6447 2011-05-09 13:46:09.000000 django-couch-utils-1.6.4/doc/conf.py
--rw-r--r--   0 elf       (1000) elf       (1010)     2484 2014-09-26 09:55:06.000000 django-couch-utils-1.6.4/doc/flatpages.rst
--rw-r--r--   0 elf       (1000) elf       (1010)      431 2011-05-09 14:19:31.000000 django-couch-utils-1.6.4/doc/helpers.rst
--rw-r--r--   0 elf       (1000) elf       (1010)      905 2011-05-18 09:15:56.000000 django-couch-utils-1.6.4/doc/index.rst
--rw-r--r--   0 elf       (1000) elf       (1010)     4090 2014-03-18 09:10:35.000000 django-couch-utils-1.6.4/doc/managepy.rst
--rw-r--r--   0 elf       (1000) elf       (1010)      619 2011-07-06 08:14:36.000000 django-couch-utils-1.6.4/doc/sitemaps.rst
--rwxr-xr-x   0 elf       (1000) elf       (1010)      315 2022-05-26 13:40:06.000000 django-couch-utils-1.6.4/publish.sh
--rw-r--r--   0 elf       (1000) elf       (1010)      109 2022-06-23 13:55:42.000000 django-couch-utils-1.6.4/setup.cfg
--rwxr-xr-x   0 elf       (1000) elf       (1010)     1339 2022-06-23 13:51:49.000000 django-couch-utils-1.6.4/setup.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/
+-rw-r--r--   0 elf       (1000) elf       (1010)      624 2021-02-24 16:06:41.000000 django-couch-utils-1.6.5/.gitignore
+-rw-r--r--   0 elf       (1000) elf       (1010)      198 2011-11-03 14:31:32.000000 django-couch-utils-1.6.5/.hgtags
+-rw-r--r--   0 elf       (1000) elf       (1010)      114 2013-03-03 12:28:30.000000 django-couch-utils-1.6.5/MANIFEST.in
+-rw-r--r--   0 elf       (1000) elf       (1010)      596 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/PKG-INFO
+-rw-r--r--   0 elf       (1000) elf       (1010)      182 2011-05-16 13:49:43.000000 django-couch-utils-1.6.5/README
+-rw-r--r--   0 elf       (1000) elf       (1010)      905 2013-09-05 19:18:11.000000 django-couch-utils-1.6.5/cluster_test.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/
+-rw-r--r--   0 elf       (1000) elf       (1010)     7422 2021-02-24 16:31:03.000000 django-couch-utils-1.6.5/django_couch/__init__.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/
+-rw-r--r--   0 elf       (1000) elf       (1010)      930 2022-05-26 12:46:36.000000 django-couch-utils-1.6.5/django_couch/admin/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     4818 2010-05-08 13:01:15.000000 django-couch-utils-1.6.5/django_couch/admin/deprecated.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1136 2010-11-03 12:31:56.000000 django-couch-utils-1.6.5/django_couch/admin/forms.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/
+-rw-r--r--   0 elf       (1000) elf       (1010)      316 2010-07-22 19:48:54.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/app.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      339 2010-07-22 19:48:45.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/attachment_delete.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      361 2010-07-22 20:24:09.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/base.html
+-rw-r--r--   0 elf       (1000) elf       (1010)     2004 2010-07-28 17:41:03.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/document.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      287 2010-07-22 19:49:25.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/document_delete.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      965 2010-07-28 17:15:22.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/documents.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      354 2010-07-22 19:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/login.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      594 2010-09-14 10:02:36.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/root.html
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/snippets/
+-rw-r--r--   0 elf       (1000) elf       (1010)      624 2010-07-20 18:36:27.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin/snippets/path.html
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/
+-rw-r--r--   0 elf       (1000) elf       (1010)     2931 2010-05-08 12:09:12.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/change_list.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      514 2010-05-08 12:12:11.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/change_list_results.html
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/includes/
+-rw-r--r--   0 elf       (1000) elf       (1010)      865 2010-05-08 13:07:56.000000 django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/includes/fieldset.html
+-rw-r--r--   0 elf       (1000) elf       (1010)     1327 2010-09-14 09:21:28.000000 django-couch-utils-1.6.5/django_couch/admin/urls.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     4977 2017-03-29 12:20:48.000000 django-couch-utils-1.6.5/django_couch/admin/views.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/auth/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-18 18:48:13.000000 django-couch-utils-1.6.5/django_couch/auth/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      197 2010-07-28 19:07:18.000000 django-couch-utils-1.6.5/django_couch/auth/admin.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1423 2017-09-25 11:05:18.000000 django-couch-utils-1.6.5/django_couch/auth/backend.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      737 2010-07-28 18:45:05.000000 django-couch-utils-1.6.5/django_couch/auth/forms.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/auth/management/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 13:37:15.000000 django-couch-utils-1.6.5/django_couch/auth/management/__init__.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/auth/management/commands/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 13:37:19.000000 django-couch-utils-1.6.5/django_couch/auth/management/commands/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     3605 2017-09-25 11:11:27.000000 django-couch-utils-1.6.5/django_couch/auth/models.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      855 2012-09-24 08:35:04.000000 django-couch-utils-1.6.5/django_couch/auth/utils.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/cluster/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2013-03-03 09:53:45.000000 django-couch-utils-1.6.5/django_couch/cluster/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     3807 2013-03-03 12:08:46.000000 django-couch-utils-1.6.5/django_couch/cluster/forms.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/cluster/templatetags/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2013-03-03 10:13:14.000000 django-couch-utils-1.6.5/django_couch/cluster/templatetags/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1096 2013-03-03 10:15:30.000000 django-couch-utils-1.6.5/django_couch/cluster/templatetags/cluster_extras.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      414 2013-03-12 09:38:02.000000 django-couch-utils-1.6.5/django_couch/cluster/urls.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     7938 2013-05-16 08:56:50.000000 django-couch-utils-1.6.5/django_couch/cluster/views.py
+-rw-r--r--   0 elf       (1000) elf       (1010)       89 2011-05-06 20:48:38.000000 django-couch-utils-1.6.5/django_couch/context_processors.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/flatpages/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-18 18:23:03.000000 django-couch-utils-1.6.5/django_couch/flatpages/__init__.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      224 2010-07-26 08:04:57.000000 django-couch-utils-1.6.5/django_couch/flatpages/admin.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      583 2010-07-21 06:32:39.000000 django-couch-utils-1.6.5/django_couch/flatpages/forms.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1529 2014-09-26 13:20:49.000000 django-couch-utils-1.6.5/django_couch/flatpages/middleware.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1427 2013-08-29 11:17:01.000000 django-couch-utils-1.6.5/django_couch/flatpages/sitemaps.py
+-rw-r--r--   0 elf       (1000) elf       (1010)      763 2010-05-31 18:36:03.000000 django-couch-utils-1.6.5/django_couch/generic.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/management/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-02-22 10:02:12.000000 django-couch-utils-1.6.5/django_couch/management/__init__.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/management/commands/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-02-22 10:02:12.000000 django-couch-utils-1.6.5/django_couch/management/commands/__init__.py
+-rwxr-xr-x   0 elf       (1000) elf       (1010)    14079 2022-05-26 12:54:08.000000 django-couch-utils-1.6.5/django_couch/management/commands/couch.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1506 2017-03-29 12:21:45.000000 django-couch-utils-1.6.5/django_couch/management/commands/couch_create_admin.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1770 2010-11-16 10:07:12.000000 django-couch-utils-1.6.5/django_couch/management/commands/couch_init.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     1272 2011-03-13 12:59:55.000000 django-couch-utils-1.6.5/django_couch/management/commands/couch_munin.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     2629 2022-06-23 13:51:17.000000 django-couch-utils-1.6.5/django_couch/management/commands/couch_ping.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/sitemaps/
+-rw-r--r--   0 elf       (1000) elf       (1010)        0 2010-07-23 19:02:02.000000 django-couch-utils-1.6.5/django_couch/sitemaps/__init__.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/sitemaps/templates/
+-rw-r--r--   0 elf       (1000) elf       (1010)      680 2010-07-23 19:12:46.000000 django-couch-utils-1.6.5/django_couch/sitemaps/templates/sitemap.xml
+-rw-r--r--   0 elf       (1000) elf       (1010)      386 2010-07-23 19:01:25.000000 django-couch-utils-1.6.5/django_couch/sitemaps/views.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/templates/
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/
+-rw-r--r--   0 elf       (1000) elf       (1010)     2266 2013-03-03 11:43:36.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/base.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      405 2013-03-03 11:56:49.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/config.html
+-rw-r--r--   0 elf       (1000) elf       (1010)     7047 2013-03-03 10:19:20.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/node.html
+-rw-r--r--   0 elf       (1000) elf       (1010)      744 2013-03-03 12:09:41.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/node_edit.html
+-rw-r--r--   0 elf       (1000) elf       (1010)     1032 2013-03-03 10:05:45.000000 django-couch-utils-1.6.5/django_couch/templates/cluster/nodes.html
+-rw-r--r--   0 elf       (1000) elf       (1010)     6094 2011-07-06 08:14:36.000000 django-couch-utils-1.6.5/django_couch/translit.py
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/
+-rw-r--r--   0 elf       (1000) elf       (1010)      596 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/PKG-INFO
+-rw-r--r--   0 elf       (1000) elf       (1010)     2706 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 elf       (1000) elf       (1010)     1766 2011-05-18 09:11:46.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt.orig
+-rw-r--r--   0 elf       (1000) elf       (1010)     1230 2011-01-20 13:41:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt~
+-rw-r--r--   0 elf       (1000) elf       (1010)        1 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 elf       (1000) elf       (1010)       24 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/requires.txt
+-rw-r--r--   0 elf       (1000) elf       (1010)       13 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/django_couch_utils.egg-info/top_level.txt
+drwxr-xr-x   0 elf       (1000) elf       (1010)        0 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/doc/
+-rw-r--r--   0 elf       (1000) elf       (1010)     3150 2011-05-09 13:44:15.000000 django-couch-utils-1.6.5/doc/Makefile
+-rw-r--r--   0 elf       (1000) elf       (1010)     1063 2011-07-06 08:14:36.000000 django-couch-utils-1.6.5/doc/authentication.rst
+-rw-r--r--   0 elf       (1000) elf       (1010)     6447 2011-05-09 13:46:09.000000 django-couch-utils-1.6.5/doc/conf.py
+-rw-r--r--   0 elf       (1000) elf       (1010)     2484 2014-09-26 09:55:06.000000 django-couch-utils-1.6.5/doc/flatpages.rst
+-rw-r--r--   0 elf       (1000) elf       (1010)      431 2011-05-09 14:19:31.000000 django-couch-utils-1.6.5/doc/helpers.rst
+-rw-r--r--   0 elf       (1000) elf       (1010)      905 2011-05-18 09:15:56.000000 django-couch-utils-1.6.5/doc/index.rst
+-rw-r--r--   0 elf       (1000) elf       (1010)     4090 2014-03-18 09:10:35.000000 django-couch-utils-1.6.5/doc/managepy.rst
+-rw-r--r--   0 elf       (1000) elf       (1010)      619 2011-07-06 08:14:36.000000 django-couch-utils-1.6.5/doc/sitemaps.rst
+-rwxr-xr-x   0 elf       (1000) elf       (1010)      315 2022-05-26 13:40:06.000000 django-couch-utils-1.6.5/publish.sh
+-rw-r--r--   0 elf       (1000) elf       (1010)      109 2023-05-03 07:45:56.000000 django-couch-utils-1.6.5/setup.cfg
+-rwxr-xr-x   0 elf       (1000) elf       (1010)     1343 2022-07-05 11:53:41.000000 django-couch-utils-1.6.5/setup.py
```

### Comparing `django-couch-utils-1.6.4/.gitignore` & `django-couch-utils-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/PKG-INFO` & `django-couch-utils-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-couch-utils
-Version: 1.6.4
+Version: 1.6.5
 Summary: Handy tools and helpers for django projects, powered by CouchDB
 Home-page: https://bitbucket.org/angry_elf/django-couch-utils/
 Author: Alexey Loshkarev
 Author-email: elf2001@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `django-couch-utils-1.6.4/cluster_test.py` & `django-couch-utils-1.6.5/cluster_test.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/__init__.py` & `django-couch-utils-1.6.5/django_couch/__init__.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/__init__.py` & `django-couch-utils-1.6.5/django_couch/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/deprecated.py` & `django-couch-utils-1.6.5/django_couch/admin/deprecated.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/forms.py` & `django-couch-utils-1.6.5/django_couch/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin/document.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin/document.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin/documents.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin/documents.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin/root.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin/root.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin/snippets/path.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin/snippets/path.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/change_list.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/change_list.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/change_list_results.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/templates/admin.deprecated/includes/fieldset.html` & `django-couch-utils-1.6.5/django_couch/admin/templates/admin.deprecated/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/urls.py` & `django-couch-utils-1.6.5/django_couch/admin/urls.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/admin/views.py` & `django-couch-utils-1.6.5/django_couch/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/auth/backend.py` & `django-couch-utils-1.6.5/django_couch/auth/backend.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/auth/forms.py` & `django-couch-utils-1.6.5/django_couch/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/auth/models.py` & `django-couch-utils-1.6.5/django_couch/auth/models.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/auth/utils.py` & `django-couch-utils-1.6.5/django_couch/auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/cluster/forms.py` & `django-couch-utils-1.6.5/django_couch/cluster/forms.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/cluster/templatetags/cluster_extras.py` & `django-couch-utils-1.6.5/django_couch/cluster/templatetags/cluster_extras.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/cluster/views.py` & `django-couch-utils-1.6.5/django_couch/cluster/views.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/flatpages/forms.py` & `django-couch-utils-1.6.5/django_couch/flatpages/forms.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/flatpages/middleware.py` & `django-couch-utils-1.6.5/django_couch/flatpages/middleware.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/flatpages/sitemaps.py` & `django-couch-utils-1.6.5/django_couch/flatpages/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/generic.py` & `django-couch-utils-1.6.5/django_couch/generic.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/management/commands/couch.py` & `django-couch-utils-1.6.5/django_couch/management/commands/couch.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/management/commands/couch_create_admin.py` & `django-couch-utils-1.6.5/django_couch/management/commands/couch_create_admin.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/management/commands/couch_init.py` & `django-couch-utils-1.6.5/django_couch/management/commands/couch_init.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/management/commands/couch_munin.py` & `django-couch-utils-1.6.5/django_couch/management/commands/couch_munin.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/management/commands/couch_ping.py` & `django-couch-utils-1.6.5/django_couch/management/commands/couch_ping.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/sitemaps/templates/sitemap.xml` & `django-couch-utils-1.6.5/django_couch/sitemaps/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/templates/cluster/base.html` & `django-couch-utils-1.6.5/django_couch/templates/cluster/base.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/templates/cluster/node.html` & `django-couch-utils-1.6.5/django_couch/templates/cluster/node.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/templates/cluster/node_edit.html` & `django-couch-utils-1.6.5/django_couch/templates/cluster/node_edit.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/templates/cluster/nodes.html` & `django-couch-utils-1.6.5/django_couch/templates/cluster/nodes.html`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch/translit.py` & `django-couch-utils-1.6.5/django_couch/translit.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch_utils.egg-info/PKG-INFO` & `django-couch-utils-1.6.5/django_couch_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-couch-utils
-Version: 1.6.4
+Version: 1.6.5
 Summary: Handy tools and helpers for django projects, powered by CouchDB
 Home-page: https://bitbucket.org/angry_elf/django-couch-utils/
 Author: Alexey Loshkarev
 Author-email: elf2001@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt` & `django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt.orig` & `django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt.orig`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/django_couch_utils.egg-info/SOURCES.txt~` & `django-couch-utils-1.6.5/django_couch_utils.egg-info/SOURCES.txt~`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/Makefile` & `django-couch-utils-1.6.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/authentication.rst` & `django-couch-utils-1.6.5/doc/authentication.rst`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/conf.py` & `django-couch-utils-1.6.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/flatpages.rst` & `django-couch-utils-1.6.5/doc/flatpages.rst`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/index.rst` & `django-couch-utils-1.6.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/managepy.rst` & `django-couch-utils-1.6.5/doc/managepy.rst`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/doc/sitemaps.rst` & `django-couch-utils-1.6.5/doc/sitemaps.rst`

 * *Files identical despite different names*

### Comparing `django-couch-utils-1.6.4/setup.py` & `django-couch-utils-1.6.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
-version = '1.6.4'
+version = '1.6.5'
 
 if __name__ == '__main__':
     setup(name='django-couch-utils',
           version=version,
           description='Handy tools and helpers for django projects, powered by CouchDB',
           author='Alexey Loshkarev',
           author_email='elf2001@gmail.com',
@@ -17,15 +17,15 @@
               "Development Status :: 5 - Production/Stable",
               "Intended Audience :: Developers",
               "License :: OSI Approved :: GNU General Public License (GPL)",
               "Natural Language :: English",
               "Programming Language :: Python",
               "Topic :: Software Development :: Libraries :: Python Modules",
               ],
-          install_requires=['couchdb-python-curl'],
+          install_requires=['couchdb-python-requests'],
           package_data={'django_couch.admin': ['templates/admin/*.html'],
                         'django_couch': ['templates/cluster/*.html'],
                         'django_couch.sitemaps': ['templates/*.xml'],
                         },
           include_package_data=True,
           #data_files = ['admin/templates/admin/base.html']
           )
```

