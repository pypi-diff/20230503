# Comparing `tmp/folio_migration_tools-1.8.0rc6.tar.gz` & `tmp/folio_migration_tools-1.8.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folio_migration_tools-1.8.0rc6.tar", max compression
+gzip compressed data, was "folio_migration_tools-1.8.0rc7.tar", max compression
```

## Comparing `folio_migration_tools-1.8.0rc6.tar` & `folio_migration_tools-1.8.0rc7.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc6/LICENSE
--rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc6/README.md
--rw-r--r--   0        0        0     1748 2023-04-27 20:24:24.872553 folio_migration_tools-1.8.0rc6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/__init__.py
--rw-r--r--   0        0        0     5322 2023-04-20 15:39:37.839264 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/__main__.py
--rw-r--r--   0        0        0    14007 2023-04-27 12:57:47.732920 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/circulation_helper.py
--rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/colors.py
--rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/custom_dict.py
--rw-r--r--   0        0        0     2374 2023-03-06 22:17:01.811751 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/custom_exceptions.py
--rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/extradata_writer.py
--rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/folder_structure.py
--rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/helper.py
--rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/holdings_helper.py
--rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/library_configuration.py
--rw-r--r--   0        0        0    19528 2023-03-27 22:22:56.113076 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapper_base.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/__init__.py
--rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
--rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
--rw-r--r--   0        0        0    10081 2023-04-19 02:19:29.618543 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
--rw-r--r--   0        0        0    37072 2023-04-19 02:19:29.621237 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
--rw-r--r--   0        0        0     3548 2023-03-24 03:05:35.503768 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
--rw-r--r--   0        0        0    14848 2023-04-19 02:22:09.374729 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
--rw-r--r--   0        0        0    14644 2023-04-19 02:22:09.385428 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
--rw-r--r--   0        0        0     8795 2023-03-06 22:17:01.816049 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
--rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/__init__.py
--rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/conditions.py
--rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
--rw-r--r--   0        0        0     9386 2023-04-19 02:22:09.393982 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
--rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
--rw-r--r--   0        0        0    10697 2023-04-23 08:03:03.483979 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
--rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
--rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
--rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
--rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
--rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
--rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_report.py
--rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/authority_transformer.py
--rw-r--r--   0        0        0    28016 2023-04-21 02:52:45.466270 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/batch_poster.py
--rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/bibs_transformer.py
--rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/courses_migrator.py
--rw-r--r--   0        0        0    19445 2023-04-25 22:44:23.946627 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
--rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
--rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/items_transformer.py
--rw-r--r--   0        0        0    32162 2023-04-19 02:22:09.411635 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/loans_migrator.py
--rw-r--r--   0        0        0    13305 2023-04-27 20:24:01.776339 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/migration_task_base.py
--rw-r--r--   0        0        0    10831 2023-04-27 19:32:26.629411 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/orders_transformer.py
--rw-r--r--   0        0        0    14387 2023-03-06 22:17:01.823616 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/organization_transformer.py
--rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/requests_migrator.py
--rw-r--r--   0        0        0     8868 2023-04-19 02:22:09.418100 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/reserves_migrator.py
--rw-r--r--   0        0        0     9305 2023-03-06 22:17:01.824396 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/user_transformer.py
--rw-r--r--   0        0        0    15521 2023-04-19 02:19:29.646947 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/report_blurbs.py
--rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/task_configuration.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/test_infrastructure/__init__.py
--rw-r--r--   0        0        0     5289 2023-03-24 03:05:35.516008 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/test_infrastructure/mocked_classes.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/__init__.py
--rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_loan.py
--rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_request.py
--rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_reserve.py
--rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/transaction_result.py
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc6/setup.py
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc7/LICENSE
+-rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc7/README.md
+-rw-r--r--   0        0        0     1748 2023-05-03 20:30:40.284410 folio_migration_tools-1.8.0rc7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__init__.py
+-rw-r--r--   0        0        0     5322 2023-05-03 19:02:35.338530 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__main__.py
+-rw-r--r--   0        0        0    14007 2023-05-03 19:02:35.494096 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/circulation_helper.py
+-rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/colors.py
+-rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_dict.py
+-rw-r--r--   0        0        0     2374 2023-03-06 22:17:01.811751 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_exceptions.py
+-rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/extradata_writer.py
+-rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/folder_structure.py
+-rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/helper.py
+-rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/holdings_helper.py
+-rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/library_configuration.py
+-rw-r--r--   0        0        0    19528 2023-03-27 22:22:56.113076 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapper_base.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/__init__.py
+-rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
+-rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
+-rw-r--r--   0        0        0    10080 2023-05-03 19:02:35.234989 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
+-rw-r--r--   0        0        0    10431 2023-05-03 19:02:35.235966 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
+-rw-r--r--   0        0        0    37072 2023-04-19 02:19:29.621237 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
+-rw-r--r--   0        0        0     3548 2023-03-24 03:05:35.503768 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
+-rw-r--r--   0        0        0    14849 2023-05-03 19:02:35.300564 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
+-rw-r--r--   0        0        0    14644 2023-05-03 19:02:35.319735 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
+-rw-r--r--   0        0        0     8855 2023-05-03 19:02:35.238368 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
+-rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/__init__.py
+-rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/conditions.py
+-rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
+-rw-r--r--   0        0        0     9386 2023-05-03 19:02:35.301485 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
+-rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
+-rw-r--r--   0        0        0    10697 2023-05-03 19:02:35.467697 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
+-rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
+-rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
+-rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
+-rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
+-rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
+-rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_report.py
+-rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/authority_transformer.py
+-rw-r--r--   0        0        0    28090 2023-05-03 19:02:35.447257 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/batch_poster.py
+-rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/bibs_transformer.py
+-rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/courses_migrator.py
+-rw-r--r--   0        0        0    19445 2023-05-03 19:02:35.480285 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
+-rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
+-rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/items_transformer.py
+-rw-r--r--   0        0        0    32162 2023-05-03 19:02:35.303753 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/loans_migrator.py
+-rw-r--r--   0        0        0     7846 2023-05-03 19:02:35.242340 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
+-rw-r--r--   0        0        0    13319 2023-05-03 19:02:35.242626 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/migration_task_base.py
+-rw-r--r--   0        0        0    10831 2023-04-30 20:40:23.950774 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/orders_transformer.py
+-rw-r--r--   0        0        0    14387 2023-03-06 22:17:01.823616 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/organization_transformer.py
+-rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/requests_migrator.py
+-rw-r--r--   0        0        0     8868 2023-05-03 19:02:35.304239 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/reserves_migrator.py
+-rw-r--r--   0        0        0     9305 2023-03-06 22:17:01.824396 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/user_transformer.py
+-rw-r--r--   0        0        0    15870 2023-05-03 19:02:35.243912 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/report_blurbs.py
+-rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/task_configuration.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/__init__.py
+-rw-r--r--   0        0        0     8199 2023-05-03 19:02:35.244774 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/mocked_classes.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/__init__.py
+-rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_loan.py
+-rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_request.py
+-rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_reserve.py
+-rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/transaction_result.py
+-rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc7/setup.py
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc7/PKG-INFO
```

### Comparing `folio_migration_tools-1.8.0rc6/LICENSE` & `folio_migration_tools-1.8.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/README.md` & `folio_migration_tools-1.8.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/pyproject.toml` & `folio_migration_tools-1.8.0rc7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folio_migration_tools"
-version = "1.8.0rc6"
+version = "1.8.0rc7"
 description =  "A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP"
 authors = ["Theodor Tolstoy <github.teddes@tolstoy.se>", "Lisa Sjögren", "Brooks Travis"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/FOLIO-FSE/folio_migration_tools"
 repository = "https://github.com/FOLIO-FSE/folio_migration_tools"
 keywords = ["FOLIO", "ILS", "LSP", "Library Systems", "MARC21", "Library data"]
@@ -33,15 +33,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 folioclient = "^0.50.0rc1"
 pyhumps = "^3.7.3"
 defusedxml = "^0.7.1"
 python-dateutil = "^2.8.2"
-folio-uuid = "^0.2.7"
+folio-uuid = "^0.2.8"
 pymarc = "^4.2.1"
 pydantic = "^1.10.2"
 argparse-prompt = "^0.0.5"
 deepdiff = "^6.2.3"
 pyaml = "^21.10.1"
 httpx = "^0.23.3"
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/__main__.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/circulation_helper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/circulation_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/custom_dict.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_dict.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/custom_exceptions.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/extradata_writer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/extradata_writer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/folder_structure.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/folder_structure.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/helper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/holdings_helper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/holdings_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/library_configuration.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/library_configuration.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapper_base.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/item_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/item_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             else:
                 self.status_mapping = {
                     v["legacy_code"]: v["folio_name"] for v in item_statuses_map
                 }
         logging.info(json.dumps(statuses, indent=True))
 
     def get_prop(self, legacy_item, folio_prop_name, index_or_id, schema_default_value):
-
         if folio_prop_name == "permanentLocationId":
             return self.get_mapped_ref_data_value(
                 self.location_mapping,
                 legacy_item,
                 folio_prop_name,
                 index_or_id,
                 False,
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/order_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/order_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         if folio_prop_name.endswith(".locationId"):
             return self.get_mapped_ref_data_value(
                 self.location_mapping,
                 legacy_order,
                 folio_prop_name,
                 index_or_id,
-                True,
+                False,
             )
 
         if folio_prop_name == "vendor":
             if mapped_value in self.vendor_code_map:
                 self.migration_report.add_general_statistics(
                     "Successfully matched Vendor against code"
                 )
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,9 +211,11 @@
         not in [
             "folio_group",
             "folio_code",
             "folio_id",
             "folio_name",
             "legacy_code",
             "folio_value",
+            "folio_owner",
+            "folio_feeFineType",
         ]
     ]
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/mapping_file_transformation/user_mapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/mapping_file_transformation/user_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/conditions.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/conditions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_report.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_report.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/authority_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/authority_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/batch_poster.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/batch_poster.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,16 @@
         "succeedingTitles": "preceding-succeeding-titles",
         "boundwithPart": "inventory-storage/bound-with-parts",
         "notes": "notes",
         "course": "coursereserves/courses",
         "courselisting": "coursereserves/courselistings",
         "contacts": "organizations-storage/contacts",
         "interfaces": "organizations-storage/interfaces",
+        "account": "accounts",
+        "feefineaction": "feefineactions",
     }
     if object_name == "instructor":
         instructor = json.loads(string_object)
         return f'coursereserves/courselistings/{instructor["courseListingId"]}/instructors'
 
     if object_name == "interfaceCredential":
         credential = json.loads(string_object)
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/bibs_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/bibs_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/courses_migrator.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/courses_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/items_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/items_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/loans_migrator.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/loans_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/migration_task_base.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/migration_task_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,21 +211,21 @@
         data_issue_file_handler.setLevel(26)
         logging.getLogger().addHandler(data_issue_file_handler)
         logger.info("Logging set up")
 
     def setup_records_map(self, mapping_file_path):
         with open(mapping_file_path) as mapping_file:
             field_map = json.load(mapping_file)
-            logging.info("%s fields in mapping file map", len(field_map["data"]))
+            logging.info("%s fields present in record mapping file", len(field_map["data"]))
             mapped_fields = (
                 f
                 for f in field_map["data"]
                 if f["legacy_field"] and f["legacy_field"] != "Not mapped"
             )
-            logging.info("%s Mapped fields in mapping file map", len(list(mapped_fields)))
+            logging.info("%s fields mapped in record mapping file", len(list(mapped_fields)))
             return field_map
 
     def log_and_exit_if_too_many_errors(self, error: TransformationRecordFailedError, idx):
         self.num_exeptions += 1
         error.log_it()
         if self.num_exeptions / (1 + idx) > 0.2 and self.num_exeptions > 5000:
             logging.fatal(
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/orders_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/orders_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/organization_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/organization_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/requests_migrator.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/requests_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/reserves_migrator.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/reserves_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/migration_tasks/user_transformer.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/migration_tasks/user_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/report_blurbs.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/report_blurbs.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,20 @@
         "Interfaces with malformed URIs will not be migrated. See data issues log.\nFOLIO Interface URIs must start with one of the following: 'ftp://', 'sftp://', 'http://', 'https://'.",
     )
     FieldMappingDetails = ("Mapping details", "")
     CatalogingAgency = ("Cataloging sources", "")
     Trivia = ("Trivia", "")
     LeaderManipulation = ("Leader manipulation", "")
     TermsMapping = ("Terms Mapping", "Reference data mapping for Terms.")
+    FeeFineOnwerMapping = ("Fee/Fine Owner mapping", "Reference data mapping for Fee/Fine owners.")
+    FeeFineTypesMapping = ("Fee/Fine Type mapping", "Reference data mapping for Fee/Fine types.")
+    FeeFineServicePointTypesMapping = (
+        "Fee/Fine Service Point mapping",
+        "Reference data mapping for Fee/Fine service points.",
+    )
     CategoriesMapping = (
         "Organization contact categories",
         "Reference data mapping for contacts, addresses, emails, and phones numbers.",
     )
     OrganizationTypeMapping = (
         "Organization types",
         "Reference data mapping for Organization types.",
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/test_infrastructure/mocked_classes.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/test_infrastructure/mocked_classes.py`

 * *Files 25% similar despite different names*

```diff
@@ -106,16 +106,98 @@
             },
             {
                 "id": "2f452d21-507d-4b32-a89d-8ea9753cc946",
                 "name": "FOLIO fallback user department name",
                 "code": "fb",
             },
         ]
+    elif ref_data_path == "/owners":
+        yield from [
+            {
+                "owner": "The Best Fee Fine Owner",
+                "desc": "She really is!",
+                "servicePointOwner": [
+                    {"value": "a77b55e7-f9f3-40a1-83e0-241bc606a826", "label": "lisatest"}
+                ],
+                "id": "5abfff3f-50eb-432a-9a43-21f8f7a70194",
+            },
+            {
+                "owner": "The Other Fee Fine Owner",
+                "desc": "heeey",
+                "servicePointOwner": [
+                    {"value": "1543c345-dcaf-4367-84a8-853d95837a3b", "label": "lisatest2 :) <3 "}
+                ],
+                "id": "62a0eb54-de96-46ee-b184-5be6c8114a19",
+            },
+        ]
+    elif ref_data_path == "/feefines":
+        yield from [
+            {
+                "automatic": False,
+                "feeFineType": "Coffee spill",
+                "ownerId": "5abfff3f-50eb-432a-9a43-21f8f7a70194",
+                "id": "6e8dc178-f667-45cd-90b5-338c78c3a85c",
+            },
+            {
+                "automatic": False,
+                "feeFineType": "Coffee spill",
+                "ownerId": "62a0eb54-de96-46ee-b184-5be6c8114a19",
+                "id": "031836ec-521a-4493-9f76-0e02c2e7d241",
+            },
+            {
+                "automatic": False,
+                "feeFineType": "Replacement library card",
+                "ownerId": "5abfff3f-50eb-432a-9a43-21f8f7a70194",
+                "id": "8936606d-223b-428e-9a70-4b8105f60cdb",
+            },
+            {
+                "automatic": True,
+                "feeFineType": "Replacement processing fee",
+                "id": "d20df2fb-45fd-4184-b238-0d25747ffdd9",
+            },
+        ]
+
+    elif ref_data_path == "/service-points":
+        yield from [
+            {
+                "id": "finance_office_uuid",
+                "name": "Finance Office",
+                "code": "fo",
+            },
+            {
+                "id": "library_main_desk_uuid",
+                "name": "Library Main Desk",
+                "code": "lmd",
+            },
+        ]
+
     elif ref_data_path == "/users" and query == '?query=(externalSystemId=="Some external id")':
         yield from [{"id": "some id", "barcode": "some barcode", "patronGroup": "some group"}]
+
+    elif ref_data_path == "/users" and query == '?query=(barcode=="some barcode")':
+        yield from [{"id": "a FOLIO user uuid"}]
+
+    elif ref_data_path == "/inventory/items" and query == '?query=(barcode=="some barcode")':
+        yield from [
+            {
+                "id": "a FOLIO item uuid",
+                "title": "Döda fallen i Avesta.",
+                "barcode": "some barcode",
+                "callNumber": "QB611 .C44",
+                "materialType": {
+                    "id": "4eea3f27-8910-46fc-9666-e2b44326c2b8",
+                    "name": "sound recording",
+                },
+                "effectiveLocation": {
+                    "id": "2e48e713-17f3-4c13-a9f8-23845bb210a4",
+                    "name": "Reading room",
+                },
+            }
+        ]
+
     elif ref_data_path in super_schema:
         yield from super_schema.get(ref_data_path)
     else:
         yield {}
 
 
 def folio_get_single_object_mocked(*args, **kwargs):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_loan.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_loan.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_request.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_request.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/legacy_reserve.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/legacy_reserve.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/src/folio_migration_tools/transaction_migration/transaction_result.py` & `folio_migration_tools-1.8.0rc7/src/folio_migration_tools/transaction_migration/transaction_result.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.8.0rc6/setup.py` & `folio_migration_tools-1.8.0rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['argparse-prompt>=0.0.5,<0.0.6',
  'deepdiff>=6.2.3,<7.0.0',
  'defusedxml>=0.7.1,<0.8.0',
- 'folio-uuid>=0.2.7,<0.3.0',
+ 'folio-uuid>=0.2.8,<0.3.0',
  'folioclient>=0.50.0rc1,<0.51.0',
  'httpx>=0.23.3,<0.24.0',
  'pyaml>=21.10.1,<22.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pyhumps>=3.7.3,<4.0.0',
  'pymarc>=4.2.1,<5.0.0',
  'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'folio-migration-tools',
-    'version': '1.8.0rc6',
+    'version': '1.8.0rc7',
     'description': 'A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP',
     'long_description': '# FOLIO Migration Tools\n![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)\n\nA toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)\n\n# What is it good for?\nFOLIO Migration tools enables you to migrate libraries with the most common ILS:s over to FOLIO without data losses or any major data transformation tasks. \nThe tools transforms and loads the data providing you and the library with good actionable logs and data cleaning task lists together with the migrated data.\n\n## What data does it cover?\nFOLIO Migration Tools currently covers the following data sets:\n* Catalog (Inventory and SRS in FOLIO terminology)\n* Circulation transactions (Open loans and requests)\n* Users/Patrons (In FOLIO, these share the same app/database)\n* Courses and Reserves (Course reserves)\n* Organizations (Vendor records)\n* Orders (limited support)\n\n### What additional functionality is on the roadmap?\nThis is the loose roadmap, in order of most likely implementations first\n* ERM-related objects\n* Financial records\n\n### Can I use the tools for ongoing imports and integrations?\nThe tools are primarliy maintained for performing initial data migrations. We recommend that you use native FOLIO functionality for ongoing loads where possible. \nIn theory, these tools can be used for ongoing patron loads from systems like Banner, Workday, or PeopleSoft. But we recommend you to weigh your options carefully before going down this path. \n\n# Contributing\nWant to contribute? Read the [CONTRIBUTING.MD](https://github.com/FOLIO-FSE/folio_migration_tools/blob/main/CONTRIBUTING.md)\n\n# Found an issue?\nReport it on the [Github Issue tracker](https://github.com/FOLIO-FSE/folio_migration_tools/issues)\n\nThe scripts requires a FOLIO tenant with reference data properly set up. The script will throw messages telling what reference data is missing.\n# Installing\nMake sure you are running Python 3.9 or above. \n## 1. Using pip and venv\n### 2.1. Create and activate a [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)   \n```   \npython -m venv ./.venv     # Creates a virtual env in the current folder\nsource .venv/bin/activate  # Activates the venv    \n```\n### 2. Install using pip: \n```\npython -m pip install folio_migration_tools\n```\n### 3. Test the installation by showing the help pages \n```   \npython -m folio_migration_tools -h\n```    \n\n## 2. Using pipenv\n### 1. Run\n```   \npipenv install folio-migration-tools\n```   \n### 2. Test the installation by showing the help pages\n```  \npipenv run python3 -m folio_migration_tools -h\n```  \n\n# FOLIO migration process\nThis repo plays the main part in a process using a collection of tools. The process itself is documented in more detail, including example configuration files, at [this template repository](https://github.com/FOLIO-FSE/migration_repo_template)\nIn order to perform migrations according to this process, you need the following:\n* An Installation of [FOLIO Migration Tools](https://pypi.org/project/folio-migration-tools/). Installation instructions above.\n* A clone, or a separate repo created from [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)\n* Access to the [Data mapping file creator](https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation) web tool\n* A FOLIO tenant running the latest or the second latest version of FOLIO\n\n\n\n# Running the scripts\nFor information on syntax, what files are needed and produced by the toolkit, refer to the documentation and example files in the [template repository](https://github.com/FOLIO-FSE/migration_repo_template). We are building out the docs section in this repository as well:[Documentation](https://folio-migration-tools.readthedocs.io/en/latest/)\n¨\n',
     'author': 'Theodor Tolstoy',
     'author_email': 'github.teddes@tolstoy.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FOLIO-FSE/folio_migration_tools',
```

### Comparing `folio_migration_tools-1.8.0rc6/PKG-INFO` & `folio_migration_tools-1.8.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folio-migration-tools
-Version: 1.8.0rc6
+Version: 1.8.0rc7
 Summary: A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP
 Home-page: https://github.com/FOLIO-FSE/folio_migration_tools
 License: MIT
 Keywords: FOLIO,ILS,LSP,Library Systems,MARC21,Library data
 Author: Theodor Tolstoy
 Author-email: github.teddes@tolstoy.se
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: argparse-prompt (>=0.0.5,<0.0.6)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: folio-uuid (>=0.2.7,<0.3.0)
+Requires-Dist: folio-uuid (>=0.2.8,<0.3.0)
 Requires-Dist: folioclient (>=0.50.0rc1,<0.51.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: pyaml (>=21.10.1,<22.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.3,<4.0.0)
 Requires-Dist: pymarc (>=4.2.1,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

