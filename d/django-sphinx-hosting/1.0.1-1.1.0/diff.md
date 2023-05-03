# Comparing `tmp/django-sphinx-hosting-1.0.1.tar.gz` & `tmp/django-sphinx-hosting-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.0.1.tar", last modified: Mon May  1 22:10:47 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.1.0.tar", last modified: Wed May  3 17:13:53 2023, max compression
```

## Comparing `django-sphinx-hosting-1.0.1.tar` & `django-sphinx-hosting-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.652818 django-sphinx-hosting-1.0.1/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.0.1/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.0.1/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-01 22:10:47.652970 django-sphinx-hosting-1.0.1/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.0.1/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.605493 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2521 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-01 22:10:47.653801 django-sphinx-hosting-1.0.1/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-01 22:09:56.000000 django-sphinx-hosting-1.0.1/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.614796 django-sphinx-hosting-1.0.1/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-01 22:09:56.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.618031 django-sphinx-hosting-1.0.1/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/exc.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.618787 django-sphinx-hosting-1.0.1/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/fixtures/classifiers.json
--rw-rw-r--   0 cmalek     (501) admin       (80)     6843 2023-04-27 16:25:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    21291 2023-04-27 16:27:31.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.619653 django-sphinx-hosting-1.0.1/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.624504 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.634644 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    31797 2023-05-01 22:09:26.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/search_indexes.py
--rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/settings.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600059 django-sphinx-hosting-1.0.1/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600360 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.640666 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.641605 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.601164 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600855 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600980 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.643072 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.644102 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/base.html
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1653 2023-03-28 18:47:58.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/urls.py
--rw-r--r--   0 cmalek     (501) admin       (80)      606 2022-11-02 23:23:01.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.650803 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6553 2023-04-27 20:10:51.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.652523 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4463 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14263 2023-04-27 19:40:10.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     7084 2023-04-27 20:42:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.111848 django-sphinx-hosting-1.1.0/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.0/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.0/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 17:13:53.112105 django-sphinx-hosting-1.1.0/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.0/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.057841 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 17:13:52.000000 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2653 2023-05-03 17:13:52.000000 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-03 17:13:52.000000 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-03 17:13:52.000000 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-03 17:13:52.000000 django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-03 17:13:53.113606 django-sphinx-hosting-1.1.0/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-03 17:13:37.000000 django-sphinx-hosting-1.1.0/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.072645 django-sphinx-hosting-1.1.0/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-03 17:13:37.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.076260 django-sphinx-hosting-1.1.0/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/api/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.077122 django-sphinx-hosting-1.1.0/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/fixtures/classifiers.json
+-rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6844 2023-05-03 16:47:46.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    21291 2023-04-27 16:27:31.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.077861 django-sphinx-hosting-1.1.0/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.081790 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.092743 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    31834 2023-05-03 16:51:48.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/search_indexes.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.050795 django-sphinx-hosting-1.1.0/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.051105 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.097693 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.098704 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.051995 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.051676 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.051799 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.100312 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.101333 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/templates/sphinx_hosting/base.html
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/urls.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.109404 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6553 2023-04-27 20:10:51.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:13:53.111338 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4456 2023-05-02 23:23:03.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    14340 2023-05-03 16:34:33.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     7084 2023-04-27 20:42:19.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.0.1/LICENSE.txt` & `django-sphinx-hosting-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/PKG-INFO` & `django-sphinx-hosting-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.0.1
+Version: 1.1.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.0.1/README.md` & `django-sphinx-hosting-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.0.1
+Version: 1.1.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.1.0/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 django_sphinx_hosting.egg-info/SOURCES.txt
 django_sphinx_hosting.egg-info/dependency_links.txt
 django_sphinx_hosting.egg-info/requires.txt
 django_sphinx_hosting.egg-info/top_level.txt
 sphinx_hosting/__init__.py
 sphinx_hosting/apps.py
 sphinx_hosting/exc.py
+sphinx_hosting/fields.py
+sphinx_hosting/form_fields.py
 sphinx_hosting/forms.py
 sphinx_hosting/importers.py
 sphinx_hosting/logging.py
 sphinx_hosting/models.py
 sphinx_hosting/py.typed
 sphinx_hosting/search_indexes.py
 sphinx_hosting/settings.py
+sphinx_hosting/signals.py
 sphinx_hosting/types.py
 sphinx_hosting/urls.py
 sphinx_hosting/validators.py
 sphinx_hosting/views.py
 sphinx_hosting/api/__init__.py
 sphinx_hosting/api/apps.py
 sphinx_hosting/api/serializers.py
@@ -40,14 +43,15 @@
 sphinx_hosting/migrations/0004_next_page_FK.py
 sphinx_hosting/migrations/0005_orig_global_toc.py
 sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
 sphinx_hosting/migrations/0007_load_classifiers.py
 sphinx_hosting/migrations/0008_Version_archived.py
 sphinx_hosting/migrations/0009_SphinxPage_searchable.py
 sphinx_hosting/migrations/0010_add_groups.py
+sphinx_hosting/migrations/0011_machinenamefield.py
 sphinx_hosting/migrations/__init__.py
 sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
 sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
 sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
 sphinx_hosting/static/sphinx_hosting/images/logo.jpg
```

### Comparing `django-sphinx-hosting-1.0.1/setup.cfg` & `django-sphinx-hosting-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/setup.py` & `django-sphinx-hosting-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.0.1",
+    version="1.1.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
         "django-haystack >= 3.2.1",
         "django-rest-framework-helpers >= 8.5.0",
         "django-theme-academy >= 0.3.0",
-        "django-wildewidgets >= 0.16.4",
+        "django-wildewidgets >= 0.16.7",
         "djangorestframework >= 3.14.0",
         "drf-spectacular >= 0.25.1",
         "crispy-bootstrap5",
         "humanize",
         "lxml >= 4.9.1",
         "cssselect >= 1.2.0",
         "rich"
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.1.0/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.db.models import Model
 from django.urls import reverse, reverse_lazy
 from haystack.forms import SearchForm
 
 from .models import Project
 
 
+
 class GlobalSearchForm(SearchForm):
     """
     This is the search form at the top of the sidebar, underneath the logo.  It is
     a subclass of :py:class:`haystack.forms.SearchForm`, and does a search of our
     haystack backend.
     """
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/importers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/models.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.urls import reverse
 from django_extensions.db.models import TimeStampedModel
 from lxml import etree
 import lxml.html
 from lxml.html import HtmlElement
 from wildewidgets.models import ViewSetMixin
 
+from .fields import MachineNameField
 from .settings import MAX_GLOBAL_TOC_TREE_DEPTH
 from .validators import NoHTMLValidator
 
 
 F = models.Field
 M2M = models.ManyToManyField
 FK = models.ForeignKey
@@ -592,15 +593,15 @@
         'Brief Description',
         max_length=256,
         null=True,
         blank=True,
         help_text=_('A brief description of this project'),
         validators=[NoHTMLValidator()]
     )
-    machine_name: F = models.SlugField(
+    machine_name: F = MachineNameField(
         'Machine Name',
         unique=True,
         help_text=_(
             """Must be unique.  Set this to the slugified value of "project" in Sphinx's. conf.py"""
         )
     )
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.1.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.1.0/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 
 app_name: str = "sphinx_hosting"
 
 urlpatterns: List[URLPattern] = [
     path('', ProjectListView.as_view(), name='project--list'),
     path('project/', ProjectCreateView.as_view(), name='project--create'),
-    path('project/<slug:slug>/', ProjectDetailView.as_view(), name='project--detail'),
-    path('project/<slug:slug>/update/', ProjectUpdateView.as_view(), name='project--update'),
-    path('project/<slug:slug>/upload/', VersionUploadView.as_view(), name='version--upload'),
-    path('project/<slug:slug>/delete/', ProjectDeleteView.as_view(), name='project--delete'),
-    path('project/<slug:project_slug>/<str:version>/', VersionDetailView.as_view(), name='version--detail'),
-    path('project/<slug:project_slug>/<str:version>/delete/', VersionDeleteView.as_view(), name='version--delete'),
+    path('project/<str:slug>/', ProjectDetailView.as_view(), name='project--detail'),
+    path('project/<str:slug>/update/', ProjectUpdateView.as_view(), name='project--update'),
+    path('project/<str:slug>/upload/', VersionUploadView.as_view(), name='version--upload'),
+    path('project/<str:slug>/delete/', ProjectDeleteView.as_view(), name='project--delete'),
+    path('project/<str:project_slug>/<str:version>/', VersionDetailView.as_view(), name='version--detail'),
+    path('project/<str:project_slug>/<str:version>/delete/', VersionDeleteView.as_view(), name='version--delete'),
     re_path(
-        r'project/(?P<project_slug>[\w-]+)/(?P<version>[^/]+)/(?P<path>.*)/',
+        r'project/(?P<project_slug>[-a-zA-Z0-9_.]+)/(?P<version>[^/]+)/(?P<path>.*)/',
         SphinxPageDetailView.as_view(),
         name='sphinxpage--detail'
     ),
     path('search/', GlobalSphinxPageSearchView.as_view(), name='search'),
 ]
 urlpatterns += ClassifierViewSet(url_prefix='lookups', url_namespace=app_name).get_urlpatterns()
 urlpatterns += ProjectClassifierSelectorWidget.get_urlpatterns(url_namespace=app_name)
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/views.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,11 +127,11 @@
     wide: bool = True
 
 
 class SphinxHostingBreadcrumbs(BreadcrumbBlock):
 
     items: List[BreadcrumbItem] = [
         BreadcrumbItem(
-            title='Sphinx Hosting',
+            title=SITE_NAME,
             url=reverse_lazy('sphinx_hosting:project--list')
         )
     ]
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,20 +371,24 @@
     verbose_names: Dict[str, str] = {
         'title': 'Version',
         'num_pages': '# Pages',
         'num_images': '# Images',
     }
     #: A dict of column names to alignment ("left", "right", "center")
     alignment: Dict[str, str] = {
-        'version': 'center',
+        'version': 'left',
         'num_pages': 'right',
         'num_images': 'right',
         'created': 'left',
         'modified': 'left'
     }
+    #: Order by version number
+    order_columns: List[str] = ['version']
+    #: Sort so that the highest version number is on top
+    sort_ascending: bool = False
 
     def __init__(self, *args, **kwargs) -> None:
         """
         One of our ``kwargs`` must be ``project_id``, the ``pk`` of the
         :py:class:`sphinx_hosting.models.Project` for which we want to list
         :py:class:`sphinx_hosting.models.Version` objects.
 
@@ -401,17 +405,15 @@
         """
         Filter our :py:class:`sphinx_hosting.models.Version` objects by
         :py:attr:`project_id`.
 
         Returns:
             A filtered :py:class:`QuerySet` on :py:class:`sphinx_hosting.models.Version`
         """
-        print(f'PROJECT_ID: {self.project_id}')
-        qs = super().get_initial_queryset().filter(project_id=self.project_id)
-        return qs.order_by('-version')
+        return super().get_initial_queryset().filter(project_id=self.project_id)
 
     def render_num_pages_column(self, row: Version, column: str) -> str:
         """
         Render our ``num_pages`` column.  This is the number of
         :py:class:`sphinx_hosting.models.SphinxPage` objects imported for this
         version.
```

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.1.0/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

