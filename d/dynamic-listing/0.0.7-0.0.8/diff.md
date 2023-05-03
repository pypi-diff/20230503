# Comparing `tmp/dynamic_listing-0.0.7.tar.gz` & `tmp/dynamic_listing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_listing-0.0.7.tar", last modified: Wed May  3 01:18:48 2023, max compression
+gzip compressed data, was "dynamic_listing-0.0.8.tar", last modified: Wed May  3 01:47:17 2023, max compression
```

## Comparing `dynamic_listing-0.0.7.tar` & `dynamic_listing-0.0.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.991664 dynamic_listing-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.999664 dynamic_listing-0.0.7/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.999664 dynamic_listing-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.999664 dynamic_listing-0.0.7/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/dynamic_listing.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.999664 dynamic_listing-0.0.7/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.999664 dynamic_listing-0.0.7/blog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.003664 dynamic_listing-0.0.7/blog/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/blog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/blog/templates/blog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.003664 dynamic_listing-0.0.7/blog/templates/blog/table/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/templates/blog/table/_table_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/blog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.003664 dynamic_listing-0.0.7/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/dynamic_listing/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/dynamic_listing/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/dynamic_listing/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/dynamic_listing/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.003664 dynamic_listing-0.0.7/src/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.007664 dynamic_listing-0.0.7/src/dynamic_listing/charts/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/charts/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/charts/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.007664 dynamic_listing-0.0.7/src/dynamic_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/filters/filter_field_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/filters/filter_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/src/dynamic_listing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.007664 dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/src/dynamic_listing/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.007664 dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/5-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/charts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:47.995664 dynamic_listing-0.0.7/src/dynamic_listing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_no_data.html
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_table_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.011664 dynamic_listing-0.0.7/src/dynamic_listing/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/templatetags/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-03 01:18:38.000000 dynamic_listing-0.0.7/src/dynamic_listing/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:18:48.007664 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 01:18:47.000000 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-03 01:18:47.000000 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:18:47.000000 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 01:18:47.000000 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 01:18:47.000000 dynamic_listing-0.0.7/src/dynamic_listing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.717200 dynamic_listing-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.697199 dynamic_listing-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/dynamic_listing.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 01:47:17.717200 dynamic_listing-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.705200 dynamic_listing-0.0.8/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.705200 dynamic_listing-0.0.8/blog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.697199 dynamic_listing-0.0.8/blog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.697199 dynamic_listing-0.0.8/blog/templates/blog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.705200 dynamic_listing-0.0.8/blog/templates/blog/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/templates/blog/table/_table_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/blog/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.705200 dynamic_listing-0.0.8/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/dynamic_listing/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/dynamic_listing/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/dynamic_listing/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/dynamic_listing/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-03 01:47:17.717200 dynamic_listing-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.697199 dynamic_listing-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.705200 dynamic_listing-0.0.8/src/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.709200 dynamic_listing-0.0.8/src/dynamic_listing/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/charts/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/charts/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.709200 dynamic_listing-0.0.8/src/dynamic_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/filters/filter_field_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/filters/filter_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/src/dynamic_listing/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.709200 dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/src/dynamic_listing/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.709200 dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/5-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.701200 dynamic_listing-0.0.8/src/dynamic_listing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.713200 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_no_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_table_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.713200 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.717200 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.717200 dynamic_listing-0.0.8/src/dynamic_listing/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/templatetags/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-03 01:47:08.000000 dynamic_listing-0.0.8/src/dynamic_listing/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:17.709200 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 01:47:17.000000 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-03 01:47:17.000000 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:47:17.000000 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 01:47:17.000000 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 01:47:17.000000 dynamic_listing-0.0.8/src/dynamic_listing.egg-info/top_level.txt
```

### Comparing `dynamic_listing-0.0.7/.github/scripts/release.py` & `dynamic_listing-0.0.8/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/.gitignore` & `dynamic_listing-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/.idea/dynamic_listing.iml` & `dynamic_listing-0.0.8/.idea/dynamic_listing.iml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/.idea/inspectionProfiles/Project_Default.xml` & `dynamic_listing-0.0.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/LICENSE` & `dynamic_listing-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/PKG-INFO` & `dynamic_listing-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_listing
-Version: 0.0.7
+Version: 0.0.8
 Summary: Django package provides easy way to create listing, filters, and charts.
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `dynamic_listing-0.0.7/blog/factory.py` & `dynamic_listing-0.0.8/blog/factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/blog/migrations/0001_initial.py` & `dynamic_listing-0.0.8/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/blog/models.py` & `dynamic_listing-0.0.8/blog/models.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/blog/views.py` & `dynamic_listing-0.0.8/blog/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/dynamic_listing/settings.py` & `dynamic_listing-0.0.8/dynamic_listing/settings.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/manage.py` & `dynamic_listing-0.0.8/manage.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/setup.cfg` & `dynamic_listing-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/charts/charts.py` & `dynamic_listing-0.0.8/src/dynamic_listing/charts/charts.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/charts/datasets.py` & `dynamic_listing-0.0.8/src/dynamic_listing/charts/datasets.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/filters/__init__.py` & `dynamic_listing-0.0.8/src/dynamic_listing/filters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils.safestring import mark_safe
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from .filter_field_renderer import *
 from .filter_renderer import *
 from .filters import *
 
 
 class FilterSet(django_filters.FilterSet):
```

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/filters/filter_field_renderer.py` & `dynamic_listing-0.0.8/src/dynamic_listing/filters/filter_field_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/filters/filter_renderer.py` & `dynamic_listing-0.0.8/src/dynamic_listing/filters/filter_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/filters/filters.py` & `dynamic_listing-0.0.8/src/dynamic_listing/filters/filters.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo` & `dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po` & `dynamic_listing-0.0.8/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/5-dark.png` & `dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/5-dark.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/5.png` & `dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/5.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/charts.js` & `dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/charts.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/static/dynamic_listing/filters.js` & `dynamic_listing-0.0.8/src/dynamic_listing/static/dynamic_listing/filters.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_grid.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_grid.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_list.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_list.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_pagination.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_pagination.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_table.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_table.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/_table_view.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/_table_view.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/templates/dynamic_listing/index.html` & `dynamic_listing-0.0.8/src/dynamic_listing/templates/dynamic_listing/index.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing/views.py` & `dynamic_listing-0.0.8/src/dynamic_listing/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing.egg-info/PKG-INFO` & `dynamic_listing-0.0.8/src/dynamic_listing.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-listing
-Version: 0.0.7
+Version: 0.0.8
 Summary: Django package provides easy way to create listing, filters, and charts.
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `dynamic_listing-0.0.7/src/dynamic_listing.egg-info/SOURCES.txt` & `dynamic_listing-0.0.8/src/dynamic_listing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

