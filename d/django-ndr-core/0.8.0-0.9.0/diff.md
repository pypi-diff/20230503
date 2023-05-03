# Comparing `tmp/django-ndr-core-0.8.0.tar.gz` & `tmp/django-ndr-core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ndr-core-0.8.0.tar", last modified: Wed Apr 26 15:22:59 2023, max compression
+gzip compressed data, was "django-ndr-core-0.9.0.tar", last modified: Wed Apr 26 15:32:30 2023, max compression
```

## Comparing `django-ndr-core-0.8.0.tar` & `django-ndr-core-0.9.0.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.040842 django-ndr-core-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-26 15:22:59.040842 django-ndr-core-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.964840 django-ndr-core-0.8.0/ndr_core/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.968840 django-ndr-core-0.8.0/ndr_core/admin_forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/admin_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/api_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/color_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/corrections_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/images_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/messages_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/page_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/result_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/sample_data_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/search_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/settings_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/ui_element_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/ui_style_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_forms/upload_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.972840 django-ndr-core-0.8.0/ndr_core/admin_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/admin_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/api_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/color_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/corrections_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/export_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/images_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/messages_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/page_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/result_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/sample_data_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/search_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/settings_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/ui_element_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/ui_style_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/admin_views/uploads_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.972840 django-ndr-core-0.8.0/ndr_core/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.976840 django-ndr-core-0.8.0/ndr_core/api/api_ninjas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/api_ninjas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/api_ninjas/api_ninjas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/api_ninjas/api_ninjas_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/base_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.976840 django-ndr-core-0.8.0/ndr_core/api/ddb_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/ddb_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/ddb_api/ddb_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/ddb_api/ddb_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.976840 django-ndr-core-0.8.0/ndr_core/api/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/mongodb/mongodb_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/mongodb/mongodb_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.976840 django-ndr-core-0.8.0/ndr_core/api/ndr_core/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/ndr_core/ndr_core_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api/ndr_core/ndr_core_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.976840 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-26 15:22:58.000000 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-26 15:22:58.000000 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:22:58.000000 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 15:22:58.000000 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 15:22:58.000000 django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.980840 django-ndr-core-0.8.0/ndr_core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/api_implementations.json
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/base_styles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/color_palettes.json
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/company_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/initial_values.json
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/person_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/fixtures/schemas.json
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/form_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/geo_ip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.948839 django-ndr-core-0.8.0/ndr_core/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.980840 django-ndr-core-0.8.0/ndr_core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/management/commands/clean_ndr_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/management/commands/init_ndr_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.984840 django-ndr-core-0.8.0/ndr_core/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0002_rename_ndrcoreresulttemplate_ndrcoreresultmapping_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0003_ndrcoresearchstatisticentry_search_no_results_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0004_ndrcoresearchfield_list_choices_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0005_ndrcoreupload_alter_ndrcoreuielement_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0006_ndrcoreapiconfiguration_api_repository_url_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0007_ndrcoresearchfield_lower_value_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0008_ndrcoresearchfield_use_in_csv_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/0009_ndrcoresearchconfiguration_search_has_compact_result_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40552 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/ndr_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/ndr_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/ndr_template_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.948839 django-ndr-core-0.8.0/ndr_core/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.952839 django-ndr-core-0.8.0/ndr_core/static/ndr_core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.996841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/
--rw-r--r--   0 runner    (1001) docker     (123)  5658305 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/GeoLite2-Country.mmdb
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/_TODO.txt
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/about_us.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.948839 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/app_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.996841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/app_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1757850 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/app_static/images/under_construction.png
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/color_template.css
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/combined_search.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/contact.html
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/filtered_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/flip_book.html
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/search.html
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.000841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/
--rw-r--r--   0 runner    (1001) docker     (123)   162017 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/color_palette.css
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/custom_select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_admin.css
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_default.css
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_left.css
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_top_fixed.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.000841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.000841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.008841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/api.png
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/correct.png
--rw-r--r--   0 runner    (1001) docker     (123)  1647486 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/data.png
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/elements.png
--rw-r--r--   0 runner    (1001) docker     (123)  1542871 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/images.png
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/messages.png
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/ndr.png
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/pages.png
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/search.png
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/style.png
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/view.png
--rw-r--r--   0 runner    (1001) docker     (123)  1523798 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/welcome.png
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_default.png
--rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_left.png
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_top_fixed.png
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.008841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.008841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/admin/form_preview.js
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/admin/page_create_edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    62440 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   100190 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jscolor.js
--rw-r--r--   0 runner    (1001) docker     (123)    62361 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jscolor.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.008841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/ui_js/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/ui_js/copy_to_clipboard.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.952839 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/masonry/
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/masonry/masonry.pkgd.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.952839 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.css
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.css
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.css
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.video.play.png
--rw-r--r--   0 runner    (1001) docker     (123)    89992 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.js
--rw-r--r--   0 runner    (1001) docker     (123)    44342 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/static/ndr_core/test_server_assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/test_server_assets/02_data.json
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/static/ndr_core/test_server_assets/test.json
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:58.952839 django-ndr-core-0.8.0/ndr_core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/templates/django_tables2/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/django_tables2/bootstrap4-responsive.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.012841 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.028842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/api_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/api_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/api_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/base_copy.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/change_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_api.html
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_colors.html
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_corrections.html
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_images.html
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_pages.html
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_sample_data.html
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_search.html
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_ui.html
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_ui_elements.html
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_uploads.html
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/dashboard_old.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.028842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/about.html
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/advanced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.032842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/api_ninjas.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/ddb.html
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/mongo_db.html
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/ndr_core.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis.html
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/corrections.html
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/messages.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.032842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/about.html
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/contact.html
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/flip_book_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/list_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/search_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/template_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/pages.html
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/results.html
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.032842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/api.html
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/search_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/ui_elements.html
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/ui_style.html
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help.html
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/image_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/image_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/image_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/image_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/logo_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/message_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/palette_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/palette_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/palette_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/palette_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/password_changed.html
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/sample_data_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/sample_data_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_field_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_field_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_field_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/setting_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/setting_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/setting_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/settings_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/ui_element_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/ui_element_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/ui_element_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/upload_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/upload_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/upload_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/view_statistics.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.032842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/base_header_tags.html
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.032842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_default.html
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_left.html
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_top_fixed.html
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/dummy.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/not_found.html
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/pagination.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.036842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/base_renderer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/base_renderer_orig.html
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/default_template.html
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/default_template_orig.html
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/historical_person.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.036842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/styles/renderer_transcription_and_fragment.html
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.036842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/figure.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/file-href.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/image_card.html
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/jumbotron.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/slideshow.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/under_construction.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.040842 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/utils/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templates/ndr_core/utils/sitemap.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:59.040842 django-ndr-core-0.8.0/ndr_core/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templatetags/ndr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/templatetags/ndr_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/ndr_core/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-26 15:22:59.040842 django-ndr-core-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 15:22:40.000000 django-ndr-core-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.492397 django-ndr-core-0.9.0/ndr_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.496397 django-ndr-core-0.9.0/ndr_core/admin_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/admin_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/api_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/color_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/corrections_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/images_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/messages_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/page_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/result_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/sample_data_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/search_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/settings_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/ui_element_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/ui_style_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_forms/upload_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/admin_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/admin_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/color_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/corrections_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/export_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/images_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/messages_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/page_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/result_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/sample_data_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/search_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/settings_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/ui_element_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/ui_style_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/admin_views/uploads_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/api/api_ninjas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/api_ninjas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/api_ninjas/api_ninjas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/api_ninjas/api_ninjas_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/base_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/api/ddb_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/ddb_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/ddb_api/ddb_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/ddb_api/ddb_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/api/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/mongodb/mongodb_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/mongodb/mongodb_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.500397 django-ndr-core-0.9.0/ndr_core/api/ndr_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/ndr_core/ndr_core_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api/ndr_core/ndr_core_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.504397 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-26 15:32:30.000000 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-26 15:32:30.000000 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:32:30.000000 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 15:32:30.000000 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 15:32:30.000000 django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.504397 django-ndr-core-0.9.0/ndr_core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/api_implementations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/base_styles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/color_palettes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/company_instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/initial_values.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/person_instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/fixtures/schemas.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/form_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/geo_ip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.504397 django-ndr-core-0.9.0/ndr_core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/management/commands/clean_ndr_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/management/commands/init_ndr_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.508397 django-ndr-core-0.9.0/ndr_core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0002_rename_ndrcoreresulttemplate_ndrcoreresultmapping_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0003_ndrcoresearchstatisticentry_search_no_results_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0004_ndrcoresearchfield_list_choices_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0005_ndrcoreupload_alter_ndrcoreuielement_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0006_ndrcoreapiconfiguration_api_repository_url_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0007_ndrcoresearchfield_lower_value_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0008_ndrcoresearchfield_use_in_csv_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/0009_ndrcoresearchconfiguration_search_has_compact_result_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40552 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/ndr_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/ndr_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/ndr_template_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.516397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/
+-rw-r--r--   0 runner    (1001) docker     (123)  5658305 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/GeoLite2-Country.mmdb
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/_TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/about_us.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/app_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.516397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/app_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1757850 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/app_static/images/under_construction.png
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/color_template.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/combined_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/filtered_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/flip_book.html
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.520398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   162017 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/color_palette.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/custom_select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_admin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_left.css
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_top_fixed.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.520398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.520398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.528397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/api.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/correct.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1647486 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/data.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/elements.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1542871 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/images.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/messages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/ndr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/pages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/search.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/style.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/view.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1523798 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/welcome.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_default.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_top_fixed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.532398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/admin/form_preview.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/admin/page_create_edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62440 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   100190 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jscolor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62361 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jscolor.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/ui_js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/ui_js/copy_to_clipboard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/masonry/
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/masonry/masonry.pkgd.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.484397 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.536398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.video.play.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89992 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44342 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.540398 django-ndr-core-0.9.0/ndr_core/static/ndr_core/test_server_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/test_server_assets/02_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/static/ndr_core/test_server_assets/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.488397 django-ndr-core-0.9.0/ndr_core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.540398 django-ndr-core-0.9.0/ndr_core/templates/django_tables2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/django_tables2/bootstrap4-responsive.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.540398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.552398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/api_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/api_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/api_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/base_copy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_api.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_colors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_corrections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_sample_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_ui.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_ui_elements.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_uploads.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/dashboard_old.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.552398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/advanced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.552398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/api_ninjas.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/ddb.html
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/mongo_db.html
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/ndr_core.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/corrections.html
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/messages.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.556398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/flip_book_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/list_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/search_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/template_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.556398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/api.html
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/ui_elements.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/ui_style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/image_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/image_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/image_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/image_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/logo_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/message_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/palette_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/palette_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/palette_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/palette_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/password_changed.html
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/sample_data_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/sample_data_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_field_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_field_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_field_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/setting_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/setting_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/setting_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/settings_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/ui_element_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/ui_element_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/ui_element_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/upload_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/upload_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/upload_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/view_statistics.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.556398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/base_header_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.556398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_default.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_top_fixed.html
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/dummy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/not_found.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/pagination.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.556398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/base_renderer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/base_renderer_orig.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/default_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/default_template_orig.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/historical_person.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/styles/renderer_transcription_and_fragment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/figure.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/file-href.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/image_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/jumbotron.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/slideshow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/under_construction.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/utils/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templates/ndr_core/utils/sitemap.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/ndr_core/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templatetags/ndr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/templatetags/ndr_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/ndr_core/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 15:32:30.560398 django-ndr-core-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 15:32:08.000000 django-ndr-core-0.9.0/setup.py
```

### Comparing `django-ndr-core-0.8.0/LICENSE` & `django-ndr-core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/PKG-INFO` & `django-ndr-core-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-ndr-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Django app to search and view data from an API.
-Home-page: https://ndrcore.org/
+Home-page: https://django-ndr-core.readthedocs.io/en/latest/
 Author: Sorin Marti
 Author-email: sorin.marti@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-ndr-core-0.8.0/README.md` & `django-ndr-core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/admin_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/api_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/api_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/color_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/color_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/images_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/images_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/page_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/page_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/result_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/result_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/sample_data_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/sample_data_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/search_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/search_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/settings_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/settings_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/ui_element_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/ui_element_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_forms/upload_forms.py` & `django-ndr-core-0.9.0/ndr_core/admin_forms/upload_forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_tables.py` & `django-ndr-core-0.9.0/ndr_core/admin_tables.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/admin_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/api_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/api_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/color_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/color_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/corrections_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/corrections_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/export_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/export_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/images_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/images_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/messages_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/messages_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/page_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/page_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/result_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/result_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/sample_data_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/sample_data_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/search_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/search_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/settings_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/settings_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/ui_element_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/ui_element_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/ui_style_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/ui_style_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/admin_views/uploads_views.py` & `django-ndr-core-0.9.0/ndr_core/admin_views/uploads_views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/api_ninjas/api_ninjas_query.py` & `django-ndr-core-0.9.0/ndr_core/api/api_ninjas/api_ninjas_query.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/api_ninjas/api_ninjas_result.py` & `django-ndr-core-0.9.0/ndr_core/api/api_ninjas/api_ninjas_result.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/base_query.py` & `django-ndr-core-0.9.0/ndr_core/api/base_query.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/base_result.py` & `django-ndr-core-0.9.0/ndr_core/api/base_result.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/ddb_api/ddb_query.py` & `django-ndr-core-0.9.0/ndr_core/api/ddb_api/ddb_query.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/ddb_api/ddb_result.py` & `django-ndr-core-0.9.0/ndr_core/api/ddb_api/ddb_result.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/mongodb/mongodb_query.py` & `django-ndr-core-0.9.0/ndr_core/api/mongodb/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/mongodb/mongodb_result.py` & `django-ndr-core-0.9.0/ndr_core/api/mongodb/mongodb_result.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/ndr_core/ndr_core_query.py` & `django-ndr-core-0.9.0/ndr_core/api/ndr_core/ndr_core_query.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api/ndr_core/ndr_core_result.py` & `django-ndr-core-0.9.0/ndr_core/api/ndr_core/ndr_core_result.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/api_factory.py` & `django-ndr-core-0.9.0/ndr_core/api_factory.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/PKG-INFO` & `django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-ndr-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Django app to search and view data from an API.
-Home-page: https://ndrcore.org/
+Home-page: https://django-ndr-core.readthedocs.io/en/latest/
 Author: Sorin Marti
 Author-email: sorin.marti@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-ndr-core-0.8.0/ndr_core/django_ndr_core.egg-info/SOURCES.txt` & `django-ndr-core-0.9.0/ndr_core/django_ndr_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/api_implementations.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/api_implementations.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/base_styles.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/base_styles.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/color_palettes.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/color_palettes.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/initial_values.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/initial_values.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/person_instance.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/person_instance.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/fixtures/schemas.json` & `django-ndr-core-0.9.0/ndr_core/fixtures/schemas.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/form_preview.py` & `django-ndr-core-0.9.0/ndr_core/form_preview.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/forms.py` & `django-ndr-core-0.9.0/ndr_core/forms.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/geo_ip_utils.py` & `django-ndr-core-0.9.0/ndr_core/geo_ip_utils.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/management/commands/clean_ndr_core.py` & `django-ndr-core-0.9.0/ndr_core/management/commands/clean_ndr_core.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/management/commands/init_ndr_core.py` & `django-ndr-core-0.9.0/ndr_core/management/commands/init_ndr_core.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0001_initial.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0002_rename_ndrcoreresulttemplate_ndrcoreresultmapping_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0002_rename_ndrcoreresulttemplate_ndrcoreresultmapping_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0003_ndrcoresearchstatisticentry_search_no_results_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0003_ndrcoresearchstatisticentry_search_no_results_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0004_ndrcoresearchfield_list_choices_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0004_ndrcoresearchfield_list_choices_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0005_ndrcoreupload_alter_ndrcoreuielement_type.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0005_ndrcoreupload_alter_ndrcoreuielement_type.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0006_ndrcoreapiconfiguration_api_repository_url_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0006_ndrcoreapiconfiguration_api_repository_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0007_ndrcoresearchfield_lower_value_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0007_ndrcoresearchfield_lower_value_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/migrations/0009_ndrcoresearchconfiguration_search_has_compact_result_and_more.py` & `django-ndr-core-0.9.0/ndr_core/migrations/0009_ndrcoresearchconfiguration_search_has_compact_result_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/models.py` & `django-ndr-core-0.9.0/ndr_core/models.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/ndr_helpers.py` & `django-ndr-core-0.9.0/ndr_core/ndr_helpers.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/ndr_settings.py` & `django-ndr-core-0.9.0/ndr_core/ndr_settings.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/ndr_template_tags.py` & `django-ndr-core-0.9.0/ndr_core/ndr_template_tags.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/GeoLite2-Country.mmdb` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/GeoLite2-Country.mmdb`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/about_us.html` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/about_us.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/app_static/images/under_construction.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/app_static/images/under_construction.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/color_template.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/color_template.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/combined_search.html` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/combined_search.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/filtered_list.html` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/filtered_list.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/logo.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/logo.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/search.html` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/search.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/app_init/test.html` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/app_init/test.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/bootstrap.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/custom_select2.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/custom_select2.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_admin.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_admin.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_default.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_default.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/css/ndr_core_left.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/css/ndr_core_left.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/api.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/api.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/correct.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/correct.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/data.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/data.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/elements.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/elements.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/help.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/help.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/images.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/images.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/messages.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/messages.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/ndr.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/ndr.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/pages.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/pages.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/search.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/search.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/style.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/style.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/view.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/view.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/dashboard/welcome.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/dashboard/welcome.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/logo.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/logo.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_default.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_default.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_left.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_left.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/admin/style_top_fixed.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/admin/style_top_fixed.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/favicon.ico` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/images/logo.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/admin/form_preview.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/admin/form_preview.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/admin/page_create_edit.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/admin/page_create_edit.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/bootstrap.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jquery.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jscolor.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jscolor.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/jscolor.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/jscolor.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/popper.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/js/ui_js/copy_to_clipboard.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/js/ui_js/copy_to_clipboard.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/image-picker/image-picker.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/masonry/masonry.pkgd.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/masonry/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/LICENSE` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/README.md` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/README.md`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/ajax-loader.gif` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.min.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.carousel.min.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.min.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.default.min.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.min.css` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.theme.green.min.css`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.video.play.png` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/assets/owl.video.play.png`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.min.js` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/plugins/owl.carousel/dist/owl.carousel.min.js`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/test_server_assets/02_data.json` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/test_server_assets/02_data.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/static/ndr_core/test_server_assets/test.json` & `django-ndr-core-0.9.0/ndr_core/static/ndr_core/test_server_assets/test.json`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/django_tables2/bootstrap4-responsive.html` & `django-ndr-core-0.9.0/ndr_core/templates/django_tables2/bootstrap4-responsive.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/api_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/api_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/base.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/base.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/base_copy.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/base_copy.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_api.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_api.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_colors.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_colors.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_corrections.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_corrections.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_images.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_images.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_messages.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_messages.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_pages.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_pages.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_results.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_results.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_sample_data.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_sample_data.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_search.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_search.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_settings.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_settings.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_ui.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_ui.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_ui_elements.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_ui_elements.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/configure_uploads.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/configure_uploads.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/dashboard.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/dashboard_old.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/dashboard_old.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/advanced.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/advanced.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/api_ninjas.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/api_ninjas.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/apis/ddb.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/apis/ddb.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/corrections.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/corrections.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/images.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/images.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/messages.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/messages.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/about.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/about.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/contact.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/contact.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/flip_book_page.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/flip_book_page.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/list_page.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/list_page.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/search_page.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/search_page.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/page_types/template_page.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/page_types/template_page.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/pages.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/pages.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/api.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/search_configuration/api.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/settings.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/settings.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/statistics.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/statistics.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/ui_elements.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/ui_elements.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help/ui_style.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help/ui_style.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/help.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/help.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/image_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/image_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/message_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/message_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_create.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_create.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/page_edit.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/page_edit.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/palette_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/palette_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/password_changed.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/password_changed.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/sample_data_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/sample_data_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_create.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_create.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_config_edit.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_config_edit.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/search_field_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/search_field_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/setting_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/setting_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/ui_element_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/ui_element_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/ui_element_create.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/ui_element_create.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/upload_confirm_delete.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/upload_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/admin_views/view_statistics.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/admin_views/view_statistics.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/base_header_tags.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/base_header_tags.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/footer.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/footer.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_default.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_default.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_left.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_left.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/base/styles/base_top_fixed.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/base/styles/base_top_fixed.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/pagination.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/pagination.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/base_renderer.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/base_renderer.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/base_renderer_orig.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/base_renderer_orig.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/default_template.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/default_template.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/default_template_orig.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/default_template_orig.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/historical_person.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/historical_person.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/result_renderers/styles/renderer_transcription_and_fragment.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/result_renderers/styles/renderer_transcription_and_fragment.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/card.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/card.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/image_card.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/image_card.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/jumbotron.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/jumbotron.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/ui_elements/slideshow.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/ui_elements/slideshow.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templates/ndr_core/under_construction.html` & `django-ndr-core-0.9.0/ndr_core/templates/ndr_core/under_construction.html`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templatetags/ndr_utils.py` & `django-ndr-core-0.9.0/ndr_core/templatetags/ndr_utils.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/templatetags/ndr_values.py` & `django-ndr-core-0.9.0/ndr_core/templatetags/ndr_values.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/tests.py` & `django-ndr-core-0.9.0/ndr_core/tests.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/urls.py` & `django-ndr-core-0.9.0/ndr_core/urls.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/utils.py` & `django-ndr-core-0.9.0/ndr_core/utils.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/views.py` & `django-ndr-core-0.9.0/ndr_core/views.py`

 * *Files identical despite different names*

### Comparing `django-ndr-core-0.8.0/ndr_core/widgets.py` & `django-ndr-core-0.9.0/ndr_core/widgets.py`

 * *Files identical despite different names*

