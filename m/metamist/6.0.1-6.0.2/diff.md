# Comparing `tmp/metamist-6.0.1.tar.gz` & `tmp/metamist-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.0.1.tar", last modified: Wed May  3 09:05:17 2023, max compression
+gzip compressed data, was "metamist-6.0.2.tar", last modified: Wed May  3 09:59:32 2023, max compression
```

## Comparing `metamist-6.0.1.tar` & `metamist-6.0.2.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.772931 metamist-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 09:00:51.000000 metamist-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:05:17.772931 metamist-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-03 09:00:51.000000 metamist-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.756931 metamist-6.0.1/metamist/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.756931 metamist-6.0.1/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33327 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41921 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.756931 metamist-6.0.1/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.756931 metamist-6.0.1/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/graphql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.760931 metamist-6.0.1/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-03 09:03:01.000000 metamist-6.0.1/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-03 09:03:01.000000 metamist-6.0.1/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 09:03:01.000000 metamist-6.0.1/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-03 09:03:01.000000 metamist-6.0.1/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/nested_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/nested_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/project_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.760931 metamist-6.0.1/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.764931 metamist-6.0.1/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31001 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50478 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-03 09:00:51.000000 metamist-6.0.1/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-03 09:03:02.000000 metamist-6.0.1/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.756931 metamist-6.0.1/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 09:05:17.000000 metamist-6.0.1/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 09:00:51.000000 metamist-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:05:17.772931 metamist-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-03 09:00:51.000000 metamist-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:05:17.772931 metamist-6.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-03 09:00:51.000000 metamist-6.0.1/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-03 09:00:51.000000 metamist-6.0.1/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.287104 metamist-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 09:53:22.000000 metamist-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 09:53:22.000000 metamist-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:59:32.287104 metamist-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-03 09:53:22.000000 metamist-6.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.247102 metamist-6.0.2/metamist/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33327 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41921 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-03 09:56:31.000000 metamist-6.0.2/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.263103 metamist-6.0.2/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_assays_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/project_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.263103 metamist-6.0.2/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.267103 metamist-6.0.2/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31001 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50478 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.251103 metamist-6.0.2/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 09:53:22.000000 metamist-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:59:32.287104 metamist-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-03 09:53:22.000000 metamist-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.287104 metamist-6.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-03 09:53:22.000000 metamist-6.0.2/test/testbase.py
```

### Comparing `metamist-6.0.1/LICENSE` & `metamist-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/PKG-INFO` & `metamist-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.1
+Version: 6.0.2
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.1/README.md` & `metamist-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/__init__.py` & `metamist-6.0.2/metamist/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.0.1/metamist/api/analysis_api.py` & `metamist-6.0.2/metamist/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/assay_api.py` & `metamist-6.0.2/metamist/api/assay_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/default_api.py` & `metamist-6.0.2/metamist/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/enums_api.py` & `metamist-6.0.2/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/family_api.py` & `metamist-6.0.2/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/import_api.py` & `metamist-6.0.2/metamist/api/import_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/participant_api.py` & `metamist-6.0.2/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/project_api.py` & `metamist-6.0.2/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/sample_api.py` & `metamist-6.0.2/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/seqr_api.py` & `metamist-6.0.2/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/sequencing_group_api.py` & `metamist-6.0.2/metamist/api/sequencing_group_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api/web_api.py` & `metamist-6.0.2/metamist/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/api_client.py` & `metamist-6.0.2/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-6.0.1/metamist/apis/__init__.py` & `metamist-6.0.2/metamist/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/configuration.py` & `metamist-6.0.2/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -401,15 +401,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.0.1\n"\
+               "Version of the API: 6.0.2\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.0.1/metamist/exceptions.py` & `metamist-6.0.2/metamist/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.0.1/metamist/graphql/__init__.py` & `metamist-6.0.2/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/model/analysis.py` & `metamist-6.0.2/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/analysis_query_model.py` & `metamist-6.0.2/metamist/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/analysis_status.py` & `metamist-6.0.2/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/analysis_update_model.py` & `metamist-6.0.2/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/assay_upsert.py` & `metamist-6.0.2/metamist/model/assay_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/body_get_assays_by_criteria.py` & `metamist-6.0.2/metamist/model/body_get_assays_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-6.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/body_get_participants.py` & `metamist-6.0.2/metamist/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/body_get_samples.py` & `metamist-6.0.2/metamist/model/body_get_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/error_response.py` & `metamist-6.0.2/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/export_type.py` & `metamist-6.0.2/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/extra_participant_importer_handler.py` & `metamist-6.0.2/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/family_search_response_data.py` & `metamist-6.0.2/metamist/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/family_update_model.py` & `metamist-6.0.2/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/http_validation_error.py` & `metamist-6.0.2/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/meta_search_entity_prefix.py` & `metamist-6.0.2/metamist/model/meta_search_entity_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/nested_assay.py` & `metamist-6.0.2/metamist/model/nested_assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/nested_family.py` & `metamist-6.0.2/metamist/model/nested_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/nested_participant.py` & `metamist-6.0.2/metamist/model/nested_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/nested_sample.py` & `metamist-6.0.2/metamist/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/nested_sequencing_group.py` & `metamist-6.0.2/metamist/model/nested_sequencing_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/paging_links.py` & `metamist-6.0.2/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/participant_search_response_data.py` & `metamist-6.0.2/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/participant_upsert.py` & `metamist-6.0.2/metamist/model/participant_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/project.py` & `metamist-6.0.2/metamist/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/project_summary_response.py` & `metamist-6.0.2/metamist/model/project_summary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/sample_search_response_data.py` & `metamist-6.0.2/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/sample_upsert.py` & `metamist-6.0.2/metamist/model/sample_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/search_item.py` & `metamist-6.0.2/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/search_response.py` & `metamist-6.0.2/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/search_response_model.py` & `metamist-6.0.2/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/search_response_type.py` & `metamist-6.0.2/metamist/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/sequencing_group_upsert.py` & `metamist-6.0.2/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/validation_error.py` & `metamist-6.0.2/metamist/model/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model/web_project.py` & `metamist-6.0.2/metamist/model/web_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.1/metamist/model_utils.py` & `metamist-6.0.2/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.0.1/metamist/models/__init__.py` & `metamist-6.0.2/metamist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/parser/cloudhelper.py` & `metamist-6.0.2/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/parser/generic_metadata_parser.py` & `metamist-6.0.2/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/parser/generic_parser.py` & `metamist-6.0.2/metamist/parser/generic_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/parser/sample_file_map_parser.py` & `metamist-6.0.2/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/metamist/rest.py` & `metamist-6.0.2/metamist/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.1
+    The version of the OpenAPI document: 6.0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.0.1/metamist.egg-info/PKG-INFO` & `metamist-6.0.2/metamist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.1
+Version: 6.0.2
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.1/metamist.egg-info/SOURCES.txt` & `metamist-6.0.2/metamist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 metamist/__init__.py
 metamist/api_client.py
 metamist/configuration.py
 metamist/exceptions.py
@@ -25,14 +26,15 @@
 metamist/api/project_api.py
 metamist/api/sample_api.py
 metamist/api/seqr_api.py
 metamist/api/sequencing_group_api.py
 metamist/api/web_api.py
 metamist/apis/__init__.py
 metamist/graphql/__init__.py
+metamist/graphql/schema.graphql
 metamist/model/__init__.py
 metamist/model/analysis.py
 metamist/model/analysis_query_model.py
 metamist/model/analysis_status.py
 metamist/model/analysis_update_model.py
 metamist/model/assay_upsert.py
 metamist/model/body_get_assays_by_criteria.py
```

### Comparing `metamist-6.0.1/setup.py` & `metamist-6.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.0.1',
+    version='6.0.2',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-6.0.1/test/test_analysis.py` & `metamist-6.0.2/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_assay.py` & `metamist-6.0.2/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_generate_data.py` & `metamist-6.0.2/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_get_participants.py` & `metamist-6.0.2/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_graphql.py` & `metamist-6.0.2/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_import_individual_metadata.py` & `metamist-6.0.2/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_parse_existing_cohort.py` & `metamist-6.0.2/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_parse_file_map.py` & `metamist-6.0.2/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_parse_generic_metadata.py` & `metamist-6.0.2/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_parse_ont_processor.py` & `metamist-6.0.2/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_parse_ont_sheet.py` & `metamist-6.0.2/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_pedigree.py` & `metamist-6.0.2/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_sample.py` & `metamist-6.0.2/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_search.py` & `metamist-6.0.2/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_sequencing_groups.py` & `metamist-6.0.2/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_upsert.py` & `metamist-6.0.2/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/test_web.py` & `metamist-6.0.2/test/test_web.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.1/test/testbase.py` & `metamist-6.0.2/test/testbase.py`

 * *Files identical despite different names*

