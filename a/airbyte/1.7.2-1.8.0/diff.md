# Comparing `tmp/airbyte-1.7.2.tar.gz` & `tmp/airbyte-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-1.7.2.tar", last modified: Tue May  2 00:47:30 2023, max compression
+gzip compressed data, was "airbyte-1.8.0.tar", last modified: Wed May  3 00:46:11 2023, max compression
```

## Comparing `airbyte-1.7.2.tar` & `airbyte-1.8.0.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.571623 airbyte-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 00:47:17.000000 airbyte-1.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-02 00:47:30.571623 airbyte-1.7.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6503 2023-05-02 00:47:17.000000 airbyte-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:47:30.571623 airbyte-1.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-05-02 00:47:17.000000 airbyte-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.543623 airbyte-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.543623 airbyte-1.7.2/src/airbyte/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4743 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/destinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.543623 airbyte-1.7.2/src/airbyte/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.543623 airbyte-1.7.2/src/airbyte/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/canceljob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/createconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/createjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/createworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/deleteconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/deletedestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/deletesource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getstreamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/getworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/listconnections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/listdestinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1601 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/listjobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/listsources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/operations/listworkspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.571623 airbyte-1.7.2/src/airbyte/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    49282 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectioncreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionschedulecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionscheduleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9258 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_aws_datalake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12146 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10897 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_bigquery_denormalized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_cassandra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_convex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_databend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8016 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_databricks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_elasticsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_firestore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21027 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2044 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_keen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_kinesis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6284 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_mariadb_columnstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_meilisearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9179 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8107 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6750 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11112 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_pubsub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_pulsar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_rabbitmq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8012 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_redis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13955 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_rockset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18868 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_s3_glue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_scylla.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_sftp_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16047 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destination_typesense.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destinationcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destinationresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/destinationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/geographyenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/jobcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/jobresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/jobsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/jobstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/jobtypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/scheduletypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_airtable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7489 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_alloydb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4938 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_amazon_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5139 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_amazon_seller_partner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_amplitude.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_apify_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_asana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_auth0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_aws_cloudtrail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3043 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_azure_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1621 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_bamboo_hr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_bigcommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_bing_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_braintree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_braze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_chargebee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_chartmogul.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2895 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_clickup_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_close_com.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_coda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_coin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_coinmarketcap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_configcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_confluence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_datascope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_delighted.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_dixa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_dockerhub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_dremio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_e2e_test_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_emailoctopus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_exchange_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17556 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_facebook_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_facebook_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_faker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_fauna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10260 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_file_secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_freshcaller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_freshdesk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_freshsales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_getlago.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_github.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4124 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_gitlab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_glassfrog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_gnews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5187 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_analytics_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_analytics_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_directory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_search_console.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_webfonts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_google_workspace_admin_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_greenhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_gridly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_harvest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_hubplanner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_hubspot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_insightly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_instagram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_instatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_intercom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_ip2whois.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_iterable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_jira.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_k6_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_klarna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_klaviyo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_kustomer_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_launchdarkly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_lemlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_linkedin_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_linkedin_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_linnworks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_lokalise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mailchimp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mailgun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mailjet_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_marketo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_metabase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_microsoft_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mixpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_monday.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4394 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12174 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_my_hours.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12789 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_netsuite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3005 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_notion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_nytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_omnisend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2679 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_onesignal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_openweather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_orb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_outreach.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_paypal_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_paystack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pendo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_persistiq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pexels_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3220 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pinterest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pipedrive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pocket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pokeapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_polygon_stock_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7508 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_posthog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_postmarkapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_prestashop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_public_apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_punk_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_pypi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_qualaroo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3521 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_quickbooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_railz.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_recharge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_recreation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_recruitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_recurly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_retently.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_rki_covid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_rss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13269 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_salesforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_salesforce_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_salesloft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sap_fieldglass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_secoda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sendgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sendinblue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_senseforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sentry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sftp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3453 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sftp_bulk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_shopify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_shortio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_slack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_smaily.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      772 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_smartengage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_smartsheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_snapchat_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2194 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_sonar_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_spacex_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_square.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_strava.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_stripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_survey_sparrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3720 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_surveymonkey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_tempo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_the_guardian_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_tiktok_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_todoist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_trello.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_trustpilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_tvmaze_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_twilio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_twilio_taskrouter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_twitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_typeform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_us_census.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_vantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_webflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_whisky_hunter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_wikipedia_pageviews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_woocommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_xero.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_xkcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_yandex_metrica.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_younium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_youtube_analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_chat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_sunshine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_talk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zenloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zoho_crm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/source_zuora.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/sourcecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/sourceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/sourcesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/streamconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/streamconfigurations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/streamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/workspacecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/workspaceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/models/shared/workspacesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/sources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.571623 airbyte-1.7.2/src/airbyte/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-05-02 00:47:17.000000 airbyte-1.7.2/src/airbyte/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:47:30.543623 airbyte-1.7.2/src/airbyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-02 00:47:30.000000 airbyte-1.7.2/src/airbyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-02 00:47:30.000000 airbyte-1.7.2/src/airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:47:30.000000 airbyte-1.7.2/src/airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-02 00:47:30.000000 airbyte-1.7.2/src/airbyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 00:47:30.000000 airbyte-1.7.2/src/airbyte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:11.001534 airbyte-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 00:46:00.000000 airbyte-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-03 00:46:11.001534 airbyte-1.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6700 2023-05-03 00:46:00.000000 airbyte-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:46:11.001534 airbyte-1.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-05-03 00:46:00.000000 airbyte-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:10.973533 airbyte-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:10.973533 airbyte-1.8.0/src/airbyte/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4743 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/destinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:10.977533 airbyte-1.8.0/src/airbyte/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:10.977533 airbyte-1.8.0/src/airbyte/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/canceljob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/createconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/createjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/createworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/deleteconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/deletedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/deletesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getstreamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/getworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/listconnections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/listdestinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1601 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/listjobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/listsources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/operations/listworkspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:11.001534 airbyte-1.8.0/src/airbyte/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49058 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectioncreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionschedulecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionscheduleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9258 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_aws_datalake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12146 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10897 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_cassandra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_convex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_databend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8016 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_databricks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_elasticsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_firestore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21027 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2044 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_keen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_kinesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6284 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_meilisearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9179 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8107 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6750 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11112 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_pubsub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_pulsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_rabbitmq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8012 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_redis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13955 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_rockset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18868 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_s3_glue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_scylla.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_sftp_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16047 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destination_typesense.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destinationcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destinationresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/destinationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/geographyenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/jobcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/jobresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/jobsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/jobstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/jobtypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/scheduletypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_airtable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7489 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_alloydb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4938 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_amazon_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5139 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_amazon_seller_partner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_amplitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_apify_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_asana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_auth0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_aws_cloudtrail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3043 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_azure_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1621 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_bamboo_hr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_bigcommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_bing_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_braintree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_braze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_chargebee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_chartmogul.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2895 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_clickup_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_close_com.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_coda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_coin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_coinmarketcap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_configcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_confluence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_datascope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_delighted.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_dixa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_dockerhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_dremio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_e2e_test_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_emailoctopus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_exchange_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8735 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_facebook_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_facebook_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_faker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_fauna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10260 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_file_secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_freshcaller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_freshdesk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_freshsales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_getlago.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4124 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_gitlab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_glassfrog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_gnews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5187 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_analytics_data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_analytics_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_directory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_search_console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_webfonts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_greenhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_gridly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_harvest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_hubplanner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_hubspot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_insightly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_instagram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_instatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_intercom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_ip2whois.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_iterable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_jira.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_k6_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_klarna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_klaviyo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_kustomer_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_launchdarkly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_lemlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_linkedin_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_linkedin_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_linnworks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_lokalise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mailchimp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mailgun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mailjet_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_marketo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_metabase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_microsoft_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mixpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_monday.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4394 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12174 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_my_hours.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12789 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_netsuite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3005 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_notion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_nytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_omnisend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2679 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_onesignal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_openweather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_orb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_outreach.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_paypal_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_paystack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pendo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_persistiq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pexels_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3220 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pinterest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pipedrive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pocket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pokeapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_polygon_stock_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7508 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_posthog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_postmarkapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_prestashop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_public_apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_punk_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_pypi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_qualaroo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3521 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_quickbooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_railz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_recharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_recreation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_recruitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_recurly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_retently.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_rki_covid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_rss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12864 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_salesforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_salesforce_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_salesloft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sap_fieldglass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_secoda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sendgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sendinblue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_senseforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3453 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sftp_bulk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_shopify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_shortio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_slack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_smaily.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      772 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_smartengage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_smartsheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_snapchat_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2194 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_sonar_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_spacex_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_square.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_strava.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_stripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_survey_sparrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3720 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_surveymonkey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_tempo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_the_guardian_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_tiktok_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_todoist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_trello.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_trustpilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_tvmaze_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_twilio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_twilio_taskrouter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_twitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_typeform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_us_census.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_vantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_webflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_whisky_hunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_woocommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_xero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_xkcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_yandex_metrica.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_younium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_youtube_analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_sunshine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_talk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zenloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zoho_crm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/source_zuora.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/sourcecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/sourceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/sourcesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/streamconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/streamconfigurations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/streamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/workspacecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/workspaceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/models/shared/workspacesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/sources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:11.001534 airbyte-1.8.0/src/airbyte/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25540 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-05-03 00:46:00.000000 airbyte-1.8.0/src/airbyte/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:10.977533 airbyte-1.8.0/src/airbyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-03 00:46:10.000000 airbyte-1.8.0/src/airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-03 00:46:10.000000 airbyte-1.8.0/src/airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:46:10.000000 airbyte-1.8.0/src/airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 00:46:10.000000 airbyte-1.8.0/src/airbyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 00:46:10.000000 airbyte-1.8.0/src/airbyte.egg-info/top_level.txt
```

### Comparing `airbyte-1.7.2/LICENSE.md` & `airbyte-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/PKG-INFO` & `airbyte-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 1.7.2
+Version: 1.8.0
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -48,83 +48,83 @@
 
 
 req = shared.ConnectionCreateRequest(
     configurations=shared.StreamConfigurations(
         streams=[
             shared.StreamConfiguration(
                 cursor_field=[
-                    "distinctio",
-                    "quibusdam",
-                    "unde",
+                    'distinctio',
+                    'quibusdam',
+                    'unde',
                 ],
-                name="Johnnie Stamm",
+                name='Johnnie Stamm',
                 primary_key=[
                     [
-                        "iure",
-                        "magnam",
+                        'iure',
+                        'magnam',
                     ],
                     [
-                        "ipsa",
-                        "delectus",
-                        "tempora",
-                        "suscipit",
+                        'ipsa',
+                        'delectus',
+                        'tempora',
+                        'suscipit',
                     ],
                     [
-                        "minus",
-                        "placeat",
+                        'minus',
+                        'placeat',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "excepturi",
-                    "nisi",
+                    'excepturi',
+                    'nisi',
                 ],
-                name="Jake Bernier MD",
+                name='Jake Bernier MD',
                 primary_key=[
                     [
-                        "repellendus",
-                        "sapiente",
+                        'repellendus',
+                        'sapiente',
                     ],
                 ],
-                sync_mode="incremental_deduped_history",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "at",
+                    'at',
                 ],
-                name="Emilio Krajcik",
+                name='Emilio Krajcik',
                 primary_key=[
                     [
-                        "porro",
-                        "dolorum",
-                        "dicta",
+                        'porro',
+                        'dolorum',
+                        'dicta',
                     ],
                     [
-                        "officia",
-                        "occaecati",
-                        "fugit",
+                        'officia',
+                        'occaecati',
+                        'fugit',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
-    data_residency="eu",
-    destination_id="c816742c-b739-4205-9293-96fea7596eb1",
-    name="Lela Orn",
-    namespace_definition="source",
-    namespace_format="${SOURCE_NAMESPACE}",
-    prefix="dolorem",
+    data_residency=shared.GeographyEnumEnum.EU,
+    destination_id='c816742c-b739-4205-9293-96fea7596eb1',
+    name='Lela Orn',
+    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_format='${SOURCE_NAMESPACE}',
+    prefix='dolorem',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression="corporis",
-        schedule_type="manual",
+        cron_expression='corporis',
+        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
     ),
-    source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
+    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte Version: 1.7.2 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: airbyte Version: 1.8.0 Summary: Python Client SDK
 for Airbyte API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
 File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
@@ -21,28 +21,31 @@
 (Installation will not work until published to a package manager, please
 install locally to try it out `pip install -e ../path/to/local/clone`)  ## SDK
 Installation ```bash pip install airbyte ```  ## SDK Example Usage  ```python
 import airbyte from airbyte.models import shared s = airbyte.Airbyte
 ( security=shared.Security( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), )
 req = shared.ConnectionCreateRequest
 ( configurations=shared.StreamConfigurations( streams=
-[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
-], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
-"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
-sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
-[ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
-[ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
-shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
-primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
-"fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
-destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
-namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
-prefix="dolorem", schedule=shared.ConnectionScheduleCreate
-( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
-aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
+[ shared.StreamConfiguration( cursor_field=[ 'distinctio', 'quibusdam', 'unde',
+], name='Johnnie Stamm', primary_key=[ [ 'iure', 'magnam', ], [ 'ipsa',
+'delectus', 'tempora', 'suscipit', ], [ 'minus', 'placeat', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND, ),
+shared.StreamConfiguration( cursor_field=[ 'excepturi', 'nisi', ], name='Jake
+Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
+shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
+primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
+'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
+), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
+b739-4205-9293-96fea7596eb1', name='Lela Orn',
+namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
+schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
+schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
+4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
 Resources and Operations ### [connections](docs/connections/README.md) *
 [create_connection](docs/connections/README.md#create_connection) - Create a
 connection * [delete_connection](docs/connections/README.md#delete_connection)
 - Get Connection details * [get_connection](docs/connections/
 README.md#get_connection) - Get Connection details * [list_connections](docs/
 connections/README.md#list_connections) - List connections ### [destinations]
```

### Comparing `airbyte-1.7.2/README.md` & `airbyte-1.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -36,83 +36,83 @@
 
 
 req = shared.ConnectionCreateRequest(
     configurations=shared.StreamConfigurations(
         streams=[
             shared.StreamConfiguration(
                 cursor_field=[
-                    "distinctio",
-                    "quibusdam",
-                    "unde",
+                    'distinctio',
+                    'quibusdam',
+                    'unde',
                 ],
-                name="Johnnie Stamm",
+                name='Johnnie Stamm',
                 primary_key=[
                     [
-                        "iure",
-                        "magnam",
+                        'iure',
+                        'magnam',
                     ],
                     [
-                        "ipsa",
-                        "delectus",
-                        "tempora",
-                        "suscipit",
+                        'ipsa',
+                        'delectus',
+                        'tempora',
+                        'suscipit',
                     ],
                     [
-                        "minus",
-                        "placeat",
+                        'minus',
+                        'placeat',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "excepturi",
-                    "nisi",
+                    'excepturi',
+                    'nisi',
                 ],
-                name="Jake Bernier MD",
+                name='Jake Bernier MD',
                 primary_key=[
                     [
-                        "repellendus",
-                        "sapiente",
+                        'repellendus',
+                        'sapiente',
                     ],
                 ],
-                sync_mode="incremental_deduped_history",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "at",
+                    'at',
                 ],
-                name="Emilio Krajcik",
+                name='Emilio Krajcik',
                 primary_key=[
                     [
-                        "porro",
-                        "dolorum",
-                        "dicta",
+                        'porro',
+                        'dolorum',
+                        'dicta',
                     ],
                     [
-                        "officia",
-                        "occaecati",
-                        "fugit",
+                        'officia',
+                        'occaecati',
+                        'fugit',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
-    data_residency="eu",
-    destination_id="c816742c-b739-4205-9293-96fea7596eb1",
-    name="Lela Orn",
-    namespace_definition="source",
-    namespace_format="${SOURCE_NAMESPACE}",
-    prefix="dolorem",
+    data_residency=shared.GeographyEnumEnum.EU,
+    destination_id='c816742c-b739-4205-9293-96fea7596eb1',
+    name='Lela Orn',
+    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_format='${SOURCE_NAMESPACE}',
+    prefix='dolorem',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression="corporis",
-        schedule_type="manual",
+        cron_expression='corporis',
+        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
     ),
-    source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
+    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -17,28 +17,31 @@
 (Installation will not work until published to a package manager, please
 install locally to try it out `pip install -e ../path/to/local/clone`)  ## SDK
 Installation ```bash pip install airbyte ```  ## SDK Example Usage  ```python
 import airbyte from airbyte.models import shared s = airbyte.Airbyte
 ( security=shared.Security( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), )
 req = shared.ConnectionCreateRequest
 ( configurations=shared.StreamConfigurations( streams=
-[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
-], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
-"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
-sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
-[ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
-[ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
-shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
-primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
-"fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
-destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
-namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
-prefix="dolorem", schedule=shared.ConnectionScheduleCreate
-( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
-aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
+[ shared.StreamConfiguration( cursor_field=[ 'distinctio', 'quibusdam', 'unde',
+], name='Johnnie Stamm', primary_key=[ [ 'iure', 'magnam', ], [ 'ipsa',
+'delectus', 'tempora', 'suscipit', ], [ 'minus', 'placeat', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND, ),
+shared.StreamConfiguration( cursor_field=[ 'excepturi', 'nisi', ], name='Jake
+Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
+shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
+primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
+'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
+), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
+b739-4205-9293-96fea7596eb1', name='Lela Orn',
+namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
+schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
+schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
+4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
 Resources and Operations ### [connections](docs/connections/README.md) *
 [create_connection](docs/connections/README.md#create_connection) - Create a
 connection * [delete_connection](docs/connections/README.md#delete_connection)
 - Get Connection details * [get_connection](docs/connections/
 README.md#get_connection) - Get Connection details * [list_connections](docs/
 connections/README.md#list_connections) - List connections ### [destinations]
```

### Comparing `airbyte-1.7.2/setup.py` & `airbyte-1.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="airbyte",
-    version="1.7.2",
+    version="1.8.0",
     author="Speakeasy",
     description="Python Client SDK for Airbyte API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `airbyte-1.7.2/src/airbyte/connections.py` & `airbyte-1.8.0/src/airbyte/connections.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/destinations.py` & `airbyte-1.8.0/src/airbyte/destinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/jobs.py` & `airbyte-1.8.0/src/airbyte/jobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/__init__.py` & `airbyte-1.8.0/src/airbyte/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/canceljob.py` & `airbyte-1.8.0/src/airbyte/models/operations/canceljob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/createconnection.py` & `airbyte-1.8.0/src/airbyte/models/operations/createconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/createdestination.py` & `airbyte-1.8.0/src/airbyte/models/operations/createdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/createjob.py` & `airbyte-1.8.0/src/airbyte/models/operations/createjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/createsource.py` & `airbyte-1.8.0/src/airbyte/models/operations/createsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/createworkspace.py` & `airbyte-1.8.0/src/airbyte/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/deleteconnection.py` & `airbyte-1.8.0/src/airbyte/models/operations/deleteconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/deletedestination.py` & `airbyte-1.8.0/src/airbyte/models/operations/deletedestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/deletesource.py` & `airbyte-1.8.0/src/airbyte/models/operations/deletesource.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getconnection.py` & `airbyte-1.8.0/src/airbyte/models/operations/getconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getdestination.py` & `airbyte-1.8.0/src/airbyte/models/operations/getdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getjob.py` & `airbyte-1.8.0/src/airbyte/models/operations/getjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getsource.py` & `airbyte-1.8.0/src/airbyte/models/operations/getsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getstreamproperties.py` & `airbyte-1.8.0/src/airbyte/models/operations/getstreamproperties.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/getworkspace.py` & `airbyte-1.8.0/src/airbyte/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/listconnections.py` & `airbyte-1.8.0/src/airbyte/models/operations/listconnections.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/listdestinations.py` & `airbyte-1.8.0/src/airbyte/models/operations/listdestinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/listjobs.py` & `airbyte-1.8.0/src/airbyte/models/operations/listjobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/listsources.py` & `airbyte-1.8.0/src/airbyte/models/operations/listsources.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/operations/listworkspaces.py` & `airbyte-1.8.0/src/airbyte/models/operations/listworkspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/__init__.py` & `airbyte-1.8.0/src/airbyte/models/shared/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,8 +252,8 @@
 from .streamconfiguration import *
 from .streamconfigurations import *
 from .streamproperties import *
 from .workspacecreaterequest import *
 from .workspaceresponse import *
 from .workspacesresponse import *
 
-__all__ = ["ConnectionCreateRequest","ConnectionCreateRequestNamespaceDefinitionEnum","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionSyncModeEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodAzureBlobStorageStaging","DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureBlobStorage","SourceAzureBlobStorageAzureBlobStorageEnum","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum","SourceFacebookMarketingInsightConfigValidBreakdownsEnum","SourceFacebookMarketingInsightConfigValidEnumsEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceQuickbooks","SourceQuickbooksCredentialsOAuth20","SourceQuickbooksCredentialsOAuth20AuthTypeEnum","SourceQuickbooksQuickbooksEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatJsonlUnexpectedFieldBehaviorEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyCredentialsTitleEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraZuoraEnum","SourcesResponse","StreamConfiguration","StreamConfigurations","StreamProperties","WorkspaceCreateRequest","WorkspaceResponse","WorkspacesResponse"]
+__all__ = ["ConnectionCreateRequest","ConnectionCreateRequestNamespaceDefinitionEnum","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionSyncModeEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodAzureBlobStorageStaging","DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureBlobStorage","SourceAzureBlobStorageAzureBlobStorageEnum","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceQuickbooks","SourceQuickbooksCredentialsOAuth20","SourceQuickbooksCredentialsOAuth20AuthTypeEnum","SourceQuickbooksQuickbooksEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyCredentialsTitleEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraZuoraEnum","SourcesResponse","StreamConfiguration","StreamConfigurations","StreamProperties","WorkspaceCreateRequest","WorkspaceResponse","WorkspacesResponse"]
```

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/connectioncreaterequest.py` & `airbyte-1.8.0/src/airbyte/models/shared/connectioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/connectionresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/connectionresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/connectionschedulecreate.py` & `airbyte-1.8.0/src/airbyte/models/shared/connectionschedulecreate.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/connectionscheduleresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/connectionscheduleresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/connectionsresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/connectionsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_amazon_sqs.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_aws_datalake.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_aws_datalake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_azure_blob_storage.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_bigquery.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_bigquery_denormalized.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_bigquery_denormalized.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_cassandra.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_cassandra.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_clickhouse.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_convex.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_convex.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_databend.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_databend.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_databricks.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_databricks.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_dynamodb.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_elasticsearch.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_firebolt.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_firestore.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_firestore.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_gcs.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_google_sheets.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_keen.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_keen.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_kinesis.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_kinesis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_mariadb_columnstore.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_mariadb_columnstore.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_meilisearch.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_meilisearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_mongodb.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_mssql.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_mysql.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_oracle.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_postgres.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_pubsub.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_pubsub.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_pulsar.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_pulsar.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_rabbitmq.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_redis.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_redis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_redshift.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_rockset.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_rockset.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_s3.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_s3_glue.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_s3_glue.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_scylla.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_scylla.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_sftp_json.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_sftp_json.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_snowflake.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destination_typesense.py` & `airbyte-1.8.0/src/airbyte/models/shared/destination_typesense.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destinationcreaterequest.py` & `airbyte-1.8.0/src/airbyte/models/shared/destinationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destinationresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/destinationresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/destinationsresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/destinationsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/jobcreaterequest.py` & `airbyte-1.8.0/src/airbyte/models/shared/jobcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/jobresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/jobresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/jobsresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/jobsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_airtable.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_airtable.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_alloydb.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_alloydb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_amazon_ads.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_amazon_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_amazon_seller_partner.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_amazon_seller_partner.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_amazon_sqs.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_amplitude.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_amplitude.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_apify_dataset.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_apify_dataset.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_asana.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_asana.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_auth0.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_auth0.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_aws_cloudtrail.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_aws_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_azure_blob_storage.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_azure_table.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_azure_table.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_bamboo_hr.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_bamboo_hr.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_bigcommerce.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_bigcommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_bigquery.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_bing_ads.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_bing_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_braintree.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_braintree.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_braze.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_braze.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_chargebee.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_chargebee.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_chartmogul.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_chartmogul.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_clickhouse.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_clickup_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_clickup_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_close_com.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_close_com.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_coda.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_coda.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_coin_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_coin_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_coinmarketcap.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_configcat.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_configcat.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_confluence.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_confluence.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_datascope.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_datascope.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_delighted.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_delighted.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_dixa.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_dixa.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_dockerhub.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_dockerhub.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_dremio.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_dremio.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_dynamodb.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_e2e_test_cloud.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_e2e_test_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_emailoctopus.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_emailoctopus.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_exchange_rates.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_exchange_rates.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_facebook_pages.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_facebook_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_faker.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_faker.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_fauna.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_fauna.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_file_secure.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_file_secure.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_firebolt.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_freshcaller.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_freshcaller.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_freshdesk.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_freshdesk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_freshsales.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_freshsales.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_gcs.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_getlago.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_getlago.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_github.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_github.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_gitlab.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_gitlab.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_glassfrog.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_glassfrog.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_gnews.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_gnews.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_ads.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_analytics_data_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_analytics_data_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_analytics_v4.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_analytics_v4.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_directory.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_directory.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_search_console.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_search_console.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_sheets.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_webfonts.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_webfonts.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_google_workspace_admin_reports.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_greenhouse.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_greenhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_gridly.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_gridly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_harvest.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_harvest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_hubplanner.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_hubplanner.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_hubspot.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_hubspot.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_insightly.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_insightly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_instagram.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_instagram.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_instatus.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_instatus.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_intercom.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_intercom.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_ip2whois.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_ip2whois.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_iterable.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_iterable.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_jira.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_jira.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_k6_cloud.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_k6_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_klarna.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_klarna.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_klaviyo.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_klaviyo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_kustomer_singer.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_kustomer_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_launchdarkly.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_launchdarkly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_lemlist.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_lemlist.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_linkedin_ads.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_linkedin_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_linkedin_pages.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_linkedin_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_linnworks.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_linnworks.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_lokalise.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_lokalise.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mailchimp.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mailchimp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mailgun.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mailgun.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mailjet_sms.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mailjet_sms.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_marketo.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_marketo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_metabase.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_metabase.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_microsoft_teams.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mixpanel.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mixpanel.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_monday.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_monday.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mongodb.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mssql.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_my_hours.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_my_hours.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_mysql.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_netsuite.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_netsuite.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_notion.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_notion.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_nytimes.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_nytimes.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 
-class SourceNytimesPeriodUsedForMostPopularStreamsEnum(str, Enum):
+class SourceNytimesPeriodUsedForMostPopularStreamsEnum(int, Enum):
     r"""Period of time (in days)"""
-    ONE = '1'
-    SEVEN = '7'
-    THIRTY = '30'
+    ONE = 1
+    SEVEN = 7
+    THIRTY = 30
 
 class SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum(str, Enum):
     r"""Share Type"""
     FACEBOOK = 'facebook'
 
 class SourceNytimesNytimesEnum(str, Enum):
     NYTIMES = 'nytimes'
```

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_okta.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_okta.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_omnisend.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_omnisend.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_onesignal.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_onesignal.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_openweather.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_openweather.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_oracle.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_orb.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_orb.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_orbit.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_orbit.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_outreach.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_outreach.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_paypal_transaction.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_paypal_transaction.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_paystack.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_paystack.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pendo.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pendo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_persistiq.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_persistiq.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pexels_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pexels_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pinterest.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pinterest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pipedrive.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pipedrive.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pocket.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pocket.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pokeapi.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pokeapi.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_polygon_stock_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_polygon_stock_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_postgres.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_posthog.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_posthog.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_postmarkapp.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_postmarkapp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_prestashop.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_prestashop.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_public_apis.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_public_apis.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_punk_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_punk_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_pypi.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_pypi.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_qualaroo.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_qualaroo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_quickbooks.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_quickbooks.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_railz.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_railz.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_recharge.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_recharge.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_recreation.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_recreation.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_recruitee.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_recruitee.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_recurly.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_recurly.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_redshift.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_retently.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_retently.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_rki_covid.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_rki_covid.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_rss.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_rss.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_s3.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,32 +6,26 @@
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 
 class SourceS3FormatJsonlFiletypeEnum(str, Enum):
     JSONL = 'jsonl'
 
-class SourceS3FormatJsonlUnexpectedFieldBehaviorEnum(str, Enum):
-    r"""How JSON fields outside of explicit_schema (if given) are treated. Check <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.json.ParseOptions.html\\" target=\\"_blank\\">PyArrow documentation</a> for details"""
-    IGNORE = 'ignore'
-    INFER = 'infer'
-    ERROR = 'error'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3FormatJsonl:
     r"""This connector uses <a href=\\"https://arrow.apache.org/docs/python/json.html\\" target=\\"_blank\\">PyArrow</a> for JSON Lines (jsonl) file parsing."""
     
     block_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_size'), 'exclude': lambda f: f is None }})
     r"""The chunk size in bytes to process at a time in memory from each file. If your data is particularly wide and failing during schema detection, increasing this should solve it. Beware of raising this too high as you could hit OOM errors."""
     filetype: Optional[SourceS3FormatJsonlFiletypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filetype'), 'exclude': lambda f: f is None }})
     newlines_in_values: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newlines_in_values'), 'exclude': lambda f: f is None }})
     r"""Whether newline characters are allowed in JSON values. Turning this on may affect performance. Leave blank to default to False."""
-    unexpected_field_behavior: Optional[SourceS3FormatJsonlUnexpectedFieldBehaviorEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unexpected_field_behavior'), 'exclude': lambda f: f is None }})
+    unexpected_field_behavior: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unexpected_field_behavior'), 'exclude': lambda f: f is None }})
     r"""How JSON fields outside of explicit_schema (if given) are treated. Check <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.json.ParseOptions.html\\" target=\\"_blank\\">PyArrow documentation</a> for details"""
     
 class SourceS3FormatAvroFiletypeEnum(str, Enum):
     AVRO = 'avro'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_salesforce.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_salesforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_salesforce_singer.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_salesforce_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_salesloft.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_salesloft.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sap_fieldglass.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sap_fieldglass.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_secoda.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_secoda.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sendgrid.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sendgrid.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sendinblue.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sendinblue.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_senseforce.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_senseforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sentry.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sentry.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sftp.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sftp.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sftp_bulk.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sftp_bulk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_shopify.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_shopify.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_shortio.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_shortio.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_slack.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_slack.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_smaily.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_smaily.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_smartengage.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_smartengage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_smartsheets.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_smartsheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_snapchat_marketing.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_snapchat_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_snowflake.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_sonar_cloud.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_spacex_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_spacex_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_square.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_square.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_strava.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_strava.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_stripe.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_stripe.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_survey_sparrow.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_survey_sparrow.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_surveymonkey.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_surveymonkey.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_tempo.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_tempo.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_the_guardian_api.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_the_guardian_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_tiktok_marketing.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_tiktok_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_todoist.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_todoist.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_trello.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_trello.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_trustpilot.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_trustpilot.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_tvmaze_schedule.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_tvmaze_schedule.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_twilio.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_twilio.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_twilio_taskrouter.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_twilio_taskrouter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_twitter.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_twitter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_typeform.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_typeform.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_us_census.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_us_census.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_vantage.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_vantage.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_webflow.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_webflow.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_whisky_hunter.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_whisky_hunter.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_wikipedia_pageviews.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_wikipedia_pageviews.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_woocommerce.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_woocommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_xero.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_xero.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_xkcd.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_xkcd.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_yandex_metrica.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_yandex_metrica.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_younium.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_younium.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_youtube_analytics.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_youtube_analytics.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_chat.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_chat.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_sunshine.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_sunshine.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_support.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_support.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zendesk_talk.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zendesk_talk.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zenloop.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zenloop.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zoho_crm.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zoho_crm.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zoom.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zoom.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/source_zuora.py` & `airbyte-1.8.0/src/airbyte/models/shared/source_zuora.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/sourcecreaterequest.py` & `airbyte-1.8.0/src/airbyte/models/shared/sourcecreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/sourceresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/sourceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/sourcesresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/sourcesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/streamconfiguration.py` & `airbyte-1.8.0/src/airbyte/models/shared/streamconfiguration.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/streamconfigurations.py` & `airbyte-1.8.0/src/airbyte/models/shared/streamconfigurations.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/streamproperties.py` & `airbyte-1.8.0/src/airbyte/models/shared/streamproperties.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/workspaceresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/workspaceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/models/shared/workspacesresponse.py` & `airbyte-1.8.0/src/airbyte/models/shared/workspacesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/sdk.py` & `airbyte-1.8.0/src/airbyte/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     streams: Streams
     workspaces: Workspaces
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.7.2"
-    _gen_version: str = "2.23.6"
+    _sdk_version: str = "1.8.0"
+    _gen_version: str = "2.24.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `airbyte-1.7.2/src/airbyte/sources.py` & `airbyte-1.8.0/src/airbyte/sources.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/streams.py` & `airbyte-1.8.0/src/airbyte/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/utils/retries.py` & `airbyte-1.8.0/src/airbyte/utils/retries.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte/utils/utils.py` & `airbyte-1.8.0/src/airbyte/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,15 +727,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return val.value
+        return str(val.value)
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

### Comparing `airbyte-1.7.2/src/airbyte/workspaces.py` & `airbyte-1.8.0/src/airbyte/workspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.2/src/airbyte.egg-info/PKG-INFO` & `airbyte-1.8.0/src/airbyte.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 1.7.2
+Version: 1.8.0
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -48,83 +48,83 @@
 
 
 req = shared.ConnectionCreateRequest(
     configurations=shared.StreamConfigurations(
         streams=[
             shared.StreamConfiguration(
                 cursor_field=[
-                    "distinctio",
-                    "quibusdam",
-                    "unde",
+                    'distinctio',
+                    'quibusdam',
+                    'unde',
                 ],
-                name="Johnnie Stamm",
+                name='Johnnie Stamm',
                 primary_key=[
                     [
-                        "iure",
-                        "magnam",
+                        'iure',
+                        'magnam',
                     ],
                     [
-                        "ipsa",
-                        "delectus",
-                        "tempora",
-                        "suscipit",
+                        'ipsa',
+                        'delectus',
+                        'tempora',
+                        'suscipit',
                     ],
                     [
-                        "minus",
-                        "placeat",
+                        'minus',
+                        'placeat',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "excepturi",
-                    "nisi",
+                    'excepturi',
+                    'nisi',
                 ],
-                name="Jake Bernier MD",
+                name='Jake Bernier MD',
                 primary_key=[
                     [
-                        "repellendus",
-                        "sapiente",
+                        'repellendus',
+                        'sapiente',
                     ],
                 ],
-                sync_mode="incremental_deduped_history",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY,
             ),
             shared.StreamConfiguration(
                 cursor_field=[
-                    "at",
+                    'at',
                 ],
-                name="Emilio Krajcik",
+                name='Emilio Krajcik',
                 primary_key=[
                     [
-                        "porro",
-                        "dolorum",
-                        "dicta",
+                        'porro',
+                        'dolorum',
+                        'dicta',
                     ],
                     [
-                        "officia",
-                        "occaecati",
-                        "fugit",
+                        'officia',
+                        'occaecati',
+                        'fugit',
                     ],
                 ],
-                sync_mode="incremental_append",
+                sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
-    data_residency="eu",
-    destination_id="c816742c-b739-4205-9293-96fea7596eb1",
-    name="Lela Orn",
-    namespace_definition="source",
-    namespace_format="${SOURCE_NAMESPACE}",
-    prefix="dolorem",
+    data_residency=shared.GeographyEnumEnum.EU,
+    destination_id='c816742c-b739-4205-9293-96fea7596eb1',
+    name='Lela Orn',
+    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_format='${SOURCE_NAMESPACE}',
+    prefix='dolorem',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression="corporis",
-        schedule_type="manual",
+        cron_expression='corporis',
+        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
     ),
-    source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
+    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte Version: 1.7.2 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: airbyte Version: 1.8.0 Summary: Python Client SDK
 for Airbyte API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
 File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
@@ -21,28 +21,31 @@
 (Installation will not work until published to a package manager, please
 install locally to try it out `pip install -e ../path/to/local/clone`)  ## SDK
 Installation ```bash pip install airbyte ```  ## SDK Example Usage  ```python
 import airbyte from airbyte.models import shared s = airbyte.Airbyte
 ( security=shared.Security( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), )
 req = shared.ConnectionCreateRequest
 ( configurations=shared.StreamConfigurations( streams=
-[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
-], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
-"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
-sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
-[ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
-[ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
-shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
-primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
-"fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
-destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
-namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
-prefix="dolorem", schedule=shared.ConnectionScheduleCreate
-( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
-aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
+[ shared.StreamConfiguration( cursor_field=[ 'distinctio', 'quibusdam', 'unde',
+], name='Johnnie Stamm', primary_key=[ [ 'iure', 'magnam', ], [ 'ipsa',
+'delectus', 'tempora', 'suscipit', ], [ 'minus', 'placeat', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND, ),
+shared.StreamConfiguration( cursor_field=[ 'excepturi', 'nisi', ], name='Jake
+Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
+sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
+shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
+primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
+'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
+), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
+b739-4205-9293-96fea7596eb1', name='Lela Orn',
+namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
+schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
+schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
+4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
 Resources and Operations ### [connections](docs/connections/README.md) *
 [create_connection](docs/connections/README.md#create_connection) - Create a
 connection * [delete_connection](docs/connections/README.md#delete_connection)
 - Get Connection details * [get_connection](docs/connections/
 README.md#get_connection) - Get Connection details * [list_connections](docs/
 connections/README.md#list_connections) - List connections ### [destinations]
```

### Comparing `airbyte-1.7.2/src/airbyte.egg-info/SOURCES.txt` & `airbyte-1.8.0/src/airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

