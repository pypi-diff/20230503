# Comparing `tmp/dynamic_listing-0.0.4.tar.gz` & `tmp/dynamic_listing-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_listing-0.0.4.tar", last modified: Mon Mar 20 18:44:28 2023, max compression
+gzip compressed data, was "dynamic_listing-0.0.5.tar", last modified: Tue May  2 22:46:45 2023, max compression
```

## Comparing `dynamic_listing-0.0.4.tar` & `dynamic_listing-0.0.5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.107272 dynamic_listing-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/dynamic_listing.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-20 18:44:28.107272 dynamic_listing-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/blog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/blog/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/blog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/blog/templates/blog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/blog/templates/blog/table/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/templates/blog/table/_table_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/blog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/dynamic_listing/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/dynamic_listing/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/dynamic_listing/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/dynamic_listing/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-20 18:44:28.107272 dynamic_listing-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/charts/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/charts/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/charts/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/filters/filter_field_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/filters/filter_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/src/dynamic_listing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/src/dynamic_listing/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.095271 dynamic_listing-0.0.4/src/dynamic_listing/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/5-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/charts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.099272 dynamic_listing-0.0.4/src/dynamic_listing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_no_data.html
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_table_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.107272 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.107272 dynamic_listing-0.0.4/src/dynamic_listing/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/templatetags/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-03-20 18:44:20.000000 dynamic_listing-0.0.4/src/dynamic_listing/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 18:44:28.103272 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-20 18:44:28.000000 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-20 18:44:28.000000 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 18:44:28.000000 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 18:44:28.000000 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-20 18:44:28.000000 dynamic_listing-0.0.4/src/dynamic_listing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/dynamic_listing.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/blog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/blog/templates/blog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/templates/blog/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/templates/blog/table/_table_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.322799 dynamic_listing-0.0.5/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.322799 dynamic_listing-0.0.5/src/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_field_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.330799 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.330799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_no_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.334799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.334799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/top_level.txt
```

### Comparing `dynamic_listing-0.0.4/.github/scripts/release.py` & `dynamic_listing-0.0.5/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/.gitignore` & `dynamic_listing-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/.idea/dynamic_listing.iml` & `dynamic_listing-0.0.5/.idea/dynamic_listing.iml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/.idea/inspectionProfiles/Project_Default.xml` & `dynamic_listing-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/LICENSE` & `dynamic_listing-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/blog/factory.py` & `dynamic_listing-0.0.5/blog/factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/blog/migrations/0001_initial.py` & `dynamic_listing-0.0.5/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/blog/models.py` & `dynamic_listing-0.0.5/blog/models.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/blog/views.py` & `dynamic_listing-0.0.5/blog/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/dynamic_listing/settings.py` & `dynamic_listing-0.0.5/dynamic_listing/settings.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/manage.py` & `dynamic_listing-0.0.5/manage.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/setup.cfg` & `dynamic_listing-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/charts/charts.py` & `dynamic_listing-0.0.5/src/dynamic_listing/charts/charts.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/charts/datasets.py` & `dynamic_listing-0.0.5/src/dynamic_listing/charts/datasets.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/filters/__init__.py` & `dynamic_listing-0.0.5/src/dynamic_listing/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/filters/filter_field_renderer.py` & `dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_field_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/filters/filter_renderer.py` & `dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/filters/filters.py` & `dynamic_listing-0.0.5/src/dynamic_listing/filters/filters.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po` & `dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-16 01:40+0200\n"
+"POT-Creation-Date: 2023-05-03 01:40+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: filters/__init__.py:19 filters/__init__.py:25 filters/__init__.py:31
-#: filters/__init__.py:37
+#: filters/__init__.py:20 filters/__init__.py:26 filters/__init__.py:32
+#: filters/__init__.py:38
 msgid " & Up"
 msgstr " فاعلى"
 
 #: filters/filters.py:12
 #, python-format
 msgid "%s Descending"
 msgstr "%s من الاعلى الى الاقل"
@@ -39,11 +39,16 @@
 msgid "No items found."
 msgstr "لا يوجد محتوى"
 
 #: templates/dynamic_listing/_no_data.html:4
 msgid "No Items Available"
 msgstr "لا يوجد محتوى"
 
-#: templates/dynamic_listing/filters/inline_filter.html:22
+#: templates/dynamic_listing/_pagination.html:8
+#, python-format
+msgid "Showing %(start)s-%(end)s of total result %(count)s"
+msgstr "إظهار %(start)s-%(end)s من اجمالى النتائج %(count)s"
+
+#: templates/dynamic_listing/filters/inline_filter.html:26
 #: templates/dynamic_listing/filters/side_filter.html:9
 msgid "Clear Filters"
 msgstr "الغاء الترشيحات"
```

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/5-dark.png` & `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5-dark.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/5.png` & `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/charts.js` & `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/charts.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/static/dynamic_listing/filters.js` & `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/filters.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_grid.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_grid.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_list.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_list.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_pagination.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_pagination.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+{% load i18n %}
 {% if paginator.num_pages > 1 %}
   <div class="row">
+
     <div
-        class="col-sm-12 col-md-5 d-flex align-items-center justify-content-center justify-content-md-start"></div>
+        class="col-sm-12 col-md-5 d-flex align-items-center justify-content-center justify-content-md-start">
+      <p class="text-gray-700">
+        {% blocktrans with start=page_obj.start_index end=page_obj.end_index count=page_obj.paginator.count %}Showing {{ start }}-{{ end }} of total result {{ count }}{% endblocktrans %}
+      </p>
+    </div>
     <div class="col-sm-12 col-md-7 d-flex align-items-center justify-content-center justify-content-md-end">
       <div class="dataTables_paginate paging_simple_numbers" id="kt_table_users_paginate">
         <ul class="pagination">
           {% if page_obj.has_previous %}
             <li class="paginate_button page-item previous" id="kt_table_users_previous">
-              <a href="?page={{ page_obj.previous_page_number }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
+              <a href="?page=
+
+
+                  {{ page_obj.previous_page_number }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
                  aria-controls="kt_table_users"
                  data-dt-idx="0"
                  tabindex="0"
                  class="page-link"><i
                   class="previous"></i></a></li>
           {% else %}
             <li class="paginate_button page-item previous disabled" id="kt_table_users_previous">
@@ -27,23 +36,29 @@
             {% if page_number == page_obj.paginator.ELLIPSIS %}
               <li class="paginate_button page-item">
                 <a href="#" aria-controls="kt_table_users"
                    data-dt-idx="{{ page_num }}" tabindex="0" class="page-link">{{ page_num }}</a>
               </li>
             {% else %}
               <li class="paginate_button page-item {% if page_obj.number == page_num %} active{% endif %} ">
-                <a href="?page={{ page_num }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
+                <a href="?page=
+
+
+                    {{ page_num }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
                    aria-controls="kt_table_users" data-dt-idx="{{ page_num }}"
                    tabindex="0" class="page-link">{{ page_num }}</a></li>
             {% endif %}
           {% endfor %}
 
           {% if page_obj.has_next %}
             <li class="paginate_button page-item next" id="kt_table_users_next">
-              <a href="?page={{ page_obj.next_page_number }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
+              <a href="?page=
+
+
+                  {{ page_obj.next_page_number }}{% for key, value in request.GET.items %}{% if key != 'page' %}&{{ key }}={{ value }}{% endif %}{% endfor %}"
                  aria-controls="kt_table_users"
                  data-dt-idx="4" tabindex="0"
                  class="page-link"><i
                   class="next"></i></a></li>
           {% else %}
             <li class="paginate_button page-item next" id="kt_table_users_next">
               <a href="#"
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-{% if paginator.num_pages > 1 %}
+{% load i18n %} {% if paginator.num_pages > 1 %}
+{% blocktrans with start=page_obj.start_index end=page_obj.end_index
+count=page_obj.paginator.count %}Showing {{ start }}-{{ end }} of total result
+{{ count }}{% endblocktrans %}
     * {% if page_obj.has_previous %}
     * {% else %}
     * {% endif %} {% for page_num in paginator.get_elided_page_range %} {% if
       page_number == page_obj.paginator.ELLIPSIS %}
     * {{_page_num_}}
     * {% else %}
     * {{_page_num_}}
```

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_table.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/_table_view.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table_view.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/templates/dynamic_listing/index.html` & `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/index.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing/views.py` & `dynamic_listing-0.0.5/src/dynamic_listing/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.4/src/dynamic_listing.egg-info/SOURCES.txt` & `dynamic_listing-0.0.5/src/dynamic_listing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

