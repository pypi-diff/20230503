# Comparing `tmp/castor_extractor-0.3.5.tar.gz` & `tmp/castor_extractor-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor_extractor-0.3.5.tar", max compression
+gzip compressed data, was "castor_extractor-0.3.7.tar", max compression
```

## Comparing `castor_extractor-0.3.5.tar` & `castor_extractor-0.3.7.tar`

### file list

```diff
@@ -1,264 +1,265 @@
--rw-r--r--   0        0        0     4796 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     8254 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/LICENCE
--rw-r--r--   0        0        0     3390 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/__init__.py
--rw-r--r--   0        0        0     1252 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_bigquery.py
--rwxr-xr-x   0        0        0     1075 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_looker.py
--rwxr-xr-x   0        0        0      765 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_metabase_api.py
--rwxr-xr-x   0        0        0     1239 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_metabase_db.py
--rwxr-xr-x   0        0        0      919 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_mode.py
--rw-r--r--   0        0        0     1154 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_postgres.py
--rw-r--r--   0        0        0      850 2023-04-12 12:24:14.840696 castor_extractor-0.3.5/castor_extractor/commands/extract_powerbi.py
--rw-r--r--   0        0        0      989 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/extract_qlik.py
--rwxr-xr-x   0        0        0     1155 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/extract_redshift.py
--rwxr-xr-x   0        0        0     1799 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/extract_snowflake.py
--rwxr-xr-x   0        0        0     1390 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/extract_tableau.py
--rw-r--r--   0        0        0     2667 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/file_check.py
--rwxr-xr-x   0        0        0     1930 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/commands/upload.py
--rw-r--r--   0        0        0      119 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/column.py
--rw-r--r--   0        0        0     1935 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/column_test.py
--rw-r--r--   0        0        0      289 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/constants.py
--rw-r--r--   0        0        0      536 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/enums.py
--rw-r--r--   0        0        0     6547 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/file.py
--rw-r--r--   0        0        0     2105 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/file_test.py
--rw-r--r--   0        0        0      547 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/file_test_users.csv
--rw-r--r--   0        0        0      286 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/file_test_users_valid.csv
--rw-r--r--   0        0        0       60 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/templates/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/file_checker/templates/generic_warehouse.py
--rw-r--r--   0        0        0      886 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/logger.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/transformation/__init__.py
--rw-r--r--   0        0        0       91 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/transformation/dbt/__init__.py
--rw-r--r--   0        0        0       94 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/transformation/dbt/assets.py
--rw-r--r--   0        0        0       86 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/transformation/dbt/client/__init__.py
--rw-r--r--   0        0        0     2938 2023-04-12 12:24:14.841696 castor_extractor-0.3.5/castor_extractor/transformation/dbt/client/client.py
--rw-r--r--   0        0        0      746 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/transformation/dbt/client/credentials.py
--rw-r--r--   0        0        0       75 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/__init__.py
--rw-r--r--   0        0        0      718 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/constant.py
--rw-r--r--   0        0        0      878 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/env.py
--rw-r--r--   0        0        0      472 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/env_test.py
--rw-r--r--   0        0        0     3353 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/upload.py
--rw-r--r--   0        0        0      339 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/upload_test.py
--rw-r--r--   0        0        0      478 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/uploader/utils.py
--rw-r--r--   0        0        0      878 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/__init__.py
--rw-r--r--   0        0        0      417 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/collection.py
--rw-r--r--   0        0        0       39 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/constants.py
--rw-r--r--   0        0        0      608 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/env.py
--rw-r--r--   0        0        0     1545 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/files.py
--rw-r--r--   0        0        0     1514 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/files_test.py
--rw-r--r--   0        0        0     4543 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/formatter.py
--rw-r--r--   0        0        0     3802 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/formatter_test.csv
--rw-r--r--   0        0        0    12527 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/formatter_test.json
--rw-r--r--   0        0        0     1538 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/formatter_test.py
--rw-r--r--   0        0        0      265 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/load.py
--rw-r--r--   0        0        0     1822 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/object.py
--rw-r--r--   0        0        0     2514 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/object_test.py
--rw-r--r--   0        0        0     3894 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/pager.py
--rw-r--r--   0        0        0     3245 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/pager_test.py
--rw-r--r--   0        0        0     2664 2023-04-12 12:24:14.842696 castor_extractor-0.3.5/castor_extractor/utils/retry.py
--rw-r--r--   0        0        0     1635 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/retry_test.py
--rw-r--r--   0        0        0     1966 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/safe.py
--rw-r--r--   0        0        0     2160 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/safe_test.py
--rw-r--r--   0        0        0     2087 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/store.py
--rw-r--r--   0        0        0     1961 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/string.py
--rw-r--r--   0        0        0     2206 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/string_test.py
--rw-r--r--   0        0        0      430 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/time.py
--rw-r--r--   0        0        0      313 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/type.py
--rw-r--r--   0        0        0      150 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/uri.py
--rw-r--r--   0        0        0      259 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/uri_test.py
--rw-r--r--   0        0        0     1904 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/validation.py
--rw-r--r--   0        0        0     1181 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/validation_test.py
--rw-r--r--   0        0        0     2081 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/utils/write.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/__init__.py
--rw-r--r--   0        0        0      191 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/__init__.py
--rw-r--r--   0        0        0      181 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/__init__.py
--rw-r--r--   0        0        0     7137 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/client.py
--rw-r--r--   0        0        0      816 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/client_test.py
--rw-r--r--   0        0        0     3895 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/constants.py
--rw-r--r--   0        0        0     3526 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/sdk.py
--rw-r--r--   0        0        0     1742 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/sdk_test.py
--rw-r--r--   0        0        0     1320 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/api/utils.py
--rw-r--r--   0        0        0      364 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/assets.py
--rw-r--r--   0        0        0      467 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/constant.py
--rw-r--r--   0        0        0      864 2023-04-12 12:24:14.843696 castor_extractor-0.3.5/castor_extractor/visualization/looker/env.py
--rw-r--r--   0        0        0     3514 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/looker/extract.py
--rw-r--r--   0        0        0      636 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/looker/fields.py
--rw-r--r--   0        0        0      782 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/looker/fields_test.py
--rw-r--r--   0        0        0     1527 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/looker/parameters.py
--rw-r--r--   0        0        0      125 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/assets.py
--rw-r--r--   0        0        0       52 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/api/__init__.py
--rw-r--r--   0        0        0     5621 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/api/client.py
--rw-r--r--   0        0        0     1362 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/api/credentials.py
--rw-r--r--   0        0        0       29 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/__init__.py
--rw-r--r--   0        0        0     4103 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/client.py
--rw-r--r--   0        0        0     1891 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/credentials.py
--rw-r--r--   0        0        0       76 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
--rw-r--r--   0        0        0       79 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
--rw-r--r--   0        0        0      419 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/card.sql
--rw-r--r--   0        0        0       42 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/collection.sql
--rw-r--r--   0        0        0      439 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
--rw-r--r--   0        0        0       52 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
--rw-r--r--   0        0        0       49 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/database.sql
--rw-r--r--   0        0        0       46 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/table.sql
--rw-r--r--   0        0        0       41 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/queries/user.sql
--rw-r--r--   0        0        0     1076 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/decryption.py
--rw-r--r--   0        0        0      591 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/decryption_test.py
--rw-r--r--   0        0        0      389 2023-04-12 12:24:14.844696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/shared.py
--rw-r--r--   0        0        0     1006 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/errors.py
--rw-r--r--   0        0        0     1773 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/extract.py
--rw-r--r--   0        0        0       45 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/metabase/types.py
--rw-r--r--   0        0        0      117 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/assets.py
--rw-r--r--   0        0        0       27 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/__init__.py
--rw-r--r--   0        0        0     7803 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client.py
--rw-r--r--   0        0        0     2087 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client_test.json
--rw-r--r--   0        0        0     1400 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client_test.py
--rw-r--r--   0        0        0      453 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/constants.py
--rw-r--r--   0        0        0     1622 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/client/credentials.py
--rw-r--r--   0        0        0     1495 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/errors.py
--rw-r--r--   0        0        0     1559 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/mode/extract.py
--rw-r--r--   0        0        0      106 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/__init__.py
--rw-r--r--   0        0        0      385 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/assets.py
--rw-r--r--   0        0        0       62 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/__init__.py
--rw-r--r--   0        0        0     2088 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/constants.py
--rw-r--r--   0        0        0      482 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/credentials.py
--rw-r--r--   0        0        0     6604 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/rest.py
--rw-r--r--   0        0        0     4709 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/rest_test.py
--rw-r--r--   0        0        0      541 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/utils.py
--rw-r--r--   0        0        0      719 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/utils_test.py
--rw-r--r--   0        0        0     1561 2023-04-12 12:24:14.845696 castor_extractor-0.3.5/castor_extractor/visualization/powerbi/extract.py
--rw-r--r--   0        0        0      143 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/__init__.py
--rw-r--r--   0        0        0     1634 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/assets.py
--rw-r--r--   0        0        0       94 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/__init__.py
--rw-r--r--   0        0        0      786 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/constants.py
--rw-r--r--   0        0        0       36 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/__init__.py
--rw-r--r--   0        0        0     2512 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/client.py
--rw-r--r--   0        0        0      707 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/constants.py
--rw-r--r--   0        0        0     1229 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/error.py
--rw-r--r--   0        0        0     1005 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/error_test.py
--rw-r--r--   0        0        0     1386 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/json_rpc.py
--rw-r--r--   0        0        0     1305 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
--rw-r--r--   0        0        0     2032 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/websocket.py
--rw-r--r--   0        0        0     3209 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/master.py
--rw-r--r--   0        0        0     5966 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/rest.py
--rw-r--r--   0        0        0     1676 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/rest_test.py
--rw-r--r--   0        0        0       95 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/constants.py
--rw-r--r--   0        0        0     2397 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/qlik/extract.py
--rw-r--r--   0        0        0      114 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/tableau/__init__.py
--rw-r--r--   0        0        0      762 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/tableau/assets.py
--rw-r--r--   0        0        0       78 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/__init__.py
--rw-r--r--   0        0        0     6824 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/client.py
--rw-r--r--   0        0        0     2077 2023-04-12 12:24:14.846696 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/client_utils.py
--rw-r--r--   0        0        0     3335 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/credentials.py
--rw-r--r--   0        0        0      803 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/project.py
--rw-r--r--   0        0        0     2036 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/safe_mode.py
--rw-r--r--   0        0        0      126 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/constants.py
--rw-r--r--   0        0        0       91 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/errors.py
--rw-r--r--   0        0        0     2873 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/extract.py
--rw-r--r--   0        0        0     4728 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/gql_fields.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/__init__.py
--rw-r--r--   0        0        0      446 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
--rw-r--r--   0        0        0      447 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
--rw-r--r--   0        0        0      450 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
--rw-r--r--   0        0        0     1018 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
--rw-r--r--   0        0        0      679 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
--rw-r--r--   0        0        0     1415 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
--rw-r--r--   0        0        0     1325 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
--rw-r--r--   0        0        0     1917 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
--rw-r--r--   0        0        0        0 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
--rw-r--r--   0        0        0      422 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
--rw-r--r--   0        0        0     1779 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
--rw-r--r--   0        0        0     1384 2023-04-12 12:24:14.847697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
--rw-r--r--   0        0        0     1499 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
--rw-r--r--   0        0        0     1979 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
--rw-r--r--   0        0        0       26 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
--rw-r--r--   0        0        0      966 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/tsc_fields.py
--rw-r--r--   0        0        0      322 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/types.py
--rw-r--r--   0        0        0      427 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/visualization/tableau/usage.py
--rw-r--r--   0        0        0        1 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/__init__.py
--rw-r--r--   0        0        0      386 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/asset.py
--rw-r--r--   0        0        0     1947 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/client.py
--rw-r--r--   0        0        0     2885 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/extract.py
--rw-r--r--   0        0        0     2640 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/query.py
--rw-r--r--   0        0        0      935 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/time_filter.py
--rw-r--r--   0        0        0      449 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/abstract/time_filter_test.py
--rw-r--r--   0        0        0      125 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/__init__.py
--rw-r--r--   0        0        0     3131 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/client.py
--rw-r--r--   0        0        0     1567 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/client_test.py
--rw-r--r--   0        0        0     2795 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/extract.py
--rw-r--r--   0        0        0       30 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/.sqlfluff
--rw-r--r--   0        0        0     1815 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/column.sql
--rw-r--r--   0        0        0     1347 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
--rw-r--r--   0        0        0      207 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/database.sql
--rw-r--r--   0        0        0      660 2023-04-12 12:24:14.848697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/query.sql
--rw-r--r--   0        0        0      284 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/schema.sql
--rw-r--r--   0        0        0     1508 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/table.sql
--rw-r--r--   0        0        0     2660 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
--rw-r--r--   0        0        0      189 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/user.sql
--rw-r--r--   0        0        0      326 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
--rw-r--r--   0        0        0     4147 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/query.py
--rw-r--r--   0        0        0      140 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/types.py
--rw-r--r--   0        0        0      125 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/__init__.py
--rw-r--r--   0        0        0      871 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/client.py
--rw-r--r--   0        0        0     2099 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/extract.py
--rw-r--r--   0        0        0       30 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/.sqlfluff
--rw-r--r--   0        0        0     1632 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/column.sql
--rw-r--r--   0        0        0      241 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/database.sql
--rw-r--r--   0        0        0      101 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/group.sql
--rw-r--r--   0        0        0      592 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/schema.sql
--rw-r--r--   0        0        0     1489 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/table.sql
--rw-r--r--   0        0        0      170 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/user.sql
--rw-r--r--   0        0        0      540 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/postgres/query.py
--rw-r--r--   0        0        0      125 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/__init__.py
--rw-r--r--   0        0        0      764 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/client.py
--rw-r--r--   0        0        0     1028 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/client_test.py
--rw-r--r--   0        0        0     2238 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/extract.py
--rw-r--r--   0        0        0       30 2023-04-12 12:24:14.849697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/.sqlfluff
--rw-r--r--   0        0        0     7044 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/column.sql
--rw-r--r--   0        0        0      299 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/database.sql
--rw-r--r--   0        0        0      101 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/group.sql
--rw-r--r--   0        0        0     3258 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/query.sql
--rw-r--r--   0        0        0      585 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/schema.sql
--rw-r--r--   0        0        0     2645 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/table.sql
--rw-r--r--   0        0        0      726 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/table_freshness.sql
--rw-r--r--   0        0        0      170 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/user.sql
--rw-r--r--   0        0        0      719 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/view_ddl.sql
--rw-r--r--   0        0        0      540 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/redshift/query.py
--rw-r--r--   0        0        0      128 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/__init__.py
--rw-r--r--   0        0        0     4127 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/client.py
--rw-r--r--   0        0        0     1434 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/client_test.py
--rw-r--r--   0        0        0     2443 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/extract.py
--rw-r--r--   0        0        0       31 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/.sqlfluff
--rw-r--r--   0        0        0     1130 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/column.sql
--rw-r--r--   0        0        0     1179 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
--rw-r--r--   0        0        0      483 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/database.sql
--rw-r--r--   0        0        0      272 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
--rw-r--r--   0        0        0      143 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
--rw-r--r--   0        0        0     1779 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/query.sql
--rw-r--r--   0        0        0       96 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/role.sql
--rw-r--r--   0        0        0      730 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/schema.sql
--rw-r--r--   0        0        0     1378 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/table.sql
--rw-r--r--   0        0        0      570 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/user.sql
--rw-r--r--   0        0        0      673 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
--rw-r--r--   0        0        0     1769 2023-04-12 12:24:14.850697 castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/query.py
--rw-r--r--   0        0        0       36 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/__init__.py
--rw-r--r--   0        0        0      517 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/extract.py
--rw-r--r--   0        0        0       26 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/.sqlfluff
--rw-r--r--   0        0        0     1392 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/column.sql
--rw-r--r--   0        0        0      138 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/database.sql
--rw-r--r--   0        0        0     1110 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/query.sql
--rw-r--r--   0        0        0      250 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/schema.sql
--rw-r--r--   0        0        0     1049 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/table.sql
--rw-r--r--   0        0        0       67 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/user.sql
--rw-r--r--   0        0        0      249 2023-04-12 12:24:14.851697 castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/view_ddl.sql
--rw-r--r--   0        0        0     5142 2023-04-12 12:24:14.852697 castor_extractor-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     9553 1970-01-01 00:00:00.000000 castor_extractor-0.3.5/setup.py
--rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 castor_extractor-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4932 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0     8254 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/LICENCE
+-rw-r--r--   0        0        0     3390 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/__init__.py
+-rw-r--r--   0        0        0     1252 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_bigquery.py
+-rwxr-xr-x   0        0        0     1075 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_looker.py
+-rwxr-xr-x   0        0        0      761 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_metabase_api.py
+-rwxr-xr-x   0        0        0     1235 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_metabase_db.py
+-rwxr-xr-x   0        0        0      919 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_mode.py
+-rw-r--r--   0        0        0     1154 2023-05-03 07:50:11.899867 castor_extractor-0.3.7/castor_extractor/commands/extract_postgres.py
+-rw-r--r--   0        0        0      850 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/extract_powerbi.py
+-rw-r--r--   0        0        0      989 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/extract_qlik.py
+-rwxr-xr-x   0        0        0     1155 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/extract_redshift.py
+-rwxr-xr-x   0        0        0     1799 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/extract_snowflake.py
+-rwxr-xr-x   0        0        0     1390 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/extract_tableau.py
+-rw-r--r--   0        0        0     2667 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/file_check.py
+-rwxr-xr-x   0        0        0     1930 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/commands/upload.py
+-rw-r--r--   0        0        0      119 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/column.py
+-rw-r--r--   0        0        0     1935 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/column_test.py
+-rw-r--r--   0        0        0      289 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/constants.py
+-rw-r--r--   0        0        0      536 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/enums.py
+-rw-r--r--   0        0        0     6537 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/file.py
+-rw-r--r--   0        0        0     2082 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/file_test.py
+-rw-r--r--   0        0        0      547 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/file_test_users.csv
+-rw-r--r--   0        0        0      286 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/file_test_users_valid.csv
+-rw-r--r--   0        0        0       60 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/templates/__init__.py
+-rw-r--r--   0        0        0     2962 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/file_checker/templates/generic_warehouse.py
+-rw-r--r--   0        0        0      886 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/logger.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/transformation/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/transformation/dbt/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/transformation/dbt/assets.py
+-rw-r--r--   0        0        0       86 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/transformation/dbt/client/__init__.py
+-rw-r--r--   0        0        0     2938 2023-05-03 07:50:11.900867 castor_extractor-0.3.7/castor_extractor/transformation/dbt/client/client.py
+-rw-r--r--   0        0        0      746 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/transformation/dbt/client/credentials.py
+-rw-r--r--   0        0        0       75 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/__init__.py
+-rw-r--r--   0        0        0      718 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/constant.py
+-rw-r--r--   0        0        0      878 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/env.py
+-rw-r--r--   0        0        0      472 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/env_test.py
+-rw-r--r--   0        0        0     3353 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/upload.py
+-rw-r--r--   0        0        0      329 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/upload_test.py
+-rw-r--r--   0        0        0      478 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/uploader/utils.py
+-rw-r--r--   0        0        0      918 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/collection.py
+-rw-r--r--   0        0        0       39 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/constants.py
+-rw-r--r--   0        0        0      843 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/deprecate.py
+-rw-r--r--   0        0        0      608 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/env.py
+-rw-r--r--   0        0        0     1545 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/files.py
+-rw-r--r--   0        0        0     1514 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/files_test.py
+-rw-r--r--   0        0        0     4543 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/formatter.py
+-rw-r--r--   0        0        0     3802 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/formatter_test.csv
+-rw-r--r--   0        0        0    12527 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/formatter_test.json
+-rw-r--r--   0        0        0     1543 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/formatter_test.py
+-rw-r--r--   0        0        0      265 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/load.py
+-rw-r--r--   0        0        0     1822 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/object.py
+-rw-r--r--   0        0        0     2514 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/object_test.py
+-rw-r--r--   0        0        0     3894 2023-05-03 07:50:11.901867 castor_extractor-0.3.7/castor_extractor/utils/pager.py
+-rw-r--r--   0        0        0     3245 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/pager_test.py
+-rw-r--r--   0        0        0     2664 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/retry.py
+-rw-r--r--   0        0        0     1635 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/retry_test.py
+-rw-r--r--   0        0        0     1966 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/safe.py
+-rw-r--r--   0        0        0     2160 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/safe_test.py
+-rw-r--r--   0        0        0     2092 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/store.py
+-rw-r--r--   0        0        0     1961 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/string.py
+-rw-r--r--   0        0        0     2206 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/string_test.py
+-rw-r--r--   0        0        0      430 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/time.py
+-rw-r--r--   0        0        0      313 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/type.py
+-rw-r--r--   0        0        0      150 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/uri.py
+-rw-r--r--   0        0        0      259 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/uri_test.py
+-rw-r--r--   0        0        0     1904 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/validation.py
+-rw-r--r--   0        0        0     1181 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/validation_test.py
+-rw-r--r--   0        0        0     2135 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/utils/write.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/__init__.py
+-rw-r--r--   0        0        0     7137 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/client.py
+-rw-r--r--   0        0        0      816 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/client_test.py
+-rw-r--r--   0        0        0     3895 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/constants.py
+-rw-r--r--   0        0        0     3526 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/sdk.py
+-rw-r--r--   0        0        0     1742 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/sdk_test.py
+-rw-r--r--   0        0        0     1320 2023-05-03 07:50:11.902867 castor_extractor-0.3.7/castor_extractor/visualization/looker/api/utils.py
+-rw-r--r--   0        0        0      364 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/assets.py
+-rw-r--r--   0        0        0      467 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/constant.py
+-rw-r--r--   0        0        0      864 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/env.py
+-rw-r--r--   0        0        0     3514 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/extract.py
+-rw-r--r--   0        0        0      636 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/fields.py
+-rw-r--r--   0        0        0      782 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/fields_test.py
+-rw-r--r--   0        0        0     1527 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/looker/parameters.py
+-rw-r--r--   0        0        0      125 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/__init__.py
+-rw-r--r--   0        0        0     2814 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/assets.py
+-rw-r--r--   0        0        0       52 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/api/__init__.py
+-rw-r--r--   0        0        0     5609 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/api/client.py
+-rw-r--r--   0        0        0     1334 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/api/credentials.py
+-rw-r--r--   0        0        0       29 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/__init__.py
+-rw-r--r--   0        0        0     4095 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/client.py
+-rw-r--r--   0        0        0     1863 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/credentials.py
+-rw-r--r--   0        0        0       76 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
+-rw-r--r--   0        0        0       79 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
+-rw-r--r--   0        0        0      419 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/card.sql
+-rw-r--r--   0        0        0       42 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/collection.sql
+-rw-r--r--   0        0        0      439 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
+-rw-r--r--   0        0        0       52 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
+-rw-r--r--   0        0        0       49 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/database.sql
+-rw-r--r--   0        0        0       46 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/table.sql
+-rw-r--r--   0        0        0       41 2023-05-03 07:50:11.903868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/queries/user.sql
+-rw-r--r--   0        0        0     1076 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/decryption.py
+-rw-r--r--   0        0        0      591 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/decryption_test.py
+-rw-r--r--   0        0        0      389 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/shared.py
+-rw-r--r--   0        0        0     1006 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/errors.py
+-rw-r--r--   0        0        0     1773 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/extract.py
+-rw-r--r--   0        0        0       45 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/metabase/types.py
+-rw-r--r--   0        0        0      117 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/assets.py
+-rw-r--r--   0        0        0       27 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/__init__.py
+-rw-r--r--   0        0        0     7803 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client.py
+-rw-r--r--   0        0        0     2087 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client_test.json
+-rw-r--r--   0        0        0     1400 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client_test.py
+-rw-r--r--   0        0        0      453 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/constants.py
+-rw-r--r--   0        0        0     1622 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/client/credentials.py
+-rw-r--r--   0        0        0     1495 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/errors.py
+-rw-r--r--   0        0        0     1559 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/mode/extract.py
+-rw-r--r--   0        0        0      106 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/assets.py
+-rw-r--r--   0        0        0       62 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/constants.py
+-rw-r--r--   0        0        0      482 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/credentials.py
+-rw-r--r--   0        0        0     6604 2023-05-03 07:50:11.904868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/rest.py
+-rw-r--r--   0        0        0     4709 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/rest_test.py
+-rw-r--r--   0        0        0      541 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/utils.py
+-rw-r--r--   0        0        0      719 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/utils_test.py
+-rw-r--r--   0        0        0     1561 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/powerbi/extract.py
+-rw-r--r--   0        0        0      143 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/__init__.py
+-rw-r--r--   0        0        0     1634 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/assets.py
+-rw-r--r--   0        0        0       94 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/__init__.py
+-rw-r--r--   0        0        0      786 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/constants.py
+-rw-r--r--   0        0        0       36 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/__init__.py
+-rw-r--r--   0        0        0     2512 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/client.py
+-rw-r--r--   0        0        0      707 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/constants.py
+-rw-r--r--   0        0        0     1229 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/error.py
+-rw-r--r--   0        0        0     1005 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/error_test.py
+-rw-r--r--   0        0        0     1386 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/json_rpc.py
+-rw-r--r--   0        0        0     1305 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
+-rw-r--r--   0        0        0     2032 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/websocket.py
+-rw-r--r--   0        0        0     3209 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/master.py
+-rw-r--r--   0        0        0     5966 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/rest.py
+-rw-r--r--   0        0        0     1676 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/rest_test.py
+-rw-r--r--   0        0        0       95 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/constants.py
+-rw-r--r--   0        0        0     2397 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/qlik/extract.py
+-rw-r--r--   0        0        0      114 2023-05-03 07:50:11.905868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/__init__.py
+-rw-r--r--   0        0        0      762 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/assets.py
+-rw-r--r--   0        0        0       78 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/__init__.py
+-rw-r--r--   0        0        0     6824 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/client.py
+-rw-r--r--   0        0        0     2077 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/client_utils.py
+-rw-r--r--   0        0        0     3335 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/credentials.py
+-rw-r--r--   0        0        0      803 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/project.py
+-rw-r--r--   0        0        0     2036 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/safe_mode.py
+-rw-r--r--   0        0        0      126 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/constants.py
+-rw-r--r--   0        0        0       91 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/errors.py
+-rw-r--r--   0        0        0     2873 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/extract.py
+-rw-r--r--   0        0        0     4728 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/gql_fields.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/__init__.py
+-rw-r--r--   0        0        0      446 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
+-rw-r--r--   0        0        0      447 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
+-rw-r--r--   0        0        0      450 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
+-rw-r--r--   0        0        0     1018 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
+-rw-r--r--   0        0        0      679 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
+-rw-r--r--   0        0        0     1415 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
+-rw-r--r--   0        0        0     1325 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
+-rw-r--r--   0        0        0     1917 2023-05-03 07:50:11.906868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
+-rw-r--r--   0        0        0     1134 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
+-rw-r--r--   0        0        0      422 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
+-rw-r--r--   0        0        0     1779 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
+-rw-r--r--   0        0        0     1384 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
+-rw-r--r--   0        0        0     1499 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
+-rw-r--r--   0        0        0     1979 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
+-rw-r--r--   0        0        0       26 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
+-rw-r--r--   0        0        0      966 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/tsc_fields.py
+-rw-r--r--   0        0        0      322 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/types.py
+-rw-r--r--   0        0        0      427 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/visualization/tableau/usage.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/__init__.py
+-rw-r--r--   0        0        0     1182 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/asset.py
+-rw-r--r--   0        0        0     1947 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/client.py
+-rw-r--r--   0        0        0     2885 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/extract.py
+-rw-r--r--   0        0        0     2640 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/query.py
+-rw-r--r--   0        0        0      935 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/time_filter.py
+-rw-r--r--   0        0        0      449 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/abstract/time_filter_test.py
+-rw-r--r--   0        0        0      125 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/__init__.py
+-rw-r--r--   0        0        0     3125 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/client.py
+-rw-r--r--   0        0        0     1567 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/client_test.py
+-rw-r--r--   0        0        0     2800 2023-05-03 07:50:11.907868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/extract.py
+-rw-r--r--   0        0        0       30 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/.sqlfluff
+-rw-r--r--   0        0        0     1815 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/column.sql
+-rw-r--r--   0        0        0     1347 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
+-rw-r--r--   0        0        0      207 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/database.sql
+-rw-r--r--   0        0        0      660 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/query.sql
+-rw-r--r--   0        0        0      284 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/schema.sql
+-rw-r--r--   0        0        0     1508 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/table.sql
+-rw-r--r--   0        0        0     2660 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
+-rw-r--r--   0        0        0      189 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/user.sql
+-rw-r--r--   0        0        0      326 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
+-rw-r--r--   0        0        0     4147 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/query.py
+-rw-r--r--   0        0        0      140 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/types.py
+-rw-r--r--   0        0        0      125 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/client.py
+-rw-r--r--   0        0        0     2099 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/extract.py
+-rw-r--r--   0        0        0       30 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/.sqlfluff
+-rw-r--r--   0        0        0     1632 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/column.sql
+-rw-r--r--   0        0        0      241 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/group.sql
+-rw-r--r--   0        0        0      592 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/schema.sql
+-rw-r--r--   0        0        0     1489 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/table.sql
+-rw-r--r--   0        0        0      170 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/user.sql
+-rw-r--r--   0        0        0      540 2023-05-03 07:50:11.908868 castor_extractor-0.3.7/castor_extractor/warehouse/postgres/query.py
+-rw-r--r--   0        0        0      125 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/client.py
+-rw-r--r--   0        0        0     1028 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/client_test.py
+-rw-r--r--   0        0        0     2238 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/extract.py
+-rw-r--r--   0        0        0       30 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/.sqlfluff
+-rw-r--r--   0        0        0     7044 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/column.sql
+-rw-r--r--   0        0        0      299 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/group.sql
+-rw-r--r--   0        0        0     3258 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/query.sql
+-rw-r--r--   0        0        0      585 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/schema.sql
+-rw-r--r--   0        0        0     2645 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/table.sql
+-rw-r--r--   0        0        0      726 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/table_freshness.sql
+-rw-r--r--   0        0        0      170 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/user.sql
+-rw-r--r--   0        0        0      719 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/view_ddl.sql
+-rw-r--r--   0        0        0      540 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/redshift/query.py
+-rw-r--r--   0        0        0      128 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/__init__.py
+-rw-r--r--   0        0        0     4128 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/client.py
+-rw-r--r--   0        0        0     1434 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/client_test.py
+-rw-r--r--   0        0        0     2443 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/extract.py
+-rw-r--r--   0        0        0       31 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/.sqlfluff
+-rw-r--r--   0        0        0     1130 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/column.sql
+-rw-r--r--   0        0        0     1179 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
+-rw-r--r--   0        0        0      483 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/database.sql
+-rw-r--r--   0        0        0      272 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
+-rw-r--r--   0        0        0      143 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
+-rw-r--r--   0        0        0     1779 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/query.sql
+-rw-r--r--   0        0        0       96 2023-05-03 07:50:11.909868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/role.sql
+-rw-r--r--   0        0        0      730 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/schema.sql
+-rw-r--r--   0        0        0     1378 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/table.sql
+-rw-r--r--   0        0        0      570 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/user.sql
+-rw-r--r--   0        0        0      673 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
+-rw-r--r--   0        0        0     1769 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/query.py
+-rw-r--r--   0        0        0       36 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/extract.py
+-rw-r--r--   0        0        0       26 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/.sqlfluff
+-rw-r--r--   0        0        0     1392 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/column.sql
+-rw-r--r--   0        0        0      138 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/database.sql
+-rw-r--r--   0        0        0     1110 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/query.sql
+-rw-r--r--   0        0        0      250 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/schema.sql
+-rw-r--r--   0        0        0     1049 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/table.sql
+-rw-r--r--   0        0        0       67 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/user.sql
+-rw-r--r--   0        0        0      249 2023-05-03 07:50:11.910868 castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/view_ddl.sql
+-rw-r--r--   0        0        0     5142 2023-05-03 07:50:11.911868 castor_extractor-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     9553 1970-01-01 00:00:00.000000 castor_extractor-0.3.7/setup.py
+-rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 castor_extractor-0.3.7/PKG-INFO
```

### Comparing `castor_extractor-0.3.5/CHANGELOG.md` & `castor_extractor-0.3.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 0.3.7 - 2023-04-28
+
+* Warning message to deprecate python < 3.8
+
+## 0.3.6 - 2023-04-24
+
+* Update enum keys for Metabase credentials
+
 ## 0.3.5 - 2023-04-07
 
 * Extract metadata from successful dbt runs only
 
 ## 0.3.4 - 2023-04-05
 
 * Enhance uploader to support `QUALITY` files
```

### Comparing `castor_extractor-0.3.5/LICENCE` & `castor_extractor-0.3.7/LICENCE`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/README.md` & `castor_extractor-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_bigquery.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_bigquery.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_looker.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_looker.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_metabase_api.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_metabase_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
     parser.add_argument("-p", "--password", help="Metabase password")
 
     parser.add_argument("-o", "--output", help="Directory to write to")
 
     args = parser.parse_args()
 
     client = metabase.ApiClient(
-        base_url=args.base_url, username=args.username, password=args.password
+        base_url=args.base_url, user=args.username, password=args.password
     )
 
     metabase.extract_all(
         client,
         output_directory=args.output,
     )
```

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_metabase_db.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_metabase_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     args = parser.parse_args()
 
     client = metabase.DbClient(
         host=args.host,
         port=args.port,
         database=args.database,
         schema=args.schema,
-        username=args.username,
+        user=args.username,
         password=args.password,
         encryption_secret_key=args.encryption_secret_key,
     )
 
     metabase.extract_all(
         client,
         output_directory=args.output,
```

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_mode.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_postgres.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_postgres.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_powerbi.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_powerbi.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_qlik.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_qlik.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_redshift.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_redshift.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_snowflake.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_snowflake.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/extract_tableau.py` & `castor_extractor-0.3.7/castor_extractor/commands/extract_tableau.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/file_check.py` & `castor_extractor-0.3.7/castor_extractor/commands/file_check.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/commands/upload.py` & `castor_extractor-0.3.7/castor_extractor/commands/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/column.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/column.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/column_test.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/column_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/enums.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/enums.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/file.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         ------------------------------
         ```
         """
         if not self.verbose:
             return
         header = f"Issues detected on Row #{index+1}\n"
         for k, v in row.items():
-            header += "{:<20} {:<100}\n".format(str(k), str(v))
+            header += f"{str(k):<20} {str(v):<100}\n"
         self.logger.info(header + _SEPARATOR + issue_log + _SEPARATOR)
 
     def occurrences(self, name: str) -> Set[str]:
         """
         Return values of the given column, provided:
         - the column exists in the template
         - the column is set to UNIQUE (which means occurrences are recorded)
```

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/file_test.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/file_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 _TEST_FILE = "file_test_users.csv"
 _TEST_FILE_VALID = "file_test_users_valid.csv"
 
 
 def _content(path: str) -> Iterator[Dict]:
     absolute_path = os.path.join(os.path.dirname(__file__), path)
     with open(absolute_path) as csvfile:
-        for row in csv.DictReader(csvfile):
-            yield row
+        yield from csv.DictReader(csvfile)
 
 
 def _user_template() -> FileTemplate:
     folder_ids = {"1", "2", "3"}
     return {
         "id": ColumnChecker(is_unique=True),
         "name": ColumnChecker(),
```

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/file_test_users.csv` & `castor_extractor-0.3.7/castor_extractor/file_checker/file_test_users.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/file_checker/templates/generic_warehouse.py` & `castor_extractor-0.3.7/castor_extractor/file_checker/templates/generic_warehouse.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/logger.py` & `castor_extractor-0.3.7/castor_extractor/logger.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/transformation/dbt/client/client.py` & `castor_extractor-0.3.7/castor_extractor/transformation/dbt/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/transformation/dbt/client/credentials.py` & `castor_extractor-0.3.7/castor_extractor/transformation/dbt/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/uploader/constant.py` & `castor_extractor-0.3.7/castor_extractor/uploader/constant.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/uploader/env.py` & `castor_extractor-0.3.7/castor_extractor/uploader/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/uploader/upload.py` & `castor_extractor-0.3.7/castor_extractor/uploader/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/__init__.py` & `castor_extractor-0.3.7/castor_extractor/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .collection import group_by
 from .constants import OUTPUT_DIR
+from .deprecate import deprecate_python
 from .env import from_env
 from .files import explode, search_files
 from .formatter import to_string_array
 from .load import load_file
 from .object import deep_serialize, getproperty
 from .pager import (
     Pager,
```

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/env.py` & `castor_extractor-0.3.7/castor_extractor/utils/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/files.py` & `castor_extractor-0.3.7/castor_extractor/utils/files.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/files_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/formatter.py` & `castor_extractor-0.3.7/castor_extractor/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/formatter_test.csv` & `castor_extractor-0.3.7/castor_extractor/utils/formatter_test.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/formatter_test.json` & `castor_extractor-0.3.7/castor_extractor/utils/formatter_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/formatter_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/formatter_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 SAMPLE_FILE = "formatter_test"
 
 
 def _test(formatter: Formatter) -> None:
     root = os.path.dirname(__file__)
     path = os.path.join(root, f"{SAMPLE_FILE}.{formatter.extension()}")
-    with open(path) as file:
+    with open(path, "r") as file:
         rows = list(formatter.deserialize(file))
         first = rows[0]
 
         assert len(rows) == SAMPLE_SIZE
         assert tuple(first.keys()) == SAMPLE_KEYS
 
         with io.StringIO() as f:
```

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/object.py` & `castor_extractor-0.3.7/castor_extractor/utils/object.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/object_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/pager.py` & `castor_extractor-0.3.7/castor_extractor/utils/pager.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/pager_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/pager_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/retry.py` & `castor_extractor-0.3.7/castor_extractor/utils/retry.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/retry_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/retry_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/safe.py` & `castor_extractor-0.3.7/castor_extractor/utils/safe.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/safe_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/safe_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/store.py` & `castor_extractor-0.3.7/castor_extractor/utils/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,9 +63,9 @@
         path = self.path(name)
         with open(path, "w") as file:
             self._formatter.serialize(file, data)
         return path
 
     def get(self, name: str) -> Iterator[dict]:
         path = self.path(name)
-        with open(path) as file:
+        with open(path, "r") as file:
             return self._formatter.deserialize(StringIO(file.read()))
```

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/string.py` & `castor_extractor-0.3.7/castor_extractor/utils/string.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/string_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/string_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/validation.py` & `castor_extractor-0.3.7/castor_extractor/utils/validation.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/validation_test.py` & `castor_extractor-0.3.7/castor_extractor/utils/validation_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/utils/write.py` & `castor_extractor-0.3.7/castor_extractor/utils/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import os
+import sys
 from datetime import datetime
 from typing import Any, List
 
 import pkg_resources
 
 ENCODING = "utf8"
 SUMMARY_FILENAME = "summary.json"
@@ -47,14 +48,15 @@
     """
     write a json file containing extraction session information
     """
     summary = get_output_filename("summary", output_directory, ts)
     write_json(
         summary,
         {
+            "python_version": sys.version,
             "version": _current_version(),
             "executed_at": datetime.fromtimestamp(ts).isoformat(),
             **kwargs,
         },
     )
```

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/client_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/constants.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/sdk.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/sdk.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/sdk_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/sdk_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/api/utils.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/api/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/env.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/fields.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/fields_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/fields_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/looker/parameters.py` & `castor_extractor-0.3.7/castor_extractor/visualization/looker/parameters.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/assets.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/api/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(
         self,
         **kwargs,
     ):
         self._credentials = CredentialsApi(
             base_url=get_value(CredentialsApiKey.BASE_URL, kwargs),
-            username=get_value(CredentialsApiKey.USERNAME, kwargs),
+            user=get_value(CredentialsApiKey.USER, kwargs),
             password=get_value(CredentialsApiKey.PASSWORD, kwargs),
         )
         self._session = requests.Session()
         self._session_id = self._login()
         self._check_permissions()  # verify that the given user is superuser
 
     @staticmethod
@@ -87,15 +87,15 @@
                     error_details=err.args,
                 )
             raise
 
     def _login(self) -> str:
         url = self._url("session")
         payload = {
-            "username": self._credentials.username,
+            "username": self._credentials.user,
             "password": self._credentials.password,
         }
         response = self._session.post(url, json=payload)
         logger.info(f"Getting session_id: {response.json()}")
 
         if not response.json().get("id"):
             raise MetabaseLoginError(
```

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/api/credentials.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/api/credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import Dict
 
 from .....utils import from_env
 
 
 class CredentialsApiKey(Enum):
     BASE_URL = "base_url"
-    USERNAME = "username"
+    USER = "user"
     PASSWORD = "password"
 
 
 CREDENTIALS_ENV: Dict[CredentialsApiKey, str] = {
     CredentialsApiKey.BASE_URL: "CASTOR_METABASE_API_BASE_URL",
-    CredentialsApiKey.USERNAME: "CASTOR_METABASE_API_USERNAME",
+    CredentialsApiKey.USER: "CASTOR_METABASE_API_USERNAME",
     CredentialsApiKey.PASSWORD: "CASTOR_METABASE_API_PASSWORD",
 }
 
 
 def get_value(key: CredentialsApiKey, kwargs: dict) -> str:
     """
     Returns the value of the given key:
@@ -26,20 +26,20 @@
     env_key = CREDENTIALS_ENV[key]
     return str(kwargs.get(key.value) or from_env(env_key))
 
 
 class CredentialsApi:
     """ValueObject for the credentials"""
 
-    def __init__(self, base_url: str, username: str, password: str):
+    def __init__(self, base_url: str, user: str, password: str):
         self.base_url = base_url
-        self.username = username
+        self.user = user
         self.password = password
 
     def to_dict(self, hide: bool = False) -> Dict[str, str]:
-        safe = (CredentialsApiKey.BASE_URL, CredentialsApiKey.USERNAME)
+        safe = (CredentialsApiKey.BASE_URL, CredentialsApiKey.USER)
         unsafe = (CredentialsApiKey.PASSWORD,)
 
         def val(k: CredentialsApiKey, v: str) -> str:
             return "*" + v[-4:] if hide and k in unsafe else v
 
         return {a.value: val(a, getattr(self, a.value)) for a in safe + unsafe}
```

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         **kwargs,
     ):
         self._credentials = CredentialsDb(
             host=get_value(CredentialsDbKey.HOST, kwargs),
             port=get_value(CredentialsDbKey.PORT, kwargs),
             database=get_value(CredentialsDbKey.DATABASE, kwargs),
             schema=get_value(CredentialsDbKey.SCHEMA, kwargs),
-            username=get_value(CredentialsDbKey.USERNAME, kwargs),
+            user=get_value(CredentialsDbKey.USER, kwargs),
             password=get_value(CredentialsDbKey.PASSWORD, kwargs),
         )
         self.encryption_secret_key = kwargs.get(
             "encryption_secret_key"
         ) or from_env(ENCRYPTION_SECRET_KEY, allow_missing=True)
         self._engine = self._login()
```

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/db/credentials.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/db/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 
 class CredentialsDbKey(Enum):
     HOST = "host"
     PORT = "port"
     DATABASE = "database"
     SCHEMA = "schema"
-    USERNAME = "username"
+    USER = "user"
     PASSWORD = "password"
 
 
 CREDENTIALS_ENV: Dict[CredentialsDbKey, str] = {
     CredentialsDbKey.HOST: "CASTOR_METABASE_DB_HOST",
     CredentialsDbKey.PORT: "CASTOR_METABASE_DB_PORT",
     CredentialsDbKey.DATABASE: "CASTOR_METABASE_DB_DATABASE",
     CredentialsDbKey.SCHEMA: "CASTOR_METABASE_DB_SCHEMA",
-    CredentialsDbKey.USERNAME: "CASTOR_METABASE_DB_USERNAME",
+    CredentialsDbKey.USER: "CASTOR_METABASE_DB_USERNAME",
     CredentialsDbKey.PASSWORD: "CASTOR_METABASE_DB_PASSWORD",
 }
 
 
 def get_value(key: CredentialsDbKey, kwargs: dict) -> str:
     """
     Returns the value of the given key:
@@ -38,31 +38,31 @@
 
     def __init__(
         self,
         host: str,
         port: str,
         database: str,
         schema: str,
-        username: str,
+        user: str,
         password: str,
     ):
         self.host = host
         self.port = port
         self.database = database
         self.schema = schema
-        self.username = username
+        self.user = user
         self.password = password
 
     def to_dict(self, hide: bool = False) -> Dict[str, str]:
         safe = (
             CredentialsDbKey.HOST,
             CredentialsDbKey.PORT,
             CredentialsDbKey.DATABASE,
             CredentialsDbKey.SCHEMA,
-            CredentialsDbKey.USERNAME,
+            CredentialsDbKey.USER,
         )
         unsafe = (CredentialsDbKey.PASSWORD,)
 
         def val(k: CredentialsDbKey, v: str) -> str:
             return "*" + v[-4:] if hide and k in unsafe else v
 
         return {a.value: val(a, getattr(self, a.value)) for a in safe + unsafe}
```

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/decryption.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/decryption.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/client/decryption_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/client/decryption_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/errors.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/metabase/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/metabase/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/assets.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client_test.json` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/client/client_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/client/credentials.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/errors.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/mode/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/mode/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/constants.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/rest.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/rest_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/utils.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/client/utils_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/client/utils_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/powerbi/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/powerbi/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/assets.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/constants.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/constants.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/error.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/error.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/error_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/error_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/json_rpc.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/json_rpc.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/engine/websocket.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/engine/websocket.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/master.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/master.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/rest.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/client/rest_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/qlik/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/qlik/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/assets.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/client.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/client_utils.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/credentials.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/project.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/project.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/client/safe_mode.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/client/safe_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/extract.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/gql_fields.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/gql_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/visualization/tableau/tsc_fields.py` & `castor_extractor-0.3.7/castor_extractor/visualization/tableau/tsc_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/abstract/asset.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/abstract/asset.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/abstract/client.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/abstract/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/abstract/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/abstract/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/abstract/query.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/abstract/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/abstract/time_filter.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/abstract/time_filter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/client.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
             if self._keep_project(p.project_id)
         ]
 
     def get_regions(self) -> Set[Tuple[str, str]]:
         """
         Returns distinct (project_id, region) available for the given GCP client
         """
-        return set(
+        return {
             (ds.project, ds._properties["location"])
             for ds in self._list_datasets()
-        )
+        }
 
     def get_datasets(self) -> Set[Tuple[str, str]]:
         """
         Returns distinct (project_id, dataset_id) available for the given GCP client
         """
-        return set((ds.project, ds.dataset_id) for ds in self._list_datasets())
+        return {(ds.project, ds.dataset_id) for ds in self._list_datasets()}
```

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/client_test.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 )
 
 
 def _credentials(params: dict) -> dict:
     """extract GCP credentials"""
     path = params.get("credentials") or from_env(BIGQUERY_CREDENTIALS)
     logger.info(f"Credentials fetched from {path}")
-    with open(path) as file:
+    with open(path, "r") as file:
         return cast(dict, json.load(file))
 
 
 def extract_all(**kwargs) -> None:
     """
     Extract all assets from BigQuery and store the results in CSV files
     Time filter scope for `Queries` = the day before (0 > 23h)
```

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/column.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/query.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/table.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/bigquery/query.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/bigquery/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/client.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/column.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/schema.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/queries/table.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/postgres/query.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/postgres/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/client.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/client_test.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/column.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/query.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/schema.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/table.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/table_freshness.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/table_freshness.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/queries/view_ddl.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/redshift/query.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/redshift/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/client.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def _use(connection: Connection, resource: UseResource, name: str):
     """
     USE ROLE/WAREHOUSE do not accept SQL parameter substitution
         we do a sanity check prior to using it
     DON'T COPY THIS CODE FOR ANOTHER PURPOSE
     """
     target = resource.value
-    if not re.fullmatch("[\w_-]+", name):
+    if not re.fullmatch(r"[\w_-]+", name):
         raise NameError(f"{target} name invalid {name}")
     command = f'USE {target} "{name}"'
     logger.info(f"executing {command}")
     connection.execute(command)
 
 
 def _first_non_public_role(connection: Connection) -> str:
```

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/client_test.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/column.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/column_lineage.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/column_lineage.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/query.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/schema.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/table.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/user.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/user.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/queries/view_ddl.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/snowflake/query.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/synapse/extract.py` & `castor_extractor-0.3.7/castor_extractor/warehouse/synapse/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/column.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/query.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/castor_extractor/warehouse/synapse/queries/table.sql` & `castor_extractor-0.3.7/castor_extractor/warehouse/synapse/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.5/pyproject.toml` & `castor_extractor-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 
 [tool.poetry]
 name = "castor-extractor"
-version = "0.3.5"
+version = "0.3.7"
 description = "Extract your metadata assets."
 authors = ["Castor <support@castordoc.com>"]
 license = "EULA"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
```

### Comparing `castor_extractor-0.3.5/setup.py` & `castor_extractor-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                      'castor_extractor.commands.extract_tableau:main',
                      'castor-file-check = '
                      'castor_extractor.commands.file_check:main',
                      'castor-upload = castor_extractor.commands.upload:main']}
 
 setup_kwargs = {
     'name': 'castor-extractor',
-    'version': '0.3.5',
+    'version': '0.3.7',
     'description': 'Extract your metadata assets.',
     'long_description': '# Castor Extractor <img src="https://app.castordoc.com/images/castor_icon_dark.svg" width=30 />\n\nThis library contains utilities to extract your metadata assets into `JSON` or `CSV` files, on your local machine.\nAfter extraction, those files can be pushed to Castor for ingestion.\n\n- Visualization assets are typically:\n  - `dashboards`\n  - `users`\n  - `folders`\n  - ...\n\n- Warehouse assets are typically:\n  - `databases`\n  - `schemas`\n  - `tables`\n  - `columns`\n  - `queries`\n  - ...\n\nIt also embeds utilities to help you push your metadata to Castor:\n\n- `File Checker` to validate your [generic](https://docs.castordoc.com/integrations/data-warehouses/generic-warehouse) CSV files before pushing to Castor\n- `Uploader` to push extracted files to our Google-Cloud-Storage (GCS)\n\n# Table of contents\n\n- [Castor Extractor ](#castor-extractor-)\n- [Table of contents](#table-of-contents)\n- [Installation](#installation)\n  - [Create castor-env](#create-castor-env)\n  - [PIP install](#pip-install)\n  - [Create the output directory](#create-the-output-directory)\n- [Contact](#contact)\n\n# Installation\n\nRequirements: **python3.8+**\n<img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" width=20 />\n\n## Create castor-env\n\nWe advise to create a dedicated [Python environment](https://docs.python.org/3/library/venv.html).\n\nHere\'s an example using `Pyenv` and Python `3.8.12`:\n\n- Install Pyenv\n\n```bash\nbrew install pyenv\nbrew install pyenv-virtualenv\n```\n\n- [optional] Update your `.bashrc` if you encounter this [issue](https://stackoverflow.com/questions/45577194/failed-to-activate-virtualenv-with-pyenv/45578839)\n\n```bash\neval "$(pyenv init -)"\neval "$(pyenv init --path)"\neval "$(pyenv virtualenv-init -)"\n```\n\n- [optional] Install python 3.8+\n\n```bash\npyenv versions # check your local python installations\n\npyenv install -v 3.8.12 # if none of the installed versions satisfy requirements 8+\n```\n\n- Create your virtual env\n\n```bash\npyenv virtualenv 3.8.12 castor-env # create a dedicated env\npyenv shell castor-env # activate the environment\n\n# optional checks\npython --version # should be `3.8.12`\npyenv version # should be `castor-env`\n```\n\n## PIP install\n\n⚠️ `castor-env` must be created AND activated first.\n\n```bash\npyenv shell castor-env\n(castor-env) $ # this means the environment is now active\n```\n\nℹ️ please upgrade `PIP` before installing Castor.\n\n```\npip install --upgrade pip\n```\n\nRun the following command to install `castor-extractor`:\n\n```\npip install castor-extractor\n```\n\nDepending on your use-case, you can also install one of the following `extras`:\n\n```\npip install castor-extractor[looker]\npip install castor-extractor[tableau]\npip install castor-extractor[metabase]\npip install castor-extractor[qlik]\npip install castor-extractor[bigquery]\npip install castor-extractor[redshift]\npip install castor-extractor[snowflake]\n```\n\n## Create the output directory\n\n```bash\nmkdir /tmp/castor\n```\n\nYou will provide this path in `extraction` scripts as following:\n\n```\ncastor-extract-bigquery --output=/tmp/castor\n```\n\nAlternatively, you can also set the following `ENV` in your `bashrc`:\n\n```bash\nexport CASTOR_OUTPUT_DIRECTORY="/tmp/castor"\n````\n\n# Contact\n\nFor any questions or bug report, contact us at [support@castordoc.com](mailto:support@castordoc.com)\n\n[Castor](https://castordoc.com) helps you find, understand, use your data assets\n',
     'author': 'Castor',
     'author_email': 'support@castordoc.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.castordoc.com/',
```

### Comparing `castor_extractor-0.3.5/PKG-INFO` & `castor_extractor-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castor-extractor
-Version: 0.3.5
+Version: 0.3.7
 Summary: Extract your metadata assets.
 Home-page: https://www.castordoc.com/
 License: EULA
 Author: Castor
 Author-email: support@castordoc.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: Other/Proprietary License
```

