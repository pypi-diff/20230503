# Comparing `tmp/groupdocs-comparison-cloud-22.4.tar.gz` & `tmp/groupdocs-comparison-cloud-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-comparison-cloud-22.4.tar", last modified: Thu Apr 14 09:37:58 2022, max compression
+gzip compressed data, was "dist\groupdocs-comparison-cloud-23.4.tar", last modified: Wed May  3 07:49:14 2023, max compression
```

## Comparing `groupdocs-comparison-cloud-22.4.tar` & `groupdocs-comparison-cloud-23.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:58.000000 groupdocs-comparison-cloud-22.4/
--rw-rw-rw-   0        0        0     1105 2022-04-14 09:33:07.000000 groupdocs-comparison-cloud-22.4/LICENSE
--rw-rw-rw-   0        0        0     2937 2022-04-14 09:37:58.000000 groupdocs-comparison-cloud-22.4/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2022-04-14 09:33:07.000000 groupdocs-comparison-cloud-22.4/README.md
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/
--rw-rw-rw-   0        0        0     3186 2022-04-14 09:33:08.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/__init__.py
--rw-rw-rw-   0        0        0    26237 2022-04-14 09:33:08.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2022-04-14 09:33:08.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/
--rw-rw-rw-   0        0        0      535 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    19935 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/compare_api.py
--rw-rw-rw-   0        0        0    38688 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36298 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    11937 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6622 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0    14230 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/review_api.py
--rw-rw-rw-   0        0        0    26610 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3307 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/auth.py
--rw-rw-rw-   0        0        0     7681 2022-04-14 09:33:09.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/
--rw-rw-rw-   0        0        0     2187 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     7881 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/apply_revisions_options.py
--rw-rw-rw-   0        0        0    11825 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/change_info.py
--rw-rw-rw-   0        0        0     8297 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/comparison_options.py
--rw-rw-rw-   0        0        0     5129 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     5386 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/diagram_master_setting.py
--rw-rw-rw-   0        0        0     5187 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     6291 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6424 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5413 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     4900 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/format.py
--rw-rw-rw-   0        0        0     4186 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     6442 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/info_result.py
--rw-rw-rw-   0        0        0    10585 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/items_style.py
--rw-rw-rw-   0        0        0     7524 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/link.py
--rw-rw-rw-   0        0        0     5637 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/metadata.py
--rw-rw-rw-   0        0        0     5178 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     5843 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/page_info.py
--rw-rw-rw-   0        0        0     6281 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/rectangle.py
--rw-rw-rw-   0        0        0     8209 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/revision_info.py
--rw-rw-rw-   0        0        0    29908 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/settings.py
--rw-rw-rw-   0        0        0     4933 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/size.py
--rw-rw-rw-   0        0        0     4276 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     5881 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/style_change_info.py
--rw-rw-rw-   0        0        0     4591 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/updates_options.py
--rw-rw-rw-   0        0        0    13739 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/
--rw-rw-rw-   0        0        0     2937 2022-04-14 09:37:47.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2748 2022-04-14 09:37:49.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-14 09:37:47.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-04-14 09:37:48.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-04-14 09:37:48.000000 groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-14 09:37:58.000000 groupdocs-comparison-cloud-22.4/setup.cfg
--rw-rw-rw-   0        0        0     1699 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/test/
--rw-rw-rw-   0        0        0        0 2022-04-14 09:33:10.000000 groupdocs-comparison-cloud-22.4/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-14 09:37:57.000000 groupdocs-comparison-cloud-22.4/test/apis/
--rw-rw-rw-   0        0        0        0 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3005 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     7479 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_comparison_changes.py
--rw-rw-rw-   0        0        0     8212 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_comparison_updates.py
--rw-rw-rw-   0        0        0     7721 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_comparisons.py
--rw-rw-rw-   0        0        0     3795 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3148 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     2755 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_info_api.py
--rw-rw-rw-   0        0        0     3308 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_review_api.py
--rw-rw-rw-   0        0        0     2728 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     4904 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/test_context.py
--rw-rw-rw-   0        0        0     6593 2022-04-14 09:33:11.000000 groupdocs-comparison-cloud-22.4/test/test_file.py
--rw-rw-rw-   0        0        0     1702 2022-04-14 09:33:18.000000 groupdocs-comparison-cloud-22.4/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/
+-rw-rw-rw-   0        0        0     1105 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/LICENSE
+-rw-rw-rw-   0        0        0     2898 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/
+-rw-rw-rw-   0        0        0     3186 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26237 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/
+-rw-rw-rw-   0        0        0      535 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    19935 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/compare_api.py
+-rw-rw-rw-   0        0        0    38688 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36298 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    11937 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6622 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0    14230 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/review_api.py
+-rw-rw-rw-   0        0        0    26610 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3307 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/auth.py
+-rw-rw-rw-   0        0        0     7681 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/
+-rw-rw-rw-   0        0        0     2187 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     7881 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/apply_revisions_options.py
+-rw-rw-rw-   0        0        0    11825 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/change_info.py
+-rw-rw-rw-   0        0        0     8297 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/comparison_options.py
+-rw-rw-rw-   0        0        0     5129 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     5386 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/diagram_master_setting.py
+-rw-rw-rw-   0        0        0     5187 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     6291 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6424 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5413 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     4900 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4186 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     6442 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0    10585 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/items_style.py
+-rw-rw-rw-   0        0        0     7524 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/link.py
+-rw-rw-rw-   0        0        0     5637 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/metadata.py
+-rw-rw-rw-   0        0        0     5178 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     5843 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/page_info.py
+-rw-rw-rw-   0        0        0     6281 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/rectangle.py
+-rw-rw-rw-   0        0        0     8209 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/revision_info.py
+-rw-rw-rw-   0        0        0    29908 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/settings.py
+-rw-rw-rw-   0        0        0     4933 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/size.py
+-rw-rw-rw-   0        0        0     4276 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     5881 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/style_change_info.py
+-rw-rw-rw-   0        0        0     4591 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/updates_options.py
+-rw-rw-rw-   0        0        0    13739 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2898 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2748 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/setup.cfg
+-rw-rw-rw-   0        0        0     1699 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/test/
+-rw-rw-rw-   0        0        0        0 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:49:14.000000 groupdocs-comparison-cloud-23.4/test/apis/
+-rw-rw-rw-   0        0        0        0 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     7479 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_comparison_changes.py
+-rw-rw-rw-   0        0        0     8212 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_comparison_updates.py
+-rw-rw-rw-   0        0        0     7721 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_comparisons.py
+-rw-rw-rw-   0        0        0     3795 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3148 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     2755 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_info_api.py
+-rw-rw-rw-   0        0        0     3308 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_review_api.py
+-rw-rw-rw-   0        0        0     2728 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     4904 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/test_context.py
+-rw-rw-rw-   0        0        0     6593 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/test_file.py
+-rw-rw-rw-   0        0        0     1702 2023-05-03 07:48:51.000000 groupdocs-comparison-cloud-23.4/test/test_settings.py
```

### Comparing `groupdocs-comparison-cloud-22.4/LICENSE` & `groupdocs-comparison-cloud-23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/PKG-INFO` & `groupdocs-comparison-cloud-23.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-comparison-cloud
-Version: 22.4
+Version: 23.4
 Summary: GroupDocs.Comparison Cloud Python SDK
 Home-page: http://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,comparison,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -75,8 +73,7 @@
 + [**Product Home**](https://products.groupdocs.cloud/comparison)
 + [**Documentation**](https://docs.groupdocs.cloud/comparison)
 + [**Free Support Forum**](https://forum.groupdocs.cloud/c/comparison)
 + [**Blog**](https://blog.groupdocs.cloud/category/comparison)
 
 ## Contact Us
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/comparison).
-
```

### Comparing `groupdocs-comparison-cloud-22.4/README.md` & `groupdocs-comparison-cloud-23.4/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/__init__.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/api_client.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_client.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '22.4'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.4'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.4'
+        self.user_agent = 'python sdk 23.4'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/api_exception.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/api_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_exception.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/__init__.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/compare_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/compare_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -362,15 +362,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparisons_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -398,15 +398,15 @@
     def __init__(self, comparison_options):
         """Initializes new instance of ComparisonsRequest."""  # noqa: E501
         self.comparison_options = comparison_options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="post_changes_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -434,15 +434,15 @@
     def __init__(self, comparison_options):
         """Initializes new instance of PostChangesRequest."""  # noqa: E501
         self.comparison_options = comparison_options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="put_changes_document_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/file_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/file_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -634,15 +634,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -678,15 +678,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -718,15 +718,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="download_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -758,15 +758,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -802,15 +802,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="upload_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/folder_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -610,15 +610,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
         self.dest_path = dest_path
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -690,15 +690,15 @@
         """Initializes new instance of CreateFolderRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -730,15 +730,15 @@
         self.path = path
         self.storage_name = storage_name
         self.recursive = recursive
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_files_list_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -768,15 +768,15 @@
         """Initializes new instance of GetFilesListRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/info_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/info_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -265,15 +265,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_document_info_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/license_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/license_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/review_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/review_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -271,15 +271,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="apply_revisions_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -307,15 +307,15 @@
     def __init__(self, revision_options):
         """Initializes new instance of ApplyRevisionsRequest."""  # noqa: E501
         self.revision_options = revision_options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_revisions_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/apis/storage_api.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/apis/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="comparison_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -471,15 +471,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_disc_usage_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -507,15 +507,15 @@
     def __init__(self, storage_name=None):
         """Initializes new instance of GetDiscUsageRequest."""  # noqa: E501
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_file_versions_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -545,15 +545,15 @@
         """Initializes new instance of GetFileVersionsRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="object_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -585,15 +585,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="storage_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/auth.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="auth.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/configuration.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="configuration.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 22.4\n"\
-               "SDK Package Version: 22.4".\
+               "Version of the API: 23.4\n"\
+               "SDK Package Version: 23.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/__init__.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/apply_revisions_options.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/apply_revisions_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ApplyRevisionsOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/change_info.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/change_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ChangeInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/comparison_options.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/comparison_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ComparisonOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/consumption_result.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/consumption_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ConsumptionResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/diagram_master_setting.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/diagram_master_setting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiagramMasterSetting.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/disc_usage.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/disc_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiscUsage.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/error.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Error.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/error_details.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ErrorDetails.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_info.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_version.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersion.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/file_versions.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/file_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/files_list.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/files_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesList.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/files_upload_result.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesUploadResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/format.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Format.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/formats_result.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/formats_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormatsResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/info_result.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/info_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/items_style.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/items_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ItemsStyle.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/link.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Link.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/metadata.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Metadata.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/object_exist.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/object_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ObjectExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/page_info.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/page_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/rectangle.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/rectangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Rectangle.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/revision_info.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/revision_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="RevisionInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/settings.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Settings.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/size.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/size.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Size.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/storage_exist.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/storage_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/storage_file.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/storage_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageFile.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/style_change_info.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/style_change_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StyleChangeInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/models/updates_options.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/models/updates_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="UpdatesOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud/rest.py` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="rest.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/PKG-INFO` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-comparison-cloud
-Version: 22.4
+Version: 23.4
 Summary: GroupDocs.Comparison Cloud Python SDK
 Home-page: http://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,comparison,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -75,8 +73,7 @@
 + [**Product Home**](https://products.groupdocs.cloud/comparison)
 + [**Documentation**](https://docs.groupdocs.cloud/comparison)
 + [**Free Support Forum**](https://forum.groupdocs.cloud/c/comparison)
 + [**Blog**](https://blog.groupdocs.cloud/category/comparison)
 
 ## Contact Us
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/comparison).
-
```

### Comparing `groupdocs-comparison-cloud-22.4/groupdocs_comparison_cloud.egg-info/SOURCES.txt` & `groupdocs-comparison-cloud-23.4/groupdocs_comparison_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupdocs-comparison-cloud-22.4/setup.py` & `groupdocs-comparison-cloud-23.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-comparison-cloud"
-VERSION = "22.4"
+VERSION = "23.4"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_auth_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_auth_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_comparison_changes.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_comparison_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -50,15 +50,15 @@
         options = self.GetComparisonOptions(TestFiles.SourceEmail, TestFiles.TargetEmail)
         response = self.compare_api.post_changes(PostChangesRequest(options))
         self.assertEqual(len(response), 4)   
 
     def test_changes_html(self):
         options = self.GetComparisonOptions(TestFiles.SourceHtml, TestFiles.TargetHtml)
         response = self.compare_api.post_changes(PostChangesRequest(options))
-        self.assertEqual(len(response), 3)   
+        self.assertEqual(len(response), 2)   
 
     def test_changes_image(self):
         options = self.GetComparisonOptions(TestFiles.SourceImage, TestFiles.TargetImage)
         response = self.compare_api.post_changes(PostChangesRequest(options))
         self.assertEqual(len(response), 170)   
 
     def test_changes_note(self):
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_comparison_updates.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_comparison_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_comparisons.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_comparisons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_file_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_folder_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_info_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_info_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_review_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_review_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/apis/test_storage_api.py` & `groupdocs-comparison-cloud-23.4/test/apis/test_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/test_context.py` & `groupdocs-comparison-cloud-23.4/test/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/test_file.py` & `groupdocs-comparison-cloud-23.4/test/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_file.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-comparison-cloud-22.4/test/test_settings.py` & `groupdocs-comparison-cloud-23.4/test/test_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

