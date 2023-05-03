# Comparing `tmp/data-repo-client-1.477.0.tar.gz` & `tmp/data-repo-client-1.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-nf0s089h/data-repo-client-1.477.0.tar", last modified: Wed May  3 14:16:34 2023, max compression
+gzip compressed data, was "dist/data-repo-client-1.64.0.tar", last modified: Fri Apr 23 18:20:39 2021, max compression
```

## Comparing `data-repo-client-1.477.0.tar` & `data-repo-client-1.64.0.tar`

### file list

```diff
@@ -1,298 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40020 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   181225 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46873 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   376703 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46874 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31197 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   127526 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-03 14:16:21.000000 data-repo-client-1.477.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-03 14:16:21.000000 data-repo-client-1.477.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-03 14:16:21.000000 data-repo-client-1.477.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_index_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_index_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_metadata_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/search_query_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/sql_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:34.000000 data-repo-client-1.477.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-03 14:16:21.000000 data-repo-client-1.477.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-03 14:16:21.000000 data-repo-client-1.477.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_index_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_index_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_metadata_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_search_query_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_sql_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-03 14:16:23.000000 data-repo-client-1.477.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-03 14:16:22.000000 data-repo-client-1.477.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/
+-rw-r--r--   0 myessail   (503) staff       (20)     1545 2020-12-08 18:44:05.000000 data-repo-client-1.64.0/LICENSE
+-rw-r--r--   0 myessail   (503) staff       (20)     3077 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/PKG-INFO
+-rw-r--r--   0 myessail   (503) staff       (20)    17369 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/README.md
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/
+-rw-r--r--   0 myessail   (503) staff       (20)     9367 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/__init__.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/api/
+-rw-r--r--   0 myessail   (503) staff       (20)      367 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 myessail   (503) staff       (20)    21178 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)   220470 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    48309 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    16523 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)    28864 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/api_client.py
+-rw-r--r--   0 myessail   (503) staff       (20)    16252 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/configuration.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6399 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client/models/
+-rw-r--r--   0 myessail   (503) staff       (20)     8637 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 myessail   (503) staff       (20)    12442 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8331 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11823 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10883 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8881 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10190 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7136 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9274 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9809 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5536 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11633 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10716 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10106 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9123 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6117 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9345 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8984 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6741 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6659 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8405 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6504 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7502 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8512 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7203 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13682 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10478 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7788 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11240 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7647 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6458 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7546 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9199 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7204 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7335 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10111 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6787 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 myessail   (503) staff       (20)    19591 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9189 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6857 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6757 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6774 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5524 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6819 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8609 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11401 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13545 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5442 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)    17287 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    14206 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10890 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11107 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6103 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6515 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6010 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7892 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9869 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9717 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7087 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7388 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 myessail   (503) staff       (20)    13949 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8713 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11122 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    10905 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8570 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6271 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9573 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8439 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)    11085 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5436 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/sql_sort_direction.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5862 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)    12798 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9540 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7831 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     8182 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)    14933 2021-04-23 17:59:17.000000 data-repo-client-1.64.0/data_repo_client/rest.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/
+-rw-r--r--   0 myessail   (503) staff       (20)     3077 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 myessail   (503) staff       (20)     6884 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 myessail   (503) staff       (20)        1 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       48 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       17 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 myessail   (503) staff       (20)       69 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/setup.cfg
+-rw-r--r--   0 myessail   (503) staff       (20)     6404 2021-04-23 18:19:32.000000 data-repo-client-1.64.0/setup.py
+drwxr-xr-x   0 myessail   (503) staff       (20)        0 2021-04-23 18:20:39.000000 data-repo-client-1.64.0/test/
+-rw-r--r--   0 myessail   (503) staff       (20)     4761 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4219 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_asset_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4301 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4442 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4332 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4931 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4825 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4247 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4345 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4037 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4384 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4330 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4270 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4121 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_column_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4066 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_enable_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4230 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4345 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_fault_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4911 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_group_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4899 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_list_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4607 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4096 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_config_parameter_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4242 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4611 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4346 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3900 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6863 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     9500 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7567 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4227 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4184 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4098 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_delete_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5201 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_directory_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4331 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_access_method.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4100 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_access_url.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4059 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_checksum.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4492 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_contents_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3995 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_error.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5989 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_object.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4195 2020-12-08 18:39:39.000000 data-repo-client-1.64.0/test/test_drs_service_info.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4625 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4456 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4461 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4070 2021-04-23 17:59:15.000000 data-repo-client-1.64.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4098 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_error_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4148 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_detail_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4269 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_load_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5957 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3991 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_file_model_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4558 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_ingest_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4373 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_ingest_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4342 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4239 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_job_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4114 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_member_request.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4070 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4259 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_policy_response.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4748 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_relationship_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4197 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_relationship_term_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7673 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4337 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4703 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_status_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4250 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3899 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_resources_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     6369 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4351 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5287 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     7047 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4251 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4938 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4553 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4689 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4230 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4024 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/test/test_sql_sort_direction.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3991 2021-04-23 17:59:16.000000 data-repo-client-1.64.0/test/test_table_data_type.py
+-rw-r--r--   0 myessail   (503) staff       (20)     5064 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_table_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     3725 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4248 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_upgrade_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4171 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 myessail   (503) staff       (20)     4213 2020-12-08 18:39:40.000000 data-repo-client-1.64.0/test/test_user_status_info.py
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api/configs_api.py` & `data-repo-client-1.64.0/data_repo_client/api/data_repository_service_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -20,289 +20,312 @@
 from data_repo_client.api_client import ApiClient
 from data_repo_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ConfigsApi(object):
+class DataRepositoryServiceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_config(self, name, **kwargs):  # noqa: E501
-        """get_config  # noqa: E501
+    def get_access_url(self, object_id, access_id, **kwargs):  # noqa: E501
+        """Get a URL for fetching bytes.  # noqa: E501
 
-        Get one configuration  # noqa: E501
+        Returns a URL that can be used to fetch the object bytes. This method only needs to be called when using an `AccessMethod` that contains an `access_id` (e.g., for servers that use signed URLs for fetching object bytes).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_config(name, async_req=True)
+        >>> thread = api.get_access_url(object_id, access_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str name: name of the configuration to get (required)
+        :param str object_id: An `id` of a Data Object (required)
+        :param str access_id: An `access_id` from the `access_methods` list of a Data Object (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: ConfigModel
+        :return: DRSAccessURL
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_config_with_http_info(name, **kwargs)  # noqa: E501
+        return self.get_access_url_with_http_info(object_id, access_id, **kwargs)  # noqa: E501
 
-    def get_config_with_http_info(self, name, **kwargs):  # noqa: E501
-        """get_config  # noqa: E501
+    def get_access_url_with_http_info(self, object_id, access_id, **kwargs):  # noqa: E501
+        """Get a URL for fetching bytes.  # noqa: E501
 
-        Get one configuration  # noqa: E501
+        Returns a URL that can be used to fetch the object bytes. This method only needs to be called when using an `AccessMethod` that contains an `access_id` (e.g., for servers that use signed URLs for fetching object bytes).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_config_with_http_info(name, async_req=True)
+        >>> thread = api.get_access_url_with_http_info(object_id, access_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str name: name of the configuration to get (required)
+        :param str object_id: An `id` of a Data Object (required)
+        :param str access_id: An `access_id` from the `access_methods` list of a Data Object (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(ConfigModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(DRSAccessURL, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'name'
+            'object_id',
+            'access_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_config" % key
+                    " to method get_access_url" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'name' is set
-        if self.api_client.client_side_validation and ('name' not in local_var_params or  # noqa: E501
-                                                        local_var_params['name'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `name` when calling `get_config`")  # noqa: E501
+        # verify the required parameter 'object_id' is set
+        if self.api_client.client_side_validation and ('object_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['object_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `object_id` when calling `get_access_url`")  # noqa: E501
+        # verify the required parameter 'access_id' is set
+        if self.api_client.client_side_validation and ('access_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['access_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `access_id` when calling `get_access_url`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'name' in local_var_params:
-            path_params['name'] = local_var_params['name']  # noqa: E501
+        if 'object_id' in local_var_params:
+            path_params['object_id'] = local_var_params['object_id']  # noqa: E501
+        if 'access_id' in local_var_params:
+            path_params['access_id'] = local_var_params['access_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/configs/{name}', 'GET',
+            '/ga4gh/drs/v1/objects/{object_id}/access/{access_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ConfigModel',  # noqa: E501
+            response_type='DRSAccessURL',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_config_list(self, **kwargs):  # noqa: E501
-        """get_config_list  # noqa: E501
+    def get_object(self, object_id, **kwargs):  # noqa: E501
+        """Get info about an `Object`.  # noqa: E501
 
-        Get all configurations  # noqa: E501
+        Returns object metadata, and a list of access methods that can be used to fetch object bytes.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_config_list(async_req=True)
+        >>> thread = api.get_object(object_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str object_id: (required)
+        :param bool expand: If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains another bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: ConfigListModel
+        :return: DRSObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_config_list_with_http_info(**kwargs)  # noqa: E501
+        return self.get_object_with_http_info(object_id, **kwargs)  # noqa: E501
 
-    def get_config_list_with_http_info(self, **kwargs):  # noqa: E501
-        """get_config_list  # noqa: E501
+    def get_object_with_http_info(self, object_id, **kwargs):  # noqa: E501
+        """Get info about an `Object`.  # noqa: E501
 
-        Get all configurations  # noqa: E501
+        Returns object metadata, and a list of access methods that can be used to fetch object bytes.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_config_list_with_http_info(async_req=True)
+        >>> thread = api.get_object_with_http_info(object_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str object_id: (required)
+        :param bool expand: If false and the object_id refers to a bundle, then the ContentsObject array contains only those objects directly contained in the bundle. That is, if the bundle contains other bundles, those other bundles are not recursively included in the result. If true and the object_id refers to a bundle, then the entire set of objects in the bundle is expanded. That is, if the bundle contains another bundles, then those other bundles are recursively expanded and included in the result. Recursion continues through the entire sub-tree of the bundle. If the object_id refers to a blob, then the query parameter is ignored.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(ConfigListModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(DRSObject, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'object_id',
+            'expand'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_config_list" % key
+                    " to method get_object" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'object_id' is set
+        if self.api_client.client_side_validation and ('object_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['object_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `object_id` when calling `get_object`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'object_id' in local_var_params:
+            path_params['object_id'] = local_var_params['object_id']  # noqa: E501
 
         query_params = []
+        if 'expand' in local_var_params and local_var_params['expand'] is not None:  # noqa: E501
+            query_params.append(('expand', local_var_params['expand']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/configs', 'GET',
+            '/ga4gh/drs/v1/objects/{object_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ConfigListModel',  # noqa: E501
+            response_type='DRSObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def reset_config(self, **kwargs):  # noqa: E501
-        """reset_config  # noqa: E501
+    def get_service_info(self, **kwargs):  # noqa: E501
+        """Get information about this implementation.  # noqa: E501
 
-        Reset the configuration to original settings  # noqa: E501
+        May return service version and other information. [dd]NOTE: technically, this has been removed from DRS V1.0. It will be added back when there is a common service_info across ga4gh. I don't expect it to be too different, so just leaving this info call in place.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.reset_config(async_req=True)
+        >>> thread = api.get_service_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: DRSServiceInfo
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.reset_config_with_http_info(**kwargs)  # noqa: E501
+        return self.get_service_info_with_http_info(**kwargs)  # noqa: E501
 
-    def reset_config_with_http_info(self, **kwargs):  # noqa: E501
-        """reset_config  # noqa: E501
+    def get_service_info_with_http_info(self, **kwargs):  # noqa: E501
+        """Get information about this implementation.  # noqa: E501
 
-        Reset the configuration to original settings  # noqa: E501
+        May return service version and other information. [dd]NOTE: technically, this has been removed from DRS V1.0. It will be added back when there is a common service_info across ga4gh. I don't expect it to be too different, so just leaving this info call in place.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.reset_config_with_http_info(async_req=True)
+        >>> thread = api.get_service_info_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: tuple(DRSServiceInfo, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -316,15 +339,15 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method reset_config" % key
+                    " to method get_service_info" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -333,262 +356,29 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/configs/reset', 'PUT',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type=None,  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def set_config_list(self, **kwargs):  # noqa: E501
-        """set_config_list  # noqa: E501
-
-        Set the a group of configurations  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.set_config_list(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param ConfigGroupModel config_model:
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: ConfigListModel
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.set_config_list_with_http_info(**kwargs)  # noqa: E501
-
-    def set_config_list_with_http_info(self, **kwargs):  # noqa: E501
-        """set_config_list  # noqa: E501
-
-        Set the a group of configurations  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.set_config_list_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param ConfigGroupModel config_model:
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(ConfigListModel, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'config_model'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method set_config_list" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'config_model' in local_var_params:
-            body_params = local_var_params['config_model']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/configs', 'PUT',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='ConfigListModel',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def set_fault(self, name, **kwargs):  # noqa: E501
-        """set_fault  # noqa: E501
-
-        Enable or disable the named fault. Performing the put on a config that is not a fault is an error.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.set_fault(name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str name: name of the configuration to (required)
-        :param ConfigEnableModel config_enable:
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: None
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.set_fault_with_http_info(name, **kwargs)  # noqa: E501
-
-    def set_fault_with_http_info(self, name, **kwargs):  # noqa: E501
-        """set_fault  # noqa: E501
-
-        Enable or disable the named fault. Performing the put on a config that is not a fault is an error.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.set_fault_with_http_info(name, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str name: name of the configuration to (required)
-        :param ConfigEnableModel config_enable:
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: None
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'name',
-            'config_enable'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method set_fault" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'name' is set
-        if self.api_client.client_side_validation and ('name' not in local_var_params or  # noqa: E501
-                                                        local_var_params['name'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `name` when calling `set_fault`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'name' in local_var_params:
-            path_params['name'] = local_var_params['name']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'config_enable' in local_var_params:
-            body_params = local_var_params['config_enable']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/configs/{name}', 'PUT',
+            '/ga4gh/drs/v1/service-info', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='DRSServiceInfo',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api/datasets_api.py` & `data-repo-client-1.64.0/data_repo_client/api/repository_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -20,15 +20,15 @@
 from data_repo_client.api_client import ApiClient
 from data_repo_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DatasetsApi(object):
+class RepositoryApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
@@ -137,15 +137,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/assets', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -269,15 +269,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/policies/{policyName}/members', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -287,14 +287,146 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def add_snapshot_policy_member(self, id, policy_name, **kwargs):  # noqa: E501
+        """add_snapshot_policy_member  # noqa: E501
+
+        Adds a member to the specified policy for the snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_snapshot_policy_member(id, policy_name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param str policy_name: The relevant policy (required)
+        :param PolicyMemberRequest policy_member: Snapshot to change the policy of
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PolicyResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.add_snapshot_policy_member_with_http_info(id, policy_name, **kwargs)  # noqa: E501
+
+    def add_snapshot_policy_member_with_http_info(self, id, policy_name, **kwargs):  # noqa: E501
+        """add_snapshot_policy_member  # noqa: E501
+
+        Adds a member to the specified policy for the snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_snapshot_policy_member_with_http_info(id, policy_name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param str policy_name: The relevant policy (required)
+        :param PolicyMemberRequest policy_member: Snapshot to change the policy of
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PolicyResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'policy_name',
+            'policy_member'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_snapshot_policy_member" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `add_snapshot_policy_member`")  # noqa: E501
+        # verify the required parameter 'policy_name' is set
+        if self.api_client.client_side_validation and ('policy_name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['policy_name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `policy_name` when calling `add_snapshot_policy_member`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'policy_name' in local_var_params:
+            path_params['policyName'] = local_var_params['policy_name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'policy_member' in local_var_params:
+            body_params = local_var_params['policy_member']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/policies/{policyName}/members', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PolicyResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def apply_dataset_data_deletion(self, id, **kwargs):  # noqa: E501
         """apply_dataset_data_deletion  # noqa: E501
 
         Applies deletes to primary tabular data in a dataset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.apply_dataset_data_deletion(id, async_req=True)
@@ -392,15 +524,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/deletes', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -515,15 +647,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/files/bulk', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -638,15 +770,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/files/bulk/array', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -766,72 +898,76 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/files/bulk/{loadTag}', 'DELETE',
+            '/api/repository/v1/datasets/{id}/files/bulk/{loadtag}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='JobModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def close_transaction(self, id, transaction_id, **kwargs):  # noqa: E501
-        """close_transaction  # noqa: E501
+    def bulk_file_results_get(self, id, loadtag, **kwargs):  # noqa: E501
+        """bulk_file_results_get  # noqa: E501
 
-        Close a given transaction  # noqa: E501
+        Retrieve the results of a bulk file load. The results of each bulk load are stored in the dataset. They can be queried directly or retrieved with this paginated interface.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.close_transaction(id, transaction_id, async_req=True)
+        >>> thread = api.bulk_file_results_get(id, loadtag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str transaction_id: A UUID to used to identify a transaction in a dataset (required)
-        :param TransactionCloseModel transaction_close_model: Close transaction request
+        :param str loadtag: a load tag (required)
+        :param str job_id: The job id associated with the load
+        :param int offset: The number of items to skip before starting to collect the result set.
+        :param int limit: The numbers of items to return.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.close_transaction_with_http_info(id, transaction_id, **kwargs)  # noqa: E501
+        return self.bulk_file_results_get_with_http_info(id, loadtag, **kwargs)  # noqa: E501
 
-    def close_transaction_with_http_info(self, id, transaction_id, **kwargs):  # noqa: E501
-        """close_transaction  # noqa: E501
+    def bulk_file_results_get_with_http_info(self, id, loadtag, **kwargs):  # noqa: E501
+        """bulk_file_results_get  # noqa: E501
 
-        Close a given transaction  # noqa: E501
+        Retrieve the results of a bulk file load. The results of each bulk load are stored in the dataset. They can be queried directly or retrieved with this paginated interface.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.close_transaction_with_http_info(id, transaction_id, async_req=True)
+        >>> thread = api.bulk_file_results_get_with_http_info(id, loadtag, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str transaction_id: A UUID to used to identify a transaction in a dataset (required)
-        :param TransactionCloseModel transaction_close_model: Close transaction request
+        :param str loadtag: a load tag (required)
+        :param str job_id: The job id associated with the load
+        :param int offset: The number of items to skip before starting to collect the result set.
+        :param int limit: The numbers of items to return.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -842,74 +978,76 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'transaction_id',
-            'transaction_close_model'
+            'loadtag',
+            'job_id',
+            'offset',
+            'limit'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method close_transaction" % key
+                    " to method bulk_file_results_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `close_transaction`")  # noqa: E501
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `close_transaction`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `bulk_file_results_get`")  # noqa: E501
+        # verify the required parameter 'loadtag' is set
+        if self.api_client.client_side_validation and ('loadtag' not in local_var_params or  # noqa: E501
+                                                        local_var_params['loadtag'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `loadtag` when calling `bulk_file_results_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'transaction_id' in local_var_params:
-            path_params['transactionId'] = local_var_params['transaction_id']  # noqa: E501
+        if 'loadtag' in local_var_params:
+            path_params['loadtag'] = local_var_params['loadtag']  # noqa: E501
 
         query_params = []
+        if 'job_id' in local_var_params and local_var_params['job_id'] is not None:  # noqa: E501
+            query_params.append(('jobId', local_var_params['job_id']))  # noqa: E501
+        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
+            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
+        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
+            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'transaction_close_model' in local_var_params:
-            body_params = local_var_params['transaction_close_model']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/transactions/{transactionId}', 'POST',
+            '/api/repository/v1/datasets/{id}/files/bulk/{loadtag}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='JobModel',  # noqa: E501
@@ -1012,15 +1150,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1030,14 +1168,128 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def create_snapshot(self, **kwargs):  # noqa: E501
+        """create_snapshot  # noqa: E501
+
+        Create a new snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_snapshot(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param SnapshotRequestModel snapshot: Snapshot to create
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: JobModel
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_snapshot_with_http_info(**kwargs)  # noqa: E501
+
+    def create_snapshot_with_http_info(self, **kwargs):  # noqa: E501
+        """create_snapshot  # noqa: E501
+
+        Create a new snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_snapshot_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param SnapshotRequestModel snapshot: Snapshot to create
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'snapshot'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_snapshot" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'snapshot' in local_var_params:
+            body_params = local_var_params['snapshot']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='JobModel',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def delete_dataset(self, id, **kwargs):  # noqa: E501
         """delete_dataset  # noqa: E501
 
         Delete a dataset by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_dataset(id, async_req=True)
@@ -1126,15 +1378,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1258,15 +1510,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/policies/{policyName}/members/{memberEmail}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1381,15 +1633,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/files/{fileid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1399,14 +1651,370 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def delete_job(self, id, **kwargs):  # noqa: E501
+        """delete_job  # noqa: E501
+
+        Delete the job and data associated with it  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_job(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_job_with_http_info(id, **kwargs)  # noqa: E501
+
+    def delete_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """delete_job  # noqa: E501
+
+        Delete the job and data associated with it  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_job_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_job" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_job`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/jobs/{id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_snapshot(self, id, **kwargs):  # noqa: E501
+        """delete_snapshot  # noqa: E501
+
+        Delete a snapshot by id  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_snapshot(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: JobModel
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_snapshot_with_http_info(id, **kwargs)  # noqa: E501
+
+    def delete_snapshot_with_http_info(self, id, **kwargs):  # noqa: E501
+        """delete_snapshot  # noqa: E501
+
+        Delete a snapshot by id  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_snapshot_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_snapshot" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_snapshot`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='JobModel',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_snapshot_policy_member(self, id, policy_name, member_email, **kwargs):  # noqa: E501
+        """delete_snapshot_policy_member  # noqa: E501
+
+        Removes a member from the specified policy for the snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_snapshot_policy_member(id, policy_name, member_email, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param str policy_name: The relevant policy (required)
+        :param str member_email: The email of the user to remove (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PolicyResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_snapshot_policy_member_with_http_info(id, policy_name, member_email, **kwargs)  # noqa: E501
+
+    def delete_snapshot_policy_member_with_http_info(self, id, policy_name, member_email, **kwargs):  # noqa: E501
+        """delete_snapshot_policy_member  # noqa: E501
+
+        Removes a member from the specified policy for the snapshot  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_snapshot_policy_member_with_http_info(id, policy_name, member_email, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: A UUID to used to identify an object in the repository (required)
+        :param str policy_name: The relevant policy (required)
+        :param str member_email: The email of the user to remove (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PolicyResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'policy_name',
+            'member_email'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_snapshot_policy_member" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_snapshot_policy_member`")  # noqa: E501
+        # verify the required parameter 'policy_name' is set
+        if self.api_client.client_side_validation and ('policy_name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['policy_name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `policy_name` when calling `delete_snapshot_policy_member`")  # noqa: E501
+        # verify the required parameter 'member_email' is set
+        if self.api_client.client_side_validation and ('member_email' not in local_var_params or  # noqa: E501
+                                                        local_var_params['member_email'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `member_email` when calling `delete_snapshot_policy_member`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'policy_name' in local_var_params:
+            path_params['policyName'] = local_var_params['policy_name']  # noqa: E501
+        if 'member_email' in local_var_params:
+            path_params['memberEmail'] = local_var_params['member_email']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/policies/{policyName}/members/{memberEmail}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PolicyResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def enumerate_datasets(self, **kwargs):  # noqa: E501
         """enumerate_datasets  # noqa: E501
 
         Returns a list of all of the datasets the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.enumerate_datasets(async_req=True)
@@ -1414,16 +2022,14 @@
 
         :param async_req bool: execute request asynchronously
         :param int offset: The number of datasets to skip before when retrieving the next page
         :param int limit: The numbers datasets to retrieve and return.
         :param EnumerateSortByParam sort: The field to use for sorting.
         :param SqlSortDirection direction: The direction to sort.
         :param str filter: Filter the results where this string is a case insensitive match in the name or description.
-        :param str region: Filter the results where this string is a case insensitive match in any of the cloud storage regions used by the dataset.
-        :param list[str] tags: Filter the results where these case sensitive tags are applied to the datasets 
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1445,16 +2051,14 @@
 
         :param async_req bool: execute request asynchronously
         :param int offset: The number of datasets to skip before when retrieving the next page
         :param int limit: The numbers datasets to retrieve and return.
         :param EnumerateSortByParam sort: The field to use for sorting.
         :param SqlSortDirection direction: The direction to sort.
         :param str filter: Filter the results where this string is a case insensitive match in the name or description.
-        :param str region: Filter the results where this string is a case insensitive match in any of the cloud storage regions used by the dataset.
-        :param list[str] tags: Filter the results where these case sensitive tags are applied to the datasets 
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1468,17 +2072,15 @@
         local_var_params = locals()
 
         all_params = [
             'offset',
             'limit',
             'sort',
             'direction',
-            'filter',
-            'region',
-            'tags'
+            'filter'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -1505,32 +2107,27 @@
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'sort' in local_var_params and local_var_params['sort'] is not None:  # noqa: E501
             query_params.append(('sort', local_var_params['sort']))  # noqa: E501
         if 'direction' in local_var_params and local_var_params['direction'] is not None:  # noqa: E501
             query_params.append(('direction', local_var_params['direction']))  # noqa: E501
         if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
             query_params.append(('filter', local_var_params['filter']))  # noqa: E501
-        if 'region' in local_var_params and local_var_params['region'] is not None:  # noqa: E501
-            query_params.append(('region', local_var_params['region']))  # noqa: E501
-        if 'tags' in local_var_params and local_var_params['tags'] is not None:  # noqa: E501
-            query_params.append(('tags', local_var_params['tags']))  # noqa: E501
-            collection_formats['tags'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1540,72 +2137,69 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def enumerate_transactions(self, id, **kwargs):  # noqa: E501
-        """enumerate_transactions  # noqa: E501
+    def enumerate_jobs(self, **kwargs):  # noqa: E501
+        """enumerate_jobs  # noqa: E501
 
-        Lists transactions on the dataset  # noqa: E501
+        Returns a list of all of the jobs the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_transactions(id, async_req=True)
+        >>> thread = api.enumerate_jobs(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param int offset: The number of items to skip before starting to collect the result set.
         :param int limit: The numbers of items to return.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: list[TransactionModel]
+        :return: list[JobModel]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.enumerate_transactions_with_http_info(id, **kwargs)  # noqa: E501
+        return self.enumerate_jobs_with_http_info(**kwargs)  # noqa: E501
 
-    def enumerate_transactions_with_http_info(self, id, **kwargs):  # noqa: E501
-        """enumerate_transactions  # noqa: E501
+    def enumerate_jobs_with_http_info(self, **kwargs):  # noqa: E501
+        """enumerate_jobs  # noqa: E501
 
-        Lists transactions on the dataset  # noqa: E501
+        Returns a list of all of the jobs the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_transactions_with_http_info(id, async_req=True)
+        >>> thread = api.enumerate_jobs_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param int offset: The number of items to skip before starting to collect the result set.
         :param int limit: The numbers of items to return.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(list[TransactionModel], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[JobModel], status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
             'offset',
             'limit'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -1614,28 +2208,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method enumerate_transactions" % key
+                    " to method enumerate_jobs" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `enumerate_transactions`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
 
@@ -1646,441 +2234,425 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/transactions', 'GET',
+            '/api/repository/v1/jobs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[TransactionModel]',  # noqa: E501
+            response_type='list[JobModel]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_dataset_tags(self, **kwargs):  # noqa: E501
-        """get_dataset_tags  # noqa: E501
+    def enumerate_snapshots(self, **kwargs):  # noqa: E501
+        """enumerate_snapshots  # noqa: E501
 
-        Get accessible dataset tags  # noqa: E501
+        Returns a list of all of the snapshots the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_dataset_tags(async_req=True)
+        >>> thread = api.enumerate_snapshots(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str filter: Filter to tags with this string as a case-insensitive match.
-        :param int limit: The maximum number of tags to return, in descending order of occurrence count. All accessible tags will be returned if unspecified. 
+        :param int offset: The number of items to skip before starting to collect the result set.
+        :param int limit: The numbers of items to return.
+        :param EnumerateSortByParam sort: The field to use for sorting.
+        :param SqlSortDirection direction: The direction to sort.
+        :param str filter: Filter the results where this string is a case insensitive match in the name or description.
+        :param list[str] dataset_ids: Filter the results where these datasetIds are source datasets.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: TagCountResultModel
+        :return: EnumerateSnapshotModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_dataset_tags_with_http_info(**kwargs)  # noqa: E501
+        return self.enumerate_snapshots_with_http_info(**kwargs)  # noqa: E501
 
-    def get_dataset_tags_with_http_info(self, **kwargs):  # noqa: E501
-        """get_dataset_tags  # noqa: E501
+    def enumerate_snapshots_with_http_info(self, **kwargs):  # noqa: E501
+        """enumerate_snapshots  # noqa: E501
 
-        Get accessible dataset tags  # noqa: E501
+        Returns a list of all of the snapshots the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_dataset_tags_with_http_info(async_req=True)
+        >>> thread = api.enumerate_snapshots_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str filter: Filter to tags with this string as a case-insensitive match.
-        :param int limit: The maximum number of tags to return, in descending order of occurrence count. All accessible tags will be returned if unspecified. 
+        :param int offset: The number of items to skip before starting to collect the result set.
+        :param int limit: The numbers of items to return.
+        :param EnumerateSortByParam sort: The field to use for sorting.
+        :param SqlSortDirection direction: The direction to sort.
+        :param str filter: Filter the results where this string is a case insensitive match in the name or description.
+        :param list[str] dataset_ids: Filter the results where these datasetIds are source datasets.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(TagCountResultModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(EnumerateSnapshotModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'offset',
+            'limit',
+            'sort',
+            'direction',
             'filter',
-            'limit'
+            'dataset_ids'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_dataset_tags" % key
+                    " to method enumerate_snapshots" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
-            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
+        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
+            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
+        if 'sort' in local_var_params and local_var_params['sort'] is not None:  # noqa: E501
+            query_params.append(('sort', local_var_params['sort']))  # noqa: E501
+        if 'direction' in local_var_params and local_var_params['direction'] is not None:  # noqa: E501
+            query_params.append(('direction', local_var_params['direction']))  # noqa: E501
+        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
+            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
+        if 'dataset_ids' in local_var_params and local_var_params['dataset_ids'] is not None:  # noqa: E501
+            query_params.append(('datasetIds', local_var_params['dataset_ids']))  # noqa: E501
+            collection_formats['datasetIds'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/tags', 'GET',
+            '/api/repository/v1/snapshots', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='TagCountResultModel',  # noqa: E501
+            response_type='EnumerateSnapshotModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_load_history_for_load_tag(self, id, load_tag, **kwargs):  # noqa: E501
-        """get_load_history_for_load_tag  # noqa: E501
+    def get_config(self, name, **kwargs):  # noqa: E501
+        """get_config  # noqa: E501
 
-        Retrieve the results of a bulk file load. The results of each bulk load are stored in the dataset. They can be queried directly or retrieved with this paginated interface.  # noqa: E501
+        Get one configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_load_history_for_load_tag(id, load_tag, async_req=True)
+        >>> thread = api.get_config(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param str load_tag: a load tag (required)
-        :param int offset: The number of items to skip before starting to collect the result set.
-        :param int limit: The numbers of items to return.
+        :param str name: name of the configuration to get (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: BulkLoadHistoryModelList
+        :return: ConfigModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_load_history_for_load_tag_with_http_info(id, load_tag, **kwargs)  # noqa: E501
+        return self.get_config_with_http_info(name, **kwargs)  # noqa: E501
 
-    def get_load_history_for_load_tag_with_http_info(self, id, load_tag, **kwargs):  # noqa: E501
-        """get_load_history_for_load_tag  # noqa: E501
+    def get_config_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get_config  # noqa: E501
 
-        Retrieve the results of a bulk file load. The results of each bulk load are stored in the dataset. They can be queried directly or retrieved with this paginated interface.  # noqa: E501
+        Get one configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_load_history_for_load_tag_with_http_info(id, load_tag, async_req=True)
+        >>> thread = api.get_config_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param str load_tag: a load tag (required)
-        :param int offset: The number of items to skip before starting to collect the result set.
-        :param int limit: The numbers of items to return.
+        :param str name: name of the configuration to get (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(BulkLoadHistoryModelList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ConfigModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'load_tag',
-            'offset',
-            'limit'
+            'name'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_load_history_for_load_tag" % key
+                    " to method get_config" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_load_history_for_load_tag`")  # noqa: E501
-        # verify the required parameter 'load_tag' is set
-        if self.api_client.client_side_validation and ('load_tag' not in local_var_params or  # noqa: E501
-                                                        local_var_params['load_tag'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `load_tag` when calling `get_load_history_for_load_tag`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if self.api_client.client_side_validation and ('name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `name` when calling `get_config`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'load_tag' in local_var_params:
-            path_params['loadTag'] = local_var_params['load_tag']  # noqa: E501
+        if 'name' in local_var_params:
+            path_params['name'] = local_var_params['name']  # noqa: E501
 
         query_params = []
-        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
-            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
-        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/files/bulk/{loadTag}', 'GET',
+            '/api/repository/v1/configs/{name}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='BulkLoadHistoryModelList',  # noqa: E501
+            response_type='ConfigModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def ingest_dataset(self, id, **kwargs):  # noqa: E501
-        """ingest_dataset  # noqa: E501
+    def get_config_list(self, **kwargs):  # noqa: E501
+        """get_config_list  # noqa: E501
 
-        Ingest data into a dataset table  # noqa: E501
+        Get all configurations  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ingest_dataset(id, async_req=True)
+        >>> thread = api.get_config_list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param IngestRequestModel ingest: Ingest request
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: JobModel
+        :return: ConfigListModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.ingest_dataset_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_config_list_with_http_info(**kwargs)  # noqa: E501
 
-    def ingest_dataset_with_http_info(self, id, **kwargs):  # noqa: E501
-        """ingest_dataset  # noqa: E501
+    def get_config_list_with_http_info(self, **kwargs):  # noqa: E501
+        """get_config_list  # noqa: E501
 
-        Ingest data into a dataset table  # noqa: E501
+        Get all configurations  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ingest_dataset_with_http_info(id, async_req=True)
+        >>> thread = api.get_config_list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param IngestRequestModel ingest: Ingest request
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ConfigListModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'ingest'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method ingest_dataset" % key
+                    " to method get_config_list" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `ingest_dataset`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'ingest' in local_var_params:
-            body_params = local_var_params['ingest']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/ingest', 'POST',
+            '/api/repository/v1/configs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='JobModel',  # noqa: E501
+            response_type='ConfigListModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def ingest_file(self, id, **kwargs):  # noqa: E501
-        """ingest_file  # noqa: E501
+    def ingest_dataset(self, id, **kwargs):  # noqa: E501
+        """ingest_dataset  # noqa: E501
 
-        Ingest one file into the dataset file system; async returns a FileModel  # noqa: E501
+        Ingest data into a dataset table  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ingest_file(id, async_req=True)
+        >>> thread = api.ingest_dataset(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param FileLoadModel ingest_file: Ingest file request
+        :param IngestRequestModel ingest: Ingest request
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.ingest_file_with_http_info(id, **kwargs)  # noqa: E501
+        return self.ingest_dataset_with_http_info(id, **kwargs)  # noqa: E501
 
-    def ingest_file_with_http_info(self, id, **kwargs):  # noqa: E501
-        """ingest_file  # noqa: E501
+    def ingest_dataset_with_http_info(self, id, **kwargs):  # noqa: E501
+        """ingest_dataset  # noqa: E501
 
-        Ingest one file into the dataset file system; async returns a FileModel  # noqa: E501
+        Ingest data into a dataset table  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ingest_file_with_http_info(id, async_req=True)
+        >>> thread = api.ingest_dataset_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param FileLoadModel ingest_file: Ingest file request
+        :param IngestRequestModel ingest: Ingest request
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2091,37 +2663,37 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'ingest_file'
+            'ingest'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method ingest_file" % key
+                    " to method ingest_dataset" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `ingest_file`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `ingest_dataset`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -2129,190 +2701,159 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'ingest_file' in local_var_params:
-            body_params = local_var_params['ingest_file']
+        if 'ingest' in local_var_params:
+            body_params = local_var_params['ingest']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/files', 'POST',
+            '/api/repository/v1/datasets/{id}/ingest', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='JobModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def lookup_dataset_data_by_id(self, id, table, **kwargs):  # noqa: E501
-        """lookup_dataset_data_by_id  # noqa: E501
+    def ingest_file(self, id, **kwargs):  # noqa: E501
+        """ingest_file  # noqa: E501
 
-        Retrieve data for a table in a dataset  # noqa: E501
+        Ingest one file into the dataset file system; async returns a FileModel  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.lookup_dataset_data_by_id(id, table, async_req=True)
+        >>> thread = api.ingest_file(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str table: Name of table to get data from (required)
-        :param int offset: The number of rows to skip when retrieving the next page
-        :param int limit: The number of rows to return for the data
-        :param str sort: The table column to sort by
-        :param SqlSortDirection direction: The direction to sort.
-        :param str filter: A SQL WHERE clause to filter the table results.
+        :param FileLoadModel ingest_file: Ingest file request
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: DatasetDataModel
+        :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.lookup_dataset_data_by_id_with_http_info(id, table, **kwargs)  # noqa: E501
+        return self.ingest_file_with_http_info(id, **kwargs)  # noqa: E501
 
-    def lookup_dataset_data_by_id_with_http_info(self, id, table, **kwargs):  # noqa: E501
-        """lookup_dataset_data_by_id  # noqa: E501
+    def ingest_file_with_http_info(self, id, **kwargs):  # noqa: E501
+        """ingest_file  # noqa: E501
 
-        Retrieve data for a table in a dataset  # noqa: E501
+        Ingest one file into the dataset file system; async returns a FileModel  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.lookup_dataset_data_by_id_with_http_info(id, table, async_req=True)
+        >>> thread = api.ingest_file_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str table: Name of table to get data from (required)
-        :param int offset: The number of rows to skip when retrieving the next page
-        :param int limit: The number of rows to return for the data
-        :param str sort: The table column to sort by
-        :param SqlSortDirection direction: The direction to sort.
-        :param str filter: A SQL WHERE clause to filter the table results.
+        :param FileLoadModel ingest_file: Ingest file request
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(DatasetDataModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'table',
-            'offset',
-            'limit',
-            'sort',
-            'direction',
-            'filter'
+            'ingest_file'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method lookup_dataset_data_by_id" % key
+                    " to method ingest_file" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `lookup_dataset_data_by_id`")  # noqa: E501
-        # verify the required parameter 'table' is set
-        if self.api_client.client_side_validation and ('table' not in local_var_params or  # noqa: E501
-                                                        local_var_params['table'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `table` when calling `lookup_dataset_data_by_id`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `ingest_file`")  # noqa: E501
 
-        if self.api_client.client_side_validation and 'offset' in local_var_params and local_var_params['offset'] < 0:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `offset` when calling `lookup_dataset_data_by_id`, must be a value greater than or equal to `0`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 1000:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `lookup_dataset_data_by_id`, must be a value less than or equal to `1000`")  # noqa: E501
-        if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 1:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `limit` when calling `lookup_dataset_data_by_id`, must be a value greater than or equal to `1`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'table' in local_var_params:
-            path_params['table'] = local_var_params['table']  # noqa: E501
 
         query_params = []
-        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
-            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
-        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if 'sort' in local_var_params and local_var_params['sort'] is not None:  # noqa: E501
-            query_params.append(('sort', local_var_params['sort']))  # noqa: E501
-        if 'direction' in local_var_params and local_var_params['direction'] is not None:  # noqa: E501
-            query_params.append(('direction', local_var_params['direction']))  # noqa: E501
-        if 'filter' in local_var_params and local_var_params['filter'] is not None:  # noqa: E501
-            query_params.append(('filter', local_var_params['filter']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'ingest_file' in local_var_params:
+            body_params = local_var_params['ingest_file']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/data/{table}', 'GET',
+            '/api/repository/v1/datasets/{id}/files', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='DatasetDataModel',  # noqa: E501
+            response_type='JobModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -2422,15 +2963,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/files/{fileid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -2550,15 +3091,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/filesystem/objects', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -2568,257 +3109,263 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def open_transaction(self, id, transaction, **kwargs):  # noqa: E501
-        """open_transaction  # noqa: E501
+    def lookup_snapshot_file_by_id(self, id, fileid, **kwargs):  # noqa: E501
+        """lookup_snapshot_file_by_id  # noqa: E501
 
-        Create a transaction to be used for ingesting if you are chaining ingests together  # noqa: E501
+        Lookup metadata for one file  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.open_transaction(id, transaction, async_req=True)
+        >>> thread = api.lookup_snapshot_file_by_id(id, fileid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param TransactionCreateModel transaction: Open transaction request (required)
+        :param str fileid: A file id (required)
+        :param int depth: Enumeration depth; -1 means fully expand; 0 means no expansion; 1..N expands that many subdirectories
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: JobModel
+        :return: FileModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.open_transaction_with_http_info(id, transaction, **kwargs)  # noqa: E501
+        return self.lookup_snapshot_file_by_id_with_http_info(id, fileid, **kwargs)  # noqa: E501
 
-    def open_transaction_with_http_info(self, id, transaction, **kwargs):  # noqa: E501
-        """open_transaction  # noqa: E501
+    def lookup_snapshot_file_by_id_with_http_info(self, id, fileid, **kwargs):  # noqa: E501
+        """lookup_snapshot_file_by_id  # noqa: E501
 
-        Create a transaction to be used for ingesting if you are chaining ingests together  # noqa: E501
+        Lookup metadata for one file  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.open_transaction_with_http_info(id, transaction, async_req=True)
+        >>> thread = api.lookup_snapshot_file_by_id_with_http_info(id, fileid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param TransactionCreateModel transaction: Open transaction request (required)
+        :param str fileid: A file id (required)
+        :param int depth: Enumeration depth; -1 means fully expand; 0 means no expansion; 1..N expands that many subdirectories
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'transaction'
+            'fileid',
+            'depth'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method open_transaction" % key
+                    " to method lookup_snapshot_file_by_id" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `open_transaction`")  # noqa: E501
-        # verify the required parameter 'transaction' is set
-        if self.api_client.client_side_validation and ('transaction' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction` when calling `open_transaction`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `lookup_snapshot_file_by_id`")  # noqa: E501
+        # verify the required parameter 'fileid' is set
+        if self.api_client.client_side_validation and ('fileid' not in local_var_params or  # noqa: E501
+                                                        local_var_params['fileid'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `fileid` when calling `lookup_snapshot_file_by_id`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'fileid' in local_var_params:
+            path_params['fileid'] = local_var_params['fileid']  # noqa: E501
 
         query_params = []
+        if 'depth' in local_var_params and local_var_params['depth'] is not None:  # noqa: E501
+            query_params.append(('depth', local_var_params['depth']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'transaction' in local_var_params:
-            body_params = local_var_params['transaction']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/transactions', 'POST',
+            '/api/repository/v1/snapshots/{id}/files/{fileid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='JobModel',  # noqa: E501
+            response_type='FileModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def patch_dataset(self, id, **kwargs):  # noqa: E501
-        """patch_dataset  # noqa: E501
+    def lookup_snapshot_file_by_path(self, id, path, **kwargs):  # noqa: E501
+        """lookup_snapshot_file_by_path  # noqa: E501
 
-        Update supported fields of the specified dataset.  # noqa: E501
+        Lookup metadata for one file  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.patch_dataset(id, async_req=True)
+        >>> thread = api.lookup_snapshot_file_by_path(id, path, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param DatasetPatchRequestModel dataset_patch_request_model: A 'lite' dataset definition (used to modify supported fields of a dataset). Null assignments will be ignored.
+        :param str path: URL-encoded full path to a file or directory (required)
+        :param int depth: Enumeration depth; -1 means fully expand; 0 means no expansion; 1..N expands that many subdirectories
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: DatasetSummaryModel
+        :return: FileModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.patch_dataset_with_http_info(id, **kwargs)  # noqa: E501
+        return self.lookup_snapshot_file_by_path_with_http_info(id, path, **kwargs)  # noqa: E501
 
-    def patch_dataset_with_http_info(self, id, **kwargs):  # noqa: E501
-        """patch_dataset  # noqa: E501
+    def lookup_snapshot_file_by_path_with_http_info(self, id, path, **kwargs):  # noqa: E501
+        """lookup_snapshot_file_by_path  # noqa: E501
 
-        Update supported fields of the specified dataset.  # noqa: E501
+        Lookup metadata for one file  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.patch_dataset_with_http_info(id, async_req=True)
+        >>> thread = api.lookup_snapshot_file_by_path_with_http_info(id, path, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param DatasetPatchRequestModel dataset_patch_request_model: A 'lite' dataset definition (used to modify supported fields of a dataset). Null assignments will be ignored.
+        :param str path: URL-encoded full path to a file or directory (required)
+        :param int depth: Enumeration depth; -1 means fully expand; 0 means no expansion; 1..N expands that many subdirectories
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(DatasetSummaryModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'dataset_patch_request_model'
+            'path',
+            'depth'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method patch_dataset" % key
+                    " to method lookup_snapshot_file_by_path" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `patch_dataset`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `lookup_snapshot_file_by_path`")  # noqa: E501
+        # verify the required parameter 'path' is set
+        if self.api_client.client_side_validation and ('path' not in local_var_params or  # noqa: E501
+                                                        local_var_params['path'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `path` when calling `lookup_snapshot_file_by_path`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
+        if 'path' in local_var_params and local_var_params['path'] is not None:  # noqa: E501
+            query_params.append(('path', local_var_params['path']))  # noqa: E501
+        if 'depth' in local_var_params and local_var_params['depth'] is not None:  # noqa: E501
+            query_params.append(('depth', local_var_params['depth']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'dataset_patch_request_model' in local_var_params:
-            body_params = local_var_params['dataset_patch_request_model']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}', 'PATCH',
+            '/api/repository/v1/snapshots/{id}/filesystem/objects', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='DatasetSummaryModel',  # noqa: E501
+            response_type='FileModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -2923,15 +3470,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/assets/{assetid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -2941,26 +3488,126 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def reset_config(self, **kwargs):  # noqa: E501
+        """reset_config  # noqa: E501
+
+        Reset the configuration to original settings  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.reset_config(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.reset_config_with_http_info(**kwargs)  # noqa: E501
+
+    def reset_config_with_http_info(self, **kwargs):  # noqa: E501
+        """reset_config  # noqa: E501
+
+        Reset the configuration to original settings  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.reset_config_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method reset_config" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/configs/reset', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def retrieve_dataset(self, id, **kwargs):  # noqa: E501
         """retrieve_dataset  # noqa: E501
 
         Retrieve a dataset by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.retrieve_dataset(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param list[DatasetRequestAccessIncludeModel] include: A list of what to include with the dataset object
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2978,15 +3625,14 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.retrieve_dataset_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param list[DatasetRequestAccessIncludeModel] include: A list of what to include with the dataset object
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2996,16 +3642,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'include'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -3028,30 +3673,27 @@
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'include' in local_var_params and local_var_params['include'] is not None:  # noqa: E501
-            query_params.append(('include', local_var_params['include']))  # noqa: E501
-            collection_formats['include'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -3064,15 +3706,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def retrieve_dataset_policies(self, id, **kwargs):  # noqa: E501
         """retrieve_dataset_policies  # noqa: E501
 
-        Retrieve the read and discover policies for the dataset  # noqa: E501
+        Retrieve the read and discover policies for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.retrieve_dataset_policies(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -3089,15 +3731,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.retrieve_dataset_policies_with_http_info(id, **kwargs)  # noqa: E501
 
     def retrieve_dataset_policies_with_http_info(self, id, **kwargs):  # noqa: E501
         """retrieve_dataset_policies  # noqa: E501
 
-        Retrieve the read and discover policies for the dataset  # noqa: E501
+        Retrieve the read and discover policies for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.retrieve_dataset_policies_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -3157,15 +3799,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/repository/v1/datasets/{id}/policies', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -3175,60 +3817,60 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retrieve_dataset_summary(self, id, **kwargs):  # noqa: E501
-        """retrieve_dataset_summary  # noqa: E501
+    def retrieve_job(self, id, **kwargs):  # noqa: E501
+        """retrieve_job  # noqa: E501
 
-        Retrieve a dataset summary by id.  If the caller has permission to list the dataset in an enumeration, they will have permission to retrieve its summary, whereas they may lack necessary permissions to retrieve the full dataset object.   # noqa: E501
+        Retrieve a job's status by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_dataset_summary(id, async_req=True)
+        >>> thread = api.retrieve_job(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: DatasetSummaryModel
+        :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.retrieve_dataset_summary_with_http_info(id, **kwargs)  # noqa: E501
+        return self.retrieve_job_with_http_info(id, **kwargs)  # noqa: E501
 
-    def retrieve_dataset_summary_with_http_info(self, id, **kwargs):  # noqa: E501
-        """retrieve_dataset_summary  # noqa: E501
+    def retrieve_job_with_http_info(self, id, **kwargs):  # noqa: E501
+        """retrieve_job  # noqa: E501
 
-        Retrieve a dataset summary by id.  If the caller has permission to list the dataset in an enumeration, they will have permission to retrieve its summary, whereas they may lack necessary permissions to retrieve the full dataset object.   # noqa: E501
+        Retrieve a job's status by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_dataset_summary_with_http_info(id, async_req=True)
+        >>> thread = api.retrieve_job_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(DatasetSummaryModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -3243,22 +3885,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method retrieve_dataset_summary" % key
+                    " to method retrieve_job" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_dataset_summary`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -3271,201 +3913,192 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/summary', 'GET',
+            '/api/repository/v1/jobs/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='DatasetSummaryModel',  # noqa: E501
+            response_type='JobModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retrieve_transaction(self, id, transaction_id, **kwargs):  # noqa: E501
-        """retrieve_transaction  # noqa: E501
+    def retrieve_job_result(self, id, **kwargs):  # noqa: E501
+        """retrieve_job_result  # noqa: E501
 
-        Retrieve a given transaction  # noqa: E501
+        Retrieve a job's result by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_transaction(id, transaction_id, async_req=True)
+        >>> thread = api.retrieve_job_result(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str transaction_id: A UUID to used to identify a transaction in a dataset (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: TransactionModel
+        :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.retrieve_transaction_with_http_info(id, transaction_id, **kwargs)  # noqa: E501
+        return self.retrieve_job_result_with_http_info(id, **kwargs)  # noqa: E501
 
-    def retrieve_transaction_with_http_info(self, id, transaction_id, **kwargs):  # noqa: E501
-        """retrieve_transaction  # noqa: E501
+    def retrieve_job_result_with_http_info(self, id, **kwargs):  # noqa: E501
+        """retrieve_job_result  # noqa: E501
 
-        Retrieve a given transaction  # noqa: E501
+        Retrieve a job's result by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_transaction_with_http_info(id, transaction_id, async_req=True)
+        >>> thread = api.retrieve_job_result_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param str transaction_id: A UUID to used to identify a transaction in a dataset (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(TransactionModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(object, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'transaction_id'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method retrieve_transaction" % key
+                    " to method retrieve_job_result" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_transaction`")  # noqa: E501
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `retrieve_transaction`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_job_result`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'transaction_id' in local_var_params:
-            path_params['transactionId'] = local_var_params['transaction_id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/transactions/{transactionId}', 'GET',
+            '/api/repository/v1/jobs/{id}/result', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='TransactionModel',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retrieve_user_dataset_roles(self, id, **kwargs):  # noqa: E501
-        """retrieve_user_dataset_roles  # noqa: E501
+    def retrieve_snapshot(self, id, **kwargs):  # noqa: E501
+        """retrieve_snapshot  # noqa: E501
 
-        Retrieve the policies the calling user has on the dataset  # noqa: E501
+        Retrieve a snapshot by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_user_dataset_roles(id, async_req=True)
+        >>> thread = api.retrieve_snapshot(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: list[str]
+        :return: SnapshotModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.retrieve_user_dataset_roles_with_http_info(id, **kwargs)  # noqa: E501
+        return self.retrieve_snapshot_with_http_info(id, **kwargs)  # noqa: E501
 
-    def retrieve_user_dataset_roles_with_http_info(self, id, **kwargs):  # noqa: E501
-        """retrieve_user_dataset_roles  # noqa: E501
+    def retrieve_snapshot_with_http_info(self, id, **kwargs):  # noqa: E501
+        """retrieve_snapshot  # noqa: E501
 
-        Retrieve the policies the calling user has on the dataset  # noqa: E501
+        Retrieve a snapshot by id  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_user_dataset_roles_with_http_info(id, async_req=True)
+        >>> thread = api.retrieve_snapshot_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(list[str], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(SnapshotModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -3480,22 +4113,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method retrieve_user_dataset_roles" % key
+                    " to method retrieve_snapshot" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_user_dataset_roles`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_snapshot`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -3508,111 +4141,108 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/roles', 'GET',
+            '/api/repository/v1/snapshots/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[str]',  # noqa: E501
+            response_type='SnapshotModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_dataset_tags(self, id, **kwargs):  # noqa: E501
-        """update_dataset_tags  # noqa: E501
+    def retrieve_snapshot_policies(self, id, **kwargs):  # noqa: E501
+        """retrieve_snapshot_policies  # noqa: E501
 
-        Update tags on dataset  # noqa: E501
+        Retrieve the read and discover policies for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_dataset_tags(id, async_req=True)
+        >>> thread = api.retrieve_snapshot_policies(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param TagUpdateRequestModel tag_update_request_model:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: DatasetSummaryModel
+        :return: PolicyResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_dataset_tags_with_http_info(id, **kwargs)  # noqa: E501
+        return self.retrieve_snapshot_policies_with_http_info(id, **kwargs)  # noqa: E501
 
-    def update_dataset_tags_with_http_info(self, id, **kwargs):  # noqa: E501
-        """update_dataset_tags  # noqa: E501
+    def retrieve_snapshot_policies_with_http_info(self, id, **kwargs):  # noqa: E501
+        """retrieve_snapshot_policies  # noqa: E501
 
-        Update tags on dataset  # noqa: E501
+        Retrieve the read and discover policies for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_dataset_tags_with_http_info(id, async_req=True)
+        >>> thread = api.retrieve_snapshot_policies_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
-        :param TagUpdateRequestModel tag_update_request_model:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(DatasetSummaryModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PolicyResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'tag_update_request_model'
+            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_dataset_tags" % key
+                    " to method retrieve_snapshot_policies" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `update_dataset_tags`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_snapshot_policies`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -3620,81 +4250,310 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'tag_update_request_model' in local_var_params:
-            body_params = local_var_params['tag_update_request_model']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/policies', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PolicyResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def set_config_list(self, **kwargs):  # noqa: E501
+        """set_config_list  # noqa: E501
+
+        Set the a group of configurations  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_config_list(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param ConfigGroupModel config_model:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ConfigListModel
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.set_config_list_with_http_info(**kwargs)  # noqa: E501
+
+    def set_config_list_with_http_info(self, **kwargs):  # noqa: E501
+        """set_config_list  # noqa: E501
+
+        Set the a group of configurations  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_config_list_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param ConfigGroupModel config_model:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ConfigListModel, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'config_model'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method set_config_list" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'config_model' in local_var_params:
+            body_params = local_var_params['config_model']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/tags', 'PATCH',
+            '/api/repository/v1/configs', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='DatasetSummaryModel',  # noqa: E501
+            response_type='ConfigListModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_schema(self, id, dataset_schema_update_model, **kwargs):  # noqa: E501
-        """update_schema  # noqa: E501
+    def set_fault(self, name, **kwargs):  # noqa: E501
+        """set_fault  # noqa: E501
 
-        Modify a dataset's schema with additive changes  # noqa: E501
+        Enable or disable the named fault. Performing the put on a config that is not a fault is an error.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_schema(id, dataset_schema_update_model, async_req=True)
+        >>> thread = api.set_fault(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param DatasetSchemaUpdateModel dataset_schema_update_model: Update dataset schema (required)
+        :param str name: name of the configuration to (required)
+        :param ConfigEnableModel config_enable:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.set_fault_with_http_info(name, **kwargs)  # noqa: E501
+
+    def set_fault_with_http_info(self, name, **kwargs):  # noqa: E501
+        """set_fault  # noqa: E501
+
+        Enable or disable the named fault. Performing the put on a config that is not a fault is an error.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_fault_with_http_info(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str name: name of the configuration to (required)
+        :param ConfigEnableModel config_enable:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'name',
+            'config_enable'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method set_fault" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'name' is set
+        if self.api_client.client_side_validation and ('name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `name` when calling `set_fault`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'name' in local_var_params:
+            path_params['name'] = local_var_params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'config_enable' in local_var_params:
+            body_params = local_var_params['config_enable']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/configs/{name}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def upgrade(self, upgrade, **kwargs):  # noqa: E501
+        """upgrade  # noqa: E501
+
+        Extensible endpoint for triggering upgrade tasks in the data repository. The asynchronous result is UpgradeResponseModel  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.upgrade(upgrade, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param UpgradeModel upgrade: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: JobModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_schema_with_http_info(id, dataset_schema_update_model, **kwargs)  # noqa: E501
+        return self.upgrade_with_http_info(upgrade, **kwargs)  # noqa: E501
 
-    def update_schema_with_http_info(self, id, dataset_schema_update_model, **kwargs):  # noqa: E501
-        """update_schema  # noqa: E501
+    def upgrade_with_http_info(self, upgrade, **kwargs):  # noqa: E501
+        """upgrade  # noqa: E501
 
-        Modify a dataset's schema with additive changes  # noqa: E501
+        Extensible endpoint for triggering upgrade tasks in the data repository. The asynchronous result is UpgradeResponseModel  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_schema_with_http_info(id, dataset_schema_update_model, async_req=True)
+        >>> thread = api.upgrade_with_http_info(upgrade, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
-        :param DatasetSchemaUpdateModel dataset_schema_update_model: Update dataset schema (required)
+        :param UpgradeModel upgrade: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3704,78 +4563,176 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'dataset_schema_update_model'
+            'upgrade'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_schema" % key
+                    " to method upgrade" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `update_schema`")  # noqa: E501
-        # verify the required parameter 'dataset_schema_update_model' is set
-        if self.api_client.client_side_validation and ('dataset_schema_update_model' not in local_var_params or  # noqa: E501
-                                                        local_var_params['dataset_schema_update_model'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `dataset_schema_update_model` when calling `update_schema`")  # noqa: E501
+        # verify the required parameter 'upgrade' is set
+        if self.api_client.client_side_validation and ('upgrade' not in local_var_params or  # noqa: E501
+                                                        local_var_params['upgrade'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `upgrade` when calling `upgrade`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'dataset_schema_update_model' in local_var_params:
-            body_params = local_var_params['dataset_schema_update_model']
+        if 'upgrade' in local_var_params:
+            body_params = local_var_params['upgrade']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/updateSchema', 'POST',
+            '/api/repository/v1/upgrade', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='JobModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def user(self, **kwargs):  # noqa: E501
+        """user  # noqa: E501
+
+        Returns whether the user is registered with terra   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.user(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: UserStatusInfo
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.user_with_http_info(**kwargs)  # noqa: E501
+
+    def user_with_http_info(self, **kwargs):  # noqa: E501
+        """user  # noqa: E501
+
+        Returns whether the user is registered with terra   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.user_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(UserStatusInfo, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method user" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['googleoauth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/register/user', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='UserStatusInfo',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api/jobs_api.py` & `data-repo-client-1.64.0/data_repo_client/api/unauthenticated_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -20,371 +20,329 @@
 from data_repo_client.api_client import ApiClient
 from data_repo_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class JobsApi(object):
+class UnauthenticatedApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def enumerate_jobs(self, **kwargs):  # noqa: E501
-        """enumerate_jobs  # noqa: E501
+    def retrieve_repository_config(self, **kwargs):  # noqa: E501
+        """retrieve_repository_config  # noqa: E501
 
-        Returns a list of all of the jobs the caller has access to   # noqa: E501
+        Retrieve the repository configuration information  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_jobs(async_req=True)
+        >>> thread = api.retrieve_repository_config(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param int offset: The number of items to skip before starting to collect the result set.
-        :param int limit: The numbers of items to return.
-        :param SqlSortDirection direction: The direction to sort based on job creation time (default is descending).
-        :param str class_name: Filter by the flight's class
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: list[JobModel]
+        :return: RepositoryConfigurationModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.enumerate_jobs_with_http_info(**kwargs)  # noqa: E501
+        return self.retrieve_repository_config_with_http_info(**kwargs)  # noqa: E501
 
-    def enumerate_jobs_with_http_info(self, **kwargs):  # noqa: E501
-        """enumerate_jobs  # noqa: E501
+    def retrieve_repository_config_with_http_info(self, **kwargs):  # noqa: E501
+        """retrieve_repository_config  # noqa: E501
 
-        Returns a list of all of the jobs the caller has access to   # noqa: E501
+        Retrieve the repository configuration information  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.enumerate_jobs_with_http_info(async_req=True)
+        >>> thread = api.retrieve_repository_config_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param int offset: The number of items to skip before starting to collect the result set.
-        :param int limit: The numbers of items to return.
-        :param SqlSortDirection direction: The direction to sort based on job creation time (default is descending).
-        :param str class_name: Filter by the flight's class
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(list[JobModel], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RepositoryConfigurationModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'offset',
-            'limit',
-            'direction',
-            'class_name'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method enumerate_jobs" % key
+                    " to method retrieve_repository_config" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
-            query_params.append(('offset', local_var_params['offset']))  # noqa: E501
-        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
-            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
-        if 'direction' in local_var_params and local_var_params['direction'] is not None:  # noqa: E501
-            query_params.append(('direction', local_var_params['direction']))  # noqa: E501
-        if 'class_name' in local_var_params and local_var_params['class_name'] is not None:  # noqa: E501
-            query_params.append(('className', local_var_params['class_name']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/jobs', 'GET',
+            '/configuration', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[JobModel]',  # noqa: E501
+            response_type='RepositoryConfigurationModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retrieve_job(self, id, **kwargs):  # noqa: E501
-        """retrieve_job  # noqa: E501
+    def service_status(self, **kwargs):  # noqa: E501
+        """service_status  # noqa: E501
 
-        Retrieve a job's status by id  # noqa: E501
+        Returns the operational status of the service   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_job(id, async_req=True)
+        >>> thread = api.service_status(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: JobModel
+        :return: RepositoryStatusModel
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.retrieve_job_with_http_info(id, **kwargs)  # noqa: E501
+        return self.service_status_with_http_info(**kwargs)  # noqa: E501
 
-    def retrieve_job_with_http_info(self, id, **kwargs):  # noqa: E501
-        """retrieve_job  # noqa: E501
+    def service_status_with_http_info(self, **kwargs):  # noqa: E501
+        """service_status  # noqa: E501
 
-        Retrieve a job's status by id  # noqa: E501
+        Returns the operational status of the service   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_job_with_http_info(id, async_req=True)
+        >>> thread = api.service_status_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RepositoryStatusModel, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method retrieve_job" % key
+                    " to method service_status" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_job`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/jobs/{id}', 'GET',
+            '/status', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='JobModel',  # noqa: E501
+            response_type='RepositoryStatusModel',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def retrieve_job_result(self, id, **kwargs):  # noqa: E501
-        """retrieve_job_result  # noqa: E501
+    def shutdown_request(self, **kwargs):  # noqa: E501
+        """shutdown_request  # noqa: E501
 
-        Retrieve a job's result by id  # noqa: E501
+        Requests that this instance of DR Manager shut down. In production, this must be configured to only be callable by Kubernetes.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_job_result(id, async_req=True)
+        >>> thread = api.shutdown_request(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: object
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.retrieve_job_result_with_http_info(id, **kwargs)  # noqa: E501
+        return self.shutdown_request_with_http_info(**kwargs)  # noqa: E501
 
-    def retrieve_job_result_with_http_info(self, id, **kwargs):  # noqa: E501
-        """retrieve_job_result  # noqa: E501
+    def shutdown_request_with_http_info(self, **kwargs):  # noqa: E501
+        """shutdown_request  # noqa: E501
 
-        Retrieve a job's result by id  # noqa: E501
+        Requests that this instance of DR Manager shut down. In production, this must be configured to only be callable by Kubernetes.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.retrieve_job_result_with_http_info(id, async_req=True)
+        >>> thread = api.shutdown_request_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: A UUID to used to identify an object in the repository (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method retrieve_job_result" % key
+                    " to method shutdown_request" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `retrieve_job_result`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/jobs/{id}/result', 'GET',
+            '/shutdown', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='object',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api/profiles_api.py` & `data-repo-client-1.64.0/data_repo_client/api/resources_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -20,30 +20,30 @@
 from data_repo_client.api_client import ApiClient
 from data_repo_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ProfilesApi(object):
+class ResourcesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def add_profile_policy_member(self, id, policy_name, policy_member_request, **kwargs):  # noqa: E501
         """add_profile_policy_member  # noqa: E501
 
-        Adds a member to the specified policy for the profile. NOTE: Change may take up to 60 seconds to take effect.   # noqa: E501
+        Adds a member to the specified policy for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_profile_policy_member(id, policy_name, policy_member_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -62,15 +62,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.add_profile_policy_member_with_http_info(id, policy_name, policy_member_request, **kwargs)  # noqa: E501
 
     def add_profile_policy_member_with_http_info(self, id, policy_name, policy_member_request, **kwargs):  # noqa: E501
         """add_profile_policy_member  # noqa: E501
 
-        Adds a member to the specified policy for the profile. NOTE: Change may take up to 60 seconds to take effect.   # noqa: E501
+        Adds a member to the specified policy for the snapshot  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_profile_policy_member_with_http_info(id, policy_name, policy_member_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -150,15 +150,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles/{id}/policies/{policyName}/members', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -264,15 +264,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -378,15 +378,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -399,15 +399,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_profile_policy_member(self, id, policy_name, member_email, **kwargs):  # noqa: E501
         """delete_profile_policy_member  # noqa: E501
 
-        Removes a member from the specified policy for the profile. NOTE: Change may take up to 60 seconds to take effect.   # noqa: E501
+        Removes a member from the specified policy for the profile  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_profile_policy_member(id, policy_name, member_email, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -426,15 +426,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_profile_policy_member_with_http_info(id, policy_name, member_email, **kwargs)  # noqa: E501
 
     def delete_profile_policy_member_with_http_info(self, id, policy_name, member_email, **kwargs):  # noqa: E501
         """delete_profile_policy_member  # noqa: E501
 
-        Removes a member from the specified policy for the profile. NOTE: Change may take up to 60 seconds to take effect.   # noqa: E501
+        Removes a member from the specified policy for the profile  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_profile_policy_member_with_http_info(id, policy_name, member_email, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str id: A UUID to used to identify an object in the repository (required)
@@ -510,15 +510,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles/{id}/policies/{policyName}/members/{memberEmail}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -625,15 +625,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -739,15 +739,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -853,15 +853,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles/{id}/policies', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -971,15 +971,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
+        auth_settings = ['googleoauth']  # noqa: E501
 
         return self.api_client.call_api(
             '/api/resources/v1/profiles', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-1.64.0/test/test_snapshot_request_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,106 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-import re  # noqa: F401
+import unittest
+import datetime
 
-# python 2 and python 3 compatibility library
-import six
-
-from data_repo_client.api_client import ApiClient
-from data_repo_client.exceptions import (  # noqa: F401
-    ApiTypeError,
-    ApiValueError
-)
-
-
-class UpgradeApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient()
-        self.api_client = api_client
-
-    def upgrade(self, upgrade, **kwargs):  # noqa: E501
-        """upgrade  # noqa: E501
-
-        Extensible endpoint for triggering upgrade tasks in the data repository. The asynchronous result is UpgradeResponseModel  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.upgrade(upgrade, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param UpgradeModel upgrade: (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: JobModel
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.upgrade_with_http_info(upgrade, **kwargs)  # noqa: E501
-
-    def upgrade_with_http_info(self, upgrade, **kwargs):  # noqa: E501
-        """upgrade  # noqa: E501
-
-        Extensible endpoint for triggering upgrade tasks in the data repository. The asynchronous result is UpgradeResponseModel  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.upgrade_with_http_info(upgrade, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param UpgradeModel upgrade: (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(JobModel, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'upgrade'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
+import data_repo_client
+from data_repo_client.models.snapshot_request_model import SnapshotRequestModel  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestSnapshotRequestModel(unittest.TestCase):
+    """SnapshotRequestModel unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SnapshotRequestModel
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.snapshot_request_model.SnapshotRequestModel()  # noqa: E501
+        if include_optional :
+            return SnapshotRequestModel(
+                name = 'a', 
+                description = '0', 
+                contents = [
+                    data_repo_client.models.snapshot_request_contents_model.SnapshotRequestContentsModel(
+                        dataset_name = 'a', 
+                        mode = 'byAsset', 
+                        asset_spec = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel(
+                            asset_name = 'a', 
+                            root_values = [
+                                '0'
+                                ], ), 
+                        query_spec = data_repo_client.models.snapshot_request_query_model.SnapshotRequestQueryModel(
+                            asset_name = 'a', 
+                            query = '0', ), 
+                        row_id_spec = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel(
+                            tables = [
+                                data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                                    table_name = 'a', 
+                                    columns = [
+                                        'a'
+                                        ], 
+                                    row_ids = [
+                                        'a'
+                                        ], )
+                                ], ), )
+                    ], 
+                readers = [
+                    '0'
+                    ], 
+                profile_id = 'a'
+            )
+        else :
+            return SnapshotRequestModel(
+                name = 'a',
+                contents = [
+                    data_repo_client.models.snapshot_request_contents_model.SnapshotRequestContentsModel(
+                        dataset_name = 'a', 
+                        mode = 'byAsset', 
+                        asset_spec = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel(
+                            asset_name = 'a', 
+                            root_values = [
+                                '0'
+                                ], ), 
+                        query_spec = data_repo_client.models.snapshot_request_query_model.SnapshotRequestQueryModel(
+                            asset_name = 'a', 
+                            query = '0', ), 
+                        row_id_spec = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel(
+                            tables = [
+                                data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                                    table_name = 'a', 
+                                    columns = [
+                                        'a'
+                                        ], 
+                                    row_ids = [
+                                        'a'
+                                        ], )
+                                ], ), )
+                    ],
         )
 
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method upgrade" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'upgrade' is set
-        if self.api_client.client_side_validation and ('upgrade' not in local_var_params or  # noqa: E501
-                                                        local_var_params['upgrade'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `upgrade` when calling `upgrade`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'upgrade' in local_var_params:
-            body_params = local_var_params['upgrade']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['googleoauth', 'oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/upgrade', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='JobModel',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
+    def testSnapshotRequestModel(self):
+        """Test SnapshotRequestModel"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/api_client.py` & `data-repo-client-1.64.0/data_repo_client/api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.477.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/configuration.py` & `data-repo-client-1.64.0/data_repo_client/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -47,14 +47,33 @@
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
 
     :Example:
+
+    API Key Authentication Example.
+    Given the following security scheme in the OpenAPI specification:
+      components:
+        securitySchemes:
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
+
+    You can programmatically set the cookie:
+
+conf = data_repo_client.Configuration(
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
+)
+
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host="http://localhost",
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -314,23 +333,23 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if self.access_token is not None:
-            auth['googleoauth'] = {
-                'type': 'oauth2',
+        if 'Authorization' in self.api_key:
+            auth['authToken'] = {
+                'type': 'api_key',
                 'in': 'header',
                 'key': 'Authorization',
-                'value': 'Bearer ' + self.access_token
+                'value': self.get_api_key_with_prefix('Authorization')
             }
         if self.access_token is not None:
-            auth['oidc'] = {
+            auth['googleoauth'] = {
                 'type': 'oauth2',
                 'in': 'header',
                 'key': 'Authorization',
                 'value': 'Bearer ' + self.access_token
             }
         return auth
 
@@ -339,15 +358,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 1.477.0".\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-1.64.0/data_repo_client/models/drs_access_url.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,112 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class AccessInfoParquetModelTable(object):
+class DRSAccessURL(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
         'url': 'str',
-        'sas_token': 'str'
+        'headers': 'list[str]'
     }
 
     attribute_map = {
-        'name': 'name',
         'url': 'url',
-        'sas_token': 'sasToken'
+        'headers': 'headers'
     }
 
-    def __init__(self, name=None, url=None, sas_token=None, local_vars_configuration=None):  # noqa: E501
-        """AccessInfoParquetModelTable - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, url=None, headers=None, local_vars_configuration=None):  # noqa: E501
+        """DRSAccessURL - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
         self._url = None
-        self._sas_token = None
+        self._headers = None
         self.discriminator = None
 
-        self.name = name
         self.url = url
-        self.sas_token = sas_token
-
-    @property
-    def name(self):
-        """Gets the name of this AccessInfoParquetModelTable.  # noqa: E501
-
-        The name of the dataset table   # noqa: E501
-
-        :return: The name of this AccessInfoParquetModelTable.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this AccessInfoParquetModelTable.
-
-        The name of the dataset table   # noqa: E501
-
-        :param name: The name of this AccessInfoParquetModelTable.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-
-        self._name = name
+        if headers is not None:
+            self.headers = headers
 
     @property
     def url(self):
-        """Gets the url of this AccessInfoParquetModelTable.  # noqa: E501
+        """Gets the url of this DRSAccessURL.  # noqa: E501
 
-        The link to access the container that stores parquet files for this table   # noqa: E501
+        A fully resolvable URL that can be used to fetch the actual object bytes.  # noqa: E501
 
-        :return: The url of this AccessInfoParquetModelTable.  # noqa: E501
+        :return: The url of this DRSAccessURL.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this AccessInfoParquetModelTable.
+        """Sets the url of this DRSAccessURL.
 
-        The link to access the container that stores parquet files for this table   # noqa: E501
+        A fully resolvable URL that can be used to fetch the actual object bytes.  # noqa: E501
 
-        :param url: The url of this AccessInfoParquetModelTable.  # noqa: E501
+        :param url: The url of this DRSAccessURL.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
             raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
         self._url = url
 
     @property
-    def sas_token(self):
-        """Gets the sas_token of this AccessInfoParquetModelTable.  # noqa: E501
+    def headers(self):
+        """Gets the headers of this DRSAccessURL.  # noqa: E501
 
-        A short lived SAS token to access the parquet files for this table   # noqa: E501
+        An optional list of headers to include in the HTTP request to `url`. These headers can be used to provide auth tokens required to fetch the object bytes.  # noqa: E501
 
-        :return: The sas_token of this AccessInfoParquetModelTable.  # noqa: E501
-        :rtype: str
+        :return: The headers of this DRSAccessURL.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._sas_token
+        return self._headers
 
-    @sas_token.setter
-    def sas_token(self, sas_token):
-        """Sets the sas_token of this AccessInfoParquetModelTable.
+    @headers.setter
+    def headers(self, headers):
+        """Sets the headers of this DRSAccessURL.
 
-        A short lived SAS token to access the parquet files for this table   # noqa: E501
+        An optional list of headers to include in the HTTP request to `url`. These headers can be used to provide auth tokens required to fetch the object bytes.  # noqa: E501
 
-        :param sas_token: The sas_token of this AccessInfoParquetModelTable.  # noqa: E501
-        :type: str
+        :param headers: The headers of this DRSAccessURL.  # noqa: E501
+        :type: list[str]
         """
-        if self.local_vars_configuration.client_side_validation and sas_token is None:  # noqa: E501
-            raise ValueError("Invalid value for `sas_token`, must not be `None`")  # noqa: E501
 
-        self._sas_token = sas_token
+        self._headers = headers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -164,18 +134,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AccessInfoParquetModelTable):
+        if not isinstance(other, DRSAccessURL):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AccessInfoParquetModelTable):
+        if not isinstance(other, DRSAccessURL):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/asset_model.py` & `data-repo-client-1.64.0/data_repo_client/models/asset_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -117,26 +117,26 @@
 
         self._tables = tables
 
     @property
     def root_table(self):
         """Gets the root_table of this AssetModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :return: The root_table of this AssetModel.  # noqa: E501
         :rtype: str
         """
         return self._root_table
 
     @root_table.setter
     def root_table(self, root_table):
         """Sets the root_table of this AssetModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :param root_table: The root_table of this AssetModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and root_table is None:  # noqa: E501
             raise ValueError("Invalid value for `root_table`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
@@ -151,41 +151,41 @@
 
         self._root_table = root_table
 
     @property
     def root_column(self):
         """Gets the root_column of this AssetModel.  # noqa: E501
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :return: The root_column of this AssetModel.  # noqa: E501
         :rtype: str
         """
         return self._root_column
 
     @root_column.setter
     def root_column(self, root_column):
         """Sets the root_column of this AssetModel.
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :param root_column: The root_column of this AssetModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and root_column is None:  # noqa: E501
             raise ValueError("Invalid value for `root_column`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 root_column is not None and len(root_column) > 63):
             raise ValueError("Invalid value for `root_column`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 root_column is not None and len(root_column) < 1):
             raise ValueError("Invalid value for `root_column`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                root_column is not None and not re.search(r'^[a-zA-Z][_a-zA-Z0-9]*$', root_column)):  # noqa: E501
-            raise ValueError(r"Invalid value for `root_column`, must be a follow pattern or equal to `/^[a-zA-Z][_a-zA-Z0-9]*$/`")  # noqa: E501
+                root_column is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', root_column)):  # noqa: E501
+            raise ValueError(r"Invalid value for `root_column`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
         self._root_column = root_column
 
     @property
     def follow(self):
         """Gets the follow of this AssetModel.  # noqa: E501
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-1.64.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,110 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class AssetTableModel(object):
+class DataDeletionTableModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'columns': 'list[str]'
+        'table_name': 'str',
+        'gcs_file_spec': 'DataDeletionGcsFileModel'
     }
 
     attribute_map = {
-        'name': 'name',
-        'columns': 'columns'
+        'table_name': 'tableName',
+        'gcs_file_spec': 'gcsFileSpec'
     }
 
-    def __init__(self, name=None, columns=None, local_vars_configuration=None):  # noqa: E501
-        """AssetTableModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, table_name=None, gcs_file_spec=None, local_vars_configuration=None):  # noqa: E501
+        """DataDeletionTableModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._columns = None
+        self._table_name = None
+        self._gcs_file_spec = None
         self.discriminator = None
 
-        self.name = name
-        self.columns = columns
+        self.table_name = table_name
+        if gcs_file_spec is not None:
+            self.gcs_file_spec = gcs_file_spec
 
     @property
-    def name(self):
-        """Gets the name of this AssetTableModel.  # noqa: E501
+    def table_name(self):
+        """Gets the table_name of this DataDeletionTableModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        the name of a table in the dataset  # noqa: E501
 
-        :return: The name of this AssetTableModel.  # noqa: E501
+        :return: The table_name of this DataDeletionTableModel.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._table_name
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this AssetTableModel.
+    @table_name.setter
+    def table_name(self, table_name):
+        """Sets the table_name of this DataDeletionTableModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        the name of a table in the dataset  # noqa: E501
 
-        :param name: The name of this AssetTableModel.  # noqa: E501
+        :param table_name: The table_name of this DataDeletionTableModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 63):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and table_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._table_name = table_name
 
     @property
-    def columns(self):
-        """Gets the columns of this AssetTableModel.  # noqa: E501
+    def gcs_file_spec(self):
+        """Gets the gcs_file_spec of this DataDeletionTableModel.  # noqa: E501
 
 
-        :return: The columns of this AssetTableModel.  # noqa: E501
-        :rtype: list[str]
+        :return: The gcs_file_spec of this DataDeletionTableModel.  # noqa: E501
+        :rtype: DataDeletionGcsFileModel
         """
-        return self._columns
+        return self._gcs_file_spec
 
-    @columns.setter
-    def columns(self, columns):
-        """Sets the columns of this AssetTableModel.
+    @gcs_file_spec.setter
+    def gcs_file_spec(self, gcs_file_spec):
+        """Sets the gcs_file_spec of this DataDeletionTableModel.
 
 
-        :param columns: The columns of this AssetTableModel.  # noqa: E501
-        :type: list[str]
+        :param gcs_file_spec: The gcs_file_spec of this DataDeletionTableModel.  # noqa: E501
+        :type: DataDeletionGcsFileModel
         """
-        if self.local_vars_configuration.client_side_validation and columns is None:  # noqa: E501
-            raise ValueError("Invalid value for `columns`, must not be `None`")  # noqa: E501
 
-        self._columns = columns
+        self._gcs_file_spec = gcs_file_spec
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -142,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AssetTableModel):
+        if not isinstance(other, DataDeletionTableModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AssetTableModel):
+        if not isinstance(other, DataDeletionTableModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-1.64.0/data_repo_client/models/file_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,389 +1,329 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class BillingProfileModel(object):
+class FileModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
-        'billing_account_id': 'str',
-        'profile_name': 'str',
-        'biller': 'str',
+        'file_id': 'str',
+        'collection_id': 'str',
+        'path': 'str',
+        'size': 'int',
+        'checksums': 'list[DRSChecksum]',
+        'created': 'str',
         'description': 'str',
-        'cloud_platform': 'CloudPlatform',
-        'tenant_id': 'str',
-        'subscription_id': 'str',
-        'resource_group_name': 'str',
-        'application_deployment_name': 'str',
-        'created_date': 'str',
-        'created_by': 'str'
+        'file_type': 'FileModelType',
+        'file_detail': 'FileDetailModel',
+        'directory_detail': 'DirectoryDetailModel'
     }
 
     attribute_map = {
-        'id': 'id',
-        'billing_account_id': 'billingAccountId',
-        'profile_name': 'profileName',
-        'biller': 'biller',
+        'file_id': 'fileId',
+        'collection_id': 'collectionId',
+        'path': 'path',
+        'size': 'size',
+        'checksums': 'checksums',
+        'created': 'created',
         'description': 'description',
-        'cloud_platform': 'cloudPlatform',
-        'tenant_id': 'tenantId',
-        'subscription_id': 'subscriptionId',
-        'resource_group_name': 'resourceGroupName',
-        'application_deployment_name': 'applicationDeploymentName',
-        'created_date': 'createdDate',
-        'created_by': 'createdBy'
+        'file_type': 'fileType',
+        'file_detail': 'fileDetail',
+        'directory_detail': 'directoryDetail'
     }
 
-    def __init__(self, id=None, billing_account_id=None, profile_name=None, biller=None, description=None, cloud_platform=None, tenant_id=None, subscription_id=None, resource_group_name=None, application_deployment_name=None, created_date=None, created_by=None, local_vars_configuration=None):  # noqa: E501
-        """BillingProfileModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, file_id=None, collection_id=None, path=None, size=None, checksums=None, created=None, description=None, file_type=None, file_detail=None, directory_detail=None, local_vars_configuration=None):  # noqa: E501
+        """FileModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._billing_account_id = None
-        self._profile_name = None
-        self._biller = None
+        self._file_id = None
+        self._collection_id = None
+        self._path = None
+        self._size = None
+        self._checksums = None
+        self._created = None
         self._description = None
-        self._cloud_platform = None
-        self._tenant_id = None
-        self._subscription_id = None
-        self._resource_group_name = None
-        self._application_deployment_name = None
-        self._created_date = None
-        self._created_by = None
+        self._file_type = None
+        self._file_detail = None
+        self._directory_detail = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if billing_account_id is not None:
-            self.billing_account_id = billing_account_id
-        if profile_name is not None:
-            self.profile_name = profile_name
-        if biller is not None:
-            self.biller = biller
+        if file_id is not None:
+            self.file_id = file_id
+        if collection_id is not None:
+            self.collection_id = collection_id
+        if path is not None:
+            self.path = path
+        if size is not None:
+            self.size = size
+        if checksums is not None:
+            self.checksums = checksums
+        if created is not None:
+            self.created = created
         if description is not None:
             self.description = description
-        if cloud_platform is not None:
-            self.cloud_platform = cloud_platform
-        if tenant_id is not None:
-            self.tenant_id = tenant_id
-        if subscription_id is not None:
-            self.subscription_id = subscription_id
-        if resource_group_name is not None:
-            self.resource_group_name = resource_group_name
-        if application_deployment_name is not None:
-            self.application_deployment_name = application_deployment_name
-        if created_date is not None:
-            self.created_date = created_date
-        if created_by is not None:
-            self.created_by = created_by
+        if file_type is not None:
+            self.file_type = file_type
+        if file_detail is not None:
+            self.file_detail = file_detail
+        if directory_detail is not None:
+            self.directory_detail = directory_detail
 
     @property
-    def id(self):
-        """Gets the id of this BillingProfileModel.  # noqa: E501
+    def file_id(self):
+        """Gets the file_id of this FileModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Unique id of the filesystem object within the dataset  # noqa: E501
 
-        :return: The id of this BillingProfileModel.  # noqa: E501
+        :return: The file_id of this FileModel.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._file_id
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this BillingProfileModel.
+    @file_id.setter
+    def file_id(self, file_id):
+        """Sets the file_id of this FileModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Unique id of the filesystem object within the dataset  # noqa: E501
 
-        :param id: The id of this BillingProfileModel.  # noqa: E501
+        :param file_id: The file_id of this FileModel.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._file_id = file_id
 
     @property
-    def billing_account_id(self):
-        """Gets the billing_account_id of this BillingProfileModel.  # noqa: E501
+    def collection_id(self):
+        """Gets the collection_id of this FileModel.  # noqa: E501
 
-        unique identifier of the billing account from Google  # noqa: E501
+        Id of the dataset or snapshot directory describing the object  # noqa: E501
 
-        :return: The billing_account_id of this BillingProfileModel.  # noqa: E501
+        :return: The collection_id of this FileModel.  # noqa: E501
         :rtype: str
         """
-        return self._billing_account_id
+        return self._collection_id
 
-    @billing_account_id.setter
-    def billing_account_id(self, billing_account_id):
-        """Sets the billing_account_id of this BillingProfileModel.
+    @collection_id.setter
+    def collection_id(self, collection_id):
+        """Sets the collection_id of this FileModel.
 
-        unique identifier of the billing account from Google  # noqa: E501
+        Id of the dataset or snapshot directory describing the object  # noqa: E501
 
-        :param billing_account_id: The billing_account_id of this BillingProfileModel.  # noqa: E501
+        :param collection_id: The collection_id of this FileModel.  # noqa: E501
         :type: str
         """
 
-        self._billing_account_id = billing_account_id
+        self._collection_id = collection_id
 
     @property
-    def profile_name(self):
-        """Gets the profile_name of this BillingProfileModel.  # noqa: E501
+    def path(self):
+        """Gets the path of this FileModel.  # noqa: E501
 
-        display name to be used for the profile;  # noqa: E501
+        full path of the file in the dataset  # noqa: E501
 
-        :return: The profile_name of this BillingProfileModel.  # noqa: E501
+        :return: The path of this FileModel.  # noqa: E501
         :rtype: str
         """
-        return self._profile_name
+        return self._path
 
-    @profile_name.setter
-    def profile_name(self, profile_name):
-        """Sets the profile_name of this BillingProfileModel.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this FileModel.
 
-        display name to be used for the profile;  # noqa: E501
+        full path of the file in the dataset  # noqa: E501
 
-        :param profile_name: The profile_name of this BillingProfileModel.  # noqa: E501
+        :param path: The path of this FileModel.  # noqa: E501
         :type: str
         """
 
-        self._profile_name = profile_name
+        self._path = path
 
     @property
-    def biller(self):
-        """Gets the biller of this BillingProfileModel.  # noqa: E501
+    def size(self):
+        """Gets the size of this FileModel.  # noqa: E501
 
-        either “direct” or the reseller of the sub-account that sends the bill (like “on_spend”)  # noqa: E501
+        Always present for files - the file size in bytes Present for directories in snapshots - sum of sizes of objects in a directory   # noqa: E501
 
-        :return: The biller of this BillingProfileModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._biller
-
-    @biller.setter
-    def biller(self, biller):
-        """Sets the biller of this BillingProfileModel.
-
-        either “direct” or the reseller of the sub-account that sends the bill (like “on_spend”)  # noqa: E501
-
-        :param biller: The biller of this BillingProfileModel.  # noqa: E501
-        :type: str
-        """
-
-        self._biller = biller
-
-    @property
-    def description(self):
-        """Gets the description of this BillingProfileModel.  # noqa: E501
-
-        Free text that describes the profile  # noqa: E501
-
-        :return: The description of this BillingProfileModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this BillingProfileModel.
-
-        Free text that describes the profile  # noqa: E501
-
-        :param description: The description of this BillingProfileModel.  # noqa: E501
-        :type: str
+        :return: The size of this FileModel.  # noqa: E501
+        :rtype: int
         """
+        return self._size
 
-        self._description = description
-
-    @property
-    def cloud_platform(self):
-        """Gets the cloud_platform of this BillingProfileModel.  # noqa: E501
+    @size.setter
+    def size(self, size):
+        """Sets the size of this FileModel.
 
+        Always present for files - the file size in bytes Present for directories in snapshots - sum of sizes of objects in a directory   # noqa: E501
 
-        :return: The cloud_platform of this BillingProfileModel.  # noqa: E501
-        :rtype: CloudPlatform
+        :param size: The size of this FileModel.  # noqa: E501
+        :type: int
         """
-        return self._cloud_platform
-
-    @cloud_platform.setter
-    def cloud_platform(self, cloud_platform):
-        """Sets the cloud_platform of this BillingProfileModel.
 
-
-        :param cloud_platform: The cloud_platform of this BillingProfileModel.  # noqa: E501
-        :type: CloudPlatform
-        """
-
-        self._cloud_platform = cloud_platform
+        self._size = size
 
     @property
-    def tenant_id(self):
-        """Gets the tenant_id of this BillingProfileModel.  # noqa: E501
+    def checksums(self):
+        """Gets the checksums of this FileModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Always present for files - checksums; always includes crc32c. May include md5. Present for directories in snapshots - see DRS spec for algorithm for combining checksums of underlying directory contents.   # noqa: E501
 
-        :return: The tenant_id of this BillingProfileModel.  # noqa: E501
-        :rtype: str
+        :return: The checksums of this FileModel.  # noqa: E501
+        :rtype: list[DRSChecksum]
         """
-        return self._tenant_id
+        return self._checksums
 
-    @tenant_id.setter
-    def tenant_id(self, tenant_id):
-        """Sets the tenant_id of this BillingProfileModel.
+    @checksums.setter
+    def checksums(self, checksums):
+        """Sets the checksums of this FileModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Always present for files - checksums; always includes crc32c. May include md5. Present for directories in snapshots - see DRS spec for algorithm for combining checksums of underlying directory contents.   # noqa: E501
 
-        :param tenant_id: The tenant_id of this BillingProfileModel.  # noqa: E501
-        :type: str
+        :param checksums: The checksums of this FileModel.  # noqa: E501
+        :type: list[DRSChecksum]
         """
 
-        self._tenant_id = tenant_id
+        self._checksums = checksums
 
     @property
-    def subscription_id(self):
-        """Gets the subscription_id of this BillingProfileModel.  # noqa: E501
+    def created(self):
+        """Gets the created of this FileModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        timestamp of object creation in RFC3339  # noqa: E501
 
-        :return: The subscription_id of this BillingProfileModel.  # noqa: E501
+        :return: The created of this FileModel.  # noqa: E501
         :rtype: str
         """
-        return self._subscription_id
+        return self._created
 
-    @subscription_id.setter
-    def subscription_id(self, subscription_id):
-        """Sets the subscription_id of this BillingProfileModel.
+    @created.setter
+    def created(self, created):
+        """Sets the created of this FileModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        timestamp of object creation in RFC3339  # noqa: E501
 
-        :param subscription_id: The subscription_id of this BillingProfileModel.  # noqa: E501
+        :param created: The created of this FileModel.  # noqa: E501
         :type: str
         """
 
-        self._subscription_id = subscription_id
+        self._created = created
 
     @property
-    def resource_group_name(self):
-        """Gets the resource_group_name of this BillingProfileModel.  # noqa: E501
+    def description(self):
+        """Gets the description of this FileModel.  # noqa: E501
 
-        an optional resource group name for Azure  # noqa: E501
+        Human readable description of the file  # noqa: E501
 
-        :return: The resource_group_name of this BillingProfileModel.  # noqa: E501
+        :return: The description of this FileModel.  # noqa: E501
         :rtype: str
         """
-        return self._resource_group_name
+        return self._description
 
-    @resource_group_name.setter
-    def resource_group_name(self, resource_group_name):
-        """Sets the resource_group_name of this BillingProfileModel.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this FileModel.
 
-        an optional resource group name for Azure  # noqa: E501
+        Human readable description of the file  # noqa: E501
 
-        :param resource_group_name: The resource_group_name of this BillingProfileModel.  # noqa: E501
+        :param description: The description of this FileModel.  # noqa: E501
         :type: str
         """
 
-        self._resource_group_name = resource_group_name
+        self._description = description
 
     @property
-    def application_deployment_name(self):
-        """Gets the application_deployment_name of this BillingProfileModel.  # noqa: E501
+    def file_type(self):
+        """Gets the file_type of this FileModel.  # noqa: E501
 
-        an optional name for an application deployment for Azure  # noqa: E501
 
-        :return: The application_deployment_name of this BillingProfileModel.  # noqa: E501
-        :rtype: str
+        :return: The file_type of this FileModel.  # noqa: E501
+        :rtype: FileModelType
         """
-        return self._application_deployment_name
+        return self._file_type
 
-    @application_deployment_name.setter
-    def application_deployment_name(self, application_deployment_name):
-        """Sets the application_deployment_name of this BillingProfileModel.
+    @file_type.setter
+    def file_type(self, file_type):
+        """Sets the file_type of this FileModel.
 
-        an optional name for an application deployment for Azure  # noqa: E501
 
-        :param application_deployment_name: The application_deployment_name of this BillingProfileModel.  # noqa: E501
-        :type: str
+        :param file_type: The file_type of this FileModel.  # noqa: E501
+        :type: FileModelType
         """
 
-        self._application_deployment_name = application_deployment_name
+        self._file_type = file_type
 
     @property
-    def created_date(self):
-        """Gets the created_date of this BillingProfileModel.  # noqa: E501
+    def file_detail(self):
+        """Gets the file_detail of this FileModel.  # noqa: E501
 
-        Date the profile was created  # noqa: E501
 
-        :return: The created_date of this BillingProfileModel.  # noqa: E501
-        :rtype: str
+        :return: The file_detail of this FileModel.  # noqa: E501
+        :rtype: FileDetailModel
         """
-        return self._created_date
+        return self._file_detail
 
-    @created_date.setter
-    def created_date(self, created_date):
-        """Sets the created_date of this BillingProfileModel.
+    @file_detail.setter
+    def file_detail(self, file_detail):
+        """Sets the file_detail of this FileModel.
 
-        Date the profile was created  # noqa: E501
 
-        :param created_date: The created_date of this BillingProfileModel.  # noqa: E501
-        :type: str
+        :param file_detail: The file_detail of this FileModel.  # noqa: E501
+        :type: FileDetailModel
         """
 
-        self._created_date = created_date
+        self._file_detail = file_detail
 
     @property
-    def created_by(self):
-        """Gets the created_by of this BillingProfileModel.  # noqa: E501
+    def directory_detail(self):
+        """Gets the directory_detail of this FileModel.  # noqa: E501
 
-        Identity of the user who originally created the profile  # noqa: E501
 
-        :return: The created_by of this BillingProfileModel.  # noqa: E501
-        :rtype: str
+        :return: The directory_detail of this FileModel.  # noqa: E501
+        :rtype: DirectoryDetailModel
         """
-        return self._created_by
+        return self._directory_detail
 
-    @created_by.setter
-    def created_by(self, created_by):
-        """Sets the created_by of this BillingProfileModel.
+    @directory_detail.setter
+    def directory_detail(self, directory_detail):
+        """Sets the directory_detail of this FileModel.
 
-        Identity of the user who originally created the profile  # noqa: E501
 
-        :param created_by: The created_by of this BillingProfileModel.  # noqa: E501
-        :type: str
+        :param directory_detail: The directory_detail of this FileModel.  # noqa: E501
+        :type: DirectoryDetailModel
         """
 
-        self._created_by = created_by
+        self._directory_detail = directory_detail
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -411,18 +351,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BillingProfileModel):
+        if not isinstance(other, FileModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BillingProfileModel):
+        if not isinstance(other, FileModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-1.64.0/data_repo_client/models/dataset_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,335 +1,292 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class BillingProfileRequestModel(object):
+class DatasetModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'billing_account_id': 'str',
-        'profile_name': 'str',
-        'biller': 'str',
+        'id': 'str',
+        'name': 'str',
         'description': 'str',
-        'cloud_platform': 'CloudPlatform',
-        'tenant_id': 'str',
-        'subscription_id': 'str',
-        'resource_group_name': 'str',
-        'application_deployment_name': 'str',
-        'id': 'str'
+        'default_profile_id': 'str',
+        'data_project': 'str',
+        'default_snapshot_id': 'str',
+        'schema': 'DatasetSpecificationModel',
+        'created_date': 'str'
     }
 
     attribute_map = {
-        'billing_account_id': 'billingAccountId',
-        'profile_name': 'profileName',
-        'biller': 'biller',
+        'id': 'id',
+        'name': 'name',
         'description': 'description',
-        'cloud_platform': 'cloudPlatform',
-        'tenant_id': 'tenantId',
-        'subscription_id': 'subscriptionId',
-        'resource_group_name': 'resourceGroupName',
-        'application_deployment_name': 'applicationDeploymentName',
-        'id': 'id'
+        'default_profile_id': 'defaultProfileId',
+        'data_project': 'dataProject',
+        'default_snapshot_id': 'defaultSnapshotId',
+        'schema': 'schema',
+        'created_date': 'createdDate'
     }
 
-    def __init__(self, billing_account_id=None, profile_name=None, biller=None, description=None, cloud_platform=None, tenant_id=None, subscription_id=None, resource_group_name=None, application_deployment_name=None, id=None, local_vars_configuration=None):  # noqa: E501
-        """BillingProfileRequestModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, name=None, description=None, default_profile_id=None, data_project=None, default_snapshot_id=None, schema=None, created_date=None, local_vars_configuration=None):  # noqa: E501
+        """DatasetModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._billing_account_id = None
-        self._profile_name = None
-        self._biller = None
-        self._description = None
-        self._cloud_platform = None
-        self._tenant_id = None
-        self._subscription_id = None
-        self._resource_group_name = None
-        self._application_deployment_name = None
         self._id = None
+        self._name = None
+        self._description = None
+        self._default_profile_id = None
+        self._data_project = None
+        self._default_snapshot_id = None
+        self._schema = None
+        self._created_date = None
         self.discriminator = None
 
-        if billing_account_id is not None:
-            self.billing_account_id = billing_account_id
-        self.profile_name = profile_name
-        self.biller = biller
-        if description is not None:
-            self.description = description
-        if cloud_platform is not None:
-            self.cloud_platform = cloud_platform
-        if tenant_id is not None:
-            self.tenant_id = tenant_id
-        if subscription_id is not None:
-            self.subscription_id = subscription_id
-        if resource_group_name is not None:
-            self.resource_group_name = resource_group_name
-        if application_deployment_name is not None:
-            self.application_deployment_name = application_deployment_name
         if id is not None:
             self.id = id
+        if name is not None:
+            self.name = name
+        if description is not None:
+            self.description = description
+        if default_profile_id is not None:
+            self.default_profile_id = default_profile_id
+        if data_project is not None:
+            self.data_project = data_project
+        if default_snapshot_id is not None:
+            self.default_snapshot_id = default_snapshot_id
+        if schema is not None:
+            self.schema = schema
+        if created_date is not None:
+            self.created_date = created_date
 
     @property
-    def billing_account_id(self):
-        """Gets the billing_account_id of this BillingProfileRequestModel.  # noqa: E501
-
-        unique identifier of the billing account from Google  # noqa: E501
-
-        :return: The billing_account_id of this BillingProfileRequestModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._billing_account_id
-
-    @billing_account_id.setter
-    def billing_account_id(self, billing_account_id):
-        """Sets the billing_account_id of this BillingProfileRequestModel.
-
-        unique identifier of the billing account from Google  # noqa: E501
-
-        :param billing_account_id: The billing_account_id of this BillingProfileRequestModel.  # noqa: E501
-        :type: str
-        """
-
-        self._billing_account_id = billing_account_id
-
-    @property
-    def profile_name(self):
-        """Gets the profile_name of this BillingProfileRequestModel.  # noqa: E501
+    def id(self):
+        """Gets the id of this DatasetModel.  # noqa: E501
 
-        display name to be used for the profile;  # noqa: E501
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :return: The profile_name of this BillingProfileRequestModel.  # noqa: E501
+        :return: The id of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._profile_name
+        return self._id
 
-    @profile_name.setter
-    def profile_name(self, profile_name):
-        """Sets the profile_name of this BillingProfileRequestModel.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this DatasetModel.
 
-        display name to be used for the profile;  # noqa: E501
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :param profile_name: The profile_name of this BillingProfileRequestModel.  # noqa: E501
+        :param id: The id of this DatasetModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and profile_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `profile_name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                id is not None and not re.search(r'^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}', id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}/`")  # noqa: E501
 
-        self._profile_name = profile_name
+        self._id = id
 
     @property
-    def biller(self):
-        """Gets the biller of this BillingProfileRequestModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this DatasetModel.  # noqa: E501
 
-        either “direct” or the reseller of the sub-account that sends the bill (like “on_spend”)  # noqa: E501
+        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
 
-        :return: The biller of this BillingProfileRequestModel.  # noqa: E501
+        :return: The name of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._biller
+        return self._name
 
-    @biller.setter
-    def biller(self, biller):
-        """Sets the biller of this BillingProfileRequestModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this DatasetModel.
 
-        either “direct” or the reseller of the sub-account that sends the bill (like “on_spend”)  # noqa: E501
+        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
 
-        :param biller: The biller of this BillingProfileRequestModel.  # noqa: E501
+        :param name: The name of this DatasetModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and biller is None:  # noqa: E501
-            raise ValueError("Invalid value for `biller`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 511):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `511`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._biller = biller
+        self._name = name
 
     @property
     def description(self):
-        """Gets the description of this BillingProfileRequestModel.  # noqa: E501
+        """Gets the description of this DatasetModel.  # noqa: E501
 
-        Free text that describes the profile  # noqa: E501
+        Description of the dataset  # noqa: E501
 
-        :return: The description of this BillingProfileRequestModel.  # noqa: E501
+        :return: The description of this DatasetModel.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this BillingProfileRequestModel.
+        """Sets the description of this DatasetModel.
 
-        Free text that describes the profile  # noqa: E501
+        Description of the dataset  # noqa: E501
 
-        :param description: The description of this BillingProfileRequestModel.  # noqa: E501
+        :param description: The description of this DatasetModel.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
-    def cloud_platform(self):
-        """Gets the cloud_platform of this BillingProfileRequestModel.  # noqa: E501
-
-
-        :return: The cloud_platform of this BillingProfileRequestModel.  # noqa: E501
-        :rtype: CloudPlatform
-        """
-        return self._cloud_platform
-
-    @cloud_platform.setter
-    def cloud_platform(self, cloud_platform):
-        """Sets the cloud_platform of this BillingProfileRequestModel.
-
-
-        :param cloud_platform: The cloud_platform of this BillingProfileRequestModel.  # noqa: E501
-        :type: CloudPlatform
-        """
-
-        self._cloud_platform = cloud_platform
-
-    @property
-    def tenant_id(self):
-        """Gets the tenant_id of this BillingProfileRequestModel.  # noqa: E501
+    def default_profile_id(self):
+        """Gets the default_profile_id of this DatasetModel.  # noqa: E501
 
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :return: The tenant_id of this BillingProfileRequestModel.  # noqa: E501
+        :return: The default_profile_id of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._tenant_id
+        return self._default_profile_id
 
-    @tenant_id.setter
-    def tenant_id(self, tenant_id):
-        """Sets the tenant_id of this BillingProfileRequestModel.
+    @default_profile_id.setter
+    def default_profile_id(self, default_profile_id):
+        """Sets the default_profile_id of this DatasetModel.
 
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :param tenant_id: The tenant_id of this BillingProfileRequestModel.  # noqa: E501
+        :param default_profile_id: The default_profile_id of this DatasetModel.  # noqa: E501
         :type: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                default_profile_id is not None and not re.search(r'^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}', default_profile_id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `default_profile_id`, must be a follow pattern or equal to `/^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}/`")  # noqa: E501
 
-        self._tenant_id = tenant_id
+        self._default_profile_id = default_profile_id
 
     @property
-    def subscription_id(self):
-        """Gets the subscription_id of this BillingProfileRequestModel.  # noqa: E501
+    def data_project(self):
+        """Gets the data_project of this DatasetModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Project id of the project where tabular data in BigQuery lives  # noqa: E501
 
-        :return: The subscription_id of this BillingProfileRequestModel.  # noqa: E501
+        :return: The data_project of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._subscription_id
+        return self._data_project
 
-    @subscription_id.setter
-    def subscription_id(self, subscription_id):
-        """Sets the subscription_id of this BillingProfileRequestModel.
+    @data_project.setter
+    def data_project(self, data_project):
+        """Sets the data_project of this DatasetModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Project id of the project where tabular data in BigQuery lives  # noqa: E501
 
-        :param subscription_id: The subscription_id of this BillingProfileRequestModel.  # noqa: E501
+        :param data_project: The data_project of this DatasetModel.  # noqa: E501
         :type: str
         """
 
-        self._subscription_id = subscription_id
+        self._data_project = data_project
 
     @property
-    def resource_group_name(self):
-        """Gets the resource_group_name of this BillingProfileRequestModel.  # noqa: E501
+    def default_snapshot_id(self):
+        """Gets the default_snapshot_id of this DatasetModel.  # noqa: E501
 
-        an optional resource group name for Azure  # noqa: E501
+        Id of the auto-generated default passthru snapshot  # noqa: E501
 
-        :return: The resource_group_name of this BillingProfileRequestModel.  # noqa: E501
+        :return: The default_snapshot_id of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._resource_group_name
+        return self._default_snapshot_id
 
-    @resource_group_name.setter
-    def resource_group_name(self, resource_group_name):
-        """Sets the resource_group_name of this BillingProfileRequestModel.
+    @default_snapshot_id.setter
+    def default_snapshot_id(self, default_snapshot_id):
+        """Sets the default_snapshot_id of this DatasetModel.
 
-        an optional resource group name for Azure  # noqa: E501
+        Id of the auto-generated default passthru snapshot  # noqa: E501
 
-        :param resource_group_name: The resource_group_name of this BillingProfileRequestModel.  # noqa: E501
+        :param default_snapshot_id: The default_snapshot_id of this DatasetModel.  # noqa: E501
         :type: str
         """
 
-        self._resource_group_name = resource_group_name
+        self._default_snapshot_id = default_snapshot_id
 
     @property
-    def application_deployment_name(self):
-        """Gets the application_deployment_name of this BillingProfileRequestModel.  # noqa: E501
+    def schema(self):
+        """Gets the schema of this DatasetModel.  # noqa: E501
 
-        an optional name for an application deployment for Azure  # noqa: E501
 
-        :return: The application_deployment_name of this BillingProfileRequestModel.  # noqa: E501
-        :rtype: str
+        :return: The schema of this DatasetModel.  # noqa: E501
+        :rtype: DatasetSpecificationModel
         """
-        return self._application_deployment_name
+        return self._schema
 
-    @application_deployment_name.setter
-    def application_deployment_name(self, application_deployment_name):
-        """Sets the application_deployment_name of this BillingProfileRequestModel.
+    @schema.setter
+    def schema(self, schema):
+        """Sets the schema of this DatasetModel.
 
-        an optional name for an application deployment for Azure  # noqa: E501
 
-        :param application_deployment_name: The application_deployment_name of this BillingProfileRequestModel.  # noqa: E501
-        :type: str
+        :param schema: The schema of this DatasetModel.  # noqa: E501
+        :type: DatasetSpecificationModel
         """
 
-        self._application_deployment_name = application_deployment_name
+        self._schema = schema
 
     @property
-    def id(self):
-        """Gets the id of this BillingProfileRequestModel.  # noqa: E501
+    def created_date(self):
+        """Gets the created_date of this DatasetModel.  # noqa: E501
 
-        Deprecated: allowed for backwards compatibility. Recommendation: leave this unset for TDR to generate a universally unique identifier for your new billing profile.   # noqa: E501
+        Date the dataset was created  # noqa: E501
 
-        :return: The id of this BillingProfileRequestModel.  # noqa: E501
+        :return: The created_date of this DatasetModel.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._created_date
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this BillingProfileRequestModel.
+    @created_date.setter
+    def created_date(self, created_date):
+        """Sets the created_date of this DatasetModel.
 
-        Deprecated: allowed for backwards compatibility. Recommendation: leave this unset for TDR to generate a universally unique identifier for your new billing profile.   # noqa: E501
+        Date the dataset was created  # noqa: E501
 
-        :param id: The id of this BillingProfileRequestModel.  # noqa: E501
+        :param created_date: The created_date of this DatasetModel.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._created_date = created_date
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -357,18 +314,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BillingProfileRequestModel):
+        if not isinstance(other, DatasetModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BillingProfileRequestModel):
+        if not isinstance(other, DatasetModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -32,45 +32,41 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'profile_id': 'str',
         'load_tag': 'str',
         'max_failed_file_loads': 'int',
-        'load_array': 'list[BulkLoadFileModel]',
-        'bulk_mode': 'bool'
+        'load_array': 'list[BulkLoadFileModel]'
     }
 
     attribute_map = {
         'profile_id': 'profileId',
         'load_tag': 'loadTag',
         'max_failed_file_loads': 'maxFailedFileLoads',
-        'load_array': 'loadArray',
-        'bulk_mode': 'bulkMode'
+        'load_array': 'loadArray'
     }
 
-    def __init__(self, profile_id=None, load_tag=None, max_failed_file_loads=0, load_array=None, bulk_mode=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, profile_id=None, load_tag=None, max_failed_file_loads=0, load_array=None, local_vars_configuration=None):  # noqa: E501
         """BulkLoadArrayRequestModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._profile_id = None
         self._load_tag = None
         self._max_failed_file_loads = None
         self._load_array = None
-        self._bulk_mode = None
         self.discriminator = None
 
         self.profile_id = profile_id
         self.load_tag = load_tag
-        self.max_failed_file_loads = max_failed_file_loads
+        if max_failed_file_loads is not None:
+            self.max_failed_file_loads = max_failed_file_loads
         self.load_array = load_array
-        if bulk_mode is not None:
-            self.bulk_mode = bulk_mode
 
     @property
     def profile_id(self):
         """Gets the profile_id of this BulkLoadArrayRequestModel.  # noqa: E501
 
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
@@ -86,14 +82,17 @@
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
         :param profile_id: The profile_id of this BulkLoadArrayRequestModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and profile_id is None:  # noqa: E501
             raise ValueError("Invalid value for `profile_id`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                profile_id is not None and not re.search(r'^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}', profile_id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `profile_id`, must be a follow pattern or equal to `/^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}/`")  # noqa: E501
 
         self._profile_id = profile_id
 
     @property
     def load_tag(self):
         """Gets the load_tag of this BulkLoadArrayRequestModel.  # noqa: E501
 
@@ -134,16 +133,14 @@
         """Sets the max_failed_file_loads of this BulkLoadArrayRequestModel.
 
         max number of failed file loads before stopping; if -1, allow any number of errors  # noqa: E501
 
         :param max_failed_file_loads: The max_failed_file_loads of this BulkLoadArrayRequestModel.  # noqa: E501
         :type: int
         """
-        if self.local_vars_configuration.client_side_validation and max_failed_file_loads is None:  # noqa: E501
-            raise ValueError("Invalid value for `max_failed_file_loads`, must not be `None`")  # noqa: E501
 
         self._max_failed_file_loads = max_failed_file_loads
 
     @property
     def load_array(self):
         """Gets the load_array of this BulkLoadArrayRequestModel.  # noqa: E501
 
@@ -164,37 +161,14 @@
         :type: list[BulkLoadFileModel]
         """
         if self.local_vars_configuration.client_side_validation and load_array is None:  # noqa: E501
             raise ValueError("Invalid value for `load_array`, must not be `None`")  # noqa: E501
 
         self._load_array = load_array
 
-    @property
-    def bulk_mode(self):
-        """Gets the bulk_mode of this BulkLoadArrayRequestModel.  # noqa: E501
-
-        If true, file ingest will be performed in bulk mode.  The tradeoff for the performance improvements are that: - the dataset will be locked exclusively - some safeguards can not be enforced during loads.  Given that, it's recommended that   you use a maxFailedFileLoads value of 0 - the assumption is that file metadata must all fit into memory so configure the   deployment accordingly   # noqa: E501
-
-        :return: The bulk_mode of this BulkLoadArrayRequestModel.  # noqa: E501
-        :rtype: bool
-        """
-        return self._bulk_mode
-
-    @bulk_mode.setter
-    def bulk_mode(self, bulk_mode):
-        """Sets the bulk_mode of this BulkLoadArrayRequestModel.
-
-        If true, file ingest will be performed in bulk mode.  The tradeoff for the performance improvements are that: - the dataset will be locked exclusively - some safeguards can not be enforced during loads.  Given that, it's recommended that   you use a maxFailedFileLoads value of 0 - the assumption is that file metadata must all fit into memory so configure the   deployment accordingly   # noqa: E501
-
-        :param bulk_mode: The bulk_mode of this BulkLoadArrayRequestModel.  # noqa: E501
-        :type: bool
-        """
-
-        self._bulk_mode = bulk_mode
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -32,47 +32,42 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'source_path': 'str',
         'target_path': 'str',
         'mime_type': 'str',
-        'description': 'str',
-        'md5': 'str'
+        'description': 'str'
     }
 
     attribute_map = {
         'source_path': 'sourcePath',
         'target_path': 'targetPath',
         'mime_type': 'mimeType',
-        'description': 'description',
-        'md5': 'md5'
+        'description': 'description'
     }
 
-    def __init__(self, source_path=None, target_path=None, mime_type=None, description=None, md5=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_path=None, target_path=None, mime_type=None, description=None, local_vars_configuration=None):  # noqa: E501
         """BulkLoadFileModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_path = None
         self._target_path = None
         self._mime_type = None
         self._description = None
-        self._md5 = None
         self.discriminator = None
 
         self.source_path = source_path
         self.target_path = target_path
         if mime_type is not None:
             self.mime_type = mime_type
         if description is not None:
             self.description = description
-        if md5 is not None:
-            self.md5 = md5
 
     @property
     def source_path(self):
         """Gets the source_path of this BulkLoadFileModel.  # noqa: E501
 
         gs URL of the source file to load  # noqa: E501
 
@@ -162,37 +157,14 @@
 
         :param description: The description of this BulkLoadFileModel.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
-    @property
-    def md5(self):
-        """Gets the md5 of this BulkLoadFileModel.  # noqa: E501
-
-        A hex representation of the  md5 for the file.  If an md5 exists for the file being ingested, it will be validated against this value and the file's ingest will fail if the values do not match.  If no md5 hash is present on the file being ingested, this value will be stored for the file.  If this value is not specified, then the md5 from the file being ingested (from the cloud provider) will be used   # noqa: E501
-
-        :return: The md5 of this BulkLoadFileModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._md5
-
-    @md5.setter
-    def md5(self, md5):
-        """Sets the md5 of this BulkLoadFileModel.
-
-        A hex representation of the  md5 for the file.  If an md5 exists for the file being ingested, it will be validated against this value and the file's ingest will fail if the values do not match.  If no md5 hash is present on the file being ingested, this value will be stored for the file.  If this value is not specified, then the md5 from the file being ingested (from the cloud provider) will be used   # noqa: E501
-
-        :param md5: The md5 of this BulkLoadFileModel.  # noqa: E501
-        :type: str
-        """
-
-        self._md5 = md5
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-1.64.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,109 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class BulkLoadFileResultModel(object):
+class EnumerateBillingProfileModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'source_path': 'str',
-        'target_path': 'str',
-        'state': 'BulkLoadFileState',
-        'file_id': 'str',
-        'error': 'str'
+        'total': 'int',
+        'items': 'list[BillingProfileModel]'
     }
 
     attribute_map = {
-        'source_path': 'sourcePath',
-        'target_path': 'targetPath',
-        'state': 'state',
-        'file_id': 'fileId',
-        'error': 'error'
+        'total': 'total',
+        'items': 'items'
     }
 
-    def __init__(self, source_path=None, target_path=None, state=None, file_id=None, error=None, local_vars_configuration=None):  # noqa: E501
-        """BulkLoadFileResultModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, total=None, items=None, local_vars_configuration=None):  # noqa: E501
+        """EnumerateBillingProfileModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._source_path = None
-        self._target_path = None
-        self._state = None
-        self._file_id = None
-        self._error = None
+        self._total = None
+        self._items = None
         self.discriminator = None
 
-        self.source_path = source_path
-        self.target_path = target_path
-        if state is not None:
-            self.state = state
-        if file_id is not None:
-            self.file_id = file_id
-        if error is not None:
-            self.error = error
+        if total is not None:
+            self.total = total
+        if items is not None:
+            self.items = items
 
     @property
-    def source_path(self):
-        """Gets the source_path of this BulkLoadFileResultModel.  # noqa: E501
+    def total(self):
+        """Gets the total of this EnumerateBillingProfileModel.  # noqa: E501
 
-        gs URL of the source file to load  # noqa: E501
+        Total number of billing profiles  # noqa: E501
 
-        :return: The source_path of this BulkLoadFileResultModel.  # noqa: E501
-        :rtype: str
+        :return: The total of this EnumerateBillingProfileModel.  # noqa: E501
+        :rtype: int
         """
-        return self._source_path
+        return self._total
 
-    @source_path.setter
-    def source_path(self, source_path):
-        """Sets the source_path of this BulkLoadFileResultModel.
+    @total.setter
+    def total(self, total):
+        """Sets the total of this EnumerateBillingProfileModel.
 
-        gs URL of the source file to load  # noqa: E501
+        Total number of billing profiles  # noqa: E501
 
-        :param source_path: The source_path of this BulkLoadFileResultModel.  # noqa: E501
-        :type: str
+        :param total: The total of this EnumerateBillingProfileModel.  # noqa: E501
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and source_path is None:  # noqa: E501
-            raise ValueError("Invalid value for `source_path`, must not be `None`")  # noqa: E501
 
-        self._source_path = source_path
+        self._total = total
 
     @property
-    def target_path(self):
-        """Gets the target_path of this BulkLoadFileResultModel.  # noqa: E501
+    def items(self):
+        """Gets the items of this EnumerateBillingProfileModel.  # noqa: E501
 
-        Full path within the dataset where the file should be placed. The path must start with /.   # noqa: E501
 
-        :return: The target_path of this BulkLoadFileResultModel.  # noqa: E501
-        :rtype: str
+        :return: The items of this EnumerateBillingProfileModel.  # noqa: E501
+        :rtype: list[BillingProfileModel]
         """
-        return self._target_path
+        return self._items
 
-    @target_path.setter
-    def target_path(self, target_path):
-        """Sets the target_path of this BulkLoadFileResultModel.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this EnumerateBillingProfileModel.
 
-        Full path within the dataset where the file should be placed. The path must start with /.   # noqa: E501
 
-        :param target_path: The target_path of this BulkLoadFileResultModel.  # noqa: E501
-        :type: str
+        :param items: The items of this EnumerateBillingProfileModel.  # noqa: E501
+        :type: list[BillingProfileModel]
         """
-        if self.local_vars_configuration.client_side_validation and target_path is None:  # noqa: E501
-            raise ValueError("Invalid value for `target_path`, must not be `None`")  # noqa: E501
 
-        self._target_path = target_path
-
-    @property
-    def state(self):
-        """Gets the state of this BulkLoadFileResultModel.  # noqa: E501
-
-
-        :return: The state of this BulkLoadFileResultModel.  # noqa: E501
-        :rtype: BulkLoadFileState
-        """
-        return self._state
-
-    @state.setter
-    def state(self, state):
-        """Sets the state of this BulkLoadFileResultModel.
-
-
-        :param state: The state of this BulkLoadFileResultModel.  # noqa: E501
-        :type: BulkLoadFileState
-        """
-
-        self._state = state
-
-    @property
-    def file_id(self):
-        """Gets the file_id of this BulkLoadFileResultModel.  # noqa: E501
-
-        The fileId of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
-
-        :return: The file_id of this BulkLoadFileResultModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._file_id
-
-    @file_id.setter
-    def file_id(self, file_id):
-        """Sets the file_id of this BulkLoadFileResultModel.
-
-        The fileId of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
-
-        :param file_id: The file_id of this BulkLoadFileResultModel.  # noqa: E501
-        :type: str
-        """
-
-        self._file_id = file_id
-
-    @property
-    def error(self):
-        """Gets the error of this BulkLoadFileResultModel.  # noqa: E501
-
-        The error message if state is FAILED  # noqa: E501
-
-        :return: The error of this BulkLoadFileResultModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._error
-
-    @error.setter
-    def error(self, error):
-        """Sets the error of this BulkLoadFileResultModel.
-
-        The error message if state is FAILED  # noqa: E501
-
-        :param error: The error of this BulkLoadFileResultModel.  # noqa: E501
-        :type: str
-        """
-
-        self._error = error
+        self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -217,18 +131,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BulkLoadFileResultModel):
+        if not isinstance(other, EnumerateBillingProfileModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BulkLoadFileResultModel):
+        if not isinstance(other, EnumerateBillingProfileModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -197,26 +197,26 @@
 
         self._checksum_crc = checksum_crc
 
     @property
     def checksum_md5(self):
         """Gets the checksum_md5 of this BulkLoadHistoryModel.  # noqa: E501
 
-        The checksum md5 of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
+        The checksum mD5 of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
 
         :return: The checksum_md5 of this BulkLoadHistoryModel.  # noqa: E501
         :rtype: str
         """
         return self._checksum_md5
 
     @checksum_md5.setter
     def checksum_md5(self, checksum_md5):
         """Sets the checksum_md5 of this BulkLoadHistoryModel.
 
-        The checksum md5 of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
+        The checksum mD5 of the loaded file; non-null if state is SUCCEEDED  # noqa: E501
 
         :param checksum_md5: The checksum_md5 of this BulkLoadHistoryModel.  # noqa: E501
         :type: str
         """
 
         self._checksum_md5 = checksum_md5
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -32,45 +32,41 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'profile_id': 'str',
         'load_tag': 'str',
         'max_failed_file_loads': 'int',
-        'load_control_file': 'str',
-        'bulk_mode': 'bool'
+        'load_control_file': 'str'
     }
 
     attribute_map = {
         'profile_id': 'profileId',
         'load_tag': 'loadTag',
         'max_failed_file_loads': 'maxFailedFileLoads',
-        'load_control_file': 'loadControlFile',
-        'bulk_mode': 'bulkMode'
+        'load_control_file': 'loadControlFile'
     }
 
-    def __init__(self, profile_id=None, load_tag=None, max_failed_file_loads=0, load_control_file=None, bulk_mode=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, profile_id=None, load_tag=None, max_failed_file_loads=0, load_control_file=None, local_vars_configuration=None):  # noqa: E501
         """BulkLoadRequestModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._profile_id = None
         self._load_tag = None
         self._max_failed_file_loads = None
         self._load_control_file = None
-        self._bulk_mode = None
         self.discriminator = None
 
         self.profile_id = profile_id
         self.load_tag = load_tag
-        self.max_failed_file_loads = max_failed_file_loads
+        if max_failed_file_loads is not None:
+            self.max_failed_file_loads = max_failed_file_loads
         self.load_control_file = load_control_file
-        if bulk_mode is not None:
-            self.bulk_mode = bulk_mode
 
     @property
     def profile_id(self):
         """Gets the profile_id of this BulkLoadRequestModel.  # noqa: E501
 
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
@@ -86,14 +82,17 @@
         Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
         :param profile_id: The profile_id of this BulkLoadRequestModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and profile_id is None:  # noqa: E501
             raise ValueError("Invalid value for `profile_id`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                profile_id is not None and not re.search(r'^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}', profile_id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `profile_id`, must be a follow pattern or equal to `/^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}/`")  # noqa: E501
 
         self._profile_id = profile_id
 
     @property
     def load_tag(self):
         """Gets the load_tag of this BulkLoadRequestModel.  # noqa: E501
 
@@ -134,16 +133,14 @@
         """Sets the max_failed_file_loads of this BulkLoadRequestModel.
 
         max number of failed file loads before stopping; if -1, allow any number of errors  # noqa: E501
 
         :param max_failed_file_loads: The max_failed_file_loads of this BulkLoadRequestModel.  # noqa: E501
         :type: int
         """
-        if self.local_vars_configuration.client_side_validation and max_failed_file_loads is None:  # noqa: E501
-            raise ValueError("Invalid value for `max_failed_file_loads`, must not be `None`")  # noqa: E501
 
         self._max_failed_file_loads = max_failed_file_loads
 
     @property
     def load_control_file(self):
         """Gets the load_control_file of this BulkLoadRequestModel.  # noqa: E501
 
@@ -164,37 +161,14 @@
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and load_control_file is None:  # noqa: E501
             raise ValueError("Invalid value for `load_control_file`, must not be `None`")  # noqa: E501
 
         self._load_control_file = load_control_file
 
-    @property
-    def bulk_mode(self):
-        """Gets the bulk_mode of this BulkLoadRequestModel.  # noqa: E501
-
-        If true, file ingest will be performed in bulk mode.  The tradeoff for the performance improvements are that: - the dataset will be locked exclusively - some safeguards can not be enforced during loads.  Given that, it's recommended that   you use a maxFailedFileLoads value of 0 - the assumption is that file metadata must all fit into memory so configure the   deployment accordingly   # noqa: E501
-
-        :return: The bulk_mode of this BulkLoadRequestModel.  # noqa: E501
-        :rtype: bool
-        """
-        return self._bulk_mode
-
-    @bulk_mode.setter
-    def bulk_mode(self, bulk_mode):
-        """Sets the bulk_mode of this BulkLoadRequestModel.
-
-        If true, file ingest will be performed in bulk mode.  The tradeoff for the performance improvements are that: - the dataset will be locked exclusively - some safeguards can not be enforced during loads.  Given that, it's recommended that   you use a maxFailedFileLoads value of 0 - the assumption is that file metadata must all fit into memory so configure the   deployment accordingly   # noqa: E501
-
-        :param bulk_mode: The bulk_mode of this BulkLoadRequestModel.  # noqa: E501
-        :type: bool
-        """
-
-        self._bulk_mode = bulk_mode
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/column_model.py` & `data-repo-client-1.64.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,117 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class ColumnModel(object):
+class DataDeletionGcsFileModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'datatype': 'TableDataType',
-        'array_of': 'bool',
-        'required': 'bool'
+        'file_type': 'str',
+        'path': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'datatype': 'datatype',
-        'array_of': 'array_of',
-        'required': 'required'
+        'file_type': 'fileType',
+        'path': 'path'
     }
 
-    def __init__(self, name=None, datatype=None, array_of=False, required=None, local_vars_configuration=None):  # noqa: E501
-        """ColumnModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, file_type=None, path=None, local_vars_configuration=None):  # noqa: E501
+        """DataDeletionGcsFileModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._datatype = None
-        self._array_of = None
-        self._required = None
+        self._file_type = None
+        self._path = None
         self.discriminator = None
 
-        self.name = name
-        self.datatype = datatype
-        if array_of is not None:
-            self.array_of = array_of
-        if required is not None:
-            self.required = required
+        self.file_type = file_type
+        self.path = path
 
     @property
-    def name(self):
-        """Gets the name of this ColumnModel.  # noqa: E501
+    def file_type(self):
+        """Gets the file_type of this DataDeletionGcsFileModel.  # noqa: E501
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The name of this ColumnModel.  # noqa: E501
+        :return: The file_type of this DataDeletionGcsFileModel.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._file_type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ColumnModel.
+    @file_type.setter
+    def file_type(self, file_type):
+        """Sets the file_type of this DataDeletionGcsFileModel.
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
 
-        :param name: The name of this ColumnModel.  # noqa: E501
+        :param file_type: The file_type of this DataDeletionGcsFileModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 63):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[a-zA-Z][_a-zA-Z0-9]*$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z][_a-zA-Z0-9]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and file_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `file_type`, must not be `None`")  # noqa: E501
+        allowed_values = ["csv"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and file_type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `file_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(file_type, allowed_values)
+            )
 
-        self._name = name
+        self._file_type = file_type
 
     @property
-    def datatype(self):
-        """Gets the datatype of this ColumnModel.  # noqa: E501
+    def path(self):
+        """Gets the path of this DataDeletionGcsFileModel.  # noqa: E501
 
+        a gs://path/to/a/file that can include a wildcard (*)  # noqa: E501
 
-        :return: The datatype of this ColumnModel.  # noqa: E501
-        :rtype: TableDataType
-        """
-        return self._datatype
-
-    @datatype.setter
-    def datatype(self, datatype):
-        """Sets the datatype of this ColumnModel.
-
-
-        :param datatype: The datatype of this ColumnModel.  # noqa: E501
-        :type: TableDataType
-        """
-        if self.local_vars_configuration.client_side_validation and datatype is None:  # noqa: E501
-            raise ValueError("Invalid value for `datatype`, must not be `None`")  # noqa: E501
-
-        self._datatype = datatype
-
-    @property
-    def array_of(self):
-        """Gets the array_of of this ColumnModel.  # noqa: E501
-
-        if true, make this column an array of type datatype.  # noqa: E501
-
-        :return: The array_of of this ColumnModel.  # noqa: E501
-        :rtype: bool
-        """
-        return self._array_of
-
-    @array_of.setter
-    def array_of(self, array_of):
-        """Sets the array_of of this ColumnModel.
-
-        if true, make this column an array of type datatype.  # noqa: E501
-
-        :param array_of: The array_of of this ColumnModel.  # noqa: E501
-        :type: bool
-        """
-
-        self._array_of = array_of
-
-    @property
-    def required(self):
-        """Gets the required of this ColumnModel.  # noqa: E501
-
-        if true, mark this column as required  # noqa: E501
-
-        :return: The required of this ColumnModel.  # noqa: E501
-        :rtype: bool
+        :return: The path of this DataDeletionGcsFileModel.  # noqa: E501
+        :rtype: str
         """
-        return self._required
+        return self._path
 
-    @required.setter
-    def required(self, required):
-        """Sets the required of this ColumnModel.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this DataDeletionGcsFileModel.
 
-        if true, mark this column as required  # noqa: E501
+        a gs://path/to/a/file that can include a wildcard (*)  # noqa: E501
 
-        :param required: The required of this ColumnModel.  # noqa: E501
-        :type: bool
+        :param path: The path of this DataDeletionGcsFileModel.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
+            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._required = required
+        self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -198,18 +139,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ColumnModel):
+        if not isinstance(other, DataDeletionGcsFileModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ColumnModel):
+        if not isinstance(other, DataDeletionGcsFileModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-1.64.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/config_group_model.py` & `data-repo-client-1.64.0/data_repo_client/models/sql_sort_direction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,62 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class ConfigGroupModel(object):
+class SqlSortDirection(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    ASC = "asc"
+    DESC = "desc"
+
+    allowable_values = [ASC, DESC]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'label': 'str',
-        'group': 'list[ConfigModel]'
     }
 
     attribute_map = {
-        'label': 'label',
-        'group': 'group'
     }
 
-    def __init__(self, label=None, group=None, local_vars_configuration=None):  # noqa: E501
-        """ConfigGroupModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """SqlSortDirection - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._label = None
-        self._group = None
         self.discriminator = None
 
-        if label is not None:
-            self.label = label
-        if group is not None:
-            self.group = group
-
-    @property
-    def label(self):
-        """Gets the label of this ConfigGroupModel.  # noqa: E501
-
-        string to be logged with the settings to identify this set  # noqa: E501
-
-        :return: The label of this ConfigGroupModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._label
-
-    @label.setter
-    def label(self, label):
-        """Sets the label of this ConfigGroupModel.
-
-        string to be logged with the settings to identify this set  # noqa: E501
-
-        :param label: The label of this ConfigGroupModel.  # noqa: E501
-        :type: str
-        """
-
-        self._label = label
-
-    @property
-    def group(self):
-        """Gets the group of this ConfigGroupModel.  # noqa: E501
-
-
-        :return: The group of this ConfigGroupModel.  # noqa: E501
-        :rtype: list[ConfigModel]
-        """
-        return self._group
-
-    @group.setter
-    def group(self, group):
-        """Sets the group of this ConfigGroupModel.
-
-
-        :param group: The group of this ConfigGroupModel.  # noqa: E501
-        :type: list[ConfigModel]
-        """
-
-        self._group = group
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -131,18 +83,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ConfigGroupModel):
+        if not isinstance(other, SqlSortDirection):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ConfigGroupModel):
+        if not isinstance(other, SqlSortDirection):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/config_list_model.py` & `data-repo-client-1.64.0/data_repo_client/models/file_model_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,62 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class ConfigListModel(object):
+class FileModelType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    FILE = "file"
+    DIRECTORY = "directory"
+
+    allowable_values = [FILE, DIRECTORY]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'total': 'int',
-        'items': 'list[ConfigModel]'
     }
 
     attribute_map = {
-        'total': 'total',
-        'items': 'items'
     }
 
-    def __init__(self, total=None, items=None, local_vars_configuration=None):  # noqa: E501
-        """ConfigListModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """FileModelType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._total = None
-        self._items = None
         self.discriminator = None
 
-        if total is not None:
-            self.total = total
-        if items is not None:
-            self.items = items
-
-    @property
-    def total(self):
-        """Gets the total of this ConfigListModel.  # noqa: E501
-
-        Total number of configs  # noqa: E501
-
-        :return: The total of this ConfigListModel.  # noqa: E501
-        :rtype: int
-        """
-        return self._total
-
-    @total.setter
-    def total(self, total):
-        """Sets the total of this ConfigListModel.
-
-        Total number of configs  # noqa: E501
-
-        :param total: The total of this ConfigListModel.  # noqa: E501
-        :type: int
-        """
-
-        self._total = total
-
-    @property
-    def items(self):
-        """Gets the items of this ConfigListModel.  # noqa: E501
-
-
-        :return: The items of this ConfigListModel.  # noqa: E501
-        :rtype: list[ConfigModel]
-        """
-        return self._items
-
-    @items.setter
-    def items(self, items):
-        """Sets the items of this ConfigListModel.
-
-
-        :param items: The items of this ConfigListModel.  # noqa: E501
-        :type: list[ConfigModel]
-        """
-
-        self._items = items
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -131,18 +83,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ConfigListModel):
+        if not isinstance(other, FileModelType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ConfigListModel):
+        if not isinstance(other, FileModelType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/config_model.py` & `data-repo-client-1.64.0/data_repo_client/models/config_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-1.64.0/data_repo_client/models/config_enable_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class ConfigParameterModel(object):
+class ConfigEnableModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'value': 'str'
+        'enabled': 'bool'
     }
 
     attribute_map = {
-        'value': 'value'
+        'enabled': 'enabled'
     }
 
-    def __init__(self, value=None, local_vars_configuration=None):  # noqa: E501
-        """ConfigParameterModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, enabled=True, local_vars_configuration=None):  # noqa: E501
+        """ConfigEnableModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._value = None
+        self._enabled = None
         self.discriminator = None
 
-        if value is not None:
-            self.value = value
+        if enabled is not None:
+            self.enabled = enabled
 
     @property
-    def value(self):
-        """Gets the value of this ConfigParameterModel.  # noqa: E501
+    def enabled(self):
+        """Gets the enabled of this ConfigEnableModel.  # noqa: E501
 
-        Configuration parameters are always passed as strings and converted within the service. That keeps the JSON simple. Sending in specific types doesn't help much, because there still might be a mismatch between the type passed in and the type required.   # noqa: E501
+        whether to enable (default) or disable the fault  # noqa: E501
 
-        :return: The value of this ConfigParameterModel.  # noqa: E501
-        :rtype: str
+        :return: The enabled of this ConfigEnableModel.  # noqa: E501
+        :rtype: bool
         """
-        return self._value
+        return self._enabled
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this ConfigParameterModel.
+    @enabled.setter
+    def enabled(self, enabled):
+        """Sets the enabled of this ConfigEnableModel.
 
-        Configuration parameters are always passed as strings and converted within the service. That keeps the JSON simple. Sending in specific types doesn't help much, because there still might be a mismatch between the type passed in and the type required.   # noqa: E501
+        whether to enable (default) or disable the fault  # noqa: E501
 
-        :param value: The value of this ConfigParameterModel.  # noqa: E501
-        :type: str
+        :param enabled: The enabled of this ConfigEnableModel.  # noqa: E501
+        :type: bool
         """
 
-        self._value = value
+        self._enabled = enabled
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ConfigParameterModel):
+        if not isinstance(other, ConfigEnableModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ConfigParameterModel):
+        if not isinstance(other, ConfigEnableModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-1.64.0/data_repo_client/models/dataset_specification_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,134 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class DataDeletionRequest(object):
+class DatasetSpecificationModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'delete_type': 'str',
-        'transaction_id': 'str',
-        'spec_type': 'str',
-        'tables': 'list[DataDeletionTableModel]'
+        'tables': 'list[TableModel]',
+        'relationships': 'list[RelationshipModel]',
+        'assets': 'list[AssetModel]'
     }
 
     attribute_map = {
-        'delete_type': 'deleteType',
-        'transaction_id': 'transactionId',
-        'spec_type': 'specType',
-        'tables': 'tables'
+        'tables': 'tables',
+        'relationships': 'relationships',
+        'assets': 'assets'
     }
 
-    def __init__(self, delete_type=None, transaction_id=None, spec_type=None, tables=None, local_vars_configuration=None):  # noqa: E501
-        """DataDeletionRequest - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, tables=None, relationships=None, assets=None, local_vars_configuration=None):  # noqa: E501
+        """DatasetSpecificationModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._delete_type = None
-        self._transaction_id = None
-        self._spec_type = None
         self._tables = None
+        self._relationships = None
+        self._assets = None
         self.discriminator = None
 
-        self.delete_type = delete_type
-        if transaction_id is not None:
-            self.transaction_id = transaction_id
-        self.spec_type = spec_type
-        if tables is not None:
-            self.tables = tables
+        self.tables = tables
+        if relationships is not None:
+            self.relationships = relationships
+        if assets is not None:
+            self.assets = assets
 
     @property
-    def delete_type(self):
-        """Gets the delete_type of this DataDeletionRequest.  # noqa: E501
-
-
-        :return: The delete_type of this DataDeletionRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._delete_type
-
-    @delete_type.setter
-    def delete_type(self, delete_type):
-        """Sets the delete_type of this DataDeletionRequest.
-
-
-        :param delete_type: The delete_type of this DataDeletionRequest.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and delete_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `delete_type`, must not be `None`")  # noqa: E501
-        allowed_values = ["soft"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and delete_type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `delete_type` ({0}), must be one of {1}"  # noqa: E501
-                .format(delete_type, allowed_values)
-            )
-
-        self._delete_type = delete_type
-
-    @property
-    def transaction_id(self):
-        """Gets the transaction_id of this DataDeletionRequest.  # noqa: E501
+    def tables(self):
+        """Gets the tables of this DatasetSpecificationModel.  # noqa: E501
 
-        If specified, the deleted data will remain visible to users and snapshot creation until the transaction in question is committed. If the transaction is rolled back, then the changes from this delete and any other operations using this transaction will be undone.   # noqa: E501
 
-        :return: The transaction_id of this DataDeletionRequest.  # noqa: E501
-        :rtype: str
+        :return: The tables of this DatasetSpecificationModel.  # noqa: E501
+        :rtype: list[TableModel]
         """
-        return self._transaction_id
+        return self._tables
 
-    @transaction_id.setter
-    def transaction_id(self, transaction_id):
-        """Sets the transaction_id of this DataDeletionRequest.
+    @tables.setter
+    def tables(self, tables):
+        """Sets the tables of this DatasetSpecificationModel.
 
-        If specified, the deleted data will remain visible to users and snapshot creation until the transaction in question is committed. If the transaction is rolled back, then the changes from this delete and any other operations using this transaction will be undone.   # noqa: E501
 
-        :param transaction_id: The transaction_id of this DataDeletionRequest.  # noqa: E501
-        :type: str
+        :param tables: The tables of this DatasetSpecificationModel.  # noqa: E501
+        :type: list[TableModel]
         """
+        if self.local_vars_configuration.client_side_validation and tables is None:  # noqa: E501
+            raise ValueError("Invalid value for `tables`, must not be `None`")  # noqa: E501
 
-        self._transaction_id = transaction_id
+        self._tables = tables
 
     @property
-    def spec_type(self):
-        """Gets the spec_type of this DataDeletionRequest.  # noqa: E501
+    def relationships(self):
+        """Gets the relationships of this DatasetSpecificationModel.  # noqa: E501
 
 
-        :return: The spec_type of this DataDeletionRequest.  # noqa: E501
-        :rtype: str
+        :return: The relationships of this DatasetSpecificationModel.  # noqa: E501
+        :rtype: list[RelationshipModel]
         """
-        return self._spec_type
+        return self._relationships
 
-    @spec_type.setter
-    def spec_type(self, spec_type):
-        """Sets the spec_type of this DataDeletionRequest.
+    @relationships.setter
+    def relationships(self, relationships):
+        """Sets the relationships of this DatasetSpecificationModel.
 
 
-        :param spec_type: The spec_type of this DataDeletionRequest.  # noqa: E501
-        :type: str
+        :param relationships: The relationships of this DatasetSpecificationModel.  # noqa: E501
+        :type: list[RelationshipModel]
         """
-        if self.local_vars_configuration.client_side_validation and spec_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `spec_type`, must not be `None`")  # noqa: E501
-        allowed_values = ["gcsFile", "jsonArray"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and spec_type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `spec_type` ({0}), must be one of {1}"  # noqa: E501
-                .format(spec_type, allowed_values)
-            )
 
-        self._spec_type = spec_type
+        self._relationships = relationships
 
     @property
-    def tables(self):
-        """Gets the tables of this DataDeletionRequest.  # noqa: E501
+    def assets(self):
+        """Gets the assets of this DatasetSpecificationModel.  # noqa: E501
 
 
-        :return: The tables of this DataDeletionRequest.  # noqa: E501
-        :rtype: list[DataDeletionTableModel]
+        :return: The assets of this DatasetSpecificationModel.  # noqa: E501
+        :rtype: list[AssetModel]
         """
-        return self._tables
+        return self._assets
 
-    @tables.setter
-    def tables(self, tables):
-        """Sets the tables of this DataDeletionRequest.
+    @assets.setter
+    def assets(self, assets):
+        """Sets the assets of this DatasetSpecificationModel.
 
 
-        :param tables: The tables of this DataDeletionRequest.  # noqa: E501
-        :type: list[DataDeletionTableModel]
+        :param assets: The assets of this DatasetSpecificationModel.  # noqa: E501
+        :type: list[AssetModel]
         """
 
-        self._tables = tables
+        self._assets = assets
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -197,18 +156,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DataDeletionRequest):
+        if not isinstance(other, DatasetSpecificationModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DataDeletionRequest):
+        if not isinstance(other, DatasetSpecificationModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-1.64.0/test/test_snapshot_request_asset_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,59 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import pprint
-import re  # noqa: F401
+from __future__ import absolute_import
 
-import six
+import unittest
+import datetime
 
-from data_repo_client.configuration import Configuration
+import data_repo_client
+from data_repo_client.models.snapshot_request_asset_model import SnapshotRequestAssetModel  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestSnapshotRequestAssetModel(unittest.TestCase):
+    """SnapshotRequestAssetModel unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SnapshotRequestAssetModel
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.snapshot_request_asset_model.SnapshotRequestAssetModel()  # noqa: E501
+        if include_optional :
+            return SnapshotRequestAssetModel(
+                asset_name = 'a', 
+                root_values = [
+                    '0'
+                    ]
+            )
+        else :
+            return SnapshotRequestAssetModel(
+                asset_name = 'a',
+                root_values = [
+                    '0'
+                    ],
+        )
+
+    def testSnapshotRequestAssetModel(self):
+        """Test SnapshotRequestAssetModel"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-class DatasetRequestAccessIncludeModel(object):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    """
-    allowed enum values
-    """
-    NONE = "NONE"
-    SCHEMA = "SCHEMA"
-    ACCESS_INFORMATION = "ACCESS_INFORMATION"
-    PROFILE = "PROFILE"
-    PROPERTIES = "PROPERTIES"
-    DATA_PROJECT = "DATA_PROJECT"
-    STORAGE = "STORAGE"
-
-    allowable_values = [NONE, SCHEMA, ACCESS_INFORMATION, PROFILE, PROPERTIES, DATA_PROJECT, STORAGE]  # noqa: E501
-
-    """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-    }
-
-    attribute_map = {
-    }
-
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """DatasetRequestAccessIncludeModel - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-        self.discriminator = None
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DatasetRequestAccessIncludeModel):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DatasetRequestAccessIncludeModel):
-            return True
-
-        return self.to_dict() != other.to_dict()
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-1.64.0/data_repo_client/models/ingest_request_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,448 +1,375 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class DatasetSummaryModel(object):
+class IngestRequestModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
-        'name': 'str',
-        'description': 'str',
-        'default_profile_id': 'str',
-        'created_date': 'str',
-        'storage': 'list[StorageResourceModel]',
-        'secure_monitoring_enabled': 'bool',
-        'cloud_platform': 'CloudPlatform',
-        'data_project': 'str',
-        'storage_account': 'str',
-        'phs_id': 'str',
-        'self_hosted': 'bool',
-        'predictable_file_ids': 'bool',
-        'tags': 'list[str]'
+        'table': 'str',
+        'path': 'str',
+        'format': 'str',
+        'load_tag': 'str',
+        'max_bad_records': 'int',
+        'ignore_unknown_values': 'bool',
+        'csv_field_delimiter': 'str',
+        'csv_quote': 'str',
+        'csv_skip_leading_rows': 'int',
+        'csv_allow_quoted_newlines': 'bool',
+        'csv_null_marker': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
-        'name': 'name',
-        'description': 'description',
-        'default_profile_id': 'defaultProfileId',
-        'created_date': 'createdDate',
-        'storage': 'storage',
-        'secure_monitoring_enabled': 'secureMonitoringEnabled',
-        'cloud_platform': 'cloudPlatform',
-        'data_project': 'dataProject',
-        'storage_account': 'storageAccount',
-        'phs_id': 'phsId',
-        'self_hosted': 'selfHosted',
-        'predictable_file_ids': 'predictableFileIds',
-        'tags': 'tags'
+        'table': 'table',
+        'path': 'path',
+        'format': 'format',
+        'load_tag': 'load_tag',
+        'max_bad_records': 'max_bad_records',
+        'ignore_unknown_values': 'ignore_unknown_values',
+        'csv_field_delimiter': 'csv_field_delimiter',
+        'csv_quote': 'csv_quote',
+        'csv_skip_leading_rows': 'csv_skip_leading_rows',
+        'csv_allow_quoted_newlines': 'csv_allow_quoted_newlines',
+        'csv_null_marker': 'csv_null_marker'
     }
 
-    def __init__(self, id=None, name=None, description=None, default_profile_id=None, created_date=None, storage=None, secure_monitoring_enabled=False, cloud_platform=None, data_project=None, storage_account=None, phs_id=None, self_hosted=False, predictable_file_ids=False, tags=None, local_vars_configuration=None):  # noqa: E501
-        """DatasetSummaryModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, table=None, path=None, format=None, load_tag=None, max_bad_records=None, ignore_unknown_values=True, csv_field_delimiter=',', csv_quote='"', csv_skip_leading_rows=None, csv_allow_quoted_newlines=True, csv_null_marker='', local_vars_configuration=None):  # noqa: E501
+        """IngestRequestModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._name = None
-        self._description = None
-        self._default_profile_id = None
-        self._created_date = None
-        self._storage = None
-        self._secure_monitoring_enabled = None
-        self._cloud_platform = None
-        self._data_project = None
-        self._storage_account = None
-        self._phs_id = None
-        self._self_hosted = None
-        self._predictable_file_ids = None
-        self._tags = None
+        self._table = None
+        self._path = None
+        self._format = None
+        self._load_tag = None
+        self._max_bad_records = None
+        self._ignore_unknown_values = None
+        self._csv_field_delimiter = None
+        self._csv_quote = None
+        self._csv_skip_leading_rows = None
+        self._csv_allow_quoted_newlines = None
+        self._csv_null_marker = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
-        if description is not None:
-            self.description = description
-        if default_profile_id is not None:
-            self.default_profile_id = default_profile_id
-        if created_date is not None:
-            self.created_date = created_date
-        if storage is not None:
-            self.storage = storage
-        if secure_monitoring_enabled is not None:
-            self.secure_monitoring_enabled = secure_monitoring_enabled
-        if cloud_platform is not None:
-            self.cloud_platform = cloud_platform
-        if data_project is not None:
-            self.data_project = data_project
-        if storage_account is not None:
-            self.storage_account = storage_account
-        if phs_id is not None:
-            self.phs_id = phs_id
-        if self_hosted is not None:
-            self.self_hosted = self_hosted
-        if predictable_file_ids is not None:
-            self.predictable_file_ids = predictable_file_ids
-        if tags is not None:
-            self.tags = tags
+        self.table = table
+        self.path = path
+        self.format = format
+        if load_tag is not None:
+            self.load_tag = load_tag
+        if max_bad_records is not None:
+            self.max_bad_records = max_bad_records
+        if ignore_unknown_values is not None:
+            self.ignore_unknown_values = ignore_unknown_values
+        if csv_field_delimiter is not None:
+            self.csv_field_delimiter = csv_field_delimiter
+        if csv_quote is not None:
+            self.csv_quote = csv_quote
+        if csv_skip_leading_rows is not None:
+            self.csv_skip_leading_rows = csv_skip_leading_rows
+        if csv_allow_quoted_newlines is not None:
+            self.csv_allow_quoted_newlines = csv_allow_quoted_newlines
+        if csv_null_marker is not None:
+            self.csv_null_marker = csv_null_marker
 
     @property
-    def id(self):
-        """Gets the id of this DatasetSummaryModel.  # noqa: E501
+    def table(self):
+        """Gets the table of this IngestRequestModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The id of this DatasetSummaryModel.  # noqa: E501
+        :return: The table of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._table
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this DatasetSummaryModel.
+    @table.setter
+    def table(self, table):
+        """Sets the table of this IngestRequestModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param id: The id of this DatasetSummaryModel.  # noqa: E501
-        :type: str
-        """
-
-        self._id = id
-
-    @property
-    def name(self):
-        """Gets the name of this DatasetSummaryModel.  # noqa: E501
-
-        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
-
-        :return: The name of this DatasetSummaryModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this DatasetSummaryModel.
-
-        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
-
-        :param name: The name of this DatasetSummaryModel.  # noqa: E501
+        :param table: The table of this IngestRequestModel.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and table is None:  # noqa: E501
+            raise ValueError("Invalid value for `table`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 511):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `511`")  # noqa: E501
+                table is not None and len(table) > 63):
+            raise ValueError("Invalid value for `table`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+                table is not None and len(table) < 1):
+            raise ValueError("Invalid value for `table`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                table is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', table)):  # noqa: E501
+            raise ValueError(r"Invalid value for `table`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._name = name
+        self._table = table
 
     @property
-    def description(self):
-        """Gets the description of this DatasetSummaryModel.  # noqa: E501
+    def path(self):
+        """Gets the path of this IngestRequestModel.  # noqa: E501
 
-        Description of the dataset  # noqa: E501
+        gs path to a file in a bucket accessible to data repo  # noqa: E501
 
-        :return: The description of this DatasetSummaryModel.  # noqa: E501
+        :return: The path of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._path
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this DatasetSummaryModel.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this IngestRequestModel.
 
-        Description of the dataset  # noqa: E501
+        gs path to a file in a bucket accessible to data repo  # noqa: E501
 
-        :param description: The description of this DatasetSummaryModel.  # noqa: E501
+        :param path: The path of this IngestRequestModel.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
+            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._description = description
+        self._path = path
 
     @property
-    def default_profile_id(self):
-        """Gets the default_profile_id of this DatasetSummaryModel.  # noqa: E501
+    def format(self):
+        """Gets the format of this IngestRequestModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :return: The default_profile_id of this DatasetSummaryModel.  # noqa: E501
+        :return: The format of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._default_profile_id
+        return self._format
 
-    @default_profile_id.setter
-    def default_profile_id(self, default_profile_id):
-        """Sets the default_profile_id of this DatasetSummaryModel.
+    @format.setter
+    def format(self, format):
+        """Sets the format of this IngestRequestModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :param default_profile_id: The default_profile_id of this DatasetSummaryModel.  # noqa: E501
+        :param format: The format of this IngestRequestModel.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and format is None:  # noqa: E501
+            raise ValueError("Invalid value for `format`, must not be `None`")  # noqa: E501
+        allowed_values = ["csv", "json"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and format not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `format` ({0}), must be one of {1}"  # noqa: E501
+                .format(format, allowed_values)
+            )
 
-        self._default_profile_id = default_profile_id
+        self._format = format
 
     @property
-    def created_date(self):
-        """Gets the created_date of this DatasetSummaryModel.  # noqa: E501
+    def load_tag(self):
+        """Gets the load_tag of this IngestRequestModel.  # noqa: E501
 
-        Date the dataset was created  # noqa: E501
+        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
 
-        :return: The created_date of this DatasetSummaryModel.  # noqa: E501
+        :return: The load_tag of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._created_date
+        return self._load_tag
 
-    @created_date.setter
-    def created_date(self, created_date):
-        """Sets the created_date of this DatasetSummaryModel.
+    @load_tag.setter
+    def load_tag(self, load_tag):
+        """Sets the load_tag of this IngestRequestModel.
 
-        Date the dataset was created  # noqa: E501
+        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
 
-        :param created_date: The created_date of this DatasetSummaryModel.  # noqa: E501
+        :param load_tag: The load_tag of this IngestRequestModel.  # noqa: E501
         :type: str
         """
 
-        self._created_date = created_date
+        self._load_tag = load_tag
 
     @property
-    def storage(self):
-        """Gets the storage of this DatasetSummaryModel.  # noqa: E501
+    def max_bad_records(self):
+        """Gets the max_bad_records of this IngestRequestModel.  # noqa: E501
 
+        max number of bad records to skip; applies to JSON and CSV  # noqa: E501
 
-        :return: The storage of this DatasetSummaryModel.  # noqa: E501
-        :rtype: list[StorageResourceModel]
+        :return: The max_bad_records of this IngestRequestModel.  # noqa: E501
+        :rtype: int
         """
-        return self._storage
+        return self._max_bad_records
 
-    @storage.setter
-    def storage(self, storage):
-        """Sets the storage of this DatasetSummaryModel.
+    @max_bad_records.setter
+    def max_bad_records(self, max_bad_records):
+        """Sets the max_bad_records of this IngestRequestModel.
 
+        max number of bad records to skip; applies to JSON and CSV  # noqa: E501
 
-        :param storage: The storage of this DatasetSummaryModel.  # noqa: E501
-        :type: list[StorageResourceModel]
+        :param max_bad_records: The max_bad_records of this IngestRequestModel.  # noqa: E501
+        :type: int
         """
 
-        self._storage = storage
+        self._max_bad_records = max_bad_records
 
     @property
-    def secure_monitoring_enabled(self):
-        """Gets the secure_monitoring_enabled of this DatasetSummaryModel.  # noqa: E501
+    def ignore_unknown_values(self):
+        """Gets the ignore_unknown_values of this IngestRequestModel.  # noqa: E501
 
+        skip extra data; applies to JSON and CSV  # noqa: E501
 
-        :return: The secure_monitoring_enabled of this DatasetSummaryModel.  # noqa: E501
+        :return: The ignore_unknown_values of this IngestRequestModel.  # noqa: E501
         :rtype: bool
         """
-        return self._secure_monitoring_enabled
+        return self._ignore_unknown_values
 
-    @secure_monitoring_enabled.setter
-    def secure_monitoring_enabled(self, secure_monitoring_enabled):
-        """Sets the secure_monitoring_enabled of this DatasetSummaryModel.
+    @ignore_unknown_values.setter
+    def ignore_unknown_values(self, ignore_unknown_values):
+        """Sets the ignore_unknown_values of this IngestRequestModel.
 
+        skip extra data; applies to JSON and CSV  # noqa: E501
 
-        :param secure_monitoring_enabled: The secure_monitoring_enabled of this DatasetSummaryModel.  # noqa: E501
+        :param ignore_unknown_values: The ignore_unknown_values of this IngestRequestModel.  # noqa: E501
         :type: bool
         """
 
-        self._secure_monitoring_enabled = secure_monitoring_enabled
-
-    @property
-    def cloud_platform(self):
-        """Gets the cloud_platform of this DatasetSummaryModel.  # noqa: E501
-
-
-        :return: The cloud_platform of this DatasetSummaryModel.  # noqa: E501
-        :rtype: CloudPlatform
-        """
-        return self._cloud_platform
-
-    @cloud_platform.setter
-    def cloud_platform(self, cloud_platform):
-        """Sets the cloud_platform of this DatasetSummaryModel.
-
-
-        :param cloud_platform: The cloud_platform of this DatasetSummaryModel.  # noqa: E501
-        :type: CloudPlatform
-        """
-
-        self._cloud_platform = cloud_platform
+        self._ignore_unknown_values = ignore_unknown_values
 
     @property
-    def data_project(self):
-        """Gets the data_project of this DatasetSummaryModel.  # noqa: E501
+    def csv_field_delimiter(self):
+        """Gets the csv_field_delimiter of this IngestRequestModel.  # noqa: E501
 
-        The google project of this dataset  # noqa: E501
+        field separator  # noqa: E501
 
-        :return: The data_project of this DatasetSummaryModel.  # noqa: E501
+        :return: The csv_field_delimiter of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._data_project
+        return self._csv_field_delimiter
 
-    @data_project.setter
-    def data_project(self, data_project):
-        """Sets the data_project of this DatasetSummaryModel.
+    @csv_field_delimiter.setter
+    def csv_field_delimiter(self, csv_field_delimiter):
+        """Sets the csv_field_delimiter of this IngestRequestModel.
 
-        The google project of this dataset  # noqa: E501
+        field separator  # noqa: E501
 
-        :param data_project: The data_project of this DatasetSummaryModel.  # noqa: E501
+        :param csv_field_delimiter: The csv_field_delimiter of this IngestRequestModel.  # noqa: E501
         :type: str
         """
 
-        self._data_project = data_project
+        self._csv_field_delimiter = csv_field_delimiter
 
     @property
-    def storage_account(self):
-        """Gets the storage_account of this DatasetSummaryModel.  # noqa: E501
+    def csv_quote(self):
+        """Gets the csv_quote of this IngestRequestModel.  # noqa: E501
 
-        The azure storage account of this dataset  # noqa: E501
+        quoting character  # noqa: E501
 
-        :return: The storage_account of this DatasetSummaryModel.  # noqa: E501
+        :return: The csv_quote of this IngestRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._storage_account
+        return self._csv_quote
 
-    @storage_account.setter
-    def storage_account(self, storage_account):
-        """Sets the storage_account of this DatasetSummaryModel.
+    @csv_quote.setter
+    def csv_quote(self, csv_quote):
+        """Sets the csv_quote of this IngestRequestModel.
 
-        The azure storage account of this dataset  # noqa: E501
+        quoting character  # noqa: E501
 
-        :param storage_account: The storage_account of this DatasetSummaryModel.  # noqa: E501
+        :param csv_quote: The csv_quote of this IngestRequestModel.  # noqa: E501
         :type: str
         """
 
-        self._storage_account = storage_account
+        self._csv_quote = csv_quote
 
     @property
-    def phs_id(self):
-        """Gets the phs_id of this DatasetSummaryModel.  # noqa: E501
+    def csv_skip_leading_rows(self):
+        """Gets the csv_skip_leading_rows of this IngestRequestModel.  # noqa: E501
 
-        PHS ID (DbGap Phenotype Study Identifer) associated with dataset  # noqa: E501
+        number of header rows to skip  # noqa: E501
 
-        :return: The phs_id of this DatasetSummaryModel.  # noqa: E501
-        :rtype: str
+        :return: The csv_skip_leading_rows of this IngestRequestModel.  # noqa: E501
+        :rtype: int
         """
-        return self._phs_id
+        return self._csv_skip_leading_rows
 
-    @phs_id.setter
-    def phs_id(self, phs_id):
-        """Sets the phs_id of this DatasetSummaryModel.
+    @csv_skip_leading_rows.setter
+    def csv_skip_leading_rows(self, csv_skip_leading_rows):
+        """Sets the csv_skip_leading_rows of this IngestRequestModel.
 
-        PHS ID (DbGap Phenotype Study Identifer) associated with dataset  # noqa: E501
+        number of header rows to skip  # noqa: E501
 
-        :param phs_id: The phs_id of this DatasetSummaryModel.  # noqa: E501
-        :type: str
+        :param csv_skip_leading_rows: The csv_skip_leading_rows of this IngestRequestModel.  # noqa: E501
+        :type: int
         """
 
-        self._phs_id = phs_id
+        self._csv_skip_leading_rows = csv_skip_leading_rows
 
     @property
-    def self_hosted(self):
-        """Gets the self_hosted of this DatasetSummaryModel.  # noqa: E501
+    def csv_allow_quoted_newlines(self):
+        """Gets the csv_allow_quoted_newlines of this IngestRequestModel.  # noqa: E501
 
-        denotes whether data files in the dataset are self-hosted or not  # noqa: E501
 
-        :return: The self_hosted of this DatasetSummaryModel.  # noqa: E501
+        :return: The csv_allow_quoted_newlines of this IngestRequestModel.  # noqa: E501
         :rtype: bool
         """
-        return self._self_hosted
+        return self._csv_allow_quoted_newlines
 
-    @self_hosted.setter
-    def self_hosted(self, self_hosted):
-        """Sets the self_hosted of this DatasetSummaryModel.
+    @csv_allow_quoted_newlines.setter
+    def csv_allow_quoted_newlines(self, csv_allow_quoted_newlines):
+        """Sets the csv_allow_quoted_newlines of this IngestRequestModel.
 
-        denotes whether data files in the dataset are self-hosted or not  # noqa: E501
 
-        :param self_hosted: The self_hosted of this DatasetSummaryModel.  # noqa: E501
+        :param csv_allow_quoted_newlines: The csv_allow_quoted_newlines of this IngestRequestModel.  # noqa: E501
         :type: bool
         """
 
-        self._self_hosted = self_hosted
+        self._csv_allow_quoted_newlines = csv_allow_quoted_newlines
 
     @property
-    def predictable_file_ids(self):
-        """Gets the predictable_file_ids of this DatasetSummaryModel.  # noqa: E501
-
-        If false, random ids will be created. If true, full target path (e.g. path + name), size and md5 hash will be used Note: this only applies to files.  Directories still have random ids regardless of this value   # noqa: E501
-
-        :return: The predictable_file_ids of this DatasetSummaryModel.  # noqa: E501
-        :rtype: bool
-        """
-        return self._predictable_file_ids
-
-    @predictable_file_ids.setter
-    def predictable_file_ids(self, predictable_file_ids):
-        """Sets the predictable_file_ids of this DatasetSummaryModel.
+    def csv_null_marker(self):
+        """Gets the csv_null_marker of this IngestRequestModel.  # noqa: E501
 
-        If false, random ids will be created. If true, full target path (e.g. path + name), size and md5 hash will be used Note: this only applies to files.  Directories still have random ids regardless of this value   # noqa: E501
 
-        :param predictable_file_ids: The predictable_file_ids of this DatasetSummaryModel.  # noqa: E501
-        :type: bool
-        """
-
-        self._predictable_file_ids = predictable_file_ids
-
-    @property
-    def tags(self):
-        """Gets the tags of this DatasetSummaryModel.  # noqa: E501
-
-
-        :return: The tags of this DatasetSummaryModel.  # noqa: E501
-        :rtype: list[str]
+        :return: The csv_null_marker of this IngestRequestModel.  # noqa: E501
+        :rtype: str
         """
-        return self._tags
+        return self._csv_null_marker
 
-    @tags.setter
-    def tags(self, tags):
-        """Sets the tags of this DatasetSummaryModel.
+    @csv_null_marker.setter
+    def csv_null_marker(self, csv_null_marker):
+        """Sets the csv_null_marker of this IngestRequestModel.
 
 
-        :param tags: The tags of this DatasetSummaryModel.  # noqa: E501
-        :type: list[str]
+        :param csv_null_marker: The csv_null_marker of this IngestRequestModel.  # noqa: E501
+        :type: str
         """
 
-        self._tags = tags
+        self._csv_null_marker = csv_null_marker
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -470,18 +397,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DatasetSummaryModel):
+        if not isinstance(other, IngestRequestModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DatasetSummaryModel):
+        if not isinstance(other, IngestRequestModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-1.64.0/data_repo_client/models/drs_access_method.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -32,48 +32,43 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'type': 'str',
         'access_url': 'DRSAccessURL',
         'access_id': 'str',
-        'region': 'str',
-        'authorizations': 'DRSAuthorizations'
+        'region': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'access_url': 'access_url',
         'access_id': 'access_id',
-        'region': 'region',
-        'authorizations': 'authorizations'
+        'region': 'region'
     }
 
-    def __init__(self, type=None, access_url=None, access_id=None, region=None, authorizations=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, access_url=None, access_id=None, region=None, local_vars_configuration=None):  # noqa: E501
         """DRSAccessMethod - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._access_url = None
         self._access_id = None
         self._region = None
-        self._authorizations = None
         self.discriminator = None
 
         self.type = type
         if access_url is not None:
             self.access_url = access_url
         if access_id is not None:
             self.access_id = access_id
         if region is not None:
             self.region = region
-        if authorizations is not None:
-            self.authorizations = authorizations
 
     @property
     def type(self):
         """Gets the type of this DRSAccessMethod.  # noqa: E501
 
         Type of the access method.  # noqa: E501
 
@@ -165,35 +160,14 @@
 
         :param region: The region of this DRSAccessMethod.  # noqa: E501
         :type: str
         """
 
         self._region = region
 
-    @property
-    def authorizations(self):
-        """Gets the authorizations of this DRSAccessMethod.  # noqa: E501
-
-
-        :return: The authorizations of this DRSAccessMethod.  # noqa: E501
-        :rtype: DRSAuthorizations
-        """
-        return self._authorizations
-
-    @authorizations.setter
-    def authorizations(self, authorizations):
-        """Sets the authorizations of this DRSAccessMethod.
-
-
-        :param authorizations: The authorizations of this DRSAccessMethod.  # noqa: E501
-        :type: DRSAuthorizations
-        """
-
-        self._authorizations = authorizations
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-1.64.0/data_repo_client/models/config_fault_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,143 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class DRSAuthorizations(object):
+class ConfigFaultModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'supported_types': 'list[str]',
-        'passport_auth_issuers': 'list[str]',
-        'bearer_auth_issuers': 'list[str]'
+        'enabled': 'bool',
+        'fault_type': 'str',
+        'counted': 'ConfigFaultCountedModel'
     }
 
     attribute_map = {
-        'supported_types': 'supported_types',
-        'passport_auth_issuers': 'passport_auth_issuers',
-        'bearer_auth_issuers': 'bearer_auth_issuers'
+        'enabled': 'enabled',
+        'fault_type': 'faultType',
+        'counted': 'counted'
     }
 
-    def __init__(self, supported_types=None, passport_auth_issuers=None, bearer_auth_issuers=None, local_vars_configuration=None):  # noqa: E501
-        """DRSAuthorizations - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, enabled=None, fault_type=None, counted=None, local_vars_configuration=None):  # noqa: E501
+        """ConfigFaultModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._supported_types = None
-        self._passport_auth_issuers = None
-        self._bearer_auth_issuers = None
+        self._enabled = None
+        self._fault_type = None
+        self._counted = None
         self.discriminator = None
 
-        if supported_types is not None:
-            self.supported_types = supported_types
-        if passport_auth_issuers is not None:
-            self.passport_auth_issuers = passport_auth_issuers
-        if bearer_auth_issuers is not None:
-            self.bearer_auth_issuers = bearer_auth_issuers
+        if enabled is not None:
+            self.enabled = enabled
+        if fault_type is not None:
+            self.fault_type = fault_type
+        if counted is not None:
+            self.counted = counted
 
     @property
-    def supported_types(self):
-        """Gets the supported_types of this DRSAuthorizations.  # noqa: E501
+    def enabled(self):
+        """Gets the enabled of this ConfigFaultModel.  # noqa: E501
 
-        An Optional list of supported authorization types. More than one can be supported and tried in sequence. Defaults to `None` if empty or missing.  # noqa: E501
+        If the fault is enabled, then is in effect. Fault points cause insert faults. Typical usage is that faults are disabled on system start and explicitly enabled by test code or via the setFault endpoint.   # noqa: E501
 
-        :return: The supported_types of this DRSAuthorizations.  # noqa: E501
-        :rtype: list[str]
+        :return: The enabled of this ConfigFaultModel.  # noqa: E501
+        :rtype: bool
         """
-        return self._supported_types
+        return self._enabled
 
-    @supported_types.setter
-    def supported_types(self, supported_types):
-        """Sets the supported_types of this DRSAuthorizations.
+    @enabled.setter
+    def enabled(self, enabled):
+        """Sets the enabled of this ConfigFaultModel.
 
-        An Optional list of supported authorization types. More than one can be supported and tried in sequence. Defaults to `None` if empty or missing.  # noqa: E501
+        If the fault is enabled, then is in effect. Fault points cause insert faults. Typical usage is that faults are disabled on system start and explicitly enabled by test code or via the setFault endpoint.   # noqa: E501
 
-        :param supported_types: The supported_types of this DRSAuthorizations.  # noqa: E501
-        :type: list[str]
+        :param enabled: The enabled of this ConfigFaultModel.  # noqa: E501
+        :type: bool
         """
-        allowed_values = ["None", "BasicAuth", "BearerAuth", "PassportAuth"]  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                not set(supported_types).issubset(set(allowed_values))):  # noqa: E501
-            raise ValueError(
-                "Invalid values for `supported_types` [{0}], must be a subset of [{1}]"  # noqa: E501
-                .format(", ".join(map(str, set(supported_types) - set(allowed_values))),  # noqa: E501
-                        ", ".join(map(str, allowed_values)))
-            )
 
-        self._supported_types = supported_types
+        self._enabled = enabled
 
     @property
-    def passport_auth_issuers(self):
-        """Gets the passport_auth_issuers of this DRSAuthorizations.  # noqa: E501
+    def fault_type(self):
+        """Gets the fault_type of this ConfigFaultModel.  # noqa: E501
 
-        If authorizations contain `PassportAuth`, this is a required list of visa issuers (as found in a visa's `iss` claim) that may authorize access to this object. The caller must only provide passports that contain visas from this list. It is strongly recommended that the caller validate that it is appropriate to send the requested passport/visa to the DRS server to mitigate attacks by malicious DRS servers requesting credentials they should not have.  # noqa: E501
+        A simple fault has no parameters. It is just enabled or disabled. This type of fault is typically used when the desired behavior of the fault is too complex for expression in the fault types and custom code is needed to get the right failure behavior. A counted fault is used to insert some number of faults in a pattern. See the ConfigFaultCountedModel for details.   # noqa: E501
 
-        :return: The passport_auth_issuers of this DRSAuthorizations.  # noqa: E501
-        :rtype: list[str]
+        :return: The fault_type of this ConfigFaultModel.  # noqa: E501
+        :rtype: str
         """
-        return self._passport_auth_issuers
+        return self._fault_type
 
-    @passport_auth_issuers.setter
-    def passport_auth_issuers(self, passport_auth_issuers):
-        """Sets the passport_auth_issuers of this DRSAuthorizations.
+    @fault_type.setter
+    def fault_type(self, fault_type):
+        """Sets the fault_type of this ConfigFaultModel.
 
-        If authorizations contain `PassportAuth`, this is a required list of visa issuers (as found in a visa's `iss` claim) that may authorize access to this object. The caller must only provide passports that contain visas from this list. It is strongly recommended that the caller validate that it is appropriate to send the requested passport/visa to the DRS server to mitigate attacks by malicious DRS servers requesting credentials they should not have.  # noqa: E501
+        A simple fault has no parameters. It is just enabled or disabled. This type of fault is typically used when the desired behavior of the fault is too complex for expression in the fault types and custom code is needed to get the right failure behavior. A counted fault is used to insert some number of faults in a pattern. See the ConfigFaultCountedModel for details.   # noqa: E501
 
-        :param passport_auth_issuers: The passport_auth_issuers of this DRSAuthorizations.  # noqa: E501
-        :type: list[str]
+        :param fault_type: The fault_type of this ConfigFaultModel.  # noqa: E501
+        :type: str
         """
+        allowed_values = ["simple", "counted"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and fault_type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `fault_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(fault_type, allowed_values)
+            )
 
-        self._passport_auth_issuers = passport_auth_issuers
+        self._fault_type = fault_type
 
     @property
-    def bearer_auth_issuers(self):
-        """Gets the bearer_auth_issuers of this DRSAuthorizations.  # noqa: E501
+    def counted(self):
+        """Gets the counted of this ConfigFaultModel.  # noqa: E501
 
-        If authorizations contain `BearerAuth`, this is an optional list of issuers that may authorize access to this object. The caller must provide a token from one of these issuers. If this is empty or missing it is assumed that the caller knows which token to send via other means. It is strongly recommended that the caller validate that it is appropriate to send the requested token to the DRS server to mitigate attacks by malicious DRS servers requesting credentials they should not have.  # noqa: E501
 
-        :return: The bearer_auth_issuers of this DRSAuthorizations.  # noqa: E501
-        :rtype: list[str]
+        :return: The counted of this ConfigFaultModel.  # noqa: E501
+        :rtype: ConfigFaultCountedModel
         """
-        return self._bearer_auth_issuers
+        return self._counted
 
-    @bearer_auth_issuers.setter
-    def bearer_auth_issuers(self, bearer_auth_issuers):
-        """Sets the bearer_auth_issuers of this DRSAuthorizations.
+    @counted.setter
+    def counted(self, counted):
+        """Sets the counted of this ConfigFaultModel.
 
-        If authorizations contain `BearerAuth`, this is an optional list of issuers that may authorize access to this object. The caller must provide a token from one of these issuers. If this is empty or missing it is assumed that the caller knows which token to send via other means. It is strongly recommended that the caller validate that it is appropriate to send the requested token to the DRS server to mitigate attacks by malicious DRS servers requesting credentials they should not have.  # noqa: E501
 
-        :param bearer_auth_issuers: The bearer_auth_issuers of this DRSAuthorizations.  # noqa: E501
-        :type: list[str]
+        :param counted: The counted of this ConfigFaultModel.  # noqa: E501
+        :type: ConfigFaultCountedModel
         """
 
-        self._bearer_auth_issuers = bearer_auth_issuers
+        self._counted = counted
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -169,18 +165,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DRSAuthorizations):
+        if not isinstance(other, ConfigFaultModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DRSAuthorizations):
+        if not isinstance(other, ConfigFaultModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-1.64.0/data_repo_client/models/drs_checksum.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-1.64.0/data_repo_client/models/upgrade_response_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,139 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class DRSContentsObject(object):
+class UpgradeResponseModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'id': 'str',
-        'drs_uri': 'list[str]',
-        'contents': 'list[DRSContentsObject]'
+        'upgrade_name': 'str',
+        'start_time': 'str',
+        'end_time': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'id': 'id',
-        'drs_uri': 'drs_uri',
-        'contents': 'contents'
+        'upgrade_name': 'upgradeName',
+        'start_time': 'startTime',
+        'end_time': 'endTime'
     }
 
-    def __init__(self, name=None, id=None, drs_uri=None, contents=None, local_vars_configuration=None):  # noqa: E501
-        """DRSContentsObject - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, upgrade_name=None, start_time=None, end_time=None, local_vars_configuration=None):  # noqa: E501
+        """UpgradeResponseModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._id = None
-        self._drs_uri = None
-        self._contents = None
+        self._upgrade_name = None
+        self._start_time = None
+        self._end_time = None
         self.discriminator = None
 
-        self.name = name
-        if id is not None:
-            self.id = id
-        if drs_uri is not None:
-            self.drs_uri = drs_uri
-        if contents is not None:
-            self.contents = contents
+        if upgrade_name is not None:
+            self.upgrade_name = upgrade_name
+        if start_time is not None:
+            self.start_time = start_time
+        if end_time is not None:
+            self.end_time = end_time
 
     @property
-    def name(self):
-        """Gets the name of this DRSContentsObject.  # noqa: E501
+    def upgrade_name(self):
+        """Gets the upgrade_name of this UpgradeResponseModel.  # noqa: E501
 
-        A name declared by the bundle author that must be used when materialising this object, overriding any name directly associated with the object itself. The name must be unique with the containing bundle. This string is made up of uppercase and lowercase letters, decimal digits, hypen, period, and underscore [A-Za-z0-9.-_]. See http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_282[portable filenames].  # noqa: E501
+        Unique name for the upgrade  # noqa: E501
 
-        :return: The name of this DRSContentsObject.  # noqa: E501
+        :return: The upgrade_name of this UpgradeResponseModel.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._upgrade_name
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this DRSContentsObject.
+    @upgrade_name.setter
+    def upgrade_name(self, upgrade_name):
+        """Sets the upgrade_name of this UpgradeResponseModel.
 
-        A name declared by the bundle author that must be used when materialising this object, overriding any name directly associated with the object itself. The name must be unique with the containing bundle. This string is made up of uppercase and lowercase letters, decimal digits, hypen, period, and underscore [A-Za-z0-9.-_]. See http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_282[portable filenames].  # noqa: E501
+        Unique name for the upgrade  # noqa: E501
 
-        :param name: The name of this DRSContentsObject.  # noqa: E501
+        :param upgrade_name: The upgrade_name of this UpgradeResponseModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._upgrade_name = upgrade_name
 
     @property
-    def id(self):
-        """Gets the id of this DRSContentsObject.  # noqa: E501
+    def start_time(self):
+        """Gets the start_time of this UpgradeResponseModel.  # noqa: E501
 
-        A DRS identifier of an `Object` (either a single blob or a nested bundle). If this ContentsObject is an object within a nested bundle, then the id is optional. Otherwise, the id is required.  # noqa: E501
+        Timestamp the upgrade was started  # noqa: E501
 
-        :return: The id of this DRSContentsObject.  # noqa: E501
+        :return: The start_time of this UpgradeResponseModel.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._start_time
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this DRSContentsObject.
+    @start_time.setter
+    def start_time(self, start_time):
+        """Sets the start_time of this UpgradeResponseModel.
 
-        A DRS identifier of an `Object` (either a single blob or a nested bundle). If this ContentsObject is an object within a nested bundle, then the id is optional. Otherwise, the id is required.  # noqa: E501
+        Timestamp the upgrade was started  # noqa: E501
 
-        :param id: The id of this DRSContentsObject.  # noqa: E501
+        :param start_time: The start_time of this UpgradeResponseModel.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._start_time = start_time
 
     @property
-    def drs_uri(self):
-        """Gets the drs_uri of this DRSContentsObject.  # noqa: E501
+    def end_time(self):
+        """Gets the end_time of this UpgradeResponseModel.  # noqa: E501
 
-        A list of full DRS identifier URI paths that may be used to obtain the object. These URIs may be external to this DRS instance.  # noqa: E501
+        Timestamp the upgrade completed  # noqa: E501
 
-        :return: The drs_uri of this DRSContentsObject.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._drs_uri
-
-    @drs_uri.setter
-    def drs_uri(self, drs_uri):
-        """Sets the drs_uri of this DRSContentsObject.
-
-        A list of full DRS identifier URI paths that may be used to obtain the object. These URIs may be external to this DRS instance.  # noqa: E501
-
-        :param drs_uri: The drs_uri of this DRSContentsObject.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._drs_uri = drs_uri
-
-    @property
-    def contents(self):
-        """Gets the contents of this DRSContentsObject.  # noqa: E501
-
-        If this ContentsObject describes a nested bundle and the caller specified \"?expand=true\" on the request, then this contents array must be present and describe the objects within the nested bundle.  # noqa: E501
-
-        :return: The contents of this DRSContentsObject.  # noqa: E501
-        :rtype: list[DRSContentsObject]
+        :return: The end_time of this UpgradeResponseModel.  # noqa: E501
+        :rtype: str
         """
-        return self._contents
+        return self._end_time
 
-    @contents.setter
-    def contents(self, contents):
-        """Sets the contents of this DRSContentsObject.
+    @end_time.setter
+    def end_time(self, end_time):
+        """Sets the end_time of this UpgradeResponseModel.
 
-        If this ContentsObject describes a nested bundle and the caller specified \"?expand=true\" on the request, then this contents array must be present and describe the objects within the nested bundle.  # noqa: E501
+        Timestamp the upgrade completed  # noqa: E501
 
-        :param contents: The contents of this DRSContentsObject.  # noqa: E501
-        :type: list[DRSContentsObject]
+        :param end_time: The end_time of this UpgradeResponseModel.  # noqa: E501
+        :type: str
         """
 
-        self._contents = contents
+        self._end_time = end_time
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -190,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DRSContentsObject):
+        if not isinstance(other, UpgradeResponseModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DRSContentsObject):
+        if not isinstance(other, UpgradeResponseModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/drs_object.py` & `data-repo-client-1.64.0/data_repo_client/models/drs_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-1.64.0/data_repo_client/models/policy_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,81 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class DuosFirecloudGroupsSyncResponse(object):
+class PolicyResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'synced': 'list[DuosFirecloudGroupModel]',
-        'errors': 'list[ErrorModel]'
+        'policies': 'list[PolicyModel]'
     }
 
     attribute_map = {
-        'synced': 'synced',
-        'errors': 'errors'
+        'policies': 'policies'
     }
 
-    def __init__(self, synced=None, errors=None, local_vars_configuration=None):  # noqa: E501
-        """DuosFirecloudGroupsSyncResponse - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, policies=None, local_vars_configuration=None):  # noqa: E501
+        """PolicyResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._synced = None
-        self._errors = None
+        self._policies = None
         self.discriminator = None
 
-        if synced is not None:
-            self.synced = synced
-        if errors is not None:
-            self.errors = errors
+        if policies is not None:
+            self.policies = policies
 
     @property
-    def synced(self):
-        """Gets the synced of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
+    def policies(self):
+        """Gets the policies of this PolicyResponse.  # noqa: E501
 
-        The Firecloud groups whose contents were successfully updated.   # noqa: E501
 
-        :return: The synced of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
-        :rtype: list[DuosFirecloudGroupModel]
+        :return: The policies of this PolicyResponse.  # noqa: E501
+        :rtype: list[PolicyModel]
         """
-        return self._synced
+        return self._policies
 
-    @synced.setter
-    def synced(self, synced):
-        """Sets the synced of this DuosFirecloudGroupsSyncResponse.
+    @policies.setter
+    def policies(self, policies):
+        """Sets the policies of this PolicyResponse.
 
-        The Firecloud groups whose contents were successfully updated.   # noqa: E501
 
-        :param synced: The synced of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
-        :type: list[DuosFirecloudGroupModel]
+        :param policies: The policies of this PolicyResponse.  # noqa: E501
+        :type: list[PolicyModel]
         """
 
-        self._synced = synced
-
-    @property
-    def errors(self):
-        """Gets the errors of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
-
-        Errors which may have interfered in the syncing for select DUOS Firecloud groups.   # noqa: E501
-
-        :return: The errors of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
-        :rtype: list[ErrorModel]
-        """
-        return self._errors
-
-    @errors.setter
-    def errors(self, errors):
-        """Sets the errors of this DuosFirecloudGroupsSyncResponse.
-
-        Errors which may have interfered in the syncing for select DUOS Firecloud groups.   # noqa: E501
-
-        :param errors: The errors of this DuosFirecloudGroupsSyncResponse.  # noqa: E501
-        :type: list[ErrorModel]
-        """
-
-        self._errors = errors
+        self._policies = policies
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +103,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DuosFirecloudGroupsSyncResponse):
+        if not isinstance(other, PolicyResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DuosFirecloudGroupsSyncResponse):
+        if not isinstance(other, PolicyResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-1.64.0/data_repo_client/models/repository_status_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,165 +1,111 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class FileDetailModel(object):
+class RepositoryStatusModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'dataset_id': 'str',
-        'mime_type': 'str',
-        'access_url': 'str',
-        'load_tag': 'str'
+        'ok': 'bool',
+        'systems': 'dict(str, RepositoryStatusModelSystems)'
     }
 
     attribute_map = {
-        'dataset_id': 'datasetId',
-        'mime_type': 'mimeType',
-        'access_url': 'accessUrl',
-        'load_tag': 'loadTag'
+        'ok': 'ok',
+        'systems': 'systems'
     }
 
-    def __init__(self, dataset_id=None, mime_type=None, access_url=None, load_tag=None, local_vars_configuration=None):  # noqa: E501
-        """FileDetailModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, ok=None, systems=None, local_vars_configuration=None):  # noqa: E501
+        """RepositoryStatusModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._dataset_id = None
-        self._mime_type = None
-        self._access_url = None
-        self._load_tag = None
+        self._ok = None
+        self._systems = None
         self.discriminator = None
 
-        if dataset_id is not None:
-            self.dataset_id = dataset_id
-        if mime_type is not None:
-            self.mime_type = mime_type
-        if access_url is not None:
-            self.access_url = access_url
-        if load_tag is not None:
-            self.load_tag = load_tag
+        self.ok = ok
+        self.systems = systems
 
     @property
-    def dataset_id(self):
-        """Gets the dataset_id of this FileDetailModel.  # noqa: E501
+    def ok(self):
+        """Gets the ok of this RepositoryStatusModel.  # noqa: E501
 
-        Id of the dataset that holds the file  # noqa: E501
+        status of this service  # noqa: E501
 
-        :return: The dataset_id of this FileDetailModel.  # noqa: E501
-        :rtype: str
+        :return: The ok of this RepositoryStatusModel.  # noqa: E501
+        :rtype: bool
         """
-        return self._dataset_id
+        return self._ok
 
-    @dataset_id.setter
-    def dataset_id(self, dataset_id):
-        """Sets the dataset_id of this FileDetailModel.
+    @ok.setter
+    def ok(self, ok):
+        """Sets the ok of this RepositoryStatusModel.
 
-        Id of the dataset that holds the file  # noqa: E501
+        status of this service  # noqa: E501
 
-        :param dataset_id: The dataset_id of this FileDetailModel.  # noqa: E501
-        :type: str
+        :param ok: The ok of this RepositoryStatusModel.  # noqa: E501
+        :type: bool
         """
+        if self.local_vars_configuration.client_side_validation and ok is None:  # noqa: E501
+            raise ValueError("Invalid value for `ok`, must not be `None`")  # noqa: E501
 
-        self._dataset_id = dataset_id
+        self._ok = ok
 
     @property
-    def mime_type(self):
-        """Gets the mime_type of this FileDetailModel.  # noqa: E501
+    def systems(self):
+        """Gets the systems of this RepositoryStatusModel.  # noqa: E501
 
 
-        :return: The mime_type of this FileDetailModel.  # noqa: E501
-        :rtype: str
+        :return: The systems of this RepositoryStatusModel.  # noqa: E501
+        :rtype: dict(str, RepositoryStatusModelSystems)
         """
-        return self._mime_type
+        return self._systems
 
-    @mime_type.setter
-    def mime_type(self, mime_type):
-        """Sets the mime_type of this FileDetailModel.
+    @systems.setter
+    def systems(self, systems):
+        """Sets the systems of this RepositoryStatusModel.
 
 
-        :param mime_type: The mime_type of this FileDetailModel.  # noqa: E501
-        :type: str
+        :param systems: The systems of this RepositoryStatusModel.  # noqa: E501
+        :type: dict(str, RepositoryStatusModelSystems)
         """
+        if self.local_vars_configuration.client_side_validation and systems is None:  # noqa: E501
+            raise ValueError("Invalid value for `systems`, must not be `None`")  # noqa: E501
 
-        self._mime_type = mime_type
-
-    @property
-    def access_url(self):
-        """Gets the access_url of this FileDetailModel.  # noqa: E501
-
-        URL of the file in cloud storage  # noqa: E501
-
-        :return: The access_url of this FileDetailModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._access_url
-
-    @access_url.setter
-    def access_url(self, access_url):
-        """Sets the access_url of this FileDetailModel.
-
-        URL of the file in cloud storage  # noqa: E501
-
-        :param access_url: The access_url of this FileDetailModel.  # noqa: E501
-        :type: str
-        """
-
-        self._access_url = access_url
-
-    @property
-    def load_tag(self):
-        """Gets the load_tag of this FileDetailModel.  # noqa: E501
-
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
-
-        :return: The load_tag of this FileDetailModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._load_tag
-
-    @load_tag.setter
-    def load_tag(self, load_tag):
-        """Sets the load_tag of this FileDetailModel.
-
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
-
-        :param load_tag: The load_tag of this FileDetailModel.  # noqa: E501
-        :type: str
-        """
-
-        self._load_tag = load_tag
+        self._systems = systems
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -187,18 +133,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FileDetailModel):
+        if not isinstance(other, RepositoryStatusModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FileDetailModel):
+        if not isinstance(other, RepositoryStatusModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/file_load_model.py` & `data-repo-client-1.64.0/data_repo_client/models/repository_configuration_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,195 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class FileLoadModel(object):
+class RepositoryConfigurationModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'source_path': 'str',
-        'target_path': 'str',
-        'mime_type': 'str',
-        'profile_id': 'str',
-        'load_tag': 'str',
-        'description': 'str',
-        'md5': 'str'
+        'client_id': 'str',
+        'active_profiles': 'list[str]',
+        'sem_ver': 'str',
+        'git_hash': 'str',
+        'sam_url': 'str'
     }
 
     attribute_map = {
-        'source_path': 'source_path',
-        'target_path': 'target_path',
-        'mime_type': 'mime_type',
-        'profile_id': 'profileId',
-        'load_tag': 'loadTag',
-        'description': 'description',
-        'md5': 'md5'
+        'client_id': 'clientId',
+        'active_profiles': 'activeProfiles',
+        'sem_ver': 'semVer',
+        'git_hash': 'gitHash',
+        'sam_url': 'samUrl'
     }
 
-    def __init__(self, source_path=None, target_path=None, mime_type=None, profile_id=None, load_tag=None, description=None, md5=None, local_vars_configuration=None):  # noqa: E501
-        """FileLoadModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, client_id=None, active_profiles=None, sem_ver=None, git_hash=None, sam_url=None, local_vars_configuration=None):  # noqa: E501
+        """RepositoryConfigurationModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._source_path = None
-        self._target_path = None
-        self._mime_type = None
-        self._profile_id = None
-        self._load_tag = None
-        self._description = None
-        self._md5 = None
+        self._client_id = None
+        self._active_profiles = None
+        self._sem_ver = None
+        self._git_hash = None
+        self._sam_url = None
         self.discriminator = None
 
-        self.source_path = source_path
-        self.target_path = target_path
-        if mime_type is not None:
-            self.mime_type = mime_type
-        if profile_id is not None:
-            self.profile_id = profile_id
-        if load_tag is not None:
-            self.load_tag = load_tag
-        if description is not None:
-            self.description = description
-        if md5 is not None:
-            self.md5 = md5
+        if client_id is not None:
+            self.client_id = client_id
+        if active_profiles is not None:
+            self.active_profiles = active_profiles
+        if sem_ver is not None:
+            self.sem_ver = sem_ver
+        if git_hash is not None:
+            self.git_hash = git_hash
+        if sam_url is not None:
+            self.sam_url = sam_url
 
     @property
-    def source_path(self):
-        """Gets the source_path of this FileLoadModel.  # noqa: E501
+    def client_id(self):
+        """Gets the client_id of this RepositoryConfigurationModel.  # noqa: E501
 
-        gs URL of the source file to load  # noqa: E501
+        the google defined client id for the repository  # noqa: E501
 
-        :return: The source_path of this FileLoadModel.  # noqa: E501
+        :return: The client_id of this RepositoryConfigurationModel.  # noqa: E501
         :rtype: str
         """
-        return self._source_path
+        return self._client_id
 
-    @source_path.setter
-    def source_path(self, source_path):
-        """Sets the source_path of this FileLoadModel.
+    @client_id.setter
+    def client_id(self, client_id):
+        """Sets the client_id of this RepositoryConfigurationModel.
 
-        gs URL of the source file to load  # noqa: E501
+        the google defined client id for the repository  # noqa: E501
 
-        :param source_path: The source_path of this FileLoadModel.  # noqa: E501
+        :param client_id: The client_id of this RepositoryConfigurationModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and source_path is None:  # noqa: E501
-            raise ValueError("Invalid value for `source_path`, must not be `None`")  # noqa: E501
 
-        self._source_path = source_path
+        self._client_id = client_id
 
     @property
-    def target_path(self):
-        """Gets the target_path of this FileLoadModel.  # noqa: E501
+    def active_profiles(self):
+        """Gets the active_profiles of this RepositoryConfigurationModel.  # noqa: E501
 
-        Full path within the dataset where the file should be placed. The path must start with /.   # noqa: E501
+        the active profiles for this instance  # noqa: E501
 
-        :return: The target_path of this FileLoadModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._target_path
-
-    @target_path.setter
-    def target_path(self, target_path):
-        """Sets the target_path of this FileLoadModel.
-
-        Full path within the dataset where the file should be placed. The path must start with /.   # noqa: E501
-
-        :param target_path: The target_path of this FileLoadModel.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and target_path is None:  # noqa: E501
-            raise ValueError("Invalid value for `target_path`, must not be `None`")  # noqa: E501
-
-        self._target_path = target_path
-
-    @property
-    def mime_type(self):
-        """Gets the mime_type of this FileLoadModel.  # noqa: E501
-
-        A string providing the mime-type of the Data Object. For example, \"application/json\".  # noqa: E501
-
-        :return: The mime_type of this FileLoadModel.  # noqa: E501
-        :rtype: str
+        :return: The active_profiles of this RepositoryConfigurationModel.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._mime_type
+        return self._active_profiles
 
-    @mime_type.setter
-    def mime_type(self, mime_type):
-        """Sets the mime_type of this FileLoadModel.
+    @active_profiles.setter
+    def active_profiles(self, active_profiles):
+        """Sets the active_profiles of this RepositoryConfigurationModel.
 
-        A string providing the mime-type of the Data Object. For example, \"application/json\".  # noqa: E501
+        the active profiles for this instance  # noqa: E501
 
-        :param mime_type: The mime_type of this FileLoadModel.  # noqa: E501
-        :type: str
-        """
-
-        self._mime_type = mime_type
-
-    @property
-    def profile_id(self):
-        """Gets the profile_id of this FileLoadModel.  # noqa: E501
-
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
-
-        :return: The profile_id of this FileLoadModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._profile_id
-
-    @profile_id.setter
-    def profile_id(self, profile_id):
-        """Sets the profile_id of this FileLoadModel.
-
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
-
-        :param profile_id: The profile_id of this FileLoadModel.  # noqa: E501
-        :type: str
+        :param active_profiles: The active_profiles of this RepositoryConfigurationModel.  # noqa: E501
+        :type: list[str]
         """
 
-        self._profile_id = profile_id
+        self._active_profiles = active_profiles
 
     @property
-    def load_tag(self):
-        """Gets the load_tag of this FileLoadModel.  # noqa: E501
+    def sem_ver(self):
+        """Gets the sem_ver of this RepositoryConfigurationModel.  # noqa: E501
 
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
+        the semantic version of the data repository  # noqa: E501
 
-        :return: The load_tag of this FileLoadModel.  # noqa: E501
+        :return: The sem_ver of this RepositoryConfigurationModel.  # noqa: E501
         :rtype: str
         """
-        return self._load_tag
+        return self._sem_ver
 
-    @load_tag.setter
-    def load_tag(self, load_tag):
-        """Sets the load_tag of this FileLoadModel.
+    @sem_ver.setter
+    def sem_ver(self, sem_ver):
+        """Sets the sem_ver of this RepositoryConfigurationModel.
 
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
+        the semantic version of the data repository  # noqa: E501
 
-        :param load_tag: The load_tag of this FileLoadModel.  # noqa: E501
+        :param sem_ver: The sem_ver of this RepositoryConfigurationModel.  # noqa: E501
         :type: str
         """
 
-        self._load_tag = load_tag
+        self._sem_ver = sem_ver
 
     @property
-    def description(self):
-        """Gets the description of this FileLoadModel.  # noqa: E501
+    def git_hash(self):
+        """Gets the git_hash of this RepositoryConfigurationModel.  # noqa: E501
 
-        A human readable description of the contents of the Data Object.  # noqa: E501
+        the git hash of the data repository  # noqa: E501
 
-        :return: The description of this FileLoadModel.  # noqa: E501
+        :return: The git_hash of this RepositoryConfigurationModel.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._git_hash
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this FileLoadModel.
+    @git_hash.setter
+    def git_hash(self, git_hash):
+        """Sets the git_hash of this RepositoryConfigurationModel.
 
-        A human readable description of the contents of the Data Object.  # noqa: E501
+        the git hash of the data repository  # noqa: E501
 
-        :param description: The description of this FileLoadModel.  # noqa: E501
+        :param git_hash: The git_hash of this RepositoryConfigurationModel.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._git_hash = git_hash
 
     @property
-    def md5(self):
-        """Gets the md5 of this FileLoadModel.  # noqa: E501
+    def sam_url(self):
+        """Gets the sam_url of this RepositoryConfigurationModel.  # noqa: E501
 
-        A hex representation of the  md5 for the file.  If an md5 exists for the file being ingested, it will be validated against this value and the file's ingest will fail if the values do not match.  If no md5 hash is present on the file being ingested, this value will be stored for the file.  If this value is not specified, then the md5 from the file being ingested (from the cloud provider) will be used   # noqa: E501
+        the URI of SAM this instance uses  # noqa: E501
 
-        :return: The md5 of this FileLoadModel.  # noqa: E501
+        :return: The sam_url of this RepositoryConfigurationModel.  # noqa: E501
         :rtype: str
         """
-        return self._md5
+        return self._sam_url
 
-    @md5.setter
-    def md5(self, md5):
-        """Sets the md5 of this FileLoadModel.
+    @sam_url.setter
+    def sam_url(self, sam_url):
+        """Sets the sam_url of this RepositoryConfigurationModel.
 
-        A hex representation of the  md5 for the file.  If an md5 exists for the file being ingested, it will be validated against this value and the file's ingest will fail if the values do not match.  If no md5 hash is present on the file being ingested, this value will be stored for the file.  If this value is not specified, then the md5 from the file being ingested (from the cloud provider) will be used   # noqa: E501
+        the URI of SAM this instance uses  # noqa: E501
 
-        :param md5: The md5 of this FileLoadModel.  # noqa: E501
+        :param sam_url: The sam_url of this RepositoryConfigurationModel.  # noqa: E501
         :type: str
         """
 
-        self._md5 = md5
+        self._sam_url = sam_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -275,18 +217,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FileLoadModel):
+        if not isinstance(other, RepositoryConfigurationModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FileLoadModel):
+        if not isinstance(other, RepositoryConfigurationModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/file_model_type.py` & `data-repo-client-1.64.0/test/test_column_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,56 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import pprint
-import re  # noqa: F401
+from __future__ import absolute_import
 
-import six
+import unittest
+import datetime
 
-from data_repo_client.configuration import Configuration
+import data_repo_client
+from data_repo_client.models.column_model import ColumnModel  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestColumnModel(unittest.TestCase):
+    """ColumnModel unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ColumnModel
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.column_model.ColumnModel()  # noqa: E501
+        if include_optional :
+            return ColumnModel(
+                name = 'a', 
+                datatype = '0', 
+                array_of = True
+            )
+        else :
+            return ColumnModel(
+                name = 'a',
+                datatype = '0',
+        )
+
+    def testColumnModel(self):
+        """Test ColumnModel"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-class FileModelType(object):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    """
-    allowed enum values
-    """
-    FILE = "file"
-    DIRECTORY = "directory"
-
-    allowable_values = [FILE, DIRECTORY]  # noqa: E501
-
-    """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-    }
-
-    attribute_map = {
-    }
-
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """FileModelType - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-        self.discriminator = None
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, FileModelType):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, FileModelType):
-            return True
-
-        return self.to_dict() != other.to_dict()
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-1.64.0/data_repo_client/models/table_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,296 +1,256 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class IngestResponseModel(object):
+class TableModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'dataset_id': 'str',
-        'dataset': 'str',
-        'table': 'str',
-        'path': 'str',
-        'load_tag': 'str',
-        'row_count': 'int',
-        'bad_row_count': 'int',
-        'load_result': 'BulkLoadArrayResultModel'
+        'name': 'str',
+        'columns': 'list[ColumnModel]',
+        'primary_key': 'list[str]',
+        'partition_mode': 'str',
+        'date_partition_options': 'DatePartitionOptionsModel',
+        'int_partition_options': 'IntPartitionOptionsModel',
+        'row_count': 'int'
     }
 
     attribute_map = {
-        'dataset_id': 'dataset_id',
-        'dataset': 'dataset',
-        'table': 'table',
-        'path': 'path',
-        'load_tag': 'load_tag',
-        'row_count': 'row_count',
-        'bad_row_count': 'bad_row_count',
-        'load_result': 'load_result'
+        'name': 'name',
+        'columns': 'columns',
+        'primary_key': 'primaryKey',
+        'partition_mode': 'partitionMode',
+        'date_partition_options': 'datePartitionOptions',
+        'int_partition_options': 'intPartitionOptions',
+        'row_count': 'rowCount'
     }
 
-    def __init__(self, dataset_id=None, dataset=None, table=None, path=None, load_tag=None, row_count=None, bad_row_count=None, load_result=None, local_vars_configuration=None):  # noqa: E501
-        """IngestResponseModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, columns=None, primary_key=None, partition_mode='none', date_partition_options=None, int_partition_options=None, row_count=None, local_vars_configuration=None):  # noqa: E501
+        """TableModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._dataset_id = None
-        self._dataset = None
-        self._table = None
-        self._path = None
-        self._load_tag = None
+        self._name = None
+        self._columns = None
+        self._primary_key = None
+        self._partition_mode = None
+        self._date_partition_options = None
+        self._int_partition_options = None
         self._row_count = None
-        self._bad_row_count = None
-        self._load_result = None
         self.discriminator = None
 
-        if dataset_id is not None:
-            self.dataset_id = dataset_id
-        if dataset is not None:
-            self.dataset = dataset
-        self.table = table
-        self.path = path
-        if load_tag is not None:
-            self.load_tag = load_tag
-        self.row_count = row_count
-        if bad_row_count is not None:
-            self.bad_row_count = bad_row_count
-        if load_result is not None:
-            self.load_result = load_result
+        self.name = name
+        self.columns = columns
+        if primary_key is not None:
+            self.primary_key = primary_key
+        if partition_mode is not None:
+            self.partition_mode = partition_mode
+        if date_partition_options is not None:
+            self.date_partition_options = date_partition_options
+        if int_partition_options is not None:
+            self.int_partition_options = int_partition_options
+        if row_count is not None:
+            self.row_count = row_count
 
     @property
-    def dataset_id(self):
-        """Gets the dataset_id of this IngestResponseModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this TableModel.  # noqa: E501
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The dataset_id of this IngestResponseModel.  # noqa: E501
+        :return: The name of this TableModel.  # noqa: E501
         :rtype: str
         """
-        return self._dataset_id
+        return self._name
 
-    @dataset_id.setter
-    def dataset_id(self, dataset_id):
-        """Sets the dataset_id of this IngestResponseModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this TableModel.
 
-        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param dataset_id: The dataset_id of this IngestResponseModel.  # noqa: E501
-        :type: str
-        """
-
-        self._dataset_id = dataset_id
-
-    @property
-    def dataset(self):
-        """Gets the dataset of this IngestResponseModel.  # noqa: E501
-
-        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
-
-        :return: The dataset of this IngestResponseModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._dataset
-
-    @dataset.setter
-    def dataset(self, dataset):
-        """Sets the dataset of this IngestResponseModel.
-
-        Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
-
-        :param dataset: The dataset of this IngestResponseModel.  # noqa: E501
+        :param name: The name of this TableModel.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset is not None and len(dataset) > 511):
-            raise ValueError("Invalid value for `dataset`, length must be less than or equal to `511`")  # noqa: E501
+                name is not None and len(name) > 63):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset is not None and len(dataset) < 1):
-            raise ValueError("Invalid value for `dataset`, length must be greater than or equal to `1`")  # noqa: E501
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', dataset)):  # noqa: E501
-            raise ValueError(r"Invalid value for `dataset`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._dataset = dataset
+        self._name = name
 
     @property
-    def table(self):
-        """Gets the table of this IngestResponseModel.  # noqa: E501
+    def columns(self):
+        """Gets the columns of this TableModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The table of this IngestResponseModel.  # noqa: E501
-        :rtype: str
+        :return: The columns of this TableModel.  # noqa: E501
+        :rtype: list[ColumnModel]
         """
-        return self._table
+        return self._columns
 
-    @table.setter
-    def table(self, table):
-        """Sets the table of this IngestResponseModel.
+    @columns.setter
+    def columns(self, columns):
+        """Sets the columns of this TableModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param table: The table of this IngestResponseModel.  # noqa: E501
-        :type: str
+        :param columns: The columns of this TableModel.  # noqa: E501
+        :type: list[ColumnModel]
         """
-        if self.local_vars_configuration.client_side_validation and table is None:  # noqa: E501
-            raise ValueError("Invalid value for `table`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                table is not None and len(table) > 63):
-            raise ValueError("Invalid value for `table`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                table is not None and len(table) < 1):
-            raise ValueError("Invalid value for `table`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                table is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', table)):  # noqa: E501
-            raise ValueError(r"Invalid value for `table`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and columns is None:  # noqa: E501
+            raise ValueError("Invalid value for `columns`, must not be `None`")  # noqa: E501
 
-        self._table = table
+        self._columns = columns
 
     @property
-    def path(self):
-        """Gets the path of this IngestResponseModel.  # noqa: E501
+    def primary_key(self):
+        """Gets the primary_key of this TableModel.  # noqa: E501
 
 
-        :return: The path of this IngestResponseModel.  # noqa: E501
-        :rtype: str
+        :return: The primary_key of this TableModel.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._path
+        return self._primary_key
 
-    @path.setter
-    def path(self, path):
-        """Sets the path of this IngestResponseModel.
+    @primary_key.setter
+    def primary_key(self, primary_key):
+        """Sets the primary_key of this TableModel.
 
 
-        :param path: The path of this IngestResponseModel.  # noqa: E501
-        :type: str
+        :param primary_key: The primary_key of this TableModel.  # noqa: E501
+        :type: list[str]
         """
-        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
-            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._path = path
+        self._primary_key = primary_key
 
     @property
-    def load_tag(self):
-        """Gets the load_tag of this IngestResponseModel.  # noqa: E501
+    def partition_mode(self):
+        """Gets the partition_mode of this TableModel.  # noqa: E501
 
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
 
-        :return: The load_tag of this IngestResponseModel.  # noqa: E501
+        :return: The partition_mode of this TableModel.  # noqa: E501
         :rtype: str
         """
-        return self._load_tag
+        return self._partition_mode
 
-    @load_tag.setter
-    def load_tag(self, load_tag):
-        """Sets the load_tag of this IngestResponseModel.
+    @partition_mode.setter
+    def partition_mode(self, partition_mode):
+        """Sets the partition_mode of this TableModel.
 
-        client-specified tag for a data or file load. If no id is specified, we use the string form of the job create time as the tag.   # noqa: E501
 
-        :param load_tag: The load_tag of this IngestResponseModel.  # noqa: E501
+        :param partition_mode: The partition_mode of this TableModel.  # noqa: E501
         :type: str
         """
+        allowed_values = ["none", "date", "int"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and partition_mode not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `partition_mode` ({0}), must be one of {1}"  # noqa: E501
+                .format(partition_mode, allowed_values)
+            )
 
-        self._load_tag = load_tag
+        self._partition_mode = partition_mode
 
     @property
-    def row_count(self):
-        """Gets the row_count of this IngestResponseModel.  # noqa: E501
+    def date_partition_options(self):
+        """Gets the date_partition_options of this TableModel.  # noqa: E501
 
-        number of rows successfully ingested  # noqa: E501
 
-        :return: The row_count of this IngestResponseModel.  # noqa: E501
-        :rtype: int
+        :return: The date_partition_options of this TableModel.  # noqa: E501
+        :rtype: DatePartitionOptionsModel
         """
-        return self._row_count
+        return self._date_partition_options
 
-    @row_count.setter
-    def row_count(self, row_count):
-        """Sets the row_count of this IngestResponseModel.
+    @date_partition_options.setter
+    def date_partition_options(self, date_partition_options):
+        """Sets the date_partition_options of this TableModel.
 
-        number of rows successfully ingested  # noqa: E501
 
-        :param row_count: The row_count of this IngestResponseModel.  # noqa: E501
-        :type: int
+        :param date_partition_options: The date_partition_options of this TableModel.  # noqa: E501
+        :type: DatePartitionOptionsModel
         """
-        if self.local_vars_configuration.client_side_validation and row_count is None:  # noqa: E501
-            raise ValueError("Invalid value for `row_count`, must not be `None`")  # noqa: E501
 
-        self._row_count = row_count
+        self._date_partition_options = date_partition_options
 
     @property
-    def bad_row_count(self):
-        """Gets the bad_row_count of this IngestResponseModel.  # noqa: E501
+    def int_partition_options(self):
+        """Gets the int_partition_options of this TableModel.  # noqa: E501
 
-        number of bad rows skipped  # noqa: E501
 
-        :return: The bad_row_count of this IngestResponseModel.  # noqa: E501
-        :rtype: int
+        :return: The int_partition_options of this TableModel.  # noqa: E501
+        :rtype: IntPartitionOptionsModel
         """
-        return self._bad_row_count
+        return self._int_partition_options
 
-    @bad_row_count.setter
-    def bad_row_count(self, bad_row_count):
-        """Sets the bad_row_count of this IngestResponseModel.
+    @int_partition_options.setter
+    def int_partition_options(self, int_partition_options):
+        """Sets the int_partition_options of this TableModel.
 
-        number of bad rows skipped  # noqa: E501
 
-        :param bad_row_count: The bad_row_count of this IngestResponseModel.  # noqa: E501
-        :type: int
+        :param int_partition_options: The int_partition_options of this TableModel.  # noqa: E501
+        :type: IntPartitionOptionsModel
         """
 
-        self._bad_row_count = bad_row_count
+        self._int_partition_options = int_partition_options
 
     @property
-    def load_result(self):
-        """Gets the load_result of this IngestResponseModel.  # noqa: E501
+    def row_count(self):
+        """Gets the row_count of this TableModel.  # noqa: E501
 
 
-        :return: The load_result of this IngestResponseModel.  # noqa: E501
-        :rtype: BulkLoadArrayResultModel
+        :return: The row_count of this TableModel.  # noqa: E501
+        :rtype: int
         """
-        return self._load_result
+        return self._row_count
 
-    @load_result.setter
-    def load_result(self, load_result):
-        """Sets the load_result of this IngestResponseModel.
+    @row_count.setter
+    def row_count(self, row_count):
+        """Sets the row_count of this TableModel.
 
 
-        :param load_result: The load_result of this IngestResponseModel.  # noqa: E501
-        :type: BulkLoadArrayResultModel
+        :param row_count: The row_count of this TableModel.  # noqa: E501
+        :type: int
         """
 
-        self._load_result = load_result
+        self._row_count = row_count
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -318,18 +278,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IngestResponseModel):
+        if not isinstance(other, TableModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, IngestResponseModel):
+        if not isinstance(other, TableModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-1.64.0/data_repo_client/models/int_partition_options_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -63,41 +63,41 @@
         self.max = max
         self.interval = interval
 
     @property
     def column(self):
         """Gets the column of this IntPartitionOptionsModel.  # noqa: E501
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :return: The column of this IntPartitionOptionsModel.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
         """Sets the column of this IntPartitionOptionsModel.
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
         :param column: The column of this IntPartitionOptionsModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and column is None:  # noqa: E501
             raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 column is not None and len(column) > 63):
             raise ValueError("Invalid value for `column`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 column is not None and len(column) < 1):
             raise ValueError("Invalid value for `column`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                column is not None and not re.search(r'^[a-zA-Z][_a-zA-Z0-9]*$', column)):  # noqa: E501
-            raise ValueError(r"Invalid value for `column`, must be a follow pattern or equal to `/^[a-zA-Z][_a-zA-Z0-9]*$/`")  # noqa: E501
+                column is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', column)):  # noqa: E501
+            raise ValueError(r"Invalid value for `column`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
         self._column = column
 
     @property
     def min(self):
         """Gets the min of this IntPartitionOptionsModel.  # noqa: E501
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/job_model.py` & `data-repo-client-1.64.0/data_repo_client/models/job_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -34,80 +34,75 @@
     """
     openapi_types = {
         'id': 'str',
         'description': 'str',
         'job_status': 'str',
         'status_code': 'int',
         'submitted': 'str',
-        'completed': 'str',
-        'class_name': 'str'
+        'completed': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'description': 'description',
         'job_status': 'job_status',
         'status_code': 'status_code',
         'submitted': 'submitted',
-        'completed': 'completed',
-        'class_name': 'class_name'
+        'completed': 'completed'
     }
 
-    def __init__(self, id=None, description=None, job_status=None, status_code=None, submitted=None, completed=None, class_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, description=None, job_status=None, status_code=None, submitted=None, completed=None, local_vars_configuration=None):  # noqa: E501
         """JobModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._description = None
         self._job_status = None
         self._status_code = None
         self._submitted = None
         self._completed = None
-        self._class_name = None
         self.discriminator = None
 
         self.id = id
         if description is not None:
             self.description = description
         self.job_status = job_status
         self.status_code = status_code
         if submitted is not None:
             self.submitted = submitted
         if completed is not None:
             self.completed = completed
-        if class_name is not None:
-            self.class_name = class_name
 
     @property
     def id(self):
         """Gets the id of this JobModel.  # noqa: E501
 
-        Unique identifier for flights, jobs, etc.   # noqa: E501
+        Unique identifier for a flights, jobs, etc.   # noqa: E501
 
         :return: The id of this JobModel.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this JobModel.
 
-        Unique identifier for flights, jobs, etc.   # noqa: E501
+        Unique identifier for a flights, jobs, etc.   # noqa: E501
 
         :param id: The id of this JobModel.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                id is not None and not re.search(r'[A-Za-z0-9_\\-]{22}', id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[A-Za-z0-9_\\-]{22}/`")  # noqa: E501
+                id is not None and not re.search(r'[A-za-z0-9_\\-]{22}', id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/[A-za-z0-9_\\-]{22}/`")  # noqa: E501
 
         self._id = id
 
     @property
     def description(self):
         """Gets the description of this JobModel.  # noqa: E501
 
@@ -228,37 +223,14 @@
 
         :param completed: The completed of this JobModel.  # noqa: E501
         :type: str
         """
 
         self._completed = completed
 
-    @property
-    def class_name(self):
-        """Gets the class_name of this JobModel.  # noqa: E501
-
-        Class name of the flight  # noqa: E501
-
-        :return: The class_name of this JobModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._class_name
-
-    @class_name.setter
-    def class_name(self, class_name):
-        """Sets the class_name of this JobModel.
-
-        Class name of the flight  # noqa: E501
-
-        :param class_name: The class_name of this JobModel.  # noqa: E501
-        :type: str
-        """
-
-        self._class_name = class_name
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/relationship_model.py` & `data-repo-client-1.64.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,82 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class RelationshipModel(object):
+class SnapshotRequestRowIdModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        '_from': 'RelationshipTermModel',
-        'to': 'RelationshipTermModel'
+        'tables': 'list[SnapshotRequestRowIdTableModel]'
     }
 
     attribute_map = {
-        'name': 'name',
-        '_from': 'from',
-        'to': 'to'
+        'tables': 'tables'
     }
 
-    def __init__(self, name=None, _from=None, to=None, local_vars_configuration=None):  # noqa: E501
-        """RelationshipModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, tables=None, local_vars_configuration=None):  # noqa: E501
+        """SnapshotRequestRowIdModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self.__from = None
-        self._to = None
+        self._tables = None
         self.discriminator = None
 
-        self.name = name
-        self._from = _from
-        self.to = to
+        self.tables = tables
 
     @property
-    def name(self):
-        """Gets the name of this RelationshipModel.  # noqa: E501
+    def tables(self):
+        """Gets the tables of this SnapshotRequestRowIdModel.  # noqa: E501
 
 
-        :return: The name of this RelationshipModel.  # noqa: E501
-        :rtype: str
+        :return: The tables of this SnapshotRequestRowIdModel.  # noqa: E501
+        :rtype: list[SnapshotRequestRowIdTableModel]
         """
-        return self._name
+        return self._tables
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RelationshipModel.
+    @tables.setter
+    def tables(self, tables):
+        """Sets the tables of this SnapshotRequestRowIdModel.
 
 
-        :param name: The name of this RelationshipModel.  # noqa: E501
-        :type: str
+        :param tables: The tables of this SnapshotRequestRowIdModel.  # noqa: E501
+        :type: list[SnapshotRequestRowIdTableModel]
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and tables is None:  # noqa: E501
+            raise ValueError("Invalid value for `tables`, must not be `None`")  # noqa: E501
 
-        self._name = name
-
-    @property
-    def _from(self):
-        """Gets the _from of this RelationshipModel.  # noqa: E501
-
-
-        :return: The _from of this RelationshipModel.  # noqa: E501
-        :rtype: RelationshipTermModel
-        """
-        return self.__from
-
-    @_from.setter
-    def _from(self, _from):
-        """Sets the _from of this RelationshipModel.
-
-
-        :param _from: The _from of this RelationshipModel.  # noqa: E501
-        :type: RelationshipTermModel
-        """
-        if self.local_vars_configuration.client_side_validation and _from is None:  # noqa: E501
-            raise ValueError("Invalid value for `_from`, must not be `None`")  # noqa: E501
-
-        self.__from = _from
-
-    @property
-    def to(self):
-        """Gets the to of this RelationshipModel.  # noqa: E501
-
-
-        :return: The to of this RelationshipModel.  # noqa: E501
-        :rtype: RelationshipTermModel
-        """
-        return self._to
-
-    @to.setter
-    def to(self, to):
-        """Sets the to of this RelationshipModel.
-
-
-        :param to: The to of this RelationshipModel.  # noqa: E501
-        :type: RelationshipTermModel
-        """
-        if self.local_vars_configuration.client_side_validation and to is None:  # noqa: E501
-            raise ValueError("Invalid value for `to`, must not be `None`")  # noqa: E501
-
-        self._to = to
+        self._tables = tables
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -161,18 +104,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RelationshipModel):
+        if not isinstance(other, SnapshotRequestRowIdModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RelationshipModel):
+        if not isinstance(other, SnapshotRequestRowIdModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-1.64.0/data_repo_client/models/relationship_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,139 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class RelationshipTermModel(object):
+class RelationshipModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'table': 'str',
-        'column': 'str'
+        'name': 'str',
+        '_from': 'RelationshipTermModel',
+        'to': 'RelationshipTermModel'
     }
 
     attribute_map = {
-        'table': 'table',
-        'column': 'column'
+        'name': 'name',
+        '_from': 'from',
+        'to': 'to'
     }
 
-    def __init__(self, table=None, column=None, local_vars_configuration=None):  # noqa: E501
-        """RelationshipTermModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, _from=None, to=None, local_vars_configuration=None):  # noqa: E501
+        """RelationshipModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._table = None
-        self._column = None
+        self._name = None
+        self.__from = None
+        self._to = None
         self.discriminator = None
 
-        self.table = table
-        self.column = column
+        self.name = name
+        self._from = _from
+        self.to = to
 
     @property
-    def table(self):
-        """Gets the table of this RelationshipTermModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this RelationshipModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The table of this RelationshipTermModel.  # noqa: E501
+        :return: The name of this RelationshipModel.  # noqa: E501
         :rtype: str
         """
-        return self._table
+        return self._name
 
-    @table.setter
-    def table(self, table):
-        """Sets the table of this RelationshipTermModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this RelationshipModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param table: The table of this RelationshipTermModel.  # noqa: E501
+        :param name: The name of this RelationshipModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and table is None:  # noqa: E501
-            raise ValueError("Invalid value for `table`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                table is not None and len(table) > 63):
-            raise ValueError("Invalid value for `table`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                table is not None and len(table) < 1):
-            raise ValueError("Invalid value for `table`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                table is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', table)):  # noqa: E501
-            raise ValueError(r"Invalid value for `table`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._table = table
+        self._name = name
 
     @property
-    def column(self):
-        """Gets the column of this RelationshipTermModel.  # noqa: E501
+    def _from(self):
+        """Gets the _from of this RelationshipModel.  # noqa: E501
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The column of this RelationshipTermModel.  # noqa: E501
-        :rtype: str
+        :return: The _from of this RelationshipModel.  # noqa: E501
+        :rtype: RelationshipTermModel
         """
-        return self._column
+        return self.__from
 
-    @column.setter
-    def column(self, column):
-        """Sets the column of this RelationshipTermModel.
+    @_from.setter
+    def _from(self, _from):
+        """Sets the _from of this RelationshipModel.
 
-        Column names follow this pattern. This should be used for the name of any column in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. This is shorter than what BigQuery allows.   # noqa: E501
 
-        :param column: The column of this RelationshipTermModel.  # noqa: E501
-        :type: str
+        :param _from: The _from of this RelationshipModel.  # noqa: E501
+        :type: RelationshipTermModel
         """
-        if self.local_vars_configuration.client_side_validation and column is None:  # noqa: E501
-            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                column is not None and len(column) > 63):
-            raise ValueError("Invalid value for `column`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                column is not None and len(column) < 1):
-            raise ValueError("Invalid value for `column`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                column is not None and not re.search(r'^[a-zA-Z][_a-zA-Z0-9]*$', column)):  # noqa: E501
-            raise ValueError(r"Invalid value for `column`, must be a follow pattern or equal to `/^[a-zA-Z][_a-zA-Z0-9]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and _from is None:  # noqa: E501
+            raise ValueError("Invalid value for `_from`, must not be `None`")  # noqa: E501
+
+        self.__from = _from
+
+    @property
+    def to(self):
+        """Gets the to of this RelationshipModel.  # noqa: E501
+
+
+        :return: The to of this RelationshipModel.  # noqa: E501
+        :rtype: RelationshipTermModel
+        """
+        return self._to
+
+    @to.setter
+    def to(self, to):
+        """Sets the to of this RelationshipModel.
+
+
+        :param to: The to of this RelationshipModel.  # noqa: E501
+        :type: RelationshipTermModel
+        """
+        if self.local_vars_configuration.client_side_validation and to is None:  # noqa: E501
+            raise ValueError("Invalid value for `to`, must not be `None`")  # noqa: E501
 
-        self._column = column
+        self._to = to
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -153,18 +161,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RelationshipTermModel):
+        if not isinstance(other, RelationshipModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RelationshipTermModel):
+        if not isinstance(other, RelationshipModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/search_index_request.py` & `data-repo-client-1.64.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,63 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SearchIndexRequest(object):
+class EnumerateSortByParam(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    NAME = "name"
+    DESCRIPTION = "description"
+    CREATED_DATE = "created_date"
+
+    allowable_values = [NAME, DESCRIPTION, CREATED_DATE]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'sql': 'str'
     }
 
     attribute_map = {
-        'sql': 'sql'
     }
 
-    def __init__(self, sql=None, local_vars_configuration=None):  # noqa: E501
-        """SearchIndexRequest - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """EnumerateSortByParam - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._sql = None
         self.discriminator = None
 
-        self.sql = sql
-
-    @property
-    def sql(self):
-        """Gets the sql of this SearchIndexRequest.  # noqa: E501
-
-        SQL to index BigQuery columns for searching   # noqa: E501
-
-        :return: The sql of this SearchIndexRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._sql
-
-    @sql.setter
-    def sql(self, sql):
-        """Sets the sql of this SearchIndexRequest.
-
-        SQL to index BigQuery columns for searching   # noqa: E501
-
-        :param sql: The sql of this SearchIndexRequest.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and sql is None:  # noqa: E501
-            raise ValueError("Invalid value for `sql`, must not be `None`")  # noqa: E501
-
-        self._sql = sql
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -106,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchIndexRequest):
+        if not isinstance(other, EnumerateSortByParam):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SearchIndexRequest):
+        if not isinstance(other, EnumerateSortByParam):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-1.64.0/data_repo_client/models/date_partition_options_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,93 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotRequestAssetModel(object):
+class DatePartitionOptionsModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'asset_name': 'str',
-        'root_values': 'list[str]'
+        'column': 'str'
     }
 
     attribute_map = {
-        'asset_name': 'assetName',
-        'root_values': 'rootValues'
+        'column': 'column'
     }
 
-    def __init__(self, asset_name=None, root_values=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotRequestAssetModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, local_vars_configuration=None):  # noqa: E501
+        """DatePartitionOptionsModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._asset_name = None
-        self._root_values = None
+        self._column = None
         self.discriminator = None
 
-        self.asset_name = asset_name
-        self.root_values = root_values
+        self.column = column
 
     @property
-    def asset_name(self):
-        """Gets the asset_name of this SnapshotRequestAssetModel.  # noqa: E501
+    def column(self):
+        """Gets the column of this DatePartitionOptionsModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The asset_name of this SnapshotRequestAssetModel.  # noqa: E501
+        :return: The column of this DatePartitionOptionsModel.  # noqa: E501
         :rtype: str
         """
-        return self._asset_name
+        return self._column
 
-    @asset_name.setter
-    def asset_name(self, asset_name):
-        """Sets the asset_name of this SnapshotRequestAssetModel.
+    @column.setter
+    def column(self, column):
+        """Sets the column of this DatePartitionOptionsModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param asset_name: The asset_name of this SnapshotRequestAssetModel.  # noqa: E501
+        :param column: The column of this DatePartitionOptionsModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and asset_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `asset_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and column is None:  # noqa: E501
+            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and len(asset_name) > 63):
-            raise ValueError("Invalid value for `asset_name`, length must be less than or equal to `63`")  # noqa: E501
+                column is not None and len(column) > 63):
+            raise ValueError("Invalid value for `column`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and len(asset_name) < 1):
-            raise ValueError("Invalid value for `asset_name`, length must be greater than or equal to `1`")  # noqa: E501
+                column is not None and len(column) < 1):
+            raise ValueError("Invalid value for `column`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', asset_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `asset_name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                column is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', column)):  # noqa: E501
+            raise ValueError(r"Invalid value for `column`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._asset_name = asset_name
-
-    @property
-    def root_values(self):
-        """Gets the root_values of this SnapshotRequestAssetModel.  # noqa: E501
-
-
-        :return: The root_values of this SnapshotRequestAssetModel.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._root_values
-
-    @root_values.setter
-    def root_values(self, root_values):
-        """Sets the root_values of this SnapshotRequestAssetModel.
-
-
-        :param root_values: The root_values of this SnapshotRequestAssetModel.  # noqa: E501
-        :type: list[str]
-        """
-        if self.local_vars_configuration.client_side_validation and root_values is None:  # noqa: E501
-            raise ValueError("Invalid value for `root_values`, must not be `None`")  # noqa: E501
-
-        self._root_values = root_values
+        self._column = column
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -142,18 +115,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotRequestAssetModel):
+        if not isinstance(other, DatePartitionOptionsModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotRequestAssetModel):
+        if not isinstance(other, DatePartitionOptionsModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-1.64.0/data_repo_client/models/snapshot_request_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,205 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotRequestContentsModel(object):
+class SnapshotRequestModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'dataset_name': 'str',
-        'mode': 'str',
-        'asset_spec': 'SnapshotRequestAssetModel',
-        'query_spec': 'SnapshotRequestQueryModel',
-        'row_id_spec': 'SnapshotRequestRowIdModel'
+        'name': 'str',
+        'description': 'str',
+        'contents': 'list[SnapshotRequestContentsModel]',
+        'readers': 'list[str]',
+        'profile_id': 'str'
     }
 
     attribute_map = {
-        'dataset_name': 'datasetName',
-        'mode': 'mode',
-        'asset_spec': 'assetSpec',
-        'query_spec': 'querySpec',
-        'row_id_spec': 'rowIdSpec'
+        'name': 'name',
+        'description': 'description',
+        'contents': 'contents',
+        'readers': 'readers',
+        'profile_id': 'profileId'
     }
 
-    def __init__(self, dataset_name=None, mode=None, asset_spec=None, query_spec=None, row_id_spec=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotRequestContentsModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, description=None, contents=None, readers=None, profile_id=None, local_vars_configuration=None):  # noqa: E501
+        """SnapshotRequestModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._dataset_name = None
-        self._mode = None
-        self._asset_spec = None
-        self._query_spec = None
-        self._row_id_spec = None
+        self._name = None
+        self._description = None
+        self._contents = None
+        self._readers = None
+        self._profile_id = None
         self.discriminator = None
 
-        self.dataset_name = dataset_name
-        self.mode = mode
-        if asset_spec is not None:
-            self.asset_spec = asset_spec
-        if query_spec is not None:
-            self.query_spec = query_spec
-        if row_id_spec is not None:
-            self.row_id_spec = row_id_spec
+        self.name = name
+        if description is not None:
+            self.description = description
+        self.contents = contents
+        if readers is not None:
+            self.readers = readers
+        if profile_id is not None:
+            self.profile_id = profile_id
 
     @property
-    def dataset_name(self):
-        """Gets the dataset_name of this SnapshotRequestContentsModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this SnapshotRequestModel.  # noqa: E501
 
         Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
 
-        :return: The dataset_name of this SnapshotRequestContentsModel.  # noqa: E501
+        :return: The name of this SnapshotRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._dataset_name
+        return self._name
 
-    @dataset_name.setter
-    def dataset_name(self, dataset_name):
-        """Sets the dataset_name of this SnapshotRequestContentsModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this SnapshotRequestModel.
 
         Dataset and snapshot names follow this pattern. It is the same as ObjectNameProperty, but has a greater maxLength.   # noqa: E501
 
-        :param dataset_name: The dataset_name of this SnapshotRequestContentsModel.  # noqa: E501
+        :param name: The name of this SnapshotRequestModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and dataset_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `dataset_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset_name is not None and len(dataset_name) > 511):
-            raise ValueError("Invalid value for `dataset_name`, length must be less than or equal to `511`")  # noqa: E501
+                name is not None and len(name) > 511):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `511`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset_name is not None and len(dataset_name) < 1):
-            raise ValueError("Invalid value for `dataset_name`, length must be greater than or equal to `1`")  # noqa: E501
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                dataset_name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', dataset_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `dataset_name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._dataset_name = dataset_name
+        self._name = name
 
     @property
-    def mode(self):
-        """Gets the mode of this SnapshotRequestContentsModel.  # noqa: E501
+    def description(self):
+        """Gets the description of this SnapshotRequestModel.  # noqa: E501
 
+        Description of the snapshot  # noqa: E501
 
-        :return: The mode of this SnapshotRequestContentsModel.  # noqa: E501
+        :return: The description of this SnapshotRequestModel.  # noqa: E501
         :rtype: str
         """
-        return self._mode
+        return self._description
 
-    @mode.setter
-    def mode(self, mode):
-        """Sets the mode of this SnapshotRequestContentsModel.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this SnapshotRequestModel.
 
+        Description of the snapshot  # noqa: E501
 
-        :param mode: The mode of this SnapshotRequestContentsModel.  # noqa: E501
+        :param description: The description of this SnapshotRequestModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and mode is None:  # noqa: E501
-            raise ValueError("Invalid value for `mode`, must not be `None`")  # noqa: E501
-        allowed_values = ["byAsset", "byFullView", "byQuery", "byRowId"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and mode not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `mode` ({0}), must be one of {1}"  # noqa: E501
-                .format(mode, allowed_values)
-            )
 
-        self._mode = mode
+        self._description = description
 
     @property
-    def asset_spec(self):
-        """Gets the asset_spec of this SnapshotRequestContentsModel.  # noqa: E501
+    def contents(self):
+        """Gets the contents of this SnapshotRequestModel.  # noqa: E501
 
 
-        :return: The asset_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :rtype: SnapshotRequestAssetModel
+        :return: The contents of this SnapshotRequestModel.  # noqa: E501
+        :rtype: list[SnapshotRequestContentsModel]
         """
-        return self._asset_spec
+        return self._contents
 
-    @asset_spec.setter
-    def asset_spec(self, asset_spec):
-        """Sets the asset_spec of this SnapshotRequestContentsModel.
+    @contents.setter
+    def contents(self, contents):
+        """Sets the contents of this SnapshotRequestModel.
 
 
-        :param asset_spec: The asset_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :type: SnapshotRequestAssetModel
+        :param contents: The contents of this SnapshotRequestModel.  # noqa: E501
+        :type: list[SnapshotRequestContentsModel]
         """
+        if self.local_vars_configuration.client_side_validation and contents is None:  # noqa: E501
+            raise ValueError("Invalid value for `contents`, must not be `None`")  # noqa: E501
 
-        self._asset_spec = asset_spec
+        self._contents = contents
 
     @property
-    def query_spec(self):
-        """Gets the query_spec of this SnapshotRequestContentsModel.  # noqa: E501
+    def readers(self):
+        """Gets the readers of this SnapshotRequestModel.  # noqa: E501
 
 
-        :return: The query_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :rtype: SnapshotRequestQueryModel
+        :return: The readers of this SnapshotRequestModel.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._query_spec
+        return self._readers
 
-    @query_spec.setter
-    def query_spec(self, query_spec):
-        """Sets the query_spec of this SnapshotRequestContentsModel.
+    @readers.setter
+    def readers(self, readers):
+        """Sets the readers of this SnapshotRequestModel.
 
 
-        :param query_spec: The query_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :type: SnapshotRequestQueryModel
+        :param readers: The readers of this SnapshotRequestModel.  # noqa: E501
+        :type: list[str]
         """
 
-        self._query_spec = query_spec
+        self._readers = readers
 
     @property
-    def row_id_spec(self):
-        """Gets the row_id_spec of this SnapshotRequestContentsModel.  # noqa: E501
+    def profile_id(self):
+        """Gets the profile_id of this SnapshotRequestModel.  # noqa: E501
 
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :return: The row_id_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :rtype: SnapshotRequestRowIdModel
+        :return: The profile_id of this SnapshotRequestModel.  # noqa: E501
+        :rtype: str
         """
-        return self._row_id_spec
+        return self._profile_id
 
-    @row_id_spec.setter
-    def row_id_spec(self, row_id_spec):
-        """Sets the row_id_spec of this SnapshotRequestContentsModel.
+    @profile_id.setter
+    def profile_id(self, profile_id):
+        """Sets the profile_id of this SnapshotRequestModel.
 
+        Unique identifier for a dataset, snapshot, etc.   # noqa: E501
 
-        :param row_id_spec: The row_id_spec of this SnapshotRequestContentsModel.  # noqa: E501
-        :type: SnapshotRequestRowIdModel
+        :param profile_id: The profile_id of this SnapshotRequestModel.  # noqa: E501
+        :type: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                profile_id is not None and not re.search(r'^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}', profile_id)):  # noqa: E501
+            raise ValueError(r"Invalid value for `profile_id`, must be a follow pattern or equal to `/^[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}/`")  # noqa: E501
 
-        self._row_id_spec = row_id_spec
+        self._profile_id = profile_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -226,18 +227,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotRequestContentsModel):
+        if not isinstance(other, SnapshotRequestModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotRequestContentsModel):
+        if not isinstance(other, SnapshotRequestModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-1.64.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,109 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotRequestQueryModel(object):
+class EnumerateSnapshotModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'asset_name': 'str',
-        'query': 'str'
+        'total': 'int',
+        'items': 'list[SnapshotSummaryModel]'
     }
 
     attribute_map = {
-        'asset_name': 'assetName',
-        'query': 'query'
+        'total': 'total',
+        'items': 'items'
     }
 
-    def __init__(self, asset_name=None, query=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotRequestQueryModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, total=None, items=None, local_vars_configuration=None):  # noqa: E501
+        """EnumerateSnapshotModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._asset_name = None
-        self._query = None
+        self._total = None
+        self._items = None
         self.discriminator = None
 
-        self.asset_name = asset_name
-        self.query = query
+        if total is not None:
+            self.total = total
+        if items is not None:
+            self.items = items
 
     @property
-    def asset_name(self):
-        """Gets the asset_name of this SnapshotRequestQueryModel.  # noqa: E501
+    def total(self):
+        """Gets the total of this EnumerateSnapshotModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Total number of snapshots  # noqa: E501
 
-        :return: The asset_name of this SnapshotRequestQueryModel.  # noqa: E501
-        :rtype: str
+        :return: The total of this EnumerateSnapshotModel.  # noqa: E501
+        :rtype: int
         """
-        return self._asset_name
+        return self._total
 
-    @asset_name.setter
-    def asset_name(self, asset_name):
-        """Sets the asset_name of this SnapshotRequestQueryModel.
+    @total.setter
+    def total(self, total):
+        """Sets the total of this EnumerateSnapshotModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Total number of snapshots  # noqa: E501
 
-        :param asset_name: The asset_name of this SnapshotRequestQueryModel.  # noqa: E501
-        :type: str
+        :param total: The total of this EnumerateSnapshotModel.  # noqa: E501
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and asset_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `asset_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and len(asset_name) > 63):
-            raise ValueError("Invalid value for `asset_name`, length must be less than or equal to `63`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and len(asset_name) < 1):
-            raise ValueError("Invalid value for `asset_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                asset_name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', asset_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `asset_name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._asset_name = asset_name
+        self._total = total
 
     @property
-    def query(self):
-        """Gets the query of this SnapshotRequestQueryModel.  # noqa: E501
+    def items(self):
+        """Gets the items of this EnumerateSnapshotModel.  # noqa: E501
 
 
-        :return: The query of this SnapshotRequestQueryModel.  # noqa: E501
-        :rtype: str
+        :return: The items of this EnumerateSnapshotModel.  # noqa: E501
+        :rtype: list[SnapshotSummaryModel]
         """
-        return self._query
+        return self._items
 
-    @query.setter
-    def query(self, query):
-        """Sets the query of this SnapshotRequestQueryModel.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this EnumerateSnapshotModel.
 
 
-        :param query: The query of this SnapshotRequestQueryModel.  # noqa: E501
-        :type: str
+        :param items: The items of this EnumerateSnapshotModel.  # noqa: E501
+        :type: list[SnapshotSummaryModel]
         """
-        if self.local_vars_configuration.client_side_validation and query is None:  # noqa: E501
-            raise ValueError("Invalid value for `query`, must not be `None`")  # noqa: E501
 
-        self._query = query
+        self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -142,18 +131,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotRequestQueryModel):
+        if not isinstance(other, EnumerateSnapshotModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotRequestQueryModel):
+        if not isinstance(other, EnumerateSnapshotModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-1.64.0/data_repo_client/models/asset_table_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,121 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotRequestRowIdTableModel(object):
+class AssetTableModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'table_name': 'str',
-        'columns': 'list[str]',
-        'row_ids': 'list[str]'
+        'name': 'str',
+        'columns': 'list[str]'
     }
 
     attribute_map = {
-        'table_name': 'tableName',
-        'columns': 'columns',
-        'row_ids': 'rowIds'
+        'name': 'name',
+        'columns': 'columns'
     }
 
-    def __init__(self, table_name=None, columns=None, row_ids=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotRequestRowIdTableModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, columns=None, local_vars_configuration=None):  # noqa: E501
+        """AssetTableModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._table_name = None
+        self._name = None
         self._columns = None
-        self._row_ids = None
         self.discriminator = None
 
-        self.table_name = table_name
+        self.name = name
         self.columns = columns
-        self.row_ids = row_ids
 
     @property
-    def table_name(self):
-        """Gets the table_name of this SnapshotRequestRowIdTableModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this AssetTableModel.  # noqa: E501
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :return: The table_name of this SnapshotRequestRowIdTableModel.  # noqa: E501
+        :return: The name of this AssetTableModel.  # noqa: E501
         :rtype: str
         """
-        return self._table_name
+        return self._name
 
-    @table_name.setter
-    def table_name(self, table_name):
-        """Sets the table_name of this SnapshotRequestRowIdTableModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this AssetTableModel.
 
-        Table names follow this pattern. This should be used for the name of any non-column object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra tables the DR adds. For table names, this is shorter than what BigQuery allows.   # noqa: E501
+        Table and column names follow this pattern. This should be used for the name of any object in the system. It enforces BigQuery naming rules except it disallows a leading underscore so we avoid collisions with any extra columns the DR adds. For table and column names, this is shorter than what BigQuery allows.   # noqa: E501
 
-        :param table_name: The table_name of this SnapshotRequestRowIdTableModel.  # noqa: E501
+        :param name: The name of this AssetTableModel.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and table_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                table_name is not None and len(table_name) > 63):
-            raise ValueError("Invalid value for `table_name`, length must be less than or equal to `63`")  # noqa: E501
+                name is not None and len(name) > 63):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                table_name is not None and len(table_name) < 1):
-            raise ValueError("Invalid value for `table_name`, length must be greater than or equal to `1`")  # noqa: E501
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                table_name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', table_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `table_name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
+                name is not None and not re.search(r'^[a-zA-Z0-9][_a-zA-Z0-9]*$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9][_a-zA-Z0-9]*$/`")  # noqa: E501
 
-        self._table_name = table_name
+        self._name = name
 
     @property
     def columns(self):
-        """Gets the columns of this SnapshotRequestRowIdTableModel.  # noqa: E501
+        """Gets the columns of this AssetTableModel.  # noqa: E501
 
 
-        :return: The columns of this SnapshotRequestRowIdTableModel.  # noqa: E501
+        :return: The columns of this AssetTableModel.  # noqa: E501
         :rtype: list[str]
         """
         return self._columns
 
     @columns.setter
     def columns(self, columns):
-        """Sets the columns of this SnapshotRequestRowIdTableModel.
+        """Sets the columns of this AssetTableModel.
 
 
-        :param columns: The columns of this SnapshotRequestRowIdTableModel.  # noqa: E501
+        :param columns: The columns of this AssetTableModel.  # noqa: E501
         :type: list[str]
         """
         if self.local_vars_configuration.client_side_validation and columns is None:  # noqa: E501
             raise ValueError("Invalid value for `columns`, must not be `None`")  # noqa: E501
 
         self._columns = columns
 
-    @property
-    def row_ids(self):
-        """Gets the row_ids of this SnapshotRequestRowIdTableModel.  # noqa: E501
-
-
-        :return: The row_ids of this SnapshotRequestRowIdTableModel.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._row_ids
-
-    @row_ids.setter
-    def row_ids(self, row_ids):
-        """Sets the row_ids of this SnapshotRequestRowIdTableModel.
-
-
-        :param row_ids: The row_ids of this SnapshotRequestRowIdTableModel.  # noqa: E501
-        :type: list[str]
-        """
-        if self.local_vars_configuration.client_side_validation and row_ids is None:  # noqa: E501
-            raise ValueError("Invalid value for `row_ids`, must not be `None`")  # noqa: E501
-
-        self._row_ids = row_ids
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -169,18 +142,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotRequestRowIdTableModel):
+        if not isinstance(other, AssetTableModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotRequestRowIdTableModel):
+        if not isinstance(other, AssetTableModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/sql_sort_direction.py` & `data-repo-client-1.64.0/test/test_sql_sort_direction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,51 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import pprint
-import re  # noqa: F401
+from __future__ import absolute_import
 
-import six
+import unittest
+import datetime
 
-from data_repo_client.configuration import Configuration
+import data_repo_client
+from data_repo_client.models.sql_sort_direction import SqlSortDirection  # noqa: E501
+from data_repo_client.rest import ApiException
+
+class TestSqlSortDirection(unittest.TestCase):
+    """SqlSortDirection unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SqlSortDirection
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = data_repo_client.models.sql_sort_direction.SqlSortDirection()  # noqa: E501
+        if include_optional :
+            return SqlSortDirection(
+            )
+        else :
+            return SqlSortDirection(
+        )
+
+    def testSqlSortDirection(self):
+        """Test SqlSortDirection"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-class SqlSortDirection(object):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    """
-    allowed enum values
-    """
-    ASC = "asc"
-    DESC = "desc"
-
-    allowable_values = [ASC, DESC]  # noqa: E501
-
-    """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-    }
-
-    attribute_map = {
-    }
-
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """SqlSortDirection - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-        self.discriminator = None
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, SqlSortDirection):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, SqlSortDirection):
-            return True
-
-        return self.to_dict() != other.to_dict()
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-1.64.0/data_repo_client/models/policy_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,107 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class TagUpdateRequestModel(object):
+class PolicyModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'add': 'list[str]',
-        'remove': 'list[str]'
+        'name': 'str',
+        'members': 'list[str]'
     }
 
     attribute_map = {
-        'add': 'add',
-        'remove': 'remove'
+        'name': 'name',
+        'members': 'members'
     }
 
-    def __init__(self, add=None, remove=None, local_vars_configuration=None):  # noqa: E501
-        """TagUpdateRequestModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, members=None, local_vars_configuration=None):  # noqa: E501
+        """PolicyModel - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._add = None
-        self._remove = None
+        self._name = None
+        self._members = None
         self.discriminator = None
 
-        if add is not None:
-            self.add = add
-        if remove is not None:
-            self.remove = remove
+        if name is not None:
+            self.name = name
+        if members is not None:
+            self.members = members
 
     @property
-    def add(self):
-        """Gets the add of this TagUpdateRequestModel.  # noqa: E501
+    def name(self):
+        """Gets the name of this PolicyModel.  # noqa: E501
 
-        Tags to add to the resource.  User-inputted tags will be stripped of leading and trailing whitespace, filtered of empty elements, and deduplicated.  Adding tags already present on the resource will have no effect.   # noqa: E501
 
-        :return: The add of this TagUpdateRequestModel.  # noqa: E501
-        :rtype: list[str]
+        :return: The name of this PolicyModel.  # noqa: E501
+        :rtype: str
         """
-        return self._add
+        return self._name
 
-    @add.setter
-    def add(self, add):
-        """Sets the add of this TagUpdateRequestModel.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this PolicyModel.
 
-        Tags to add to the resource.  User-inputted tags will be stripped of leading and trailing whitespace, filtered of empty elements, and deduplicated.  Adding tags already present on the resource will have no effect.   # noqa: E501
 
-        :param add: The add of this TagUpdateRequestModel.  # noqa: E501
-        :type: list[str]
+        :param name: The name of this PolicyModel.  # noqa: E501
+        :type: str
         """
 
-        self._add = add
+        self._name = name
 
     @property
-    def remove(self):
-        """Gets the remove of this TagUpdateRequestModel.  # noqa: E501
+    def members(self):
+        """Gets the members of this PolicyModel.  # noqa: E501
 
-        Tags to remove from the resource.  User-inputted tags will be stripped of leading and trailing whitespace, filtered of empty elements, and deduplicated.  Removing tags not present on the resource will have no effect.   # noqa: E501
 
-        :return: The remove of this TagUpdateRequestModel.  # noqa: E501
+        :return: The members of this PolicyModel.  # noqa: E501
         :rtype: list[str]
         """
-        return self._remove
+        return self._members
 
-    @remove.setter
-    def remove(self, remove):
-        """Sets the remove of this TagUpdateRequestModel.
+    @members.setter
+    def members(self, members):
+        """Sets the members of this PolicyModel.
 
-        Tags to remove from the resource.  User-inputted tags will be stripped of leading and trailing whitespace, filtered of empty elements, and deduplicated.  Removing tags not present on the resource will have no effect.   # noqa: E501
 
-        :param remove: The remove of this TagUpdateRequestModel.  # noqa: E501
+        :param members: The members of this PolicyModel.  # noqa: E501
         :type: list[str]
         """
 
-        self._remove = remove
+        self._members = members
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -133,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TagUpdateRequestModel):
+        if not isinstance(other, PolicyModel):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TagUpdateRequestModel):
+        if not isinstance(other, PolicyModel):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-1.64.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,64 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class TransactionCloseModel(object):
+class BulkLoadFileState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    SUCCEEDED = "succeeded"
+    FAILED = "failed"
+    NOT_TRIED = "not_tried"
+    RUNNING = "running"
+
+    allowable_values = [SUCCEEDED, FAILED, NOT_TRIED, RUNNING]  # noqa: E501
+
+    """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'mode': 'str'
     }
 
     attribute_map = {
-        'mode': 'mode'
     }
 
-    def __init__(self, mode=None, local_vars_configuration=None):  # noqa: E501
-        """TransactionCloseModel - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, local_vars_configuration=None):  # noqa: E501
+        """BulkLoadFileState - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
-
-        self._mode = None
         self.discriminator = None
 
-        if mode is not None:
-            self.mode = mode
-
-    @property
-    def mode(self):
-        """Gets the mode of this TransactionCloseModel.  # noqa: E501
-
-
-        :return: The mode of this TransactionCloseModel.  # noqa: E501
-        :rtype: str
-        """
-        return self._mode
-
-    @mode.setter
-    def mode(self, mode):
-        """Sets the mode of this TransactionCloseModel.
-
-
-        :param mode: The mode of this TransactionCloseModel.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["commit", "rollback"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and mode not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `mode` ({0}), must be one of {1}"  # noqa: E501
-                .format(mode, allowed_values)
-            )
-
-        self._mode = mode
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -109,18 +85,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TransactionCloseModel):
+        if not isinstance(other, BulkLoadFileState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TransactionCloseModel):
+        if not isinstance(other, BulkLoadFileState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-1.477.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-1.64.0/data_repo_client/models/upgrade_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `data-repo-client-1.477.0/setup.py` & `data-repo-client-1.64.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,12 @@
-# coding: utf-8
-
-"""
-    Data Repository API
-
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
-
-    The version of the OpenAPI document: 0.1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from setuptools import setup, find_packages  # noqa: H301
-
-NAME = "data-repo-client"
-VERSION = "1.477.0"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Data Repository API",
-    author="OpenAPI Generator community",
-    author_email="team@openapitools.org",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Data Repository API"],
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    license="Apache 2.0",
-    long_description="""\
-    &lt;details&gt;&lt;summary&gt;This document defines the REST API for the Terra Data Repository.&lt;/summary&gt; &lt;p&gt; **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. &lt;p&gt; **Notes on Naming** &lt;p&gt; All of the reference items are suffixed with \\\&quot;Model\\\&quot;. Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. &lt;/details&gt;   # noqa: E501
-    """
-)
+Metadata-Version: 1.0
+Name: data-repo-client
+Version: 1.64.0
+Summary: Data Repository API
+Home-page: UNKNOWN
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
+License: Apache 2.0
+Description:     This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \&quot;Model\&quot;. Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: &#x60;&#x60;&#x60; docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor &#x60;&#x60;&#x60; Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with &#39;DRS&#39; to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
+            
+Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
+Platform: UNKNOWN
```

### Comparing `data-repo-client-1.477.0/test/test_bulk_load_file_model.py` & `data-repo-client-1.64.0/test/test_bulk_load_file_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -35,16 +35,15 @@
             optional params are included """
         # model = data_repo_client.models.bulk_load_file_model.BulkLoadFileModel()  # noqa: E501
         if include_optional :
             return BulkLoadFileModel(
                 source_path = '0', 
                 target_path = '0', 
                 mime_type = '0', 
-                description = '0', 
-                md5 = '0'
+                description = '0'
             )
         else :
             return BulkLoadFileModel(
                 source_path = '0',
                 target_path = '0',
         )
```

### Comparing `data-repo-client-1.477.0/test/test_dataset_model.py` & `data-repo-client-1.64.0/test/test_dataset_request_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.dataset_model import DatasetModel  # noqa: E501
+from data_repo_client.models.dataset_request_model import DatasetRequestModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestDatasetModel(unittest.TestCase):
-    """DatasetModel unit test stubs"""
+class TestDatasetRequestModel(unittest.TestCase):
+    """DatasetRequestModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DatasetModel
+        """Test DatasetRequestModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.dataset_model.DatasetModel()  # noqa: E501
+        # model = data_repo_client.models.dataset_request_model.DatasetRequestModel()  # noqa: E501
         if include_optional :
-            return DatasetModel(
-                id = '0', 
+            return DatasetRequestModel(
                 name = 'a', 
                 description = '0', 
-                default_profile_id = '0', 
-                data_project = '0', 
-                default_snapshot_id = '0', 
+                default_profile_id = 'a', 
                 schema = data_repo_client.models.dataset_specification_model.DatasetSpecificationModel(
                     tables = [
                         data_repo_client.models.table_model.TableModel(
                             name = 'a', 
                             columns = [
                                 data_repo_client.models.column_model.ColumnModel(
                                     name = 'a', 
-                                    datatype = 'string', 
-                                    array_of = True, 
-                                    required = True, )
+                                    datatype = '0', 
+                                    array_of = True, )
                                 ], 
                             primary_key = [
                                 'a'
                                 ], 
                             partition_mode = 'none', 
                             date_partition_options = data_repo_client.models.date_partition_options_model.DatePartitionOptionsModel(
                                 column = 'a', ), 
@@ -87,64 +83,72 @@
                                         ], )
                                 ], 
                             root_table = 'a', 
                             root_column = 'a', 
                             follow = [
                                 'a'
                                 ], )
-                        ], ), 
-                created_date = '0', 
-                storage = [
-                    data_repo_client.models.storage_resource_model.StorageResourceModel(
-                        region = '0', 
-                        cloud_resource = '0', 
-                        cloud_platform = 'gcp', )
-                    ], 
-                secure_monitoring_enabled = True, 
-                phs_id = 'phs123456', 
-                access_information = data_repo_client.models.access_info_model.AccessInfoModel(
-                    big_query = data_repo_client.models.access_info_big_query_model.AccessInfoBigQueryModel(
-                        dataset_name = '0', 
-                        dataset_id = '0', 
-                        project_id = '0', 
-                        link = '0', 
-                        tables = [
-                            data_repo_client.models.access_info_big_query_model_table.AccessInfoBigQueryModelTable(
-                                name = '0', 
-                                id = '0', 
-                                qualified_name = '0', 
-                                link = '0', 
-                                sample_query = '0', )
-                            ], ), 
-                    parquet = data_repo_client.models.access_info_parquet_model.AccessInfoParquetModel(
-                        dataset_name = '0', 
-                        dataset_id = '0', 
-                        storage_account_id = '0', 
-                        url = '0', 
-                        sas_token = '0', 
-                        tables = [
-                            data_repo_client.models.access_info_parquet_model_table.AccessInfoParquetModelTable(
-                                name = '0', 
-                                url = '0', 
-                                sas_token = '0', )
-                            ], ), ), 
-                cloud_platform = 'gcp', 
-                self_hosted = True, 
-                properties = None, 
-                ingest_service_account = '0', 
-                predictable_file_ids = True, 
-                tags = [
-                    'a-resource-tag'
-                    ]
+                        ], )
             )
         else :
-            return DatasetModel(
+            return DatasetRequestModel(
+                name = 'a',
+                default_profile_id = 'a',
+                schema = data_repo_client.models.dataset_specification_model.DatasetSpecificationModel(
+                    tables = [
+                        data_repo_client.models.table_model.TableModel(
+                            name = 'a', 
+                            columns = [
+                                data_repo_client.models.column_model.ColumnModel(
+                                    name = 'a', 
+                                    datatype = '0', 
+                                    array_of = True, )
+                                ], 
+                            primary_key = [
+                                'a'
+                                ], 
+                            partition_mode = 'none', 
+                            date_partition_options = data_repo_client.models.date_partition_options_model.DatePartitionOptionsModel(
+                                column = 'a', ), 
+                            int_partition_options = data_repo_client.models.int_partition_options_model.IntPartitionOptionsModel(
+                                column = 'a', 
+                                min = 56, 
+                                max = 56, 
+                                interval = 56, ), 
+                            row_count = 56, )
+                        ], 
+                    relationships = [
+                        data_repo_client.models.relationship_model.RelationshipModel(
+                            name = '0', 
+                            from = data_repo_client.models.relationship_term_model.RelationshipTermModel(
+                                table = 'a', 
+                                column = 'a', ), 
+                            to = data_repo_client.models.relationship_term_model.RelationshipTermModel(
+                                table = 'a', 
+                                column = 'a', ), )
+                        ], 
+                    assets = [
+                        data_repo_client.models.asset_model.AssetModel(
+                            name = '0', 
+                            tables = [
+                                data_repo_client.models.asset_table_model.AssetTableModel(
+                                    name = 'a', 
+                                    columns = [
+                                        'a'
+                                        ], )
+                                ], 
+                            root_table = 'a', 
+                            root_column = 'a', 
+                            follow = [
+                                'a'
+                                ], )
+                        ], ),
         )
 
-    def testDatasetModel(self):
-        """Test DatasetModel"""
+    def testDatasetRequestModel(self):
+        """Test DatasetRequestModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_dataset_schema_update_model.py` & `data-repo-client-1.64.0/test/test_snapshot_request_row_id_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,71 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.dataset_schema_update_model import DatasetSchemaUpdateModel  # noqa: E501
+from data_repo_client.models.snapshot_request_row_id_model import SnapshotRequestRowIdModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestDatasetSchemaUpdateModel(unittest.TestCase):
-    """DatasetSchemaUpdateModel unit test stubs"""
+class TestSnapshotRequestRowIdModel(unittest.TestCase):
+    """SnapshotRequestRowIdModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DatasetSchemaUpdateModel
+        """Test SnapshotRequestRowIdModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.dataset_schema_update_model.DatasetSchemaUpdateModel()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel()  # noqa: E501
         if include_optional :
-            return DatasetSchemaUpdateModel(
-                description = '0', 
-                changes = data_repo_client.models.dataset_schema_update_model_changes.DatasetSchemaUpdateModel_changes(
-                    add_tables = [
-                        data_repo_client.models.table_model.TableModel(
-                            name = 'a', 
-                            columns = [
-                                data_repo_client.models.column_model.ColumnModel(
-                                    name = 'a', 
-                                    datatype = 'string', 
-                                    array_of = True, 
-                                    required = True, )
-                                ], 
-                            primary_key = [
-                                'a'
-                                ], 
-                            partition_mode = 'none', 
-                            date_partition_options = data_repo_client.models.date_partition_options_model.DatePartitionOptionsModel(
-                                column = 'a', ), 
-                            int_partition_options = data_repo_client.models.int_partition_options_model.IntPartitionOptionsModel(
-                                column = 'a', 
-                                min = 56, 
-                                max = 56, 
-                                interval = 56, ), 
-                            row_count = 56, )
-                        ], 
-                    add_columns = [
-                        data_repo_client.models.dataset_schema_column_update_model.DatasetSchemaColumnUpdateModel(
-                            table_name = '0', )
-                        ], 
-                    add_relationships = [
-                        data_repo_client.models.relationship_model.RelationshipModel(
-                            name = '0', 
-                            from = data_repo_client.models.relationship_term_model.RelationshipTermModel(
-                                table = 'a', 
-                                column = 'a', ), 
-                            to = data_repo_client.models.relationship_term_model.RelationshipTermModel(
-                                table = 'a', 
-                                column = 'a', ), )
-                        ], )
+            return SnapshotRequestRowIdModel(
+                tables = [
+                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                        table_name = 'a', 
+                        columns = [
+                            'a'
+                            ], 
+                        row_ids = [
+                            'a'
+                            ], )
+                    ]
             )
         else :
-            return DatasetSchemaUpdateModel(
+            return SnapshotRequestRowIdModel(
+                tables = [
+                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
+                        table_name = 'a', 
+                        columns = [
+                            'a'
+                            ], 
+                        row_ids = [
+                            'a'
+                            ], )
+                    ],
         )
 
-    def testDatasetSchemaUpdateModel(self):
-        """Test DatasetSchemaUpdateModel"""
+    def testSnapshotRequestRowIdModel(self):
+        """Test SnapshotRequestRowIdModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_drs_checksum.py` & `data-repo-client-1.64.0/test/test_drs_checksum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `data-repo-client-1.477.0/test/test_drs_object.py` & `data-repo-client-1.64.0/test/test_file_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,92 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.drs_object import DRSObject  # noqa: E501
+from data_repo_client.models.file_model import FileModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestDRSObject(unittest.TestCase):
-    """DRSObject unit test stubs"""
+class TestFileModel(unittest.TestCase):
+    """FileModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DRSObject
+        """Test FileModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.drs_object.DRSObject()  # noqa: E501
+        # model = data_repo_client.models.file_model.FileModel()  # noqa: E501
         if include_optional :
-            return DRSObject(
-                id = '0', 
-                name = '0', 
-                self_uri = 'drs://drs.example.org/314159', 
+            return FileModel(
+                file_id = '0', 
+                collection_id = '0', 
+                path = '0', 
                 size = 56, 
-                created_time = '0', 
-                updated_time = '0', 
-                version = '0', 
-                mime_type = 'application/json', 
                 checksums = [
                     data_repo_client.models.drs_checksum.DRSChecksum(
                         checksum = '0', 
                         type = '0', )
                     ], 
-                access_methods = [
-                    data_repo_client.models.drs_access_method.DRSAccessMethod(
-                        type = 's3', 
-                        access_url = data_repo_client.models.drs_access_url.DRSAccessURL(
-                            url = '0', 
-                            headers = {"Authorization":"Basic Z2E0Z2g6ZHJz"}, ), 
-                        access_id = '0', 
-                        region = 'us-east-1', 
-                        authorizations = data_repo_client.models.drs_authorizations.DRSAuthorizations(
-                            supported_types = [
-                                'None'
-                                ], 
-                            passport_auth_issuers = [
-                                '0'
-                                ], 
-                            bearer_auth_issuers = [
-                                '0'
-                                ], ), )
-                    ], 
-                contents = [
-                    data_repo_client.models.drs_contents_object.DRSContentsObject(
-                        name = '0', 
-                        id = '0', 
-                        drs_uri = drs://example.com/ga4gh/drs/v1/objects/{object_id}, 
-                        contents = [
-                            data_repo_client.models.drs_contents_object.DRSContentsObject(
-                                name = '0', 
-                                id = '0', 
-                                drs_uri = drs://example.com/ga4gh/drs/v1/objects/{object_id}, )
-                            ], )
-                    ], 
+                created = '0', 
                 description = '0', 
-                aliases = [
-                    '0'
-                    ]
+                file_type = 'file', 
+                file_detail = data_repo_client.models.file_detail_model.FileDetailModel(
+                    dataset_id = '0', 
+                    mime_type = '0', 
+                    access_url = '0', 
+                    load_tag = '0', ), 
+                directory_detail = data_repo_client.models.directory_detail_model.DirectoryDetailModel(
+                    enumerated = True, 
+                    contents = [
+                        data_repo_client.models.file_model.FileModel(
+                            file_id = '0', 
+                            collection_id = '0', 
+                            path = '0', 
+                            size = 56, 
+                            checksums = [
+                                data_repo_client.models.drs_checksum.DRSChecksum(
+                                    checksum = '0', 
+                                    type = '0', )
+                                ], 
+                            created = '0', 
+                            description = '0', 
+                            file_type = 'file', 
+                            file_detail = data_repo_client.models.file_detail_model.FileDetailModel(
+                                dataset_id = '0', 
+                                mime_type = '0', 
+                                access_url = '0', 
+                                load_tag = '0', ), 
+                            directory_detail = data_repo_client.models.directory_detail_model.DirectoryDetailModel(
+                                enumerated = True, ), )
+                        ], )
             )
         else :
-            return DRSObject(
-                id = '0',
-                self_uri = 'drs://drs.example.org/314159',
-                size = 56,
-                checksums = [
-                    data_repo_client.models.drs_checksum.DRSChecksum(
-                        checksum = '0', 
-                        type = '0', )
-                    ],
+            return FileModel(
         )
 
-    def testDRSObject(self):
-        """Test DRSObject"""
+    def testFileModel(self):
+        """Test FileModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_enumerate_dataset_model.py` & `data-repo-client-1.64.0/test/test_relationship_term_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,55 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.enumerate_dataset_model import EnumerateDatasetModel  # noqa: E501
+from data_repo_client.models.relationship_term_model import RelationshipTermModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestEnumerateDatasetModel(unittest.TestCase):
-    """EnumerateDatasetModel unit test stubs"""
+class TestRelationshipTermModel(unittest.TestCase):
+    """RelationshipTermModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test EnumerateDatasetModel
+        """Test RelationshipTermModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.enumerate_dataset_model.EnumerateDatasetModel()  # noqa: E501
+        # model = data_repo_client.models.relationship_term_model.RelationshipTermModel()  # noqa: E501
         if include_optional :
-            return EnumerateDatasetModel(
-                total = 56, 
-                filtered_total = 56, 
-                items = [
-                    data_repo_client.models.dataset_summary_model.DatasetSummaryModel(
-                        id = '0', 
-                        name = 'a', 
-                        description = '0', 
-                        default_profile_id = '0', 
-                        created_date = '0', 
-                        storage = [
-                            data_repo_client.models.storage_resource_model.StorageResourceModel(
-                                region = '0', 
-                                cloud_resource = '0', 
-                                cloud_platform = 'gcp', )
-                            ], 
-                        secure_monitoring_enabled = True, 
-                        cloud_platform = 'gcp', 
-                        data_project = '0', 
-                        storage_account = '0', 
-                        phs_id = 'phs123456', 
-                        self_hosted = True, 
-                        predictable_file_ids = True, 
-                        tags = [
-                            'a-resource-tag'
-                            ], )
-                    ], 
-                role_map = {
-                    'key' : [
-                        '0'
-                        ]
-                    }
+            return RelationshipTermModel(
+                table = 'a', 
+                column = 'a'
             )
         else :
-            return EnumerateDatasetModel(
+            return RelationshipTermModel(
+                table = 'a',
+                column = 'a',
         )
 
-    def testEnumerateDatasetModel(self):
-        """Test EnumerateDatasetModel"""
+    def testRelationshipTermModel(self):
+        """Test RelationshipTermModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-1.64.0/test/test_snapshot_request_query_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,55 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.enumerate_snapshot_model import EnumerateSnapshotModel  # noqa: E501
+from data_repo_client.models.snapshot_request_query_model import SnapshotRequestQueryModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestEnumerateSnapshotModel(unittest.TestCase):
-    """EnumerateSnapshotModel unit test stubs"""
+class TestSnapshotRequestQueryModel(unittest.TestCase):
+    """SnapshotRequestQueryModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test EnumerateSnapshotModel
+        """Test SnapshotRequestQueryModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.enumerate_snapshot_model.EnumerateSnapshotModel()  # noqa: E501
+        # model = data_repo_client.models.snapshot_request_query_model.SnapshotRequestQueryModel()  # noqa: E501
         if include_optional :
-            return EnumerateSnapshotModel(
-                total = 56, 
-                filtered_total = 56, 
-                items = [
-                    data_repo_client.models.snapshot_summary_model.SnapshotSummaryModel(
-                        id = '0', 
-                        name = 'a', 
-                        description = '0', 
-                        created_date = '0', 
-                        profile_id = '0', 
-                        storage = [
-                            data_repo_client.models.storage_resource_model.StorageResourceModel(
-                                region = '0', 
-                                cloud_resource = '0', 
-                                cloud_platform = 'gcp', )
-                            ], 
-                        secure_monitoring_enabled = True, 
-                        consent_code = '0', 
-                        phs_id = 'phs123456', 
-                        cloud_platform = 'gcp', 
-                        data_project = '0', 
-                        storage_account = '0', 
-                        self_hosted = True, 
-                        global_file_ids = True, 
-                        tags = [
-                            'a-resource-tag'
-                            ], )
-                    ], 
-                role_map = {
-                    'key' : [
-                        '0'
-                        ]
-                    }, 
-                errors = [
-                    data_repo_client.models.error_model.ErrorModel(
-                        message = '0', 
-                        error_detail = [
-                            '0'
-                            ], )
-                    ]
+            return SnapshotRequestQueryModel(
+                asset_name = 'a', 
+                query = '0'
             )
         else :
-            return EnumerateSnapshotModel(
+            return SnapshotRequestQueryModel(
+                asset_name = 'a',
+                query = '0',
         )
 
-    def testEnumerateSnapshotModel(self):
-        """Test EnumerateSnapshotModel"""
+    def testSnapshotRequestQueryModel(self):
+        """Test SnapshotRequestQueryModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_job_model.py` & `data-repo-client-1.64.0/test/test_upgrade_response_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,54 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.job_model import JobModel  # noqa: E501
+from data_repo_client.models.upgrade_response_model import UpgradeResponseModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestJobModel(unittest.TestCase):
-    """JobModel unit test stubs"""
+class TestUpgradeResponseModel(unittest.TestCase):
+    """UpgradeResponseModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test JobModel
+        """Test UpgradeResponseModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.job_model.JobModel()  # noqa: E501
+        # model = data_repo_client.models.upgrade_response_model.UpgradeResponseModel()  # noqa: E501
         if include_optional :
-            return JobModel(
-                id = 'a', 
-                description = '0', 
-                job_status = 'running', 
-                status_code = 56, 
-                submitted = '0', 
-                completed = '0', 
-                class_name = '0'
+            return UpgradeResponseModel(
+                upgrade_name = '0', 
+                start_time = '0', 
+                end_time = '0'
             )
         else :
-            return JobModel(
-                id = 'a',
-                job_status = 'running',
-                status_code = 56,
+            return UpgradeResponseModel(
         )
 
-    def testJobModel(self):
-        """Test JobModel"""
+    def testUpgradeResponseModel(self):
+        """Test UpgradeResponseModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_policy_response.py` & `data-repo-client-1.64.0/test/test_delete_response_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,52 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.policy_response import PolicyResponse  # noqa: E501
+from data_repo_client.models.delete_response_model import DeleteResponseModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestPolicyResponse(unittest.TestCase):
-    """PolicyResponse unit test stubs"""
+class TestDeleteResponseModel(unittest.TestCase):
+    """DeleteResponseModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PolicyResponse
+        """Test DeleteResponseModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.policy_response.PolicyResponse()  # noqa: E501
+        # model = data_repo_client.models.delete_response_model.DeleteResponseModel()  # noqa: E501
         if include_optional :
-            return PolicyResponse(
-                policies = [
-                    data_repo_client.models.policy_model.PolicyModel(
-                        name = '0', 
-                        members = [
-                            '0'
-                            ], )
-                    ], 
-                workspaces = [
-                    data_repo_client.models.workspace_policy_model.WorkspacePolicyModel(
-                        workspace_id = '0', 
-                        workspace_name = '0', 
-                        workspace_namespace = '0', 
-                        workspace_link = '0', 
-                        workspace_policies = [
-                            data_repo_client.models.policy_model.PolicyModel(
-                                name = '0', 
-                                members = [
-                                    '0'
-                                    ], )
-                            ], )
-                    ], 
-                inaccessible_workspaces = [
-                    data_repo_client.models.inaccessible_workspace_policy_model.InaccessibleWorkspacePolicyModel(
-                        workspace_id = '0', 
-                        workspace_policies = [
-                            data_repo_client.models.policy_model.PolicyModel(
-                                name = '0', 
-                                members = [
-                                    '0'
-                                    ], )
-                            ], 
-                        error = data_repo_client.models.error_model.ErrorModel(
-                            message = '0', 
-                            error_detail = [
-                                '0'
-                                ], ), )
-                    ]
+            return DeleteResponseModel(
+                object_state = 'deleted'
             )
         else :
-            return PolicyResponse(
+            return DeleteResponseModel(
         )
 
-    def testPolicyResponse(self):
-        """Test PolicyResponse"""
+    def testDeleteResponseModel(self):
+        """Test DeleteResponseModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-1.64.0/test/test_unauthenticated_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,51 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
-import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_request_row_id_model import SnapshotRequestRowIdModel  # noqa: E501
+from data_repo_client.api.unauthenticated_api import UnauthenticatedApi  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotRequestRowIdModel(unittest.TestCase):
-    """SnapshotRequestRowIdModel unit test stubs"""
+
+class TestUnauthenticatedApi(unittest.TestCase):
+    """UnauthenticatedApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = data_repo_client.api.unauthenticated_api.UnauthenticatedApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test SnapshotRequestRowIdModel
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = data_repo_client.models.snapshot_request_row_id_model.SnapshotRequestRowIdModel()  # noqa: E501
-        if include_optional :
-            return SnapshotRequestRowIdModel(
-                tables = [
-                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
-                        table_name = 'a', 
-                        columns = [
-                            'a'
-                            ], 
-                        row_ids = [
-                            '0'
-                            ], )
-                    ]
-            )
-        else :
-            return SnapshotRequestRowIdModel(
-                tables = [
-                    data_repo_client.models.snapshot_request_row_id_table_model.SnapshotRequestRowIdTableModel(
-                        table_name = 'a', 
-                        columns = [
-                            'a'
-                            ], 
-                        row_ids = [
-                            '0'
-                            ], )
-                    ],
-        )
-
-    def testSnapshotRequestRowIdModel(self):
-        """Test SnapshotRequestRowIdModel"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+    def test_retrieve_repository_config(self):
+        """Test case for retrieve_repository_config
+
+        """
+        pass
+
+    def test_service_status(self):
+        """Test case for service_status
+
+        """
+        pass
+
+    def test_shutdown_request(self):
+        """Test case for shutdown_request
+
+        """
+        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_snapshot_source_model.py` & `data-repo-client-1.64.0/test/test_bulk_load_history_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,60 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_source_model import SnapshotSourceModel  # noqa: E501
+from data_repo_client.models.bulk_load_history_model import BulkLoadHistoryModel  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotSourceModel(unittest.TestCase):
-    """SnapshotSourceModel unit test stubs"""
+class TestBulkLoadHistoryModel(unittest.TestCase):
+    """BulkLoadHistoryModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotSourceModel
+        """Test BulkLoadHistoryModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_source_model.SnapshotSourceModel()  # noqa: E501
+        # model = data_repo_client.models.bulk_load_history_model.BulkLoadHistoryModel()  # noqa: E501
         if include_optional :
-            return SnapshotSourceModel(
-                dataset = data_repo_client.models.dataset_summary_model.DatasetSummaryModel(
-                    id = '0', 
-                    name = 'a', 
-                    description = '0', 
-                    default_profile_id = '0', 
-                    created_date = '0', 
-                    storage = [
-                        data_repo_client.models.storage_resource_model.StorageResourceModel(
-                            region = '0', 
-                            cloud_resource = '0', 
-                            cloud_platform = 'gcp', )
-                        ], 
-                    secure_monitoring_enabled = True, 
-                    cloud_platform = 'gcp', 
-                    data_project = '0', 
-                    storage_account = '0', 
-                    phs_id = 'phs123456', 
-                    self_hosted = True, 
-                    predictable_file_ids = True, 
-                    tags = [
-                        'a-resource-tag'
-                        ], ), 
-                dataset_properties = data_repo_client.models.dataset_properties.datasetProperties(), 
-                asset = 'a'
+            return BulkLoadHistoryModel(
+                source_path = '0', 
+                target_path = '0', 
+                state = 'succeeded', 
+                file_id = '0', 
+                checksum_crc = '0', 
+                checksum_md5 = '0', 
+                error = '0'
             )
         else :
-            return SnapshotSourceModel(
-                dataset = data_repo_client.models.dataset_summary_model.DatasetSummaryModel(
-                    id = '0', 
-                    name = 'a', 
-                    description = '0', 
-                    default_profile_id = '0', 
-                    created_date = '0', 
-                    storage = [
-                        data_repo_client.models.storage_resource_model.StorageResourceModel(
-                            region = '0', 
-                            cloud_resource = '0', 
-                            cloud_platform = 'gcp', )
-                        ], 
-                    secure_monitoring_enabled = True, 
-                    cloud_platform = 'gcp', 
-                    data_project = '0', 
-                    storage_account = '0', 
-                    phs_id = 'phs123456', 
-                    self_hosted = True, 
-                    predictable_file_ids = True, 
-                    tags = [
-                        'a-resource-tag'
-                        ], ),
+            return BulkLoadHistoryModel(
+                source_path = '0',
+                target_path = '0',
         )
 
-    def testSnapshotSourceModel(self):
-        """Test SnapshotSourceModel"""
+    def testBulkLoadHistoryModel(self):
+        """Test BulkLoadHistoryModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-1.477.0/test/test_table_model.py` & `data-repo-client-1.64.0/test/test_table_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Data Repository API
 
-    <details><summary>This document defines the REST API for the Terra Data Repository.</summary> <p> **Status: design in progress** There are a few top-level endpoints (besides some used by swagger):  * / - generated by swagger: swagger API page that provides this documentation and a live UI for submitting REST requests  * /status - provides the operational status of the service  * /configuration - provides the basic configuration and information about the service  * /api - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>   # noqa: E501
+    This document defines the REST API for Data Repository. **Status: design in progress** There are four top-level endpoints (besides some used by swagger):  * /swagger-ui.html - generated by swagger: swagger API page that provides this documentation and a live UI for      submitting REST requests  * /status - provides the operational status of the service  * /api    - is the authenticated and authorized Data Repository API  * /ga4gh/drs/v1 - is a transcription of the Data Repository Service API  The overall API (/api) currently supports two interfaces:  * Repository - a general and default interface for initial setup, managing ingest and repository metadata  * Resource - an interface for managing billing accounts and resources  The API endpoints are organized by interface. Each interface is separately versioned. ## Notes on Naming All of the reference items are suffixed with \"Model\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. ## Editing and debugging I have found it best to edit this file directly to make changes and then use the swagger-editor to validate. The errors out of swagger-codegen are not that helpful. In the swagger-editor, it gives you nice errors and links to the place in the YAML where the errors are. But... the swagger-editor has been a bit of a pain for me to run. I tried the online website and was not able to load my YAML. Instead, I run it locally in a docker container, like this: ``` docker pull swaggerapi/swagger-editor docker run -p 9090:8080 swaggerapi/swagger-editor ``` Then navigate to localhost:9090 in your browser. I have not been able to get the file upload to work. It is a bit of a PITA, but I copy-paste the source code, replacing what is in the editor. Then make any fixes. Then copy-paste the resulting, valid file back into our source code. Not elegant, but easier than playing detective with the swagger-codegen errors. This might be something about my browser or environment, so give it a try yourself and see how it goes. ## Merging the DRS standard swagger into this swagger ## The merging is done in three sections:  1. Merging the security definitions into our security definitions  2. This section of paths. We make all paths explicit (prefixed with /ga4gh/drs/v1)     All standard DRS definitions and parameters are prefixed with 'DRS' to separate them     from our native definitions and parameters. We remove the x-swagger-router-controller lines.  3. A separate part of the definitions section for the DRS definitions  NOTE: the code here does not relect the DRS spec anymore. See DR-409.   # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -36,17 +36,16 @@
         # model = data_repo_client.models.table_model.TableModel()  # noqa: E501
         if include_optional :
             return TableModel(
                 name = 'a', 
                 columns = [
                     data_repo_client.models.column_model.ColumnModel(
                         name = 'a', 
-                        datatype = 'string', 
-                        array_of = True, 
-                        required = True, )
+                        datatype = '0', 
+                        array_of = True, )
                     ], 
                 primary_key = [
                     'a'
                     ], 
                 partition_mode = 'none', 
                 date_partition_options = data_repo_client.models.date_partition_options_model.DatePartitionOptionsModel(
                     column = 'a', ), 
@@ -59,17 +58,16 @@
             )
         else :
             return TableModel(
                 name = 'a',
                 columns = [
                     data_repo_client.models.column_model.ColumnModel(
                         name = 'a', 
-                        datatype = 'string', 
-                        array_of = True, 
-                        required = True, )
+                        datatype = '0', 
+                        array_of = True, )
                     ],
         )
 
     def testTableModel(self):
         """Test TableModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

