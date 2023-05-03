# Comparing `tmp/jnt_django_toolbox-0.9.7.tar.gz` & `tmp/jnt_django_toolbox-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jnt_django_toolbox-0.9.7.tar", max compression
+gzip compressed data, was "jnt_django_toolbox-0.9.8.tar", max compression
```

## Comparing `jnt_django_toolbox-0.9.7.tar` & `jnt_django_toolbox-0.9.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0     1275 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/__init__.py
--rw-r--r--   0        0        0     4871 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/content_type.py
--rw-r--r--   0        0        0       45 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/fields/__init__.py
--rw-r--r--   0        0        0     1020 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/fields/changelist.py
--rw-r--r--   0        0        0       45 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/filters/__init__.py
--rw-r--r--   0        0        0     5012 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/filters/autocomplete.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/__init__.py
--rw-r--r--   0        0        0      193 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/__init__.py
--rw-r--r--   0        0        0      329 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/__init__.py
--rw-r--r--   0        0        0      219 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/base.py
--rw-r--r--   0        0        0      421 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/boolean.py
--rw-r--r--   0        0        0      610 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/foreign_key.py
--rw-r--r--   0        0        0      780 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/generic_foreign_key.py
--rw-r--r--   0        0        0      613 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/many_to_many.py
--rw-r--r--   0        0        0      893 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/permissions_readonly.py
--rw-r--r--   0        0        0      618 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/string_field.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/helpers/__init__.py
--rw-r--r--   0        0        0     3566 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/helpers/urls.py
--rw-r--r--   0        0        0      537 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/helpers/widgets.py
--rw-r--r--   0        0        0      445 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/__init__.py
--rw-r--r--   0        0        0      277 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/autocomplete.py
--rw-r--r--   0        0        0      912 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/autocomplete_changelist_filters.py
--rw-r--r--   0        0        0     3212 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/autocomplete_fields.py
--rw-r--r--   0        0        0      275 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/base.py
--rw-r--r--   0        0        0     1660 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/clickable_links.py
--rw-r--r--   0        0        0     6582 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/generic_foreign_key.py
--rw-r--r--   0        0        0     1267 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/generic_foreign_key_inline.py
--rw-r--r--   0        0        0     2023 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/readonly_widgets.py
--rw-r--r--   0        0        0      201 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     3508 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/autocomplete.py
--rw-r--r--   0        0        0     3647 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_admin_page.py
--rw-r--r--   0        0        0     1452 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_instance_model_admin_page.py
--rw-r--r--   0        0        0     1764 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_model_admin_page.py
--rw-r--r--   0        0        0      199 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/apps.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/consts/__init__.py
--rw-r--r--   0        0        0      229 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/consts/time.py
--rw-r--r--   0        0        0       37 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/context_managers/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/context_managers/global_lock.py
--rw-r--r--   0        0        0       37 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/decorators/__init__.py
--rw-r--r--   0        0        0      381 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/decorators/one_at_time.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/__init__.py
--rw-r--r--   0        0        0       59 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/fields/__init__.py
--rw-r--r--   0        0        0      439 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/fields/enum.py
--rw-r--r--   0        0        0     1223 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/fields/permissions.py
--rw-r--r--   0        0        0      193 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/__init__.py
--rw-r--r--   0        0        0     3699 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/autocomplete_select.py
--rw-r--r--   0        0        0     2282 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/generic_foreign_key.py
--rw-r--r--   0        0        0     3820 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/permissions.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/__init__.py
--rw-r--r--   0        0        0     1707 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/date.py
--rw-r--r--   0        0        0     1030 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/dicts.py
--rw-r--r--   0        0        0      132 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/files.py
--rw-r--r--   0        0        0      284 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/media.py
--rw-r--r--   0        0        0      279 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/model.py
--rw-r--r--   0        0        0      425 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/modules.py
--rw-r--r--   0        0        0     3309 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/object_links.py
--rw-r--r--   0        0        0      834 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/objects.py
--rw-r--r--   0        0        0     1655 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/readonly_form_field.py
--rw-r--r--   0        0        0      356 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/requests.py
--rw-r--r--   0        0        0     1639 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/text.py
--rw-r--r--   0        0        0      140 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/time.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0      622 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/commands/migrate_concurrently.py
--rw-r--r--   0        0        0      600 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/commands/reset_migrate_lock.py
--rw-r--r--   0        0        0       27 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/__init__.py
--rw-r--r--   0        0        0      124 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/__init__.py
--rw-r--r--   0        0        0      846 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/enum.py
--rw-r--r--   0        0        0     1090 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/flag_array.py
--rw-r--r--   0        0        0     1016 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/generic_foreign_key.py
--rw-r--r--   0        0        0       42 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/widgets/__init__.py
--rw-r--r--   0        0        0     1533 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/widgets/flags_array.py
--rw-r--r--   0        0        0      218 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/query.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/db/__init__.py
--rw-r--r--   0        0        0     5749 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/db/jaeger.py
--rw-r--r--   0        0        0     2233 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/db/wrapper.py
--rw-r--r--   0        0        0       35 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/decorators/__init__.py
--rw-r--r--   0        0        0     1669 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/decorators/trace_span.py
--rw-r--r--   0        0        0      695 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/middleware.py
--rw-r--r--   0        0        0      232 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/__init__.py
--rw-r--r--   0        0        0      478 2023-05-03 11:35:18.355380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/base.py
--rw-r--r--   0        0        0     2271 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/cache_calls.py
--rw-r--r--   0        0        0     1185 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/db_queries.py
--rw-r--r--   0        0        0     1496 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/jaeger.py
--rw-r--r--   0        0        0      718 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/requests.py
--rw-r--r--   0        0        0       66 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/css/autocomplete_filter/autocomplete-fix.css
--rw-r--r--   0        0        0      393 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/flags-array.css
--rw-r--r--   0        0        0      702 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/generic-foreign-key-field.css
--rw-r--r--   0        0        0       64 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/permissions.css
--rw-r--r--   0        0        0     2326 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/images/icon-broom.svg
--rw-r--r--   0        0        0     2331 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/autocomplete_filter/autocomplete-filter.js
--rw-r--r--   0        0        0     2317 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/autocomplete.js
--rw-r--r--   0        0        0     1884 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/flags-array.js
--rw-r--r--   0        0        0     8561 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/generic-foreign-key-field.js
--rw-r--r--   0        0        0     1912 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/admin/admin_page.html
--rw-r--r--   0        0        0      242 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/autocomplete_filter/autocomplete_filter.html
--rw-r--r--   0        0        0      616 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/flags_array.html
--rw-r--r--   0        0        0      810 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/generic_foreign_key.html
--rw-r--r--   0        0        0     3532 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/permissions.html
--rw-r--r--   0        0        0        0 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      295 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templatetags/order_by.py
--rw-r--r--   0        0        0      256 2023-05-03 11:35:18.359380 jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templatetags/permissions_widget_tags.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 jnt_django_toolbox-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1275 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0     4871 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/content_type.py
+-rw-r--r--   0        0        0       45 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/fields/__init__.py
+-rw-r--r--   0        0        0     1020 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/fields/changelist.py
+-rw-r--r--   0        0        0       45 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/filters/__init__.py
+-rw-r--r--   0        0        0     5012 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/filters/autocomplete.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/__init__.py
+-rw-r--r--   0        0        0      329 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-03 11:55:36.164127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/base.py
+-rw-r--r--   0        0        0      421 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/boolean.py
+-rw-r--r--   0        0        0      610 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/foreign_key.py
+-rw-r--r--   0        0        0      780 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/generic_foreign_key.py
+-rw-r--r--   0        0        0      613 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/many_to_many.py
+-rw-r--r--   0        0        0      893 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/permissions_readonly.py
+-rw-r--r--   0        0        0      618 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/string_field.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/helpers/__init__.py
+-rw-r--r--   0        0        0     3566 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/helpers/urls.py
+-rw-r--r--   0        0        0      537 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/helpers/widgets.py
+-rw-r--r--   0        0        0      445 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/autocomplete.py
+-rw-r--r--   0        0        0      912 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/autocomplete_changelist_filters.py
+-rw-r--r--   0        0        0     3212 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/autocomplete_fields.py
+-rw-r--r--   0        0        0      275 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/base.py
+-rw-r--r--   0        0        0     1660 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/clickable_links.py
+-rw-r--r--   0        0        0     6582 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/generic_foreign_key.py
+-rw-r--r--   0        0        0     1267 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/generic_foreign_key_inline.py
+-rw-r--r--   0        0        0     2023 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/readonly_widgets.py
+-rw-r--r--   0        0        0      201 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     3508 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/autocomplete.py
+-rw-r--r--   0        0        0     3647 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_admin_page.py
+-rw-r--r--   0        0        0     1452 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_instance_model_admin_page.py
+-rw-r--r--   0        0        0     1764 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_model_admin_page.py
+-rw-r--r--   0        0        0      199 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/apps.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/consts/__init__.py
+-rw-r--r--   0        0        0      229 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/consts/time.py
+-rw-r--r--   0        0        0       37 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/context_managers/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/context_managers/global_lock.py
+-rw-r--r--   0        0        0       37 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/decorators/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/decorators/one_at_time.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/fields/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/fields/enum.py
+-rw-r--r--   0        0        0     1223 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/fields/permissions.py
+-rw-r--r--   0        0        0      193 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/__init__.py
+-rw-r--r--   0        0        0     3699 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/autocomplete_select.py
+-rw-r--r--   0        0        0     2282 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/generic_foreign_key.py
+-rw-r--r--   0        0        0     3820 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/__init__.py
+-rw-r--r--   0        0        0     1707 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/date.py
+-rw-r--r--   0        0        0     1030 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/dicts.py
+-rw-r--r--   0        0        0      132 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/files.py
+-rw-r--r--   0        0        0      284 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/media.py
+-rw-r--r--   0        0        0      279 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/model.py
+-rw-r--r--   0        0        0      425 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/modules.py
+-rw-r--r--   0        0        0     3309 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/object_links.py
+-rw-r--r--   0        0        0      834 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/objects.py
+-rw-r--r--   0        0        0     1655 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/readonly_form_field.py
+-rw-r--r--   0        0        0      356 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/requests.py
+-rw-r--r--   0        0        0     1639 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/text.py
+-rw-r--r--   0        0        0      140 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/time.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/commands/migrate_concurrently.py
+-rw-r--r--   0        0        0      600 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/commands/reset_migrate_lock.py
+-rw-r--r--   0        0        0       27 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/__init__.py
+-rw-r--r--   0        0        0      846 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/enum.py
+-rw-r--r--   0        0        0     1090 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/flag_array.py
+-rw-r--r--   0        0        0     1016 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/generic_foreign_key.py
+-rw-r--r--   0        0        0       42 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/widgets/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/widgets/flags_array.py
+-rw-r--r--   0        0        0      218 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/query.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/db/__init__.py
+-rw-r--r--   0        0        0     5749 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/db/jaeger.py
+-rw-r--r--   0        0        0     2233 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/db/wrapper.py
+-rw-r--r--   0        0        0       35 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/decorators/__init__.py
+-rw-r--r--   0        0        0     1669 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/decorators/trace_span.py
+-rw-r--r--   0        0        0      695 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/middleware.py
+-rw-r--r--   0        0        0      232 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/base.py
+-rw-r--r--   0        0        0     2271 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/cache_calls.py
+-rw-r--r--   0        0        0     1185 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/db_queries.py
+-rw-r--r--   0        0        0     1496 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/jaeger.py
+-rw-r--r--   0        0        0      718 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/requests.py
+-rw-r--r--   0        0        0       66 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/css/autocomplete_filter/autocomplete-fix.css
+-rw-r--r--   0        0        0      393 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/flags-array.css
+-rw-r--r--   0        0        0      702 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/generic-foreign-key-field.css
+-rw-r--r--   0        0        0       64 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/permissions.css
+-rw-r--r--   0        0        0     2326 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/images/icon-broom.svg
+-rw-r--r--   0        0        0     2331 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/autocomplete_filter/autocomplete-filter.js
+-rw-r--r--   0        0        0     2317 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/autocomplete.js
+-rw-r--r--   0        0        0     1884 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/flags-array.js
+-rw-r--r--   0        0        0     8561 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/generic-foreign-key-field.js
+-rw-r--r--   0        0        0     1912 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/admin/admin_page.html
+-rw-r--r--   0        0        0      242 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/autocomplete_filter/autocomplete_filter.html
+-rw-r--r--   0        0        0      616 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/flags_array.html
+-rw-r--r--   0        0        0      810 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/generic_foreign_key.html
+-rw-r--r--   0        0        0     3532 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/permissions.html
+-rw-r--r--   0        0        0        0 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-03 11:55:36.168127 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templatetags/order_by.py
+-rw-r--r--   0        0        0      256 2023-05-03 11:55:36.172128 jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templatetags/permissions_widget_tags.py
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 jnt_django_toolbox-0.9.8/PKG-INFO
```

### Comparing `jnt_django_toolbox-0.9.7/pyproject.toml` & `jnt_django_toolbox-0.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jnt-django-toolbox"
-version = "0.9.7"
+version = "0.9.8"
 description = ""
 authors = ["junte <tech@junte.ru>"]
 classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/content_type.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/content_type.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/fields/changelist.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/fields/changelist.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/filters/autocomplete.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/filters/autocomplete.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/foreign_key.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/foreign_key.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/generic_foreign_key.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/generic_foreign_key.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/many_to_many.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/many_to_many.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/permissions_readonly.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/permissions_readonly.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/forms/widgets/readonly/string_field.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/forms/widgets/readonly/string_field.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/helpers/urls.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/helpers/widgets.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/helpers/widgets.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/autocomplete_changelist_filters.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/autocomplete_changelist_filters.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/autocomplete_fields.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/autocomplete_fields.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/clickable_links.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/clickable_links.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/generic_foreign_key.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/generic_foreign_key.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/generic_foreign_key_inline.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/generic_foreign_key_inline.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/mixins/readonly_widgets.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/mixins/readonly_widgets.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/autocomplete.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_admin_page.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_admin_page.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_instance_model_admin_page.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_instance_model_admin_page.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/admin/views/base_model_admin_page.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/admin/views/base_model_admin_page.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/context_managers/global_lock.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/context_managers/global_lock.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/fields/permissions.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/fields/permissions.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/autocomplete_select.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/autocomplete_select.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/generic_foreign_key.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/generic_foreign_key.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/forms/widgets/permissions.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/forms/widgets/permissions.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/date.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/date.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/dicts.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/dicts.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/object_links.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/object_links.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/objects.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/objects.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/readonly_form_field.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/readonly_form_field.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/helpers/text.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/helpers/text.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/commands/migrate_concurrently.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/commands/migrate_concurrently.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/management/commands/reset_migrate_lock.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/management/commands/reset_migrate_lock.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/enum.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/enum.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/flag_array.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/flag_array.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/generic_foreign_key.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/generic_foreign_key.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/models/fields/widgets/flags_array.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/models/fields/widgets/flags_array.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/db/jaeger.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/db/jaeger.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/db/wrapper.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/db/wrapper.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/decorators/trace_span.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/decorators/trace_span.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/middleware.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/middleware.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/cache_calls.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/cache_calls.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/db_queries.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/db_queries.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/jaeger.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/jaeger.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/profiling/profilers/requests.py` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/profiling/profilers/requests.py`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/generic-foreign-key-field.css` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/css/widgets/generic-foreign-key-field.css`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/images/icon-broom.svg` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/images/icon-broom.svg`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/autocomplete_filter/autocomplete-filter.js` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/autocomplete_filter/autocomplete-filter.js`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/autocomplete.js` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/autocomplete.js`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/flags-array.js` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/flags-array.js`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/generic-foreign-key-field.js` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/static/jnt_django_toolbox/js/widgets/generic-foreign-key-field.js`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/admin/admin_page.html` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/admin/admin_page.html`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/flags_array.html` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/flags_array.html`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/generic_foreign_key.html` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/generic_foreign_key.html`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/permissions.html` & `jnt_django_toolbox-0.9.8/src/jnt_django_toolbox/templates/jnt_django_toolbox/widgets/permissions.html`

 * *Files identical despite different names*

### Comparing `jnt_django_toolbox-0.9.7/PKG-INFO` & `jnt_django_toolbox-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jnt-django-toolbox
-Version: 0.9.7
+Version: 0.9.8
 Summary: 
 Author: junte
 Author-email: tech@junte.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
```

