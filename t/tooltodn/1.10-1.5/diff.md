# Comparing `tmp/tooltodn-1.10.tar.gz` & `tmp/tooltodn-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooltodn-1.10.tar", last modified: Wed May  3 11:42:52 2023, max compression
+gzip compressed data, was "tooltodn-1.5.tar", last modified: Wed May  3 11:40:52 2023, max compression
```

## Comparing `tooltodn-1.10.tar` & `tooltodn-1.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.069829 tooltodn-1.10/
--rw-r--r--   0 ab         (501) staff       (20)     1944 2023-05-03 11:42:52.069918 tooltodn-1.10/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     1686 2023-04-25 10:03:18.000000 tooltodn-1.10/README.md
--rw-r--r--   0 ab         (501) staff       (20)      172 2023-05-03 11:42:52.070337 tooltodn-1.10/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1053 2023-05-03 11:42:50.000000 tooltodn-1.10/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.055681 tooltodn-1.10/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.056644 tooltodn-1.10/src/dna_audit_tool/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 11:03:22.000000 tooltodn-1.10/src/dna_audit_tool/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.057129 tooltodn-1.10/src/dna_audit_tool/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.057955 tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.058716 tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.059583 tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1707 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     8531 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.060387 tooltodn-1.10/src/dna_audit_tool/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.061289 tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.062159 tooltodn-1.10/src/dna_audit_tool/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.062852 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.063470 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.064028 tooltodn-1.10/src/dna_audit_tool/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.064726 tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13466 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.065371 tooltodn-1.10/src/dna_audit_tool/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.066005 tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10942 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.066275 tooltodn-1.10/src/dna_audit_tool/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.066588 tooltodn-1.10/src/dna_audit_tool/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2102 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.067131 tooltodn-1.10/src/dna_audit_tool/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6304 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.067505 tooltodn-1.10/src/dna_audit_tool/common/templates/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/templates/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.068420 tooltodn-1.10/src/dna_audit_tool/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10224 2023-05-03 11:18:37.000000 tooltodn-1.10/src/dna_audit_tool/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1451 2023-05-03 10:19:26.000000 tooltodn-1.10/src/dna_audit_tool/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     2080 2023-05-03 11:20:40.000000 tooltodn-1.10/src/dna_audit_tool/main.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:42:52.069661 tooltodn-1.10/src/tooltodn.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     1944 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2906 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       56 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       20 2023-05-03 11:42:52.000000 tooltodn-1.10/src/tooltodn.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.720364 tooltodn-1.5/
+-rw-r--r--   0 ab         (501) staff       (20)     1943 2023-05-03 11:40:52.720479 tooltodn-1.5/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     1686 2023-04-25 10:03:18.000000 tooltodn-1.5/README.md
+-rw-r--r--   0 ab         (501) staff       (20)      172 2023-05-03 11:40:52.721005 tooltodn-1.5/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1047 2023-05-03 11:40:47.000000 tooltodn-1.5/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.706040 tooltodn-1.5/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.706901 tooltodn-1.5/src/dna_audit_tool/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 11:03:22.000000 tooltodn-1.5/src/dna_audit_tool/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.707235 tooltodn-1.5/src/dna_audit_tool/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.707913 tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.708572 tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.709276 tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1707 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     8531 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.710185 tooltodn-1.5/src/dna_audit_tool/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.711030 tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.711950 tooltodn-1.5/src/dna_audit_tool/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.712561 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.713291 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.714320 tooltodn-1.5/src/dna_audit_tool/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.714930 tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13466 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.715568 tooltodn-1.5/src/dna_audit_tool/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.716143 tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10942 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.716443 tooltodn-1.5/src/dna_audit_tool/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.716719 tooltodn-1.5/src/dna_audit_tool/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2102 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.717146 tooltodn-1.5/src/dna_audit_tool/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6304 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.717392 tooltodn-1.5/src/dna_audit_tool/common/templates/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/templates/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.718203 tooltodn-1.5/src/dna_audit_tool/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10224 2023-05-03 11:18:37.000000 tooltodn-1.5/src/dna_audit_tool/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1451 2023-05-03 10:19:26.000000 tooltodn-1.5/src/dna_audit_tool/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     2080 2023-05-03 11:20:40.000000 tooltodn-1.5/src/dna_audit_tool/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-03 11:40:52.720195 tooltodn-1.5/src/tooltodn.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     1943 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2906 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       51 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       20 2023-05-03 11:40:52.000000 tooltodn-1.5/src/tooltodn.egg-info/top_level.txt
```

### Comparing `tooltodn-1.10/PKG-INFO` & `tooltodn-1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooltodn
-Version: 1.10
+Version: 1.5
 Summary: Data And Analytics Audit Tool
 Home-page: UNKNOWN
 Author: Bhanuja
 Author-email: abhanuja@presidio.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `tooltodn-1.10/README.md` & `tooltodn-1.5/README.md`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/setup.py` & `tooltodn-1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tooltodn",                
-    version="1.10",                        
+    version="1.5",                        
     author="Bhanuja",  
     author_email="abhanuja@presidio.com",
     license= 'MIT',              
     description="Data And Analytics Audit Tool",
     long_description=long_description,     
     long_description_content_type="text/markdown",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=['main'],
     entry_points={
         'console_scripts': [
-            'my_c1=dna_audit_tool:main.callhere'
+            'my_c1=dna_audit_tool:callhere'
         ]
     },
     include_package_data=True,
     python_requires='>=3.6',                
     install_requires=["boto3==1.26.85","nose==1.3.7","Jinja2==3.1.2","moto==4.1.4","docker==6.0.1","pyparsing==3.0.9","openapi_spec_validator==0.5.6"]                    
 )
```

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/api_gateway_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/api_gateway/api_gateway_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/lambda_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/dat_lambda/lambda_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/dynamodb_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/dynamodb/dynamodb_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/emr/emr_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/emr/emr_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/fargate_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/fargate/fargate_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/glue/glue_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/glue/glue_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/firehose_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/rds/rds_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/rds/rds_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/redshift_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/redshift/redshift_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/s3/s3_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/s3/s3_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/sqs_constants.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/aws_services/sqs/sqs_service.py` & `tooltodn-1.5/src/dna_audit_tool/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/common/constants/application_constants.py` & `tooltodn-1.5/src/dna_audit_tool/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/common/service/dat_service.py` & `tooltodn-1.5/src/dna_audit_tool/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/common/utils/helper.py` & `tooltodn-1.5/src/dna_audit_tool/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/common/utils/instance_initializer.py` & `tooltodn-1.5/src/dna_audit_tool/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/dna_audit_tool/main.py` & `tooltodn-1.5/src/dna_audit_tool/main.py`

 * *Files identical despite different names*

### Comparing `tooltodn-1.10/src/tooltodn.egg-info/PKG-INFO` & `tooltodn-1.5/src/tooltodn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooltodn
-Version: 1.10
+Version: 1.5
 Summary: Data And Analytics Audit Tool
 Home-page: UNKNOWN
 Author: Bhanuja
 Author-email: abhanuja@presidio.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `tooltodn-1.10/src/tooltodn.egg-info/SOURCES.txt` & `tooltodn-1.5/src/tooltodn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

