# Comparing `tmp/macrobond-data-api-1.0.2.tar.gz` & `tmp/macrobond-data-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-e8gool95/macrobond-data-api-1.0.2.tar", last modified: Fri Apr 28 15:31:06 2023, max compression
+gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-3jiozy2n/macrobond-data-api-1.0.3.tar", last modified: Wed May  3 06:24:18 2023, max compression
```

## Comparing `macrobond-data-api-1.0.2.tar` & `macrobond-data-api-1.0.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_error_message_to_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_fill_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_fix_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_weekdays.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/_parse_iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/values_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/save_credential_to_keyring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_subscription_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_pacakge_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_error_message_to_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_fill_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/_fix_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_weekdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/_parse_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/util/save_credential_to_keyring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_subscription_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_pacakge_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-03 06:24:18.000000 macrobond-data-api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-03 06:22:25.000000 macrobond-data-api-1.0.3/setup.py
```

### Comparing `macrobond-data-api-1.0.2/LICENSE` & `macrobond-data-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/PKG-INFO` & `macrobond-data-api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.2 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.3 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.2/README.md` & `macrobond-data-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/__init__.py` & `macrobond-data-api-1.0.3/macrobond_data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/_generated.py` & `macrobond-data-api-1.0.3/macrobond_data_api/_generated.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/_get_api.py` & `macrobond-data-api-1.0.3/macrobond_data_api/_get_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/_com_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/_fill_metadata.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/_fill_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_api.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_client.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/connection.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-1.0.3/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/api.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/client.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/__init__.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/metadata_attribute_type.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/metadata_attribute_type.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/_parse_iso8601.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/_parse_iso8601.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_entity_error.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/get_entity_error.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/revision_info.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/search_result_long.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_observation_history.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/unified_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/common/types/vintage_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/util/save_credential_to_keyring.py` & `macrobond-data-api-1.0.3/macrobond_data_api/util/save_credential_to_keyring.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_subscription_list_poller.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_subscription_list_poller.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_web_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/_web_only_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     # pylint: enable=line-too-long
     params = {}
     body: Optional[DataPackageBody] = None
 
     if if_modified_since:
         params["ifModifiedSince"] = if_modified_since.isoformat()
 
-    with self._session.get("v1/series/getsubscriptionlist", params=params, stream=True) as response:
+    with self._session.get("v1/series/datapackagelist", params=params, stream=True) as response:
         _raise_on_error(response)
         ijson_parse = ijson.parse(response.raw)
 
         (
             time_stamp_for_if_modified_since,
             download_full_list_on_or_after,
             state,
```

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/session.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/session.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/subscription_list.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/subscription_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_api.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_client.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_body.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_body.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list_state.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/data_package_list_state.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/search_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,15 +258,15 @@
             params={
                 "n": series_name,
                 "t": [x.isoformat() for x in date_of_the_observation],
             },
         )
         return cast(List["SeriesObservationHistoryResponse"], response.json())
 
-    # Get /v1/series/getsubscriptionlist
+    # Get /v1/series/getdatapackagelist
     def get_data_package_list(self, if_modified_since: datetime = None) -> "FeedEntitiesResponse":
         """
         Get a list of entities in the subscription list and timestamps when they were last changed.
         You can specify a timestamp to see what has changed since then. For this the
         timeStampForIfModifiedSince in the response from a previous call is typically used.
         This guarantees that you will not miss any updates,
         but you may see the same update more than once.
@@ -281,15 +281,15 @@
             403 The account is not set up to use a subscription list.
         """
         params = {}
 
         if if_modified_since:
             params["ifModifiedSince"] = if_modified_since.isoformat()
 
-        response = self.__session.get_or_raise("v1/series/getsubscriptionlist", params=params)
+        response = self.__session.get_or_raise("v1/series/getdatapackagelist", params=params)
         return cast("FeedEntitiesResponse", response.json())
 
     # Get /v1/series/entityinfofordisplay
     def entity_info_for_display(self, *entitie_names: str) -> "EntityInfoForDisplayResponse":
         """
         Get formatted information about a time series intended to be displayed to the user
```

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/status_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-1.0.3/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-1.0.3/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.2 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.3 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.2/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-1.0.3/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/setup.cfg` & `macrobond-data-api-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.2/setup.py` & `macrobond-data-api-1.0.3/setup.py`

 * *Files identical despite different names*

