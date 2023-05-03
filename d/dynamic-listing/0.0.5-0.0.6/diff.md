# Comparing `tmp/dynamic_listing-0.0.5.tar.gz` & `tmp/dynamic_listing-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_listing-0.0.5.tar", last modified: Tue May  2 22:46:45 2023, max compression
+gzip compressed data, was "dynamic_listing-0.0.6.tar", last modified: Tue May  2 23:05:19 2023, max compression
```

## Comparing `dynamic_listing-0.0.5.tar` & `dynamic_listing-0.0.6.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.314799 dynamic_listing-0.0.5/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/dynamic_listing.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/blog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/blog/templates/blog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.318799 dynamic_listing-0.0.5/blog/templates/blog/table/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/templates/blog/table/_table_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/blog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.322799 dynamic_listing-0.0.5/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/dynamic_listing/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.306799 dynamic_listing-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.322799 dynamic_listing-0.0.5/src/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/charts/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/charts/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_field_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.330799 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/charts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.310799 dynamic_listing-0.0.5/src/dynamic_listing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.330799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_no_data.html
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.334799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.334799 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.338799 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/templatetags/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-02 22:46:33.000000 dynamic_listing-0.0.5/src/dynamic_listing/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:46:45.326799 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 22:46:45.000000 dynamic_listing-0.0.5/src/dynamic_listing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.487851 dynamic_listing-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/dynamic_listing.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/blog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.487851 dynamic_listing-0.0.6/blog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.487851 dynamic_listing-0.0.6/blog/templates/blog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/blog/templates/blog/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/templates/blog/table/_table_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/blog/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/dynamic_listing/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/dynamic_listing/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/dynamic_listing/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/dynamic_listing/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 23:05:19.503852 dynamic_listing-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.491852 dynamic_listing-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/src/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/charts/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/charts/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/filters/filter_field_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/filters/filter_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.491852 dynamic_listing-0.0.6/src/dynamic_listing/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.491852 dynamic_listing-0.0.6/src/dynamic_listing/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.491852 dynamic_listing-0.0.6/src/dynamic_listing/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/5-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45102 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.491852 dynamic_listing-0.0.6/src/dynamic_listing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_no_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_table_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_toolbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.499852 dynamic_listing-0.0.6/src/dynamic_listing/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/templatetags/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-02 23:05:09.000000 dynamic_listing-0.0.6/src/dynamic_listing/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:05:19.495852 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 23:05:19.000000 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-02 23:05:19.000000 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:05:19.000000 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 23:05:19.000000 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 23:05:19.000000 dynamic_listing-0.0.6/src/dynamic_listing.egg-info/top_level.txt
```

### Comparing `dynamic_listing-0.0.5/.github/scripts/release.py` & `dynamic_listing-0.0.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/.gitignore` & `dynamic_listing-0.0.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
 
 # Translations
-*.mo
+#*.mo
 *.pot
 
 # Django stuff:
 *.log
 local_settings.py
 db.sqlite3
 db.sqlite3-journal
@@ -154,9 +154,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
+.idea/
```

### Comparing `dynamic_listing-0.0.5/.idea/dynamic_listing.iml` & `dynamic_listing-0.0.6/.idea/dynamic_listing.iml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `dynamic_listing-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/LICENSE` & `dynamic_listing-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/PKG-INFO` & `dynamic_listing-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_listing
-Version: 0.0.5
+Version: 0.0.6
 Summary: Django package provides easy way to create listing, filters, and charts.
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `dynamic_listing-0.0.5/blog/factory.py` & `dynamic_listing-0.0.6/blog/factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/blog/migrations/0001_initial.py` & `dynamic_listing-0.0.6/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/blog/models.py` & `dynamic_listing-0.0.6/blog/models.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/blog/views.py` & `dynamic_listing-0.0.6/blog/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/dynamic_listing/settings.py` & `dynamic_listing-0.0.6/dynamic_listing/settings.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/manage.py` & `dynamic_listing-0.0.6/manage.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/setup.cfg` & `dynamic_listing-0.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 package_dir = 
 	= src
 packages = find:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	django-filter >= 22.1
-	django-base-template >= 0.0.3
+	django-base-template >= 0.0.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/charts/charts.py` & `dynamic_listing-0.0.6/src/dynamic_listing/charts/charts.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/charts/datasets.py` & `dynamic_listing-0.0.6/src/dynamic_listing/charts/datasets.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/filters/__init__.py` & `dynamic_listing-0.0.6/src/dynamic_listing/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_field_renderer.py` & `dynamic_listing-0.0.6/src/dynamic_listing/filters/filter_field_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/filters/filter_renderer.py` & `dynamic_listing-0.0.6/src/dynamic_listing/filters/filter_renderer.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/filters/filters.py` & `dynamic_listing-0.0.6/src/dynamic_listing/filters/filters.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po` & `dynamic_listing-0.0.6/src/dynamic_listing/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5-dark.png` & `dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/5-dark.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/5.png` & `dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/5.png`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/charts.js` & `dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/charts.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/static/dynamic_listing/filters.js` & `dynamic_listing-0.0.6/src/dynamic_listing/static/dynamic_listing/filters.js`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_grid.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_grid.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_list.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_list.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_pagination.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_pagination.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_table.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/_table_view.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/_table_view.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/checkbox_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/date-range.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/radio_group.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/search.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/fields/sort.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/inline_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/side_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/filters/top_filter.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/templates/dynamic_listing/index.html` & `dynamic_listing-0.0.6/src/dynamic_listing/templates/dynamic_listing/index.html`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing/views.py` & `dynamic_listing-0.0.6/src/dynamic_listing/views.py`

 * *Files identical despite different names*

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing.egg-info/PKG-INFO` & `dynamic_listing-0.0.6/src/dynamic_listing.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-listing
-Version: 0.0.5
+Version: 0.0.6
 Summary: Django package provides easy way to create listing, filters, and charts.
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `dynamic_listing-0.0.5/src/dynamic_listing.egg-info/SOURCES.txt` & `dynamic_listing-0.0.6/src/dynamic_listing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 src/dynamic_listing/charts/__init__.py
 src/dynamic_listing/charts/charts.py
 src/dynamic_listing/charts/datasets.py
 src/dynamic_listing/filters/__init__.py
 src/dynamic_listing/filters/filter_field_renderer.py
 src/dynamic_listing/filters/filter_renderer.py
 src/dynamic_listing/filters/filters.py
+src/dynamic_listing/locale/ar/LC_MESSAGES/django.mo
 src/dynamic_listing/locale/ar/LC_MESSAGES/django.po
 src/dynamic_listing/static/dynamic_listing/5-dark.png
 src/dynamic_listing/static/dynamic_listing/5.png
 src/dynamic_listing/static/dynamic_listing/charts.js
 src/dynamic_listing/static/dynamic_listing/filters.js
 src/dynamic_listing/templates/dynamic_listing/_grid.html
 src/dynamic_listing/templates/dynamic_listing/_list.html
```

