# Comparing `tmp/graphene-django-3.0.1.tar.gz` & `tmp/graphene-django-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.0.1.tar", last modified: Sat Apr 29 17:28:06 2023, max compression
+gzip compressed data, was "graphene-django-3.0.2.tar", last modified: Wed May  3 09:17:01 2023, max compression
```

## Comparing `graphene-django-3.0.1.tar` & `graphene-django-3.0.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.901130 graphene-django-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-29 17:28:03.000000 graphene-django-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-29 17:28:03.000000 graphene-django-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 17:28:06.901130 graphene-django-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 17:28:03.000000 graphene-django-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-29 17:28:03.000000 graphene-django-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.889130 graphene-django-3.0.1/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    49752 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.889130 graphene-django-3.0.1/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-29 17:28:06.901130 graphene-django-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-29 17:28:03.000000 graphene-django-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 09:16:57.000000 graphene-django-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 09:16:57.000000 graphene-django-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-03 09:17:01.089644 graphene-django-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 09:16:57.000000 graphene-django-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-03 09:16:57.000000 graphene-django-3.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49752 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-03 09:17:01.089644 graphene-django-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-03 09:16:57.000000 graphene-django-3.0.2/setup.py
```

### Comparing `graphene-django-3.0.1/LICENSE` & `graphene-django-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/PKG-INFO` & `graphene-django-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.0.1
+Version: 3.0.2
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.0.1/README.md` & `graphene-django-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/README.rst` & `graphene-django-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/compat.py` & `graphene-django-3.0.2/graphene_django/compat.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/converter.py` & `graphene-django-3.0.2/graphene_django/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -311,34 +311,15 @@
     model = field.related_model
 
     def dynamic_type():
         _type = registry.get_type_for_model(model)
         if not _type:
             return
 
-        class CustomField(Field):
-            def wrap_resolve(self, parent_resolver):
-                """
-                Implements a custom resolver which go through the `get_node` method to ensure that
-                it goes through the `get_queryset` method of the DjangoObjectType.
-                """
-                resolver = super().wrap_resolve(parent_resolver)
-
-                def custom_resolver(root, info, **args):
-                    fk_obj = resolver(root, info, **args)
-                    if not isinstance(fk_obj, model):
-                        # In case the resolver is a custom one that overwrites
-                        # the default Django resolver
-                        # This happens, for example, when using custom awaitable resolvers.
-                        return fk_obj
-                    return _type.get_node(info, fk_obj.pk)
-
-                return custom_resolver
-
-        return CustomField(
+        return Field(
             _type,
             description=get_django_field_description(field),
             required=not field.null,
         )
 
     return Dynamic(dynamic_type)
```

### Comparing `graphene-django-3.0.1/graphene_django/debug/middleware.py` & `graphene-django-3.0.2/graphene_django/debug/middleware.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/debug/sql/tracking.py` & `graphene-django-3.0.2/graphene_django/debug/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/debug/sql/types.py` & `graphene-django-3.0.2/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/debug/tests/test_query.py` & `graphene-django-3.0.2/graphene_django/debug/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/fields.py` & `graphene-django-3.0.2/graphene_django/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/__init__.py` & `graphene-django-3.0.2/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/fields.py` & `graphene-django-3.0.2/graphene_django/filter/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/__init__.py` & `graphene-django-3.0.2/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.0.2/graphene_django/filter/filters/array_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.0.2/graphene_django/filter/filters/global_id_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.0.2/graphene_django/filter/filters/list_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.0.2/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.0.2/graphene_django/filter/filters/typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/filterset.py` & `graphene-django-3.0.2/graphene_django/filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/conftest.py` & `graphene-django-3.0.2/graphene_django/filter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/filters.py` & `graphene-django-3.0.2/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_in_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.0.2/graphene_django/filter/tests/test_typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/filter/utils.py` & `graphene-django-3.0.2/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/forms/converter.py` & `graphene-django-3.0.2/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/forms/forms.py` & `graphene-django-3.0.2/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/forms/mutation.py` & `graphene-django-3.0.2/graphene_django/forms/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.0.2/graphene_django/forms/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.0.2/graphene_django/forms/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.0.2/graphene_django/management/commands/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/registry.py` & `graphene-django-3.0.2/graphene_django/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/rest_framework/mutation.py` & `graphene-django-3.0.2/graphene_django/rest_framework/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.0.2/graphene_django/rest_framework/serializer_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/settings.py` & `graphene-django-3.0.2/graphene_django/settings.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/static/graphene_django/graphiql.js` & `graphene-django-3.0.2/graphene_django/static/graphene_django/graphiql.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -58,48 +58,35 @@
         location.origin.replace(/^http/, "ws") +
         (GRAPHENE_SETTINGS.subscriptionPath || location.pathname);
 
     function trueLambda() {
         return true;
     };
 
-    var fetcher = GraphiQL.createFetcher({
+    var headers = {};
+    var cookies = ("; " + document.cookie).split("; csrftoken=");
+    if (cookies.length == 2) {
+        csrftoken = cookies.pop().split(";").shift();
+    } else {
+        csrftoken = document.querySelector("[name=csrfmiddlewaretoken]").value;
+    }
+    if (csrftoken) {
+        headers['X-CSRFToken'] = csrftoken
+    }
+
+    var graphQLFetcher = GraphiQL.createFetcher({
         url: fetchURL,
         wsClient: graphqlWs.createClient({
             url: subscribeURL,
             shouldRetry: trueLambda,
             lazy: true,
-        })
+        }),
+        headers: headers
     })
 
-    function graphQLFetcher(graphQLParams, opts) {
-        if (typeof opts === 'undefined') {
-            opts = {};
-        }
-        var headers = opts.headers || {};
-        headers['Accept'] = headers['Accept'] || 'application/json';
-        headers['Content-Type'] = headers['Content-Type'] || 'application/json';
-
-        // Parse the cookie value for a CSRF token
-        var csrftoken;
-        var cookies = ("; " + document.cookie).split("; csrftoken=");
-        if (cookies.length == 2) {
-            csrftoken = cookies.pop().split(";").shift();
-        } else {
-            csrftoken = document.querySelector("[name=csrfmiddlewaretoken]").value;
-        }
-        if (csrftoken) {
-            headers['X-CSRFToken'] = csrftoken
-        }
-
-        opts.headers = headers
-
-        return fetcher(graphQLParams, opts)
-    }
-
     // When the query and variables string is edited, update the URL bar so
     // that it can be easily shared.
     function onEditQuery(newQuery) {
         parameters.query = newQuery;
         updateURL();
     }
```

### Comparing `graphene-django-3.0.1/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.0.2/graphene_django/templates/graphene/graphiql.html`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/issues/test_520.py` & `graphene-django-3.0.2/graphene_django/tests/issues/test_520.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/models.py` & `graphene-django-3.0.2/graphene_django/tests/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/schema.py` & `graphene-django-3.0.2/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/schema_view.py` & `graphene-django-3.0.2/graphene_django/tests/schema_view.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_command.py` & `graphene-django-3.0.2/graphene_django/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_converter.py` & `graphene-django-3.0.2/graphene_django/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_fields.py` & `graphene-django-3.0.2/graphene_django/tests/test_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import datetime
-from django.db.models import Count
+import re
+from django.db.models import Count, Prefetch
 
 import pytest
 
 from graphene import List, NonNull, ObjectType, Schema, String
 
 from ..fields import DjangoListField
 from ..types import DjangoObjectType
-from .models import Article as ArticleModel
-from .models import Reporter as ReporterModel
+from .models import (
+    Article as ArticleModel,
+    Film as FilmModel,
+    FilmDetails as FilmDetailsModel,
+    Reporter as ReporterModel,
+)
 
 
 class TestDjangoListField:
     def test_only_django_object_types(self):
         class TestType(ObjectType):
             foo = String()
 
@@ -496,7 +501,149 @@
             editor=r1,
         )
 
         result = schema.execute(query)
 
         assert not result.errors
         assert result.data == {"reporters": [{"firstName": "Tara"}]}
+
+    def test_select_related_and_prefetch_related_are_respected(
+        self, django_assert_num_queries
+    ):
+        class Article(DjangoObjectType):
+            class Meta:
+                model = ArticleModel
+                fields = ("headline", "editor", "reporter")
+
+        class Film(DjangoObjectType):
+            class Meta:
+                model = FilmModel
+                fields = ("genre", "details")
+
+        class FilmDetail(DjangoObjectType):
+            class Meta:
+                model = FilmDetailsModel
+                fields = ("location",)
+
+        class Reporter(DjangoObjectType):
+            class Meta:
+                model = ReporterModel
+                fields = ("first_name", "articles", "films")
+
+        class Query(ObjectType):
+            articles = DjangoListField(Article)
+
+            @staticmethod
+            def resolve_articles(root, info):
+                # Optimize for querying associated editors and reporters, and the films and film
+                # details of those reporters. This is similar to what would happen using a library
+                # like https://github.com/tfoxy/graphene-django-optimizer for a query like the one
+                # below (albeit simplified and hardcoded here).
+                return ArticleModel.objects.select_related(
+                    "editor", "reporter"
+                ).prefetch_related(
+                    Prefetch(
+                        "reporter__films",
+                        queryset=FilmModel.objects.select_related("details"),
+                    ),
+                )
+
+        schema = Schema(query=Query)
+
+        query = """
+            query {
+                articles {
+                    headline
+
+                    editor {
+                        firstName
+                    }
+
+                    reporter {
+                        firstName
+
+                        films {
+                            genre
+
+                            details {
+                                location
+                            }
+                        }
+                    }
+                }
+            }
+        """
+
+        r1 = ReporterModel.objects.create(first_name="Tara", last_name="West")
+        r2 = ReporterModel.objects.create(first_name="Debra", last_name="Payne")
+
+        ArticleModel.objects.create(
+            headline="Amazing news",
+            reporter=r1,
+            pub_date=datetime.date.today(),
+            pub_date_time=datetime.datetime.now(),
+            editor=r2,
+        )
+        ArticleModel.objects.create(
+            headline="Not so good news",
+            reporter=r2,
+            pub_date=datetime.date.today(),
+            pub_date_time=datetime.datetime.now(),
+            editor=r1,
+        )
+
+        film1 = FilmModel.objects.create(genre="ac")
+        film2 = FilmModel.objects.create(genre="ot")
+        film3 = FilmModel.objects.create(genre="do")
+        FilmDetailsModel.objects.create(location="Hollywood", film=film1)
+        FilmDetailsModel.objects.create(location="Antarctica", film=film3)
+        r1.films.add(film1, film2)
+        r2.films.add(film3)
+
+        # We expect 2 queries to be performed based on the above resolver definition: one for all
+        # articles joined with the reporters model (for associated editors and reporters), and one
+        # for the films prefetch (which includes its `select_related` JOIN logic in its queryset)
+        with django_assert_num_queries(2) as captured:
+            result = schema.execute(query)
+
+        assert not result.errors
+        assert result.data == {
+            "articles": [
+                {
+                    "headline": "Amazing news",
+                    "editor": {"firstName": "Debra"},
+                    "reporter": {
+                        "firstName": "Tara",
+                        "films": [
+                            {"genre": "AC", "details": {"location": "Hollywood"}},
+                            {"genre": "OT", "details": None},
+                        ],
+                    },
+                },
+                {
+                    "headline": "Not so good news",
+                    "editor": {"firstName": "Tara"},
+                    "reporter": {
+                        "firstName": "Debra",
+                        "films": [
+                            {"genre": "DO", "details": {"location": "Antarctica"}},
+                        ],
+                    },
+                },
+            ]
+        }
+
+        assert len(captured.captured_queries) == 2  # Sanity-check
+
+        # First we should have queried for all articles in a single query, joining on the reporters
+        # model (for the editors and reporters ForeignKeys)
+        assert re.match(
+            r'SELECT .* "tests_article" INNER JOIN "tests_reporter"',
+            captured.captured_queries[0]["sql"],
+        )
+
+        # Then we should have queried for all of the films of all reporters, joined with the film
+        # details for each film, using a single query
+        assert re.match(
+            r'SELECT .* FROM "tests_film" INNER JOIN "tests_film_reporters" .* LEFT OUTER JOIN "tests_filmdetails"',
+            captured.captured_queries[1]["sql"],
+        )
```

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_forms.py` & `graphene-django-3.0.2/graphene_django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_query.py` & `graphene-django-3.0.2/graphene_django/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_schema.py` & `graphene-django-3.0.2/graphene_django/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_types.py` & `graphene-django-3.0.2/graphene_django/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_utils.py` & `graphene-django-3.0.2/graphene_django/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/tests/test_views.py` & `graphene-django-3.0.2/graphene_django/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/types.py` & `graphene-django-3.0.2/graphene_django/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/utils/testing.py` & `graphene-django-3.0.2/graphene_django/utils/testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.0.2/graphene_django/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/utils/utils.py` & `graphene-django-3.0.2/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django/views.py` & `graphene-django-3.0.2/graphene_django/views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/graphene_django.egg-info/PKG-INFO` & `graphene-django-3.0.2/graphene_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.0.1
+Version: 3.0.2
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.0.1/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.0.2/graphene_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/setup.cfg` & `graphene-django-3.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.1/setup.py` & `graphene-django-3.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 dev_requires = [
     "black==22.8.0",
     "flake8==5.0.4",
     "flake8-black==0.3.3",
     "flake8-bugbear==22.9.11",
+    "pre-commit",
 ] + tests_require
 
 setup(
     name="graphene-django",
     version=version,
     description="Graphene Django integration",
     long_description=open("README.rst").read(),
```

