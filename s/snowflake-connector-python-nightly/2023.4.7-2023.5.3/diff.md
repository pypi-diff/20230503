# Comparing `tmp/snowflake-connector-python-nightly-2023.4.7.tar.gz` & `tmp/snowflake-connector-python-nightly-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2023.4.7.tar", last modified: Fri Apr  7 04:06:51 2023, max compression
+gzip compressed data, was "snowflake-connector-python-nightly-2023.5.3.tar", last modified: Wed May  3 04:06:54 2023, max compression
```

## Comparing `snowflake-connector-python-nightly-2023.4.7.tar` & `snowflake-connector-python-nightly-2023.5.3.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.348451 snowflake-connector-python-nightly-2023.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-07 04:06:27.000000 snowflake-connector-python-nightly-2023.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    46191 2023-04-07 04:06:27.000000 snowflake-connector-python-nightly-2023.4.7/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-07 04:06:27.000000 snowflake-connector-python-nightly-2023.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 04:06:27.000000 snowflake-connector-python-nightly-2023.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 04:06:28.000000 snowflake-connector-python-nightly-2023.4.7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-07 04:06:51.348451 snowflake-connector-python-nightly-2023.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-07 04:06:28.000000 snowflake-connector-python-nightly-2023.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-07 04:06:28.000000 snowflake-connector-python-nightly-2023.4.7/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-07 04:06:28.000000 snowflake-connector-python-nightly-2023.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-07 04:06:51.348451 snowflake-connector-python-nightly-2023.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-04-07 04:06:28.000000 snowflake-connector-python-nightly-2023.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.328450 snowflake-connector-python-nightly-2023.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.324450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.336450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.336450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    63767 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-07 04:06:31.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.328450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-07 04:06:34.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-07 04:06:35.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    54567 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    46618 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39670 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    68441 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16816 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:32.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.340450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 04:06:36.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    33230 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.344450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    39093 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.344450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.344450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-07 04:06:37.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.344450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.344450 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.348451 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-07 04:06:38.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-07 04:06:39.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 04:06:33.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 04:06:51.348451 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 04:06:51.000000 snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-03 04:06:36.000000 snowflake-connector-python-nightly-2023.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    47245 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-03 04:06:37.000000 snowflake-connector-python-nightly-2023.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.347390 snowflake-connector-python-nightly-2023.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.347390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.355390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/arrow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/arrow_iterator.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.355390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64210 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.347390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-05-03 04:06:42.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    56974 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47199 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39886 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68441 2023-05-03 04:06:39.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 04:06:40.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-03 04:06:43.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.359390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.363390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.363390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.363390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-03 04:06:44.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-03 04:06:45.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 04:06:41.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:06:54.367390 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 04:06:54.000000 snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/CONTRIBUTING.md` & `snowflake-connector-python-nightly-2023.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/DESCRIPTION.md` & `snowflake-connector-python-nightly-2023.5.3/DESCRIPTION.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,31 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
-- v3.0.3(TBD)
+- v3.0.4(TBD)
+  - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
+  - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
+  - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
+  - Bumped vendored library urllib3 to 1.26.15
+  - Bumped vendored library requests to 2.29.0
+  - Fixed a bug when `_prefetch_hook()` was not called before yielding results of `execute_async()`.
 
+- v3.0.3(April 20, 2023)
   - Fixed a bug that prints error in logs for GET command on GCS.
   - Added a parameter that allows users to skip file uploads to stage if file exists on stage and contents of the file match.
-  - Fixed a bug when writing a Pandas DataFrame with non-default index in `snowflake.connector.pandas_tool.write_pandas`.
-  - Fixed a bug when writing a Pandas DataFrame with column names containing double quotes in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with non-default index in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with column names containing double quotes in `snowflake.connector.pandas_tool.write_pandas`.
+  - Fixed a bug that occurred when writing a Pandas DataFrame with binary data in `snowflake.connector.pandas_tool.write_pandas`.
+  - Improved type hint of `SnowflakeCursor.execute` method.
+  - Fail instantly upon receiving `403: Forbidden` HTTP response for a login-request.
+  - Improved GET logging to warn when downloading multiple files with the same name.
 
 - v3.0.2(March 23, 2023)
 
   - Fixed a memory leak in the logging module of the Cython extension.
   - Fixed a bug where the `put` command on AWS raised `AttributeError` when uploading file composed of multiple parts.
   - Fixed a bug of incorrect type hints of `SnowflakeCursor.fetch_arrow_all` and `SnowflakeCursor.fetchall`.
   - Fixed a bug where `snowflake.connector.util_text.split_statements` swallows the final line break in the case when there are no space between lines.
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/LICENSE.txt` & `snowflake-connector-python-nightly-2023.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/MANIFEST.in` & `snowflake-connector-python-nightly-2023.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/PKG-INFO` & `snowflake-connector-python-nightly-2023.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.4.7
+Version: 2023.5.3
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/README.md` & `snowflake-connector-python-nightly-2023.5.3/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/pyproject.toml` & `snowflake-connector-python-nightly-2023.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/setup.cfg` & `snowflake-connector-python-nightly-2023.5.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 	pyOpenSSL>=16.2.0,<24.0.0
 	pycryptodomex!=3.5.0,>=3.2,<4.0.0
 	pyjwt<3.0.0
 	pytz
 	requests<3.0.0
 	importlib-metadata; python_version < '3.8'
 	packaging
-	charset_normalizer>=2,<3
+	charset_normalizer>=2,<4
 	idna>=2.5,<4
 	urllib3>=1.21.1,<1.27
 	certifi>=2017.4.17
 	typing_extensions>=4.3,<5
 	filelock>=3.5,<4
 include_package_data = True
 package_dir = 
@@ -81,15 +81,15 @@
 development = 
 	Cython
 	coverage
 	more-itertools
 	numpy<1.25.0
 	pendulum!=2.1.1
 	pexpect
-	pytest<7.3.0
+	pytest<7.4.0
 	pytest-cov
 	pytest-rerunfailures
 	pytest-timeout
 	pytest-xdist
 	pytzdata
 pandas = 
 	pandas>=1.0.0,<1.6.0
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/setup.py` & `snowflake-connector-python-nightly-2023.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,11 +204,11 @@
                 ret.append(source)
 
             return ret
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2023.04.07",
+    version="2023.05.03",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/__init__.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/by_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,20 +206,21 @@
         jitter to deduce the time to sleep before retrying. The sleep
         time ranges between 1 and 16 seconds.
         """
 
         del authenticator, service_name, account, user, password
         logger.debug("Default timeout handler invoked for authenticator")
         if not self._retry_ctx.should_retry():
-            self._retry_ctx.reset()
-            raise OperationalError(
+            error = OperationalError(
                 msg=f"Could not connect to Snowflake backend after {self._retry_ctx.get_current_retry_count()} attempt(s)."
                 "Aborting",
                 errno=ER_FAILED_TO_CONNECT_TO_DB,
             )
+            self._retry_ctx.reset()
+            raise error
         else:
             logger.debug(
                 f"Hit connection timeout, attempt number {self._retry_ctx.get_current_retry_count()}."
                 " Will retry in a bit..."
             )
             self._retry_ctx.increment_retry()
             time.sleep(self._retry_ctx.next_sleep_duration())
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cache.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/compat.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/connection.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,18 @@
         None,
         (type(None), str),
     ),  # Path to connection diag whitelist json
     "log_imported_packages_in_telemetry": (
         True,
         bool,
     ),  # Whether to log imported packages in telemetry
+    "json_result_force_utf8_decoding": (
+        False,
+        bool,
+    ),  # Whether to force the JSON content to be decoded in utf-8, it is only effective when result format is JSON
 }
 
 APPLICATION_RE = re.compile(r"[\w\d_]+")
 
 # adding the exception class to Connection class
 for m in [method for method in dir(errors) if callable(getattr(errors, method))]:
     setattr(sys.modules[__name__], m, getattr(errors, m))
@@ -261,14 +265,17 @@
         is_pyformat: Whether the current argument binding is pyformat or format.
         consent_cache_id_token: Consented cache ID token.
         use_openssl_only: Use OpenSSL instead of pure Python libraries for signature verification and encryption.
         enable_stage_s3_privatelink_for_us_east_1: when true, clients use regional s3 url to upload files.
         enable_connection_diag: when true, clients will generate a connectivity diagnostic report.
         connection_diag_log_path: path to location to create diag report with enable_connection_diag.
         connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag.
+        json_result_force_utf8_decoding: When true, json result will be decoded in utf-8,
+          when false, the encoding of the content is auto-detected. Default value is false.
+          This parameter is only effective when the result format is JSON.
     """
 
     OCSP_ENV_LOCK = Lock()
 
     def __init__(self, **kwargs) -> None:
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/constants.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/cursor.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 from threading import Lock, Timer
 from types import TracebackType
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     Callable,
-    Generator,
     Iterator,
     NamedTuple,
     NoReturn,
     Sequence,
     TypeVar,
     overload,
 )
 
-from typing_extensions import Self
+from typing_extensions import Literal, Self
 
 from snowflake.connector.result_batch import create_batches_from_response
 from snowflake.connector.result_set import ResultSet
 
 from . import compat
 from ._sql_util import get_file_transfer_type
 from .bind_upload_agent import BindUploadAgent, BindUploadError
@@ -59,15 +58,14 @@
     DatabaseError,
     Error,
     IntegrityError,
     InterfaceError,
     NotSupportedError,
     ProgrammingError,
 )
-from .file_transfer_agent import SnowflakeFileTransferAgent
 from .options import installed_pandas
 from .sqlstate import SQLSTATE_FEATURE_NOT_SUPPORTED
 from .telemetry import TelemetryData, TelemetryField
 from .time_util import get_time_millis
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
@@ -603,14 +601,74 @@
             and len(processed_params) > 0
         ):
             query = command % processed_params
         else:
             query = command
         return query
 
+    @overload
+    def execute(
+        self,
+        command: str,
+        params: Sequence[Any] | dict[Any, Any] | None = None,
+        _bind_stage: str | None = None,
+        timeout: int | None = None,
+        _exec_async: bool = False,
+        _no_retry: bool = False,
+        _do_reset: bool = True,
+        _put_callback: SnowflakeProgressPercentage = None,
+        _put_azure_callback: SnowflakeProgressPercentage = None,
+        _put_callback_output_stream: IO[str] = sys.stdout,
+        _get_callback: SnowflakeProgressPercentage = None,
+        _get_azure_callback: SnowflakeProgressPercentage = None,
+        _get_callback_output_stream: IO[str] = sys.stdout,
+        _show_progress_bar: bool = True,
+        _statement_params: dict[str, str] | None = None,
+        _is_internal: bool = False,
+        _describe_only: bool = False,
+        _no_results: Literal[False] = False,
+        _is_put_get: bool | None = None,
+        _raise_put_get_error: bool = True,
+        _force_put_overwrite: bool = False,
+        _skip_upload_on_content_match: bool = False,
+        file_stream: IO[bytes] | None = None,
+        num_statements: int | None = None,
+    ) -> Self | None:
+        ...
+
+    @overload
+    def execute(
+        self,
+        command: str,
+        params: Sequence[Any] | dict[Any, Any] | None = None,
+        _bind_stage: str | None = None,
+        timeout: int | None = None,
+        _exec_async: bool = False,
+        _no_retry: bool = False,
+        _do_reset: bool = True,
+        _put_callback: SnowflakeProgressPercentage = None,
+        _put_azure_callback: SnowflakeProgressPercentage = None,
+        _put_callback_output_stream: IO[str] = sys.stdout,
+        _get_callback: SnowflakeProgressPercentage = None,
+        _get_azure_callback: SnowflakeProgressPercentage = None,
+        _get_callback_output_stream: IO[str] = sys.stdout,
+        _show_progress_bar: bool = True,
+        _statement_params: dict[str, str] | None = None,
+        _is_internal: bool = False,
+        _describe_only: bool = False,
+        _no_results: Literal[True] = True,
+        _is_put_get: bool | None = None,
+        _raise_put_get_error: bool = True,
+        _force_put_overwrite: bool = False,
+        _skip_upload_on_content_match: bool = False,
+        file_stream: IO[bytes] | None = None,
+        num_statements: int | None = None,
+    ) -> dict[str, Any] | None:
+        ...
+
     def execute(
         self,
         command: str,
         params: Sequence[Any] | dict[Any, Any] | None = None,
         _bind_stage: str | None = None,
         timeout: int | None = None,
         _exec_async: bool = False,
@@ -647,15 +705,16 @@
             _put_callback: Function to which GET command should call back to.
             _put_azure_callback: Function to which an Azure GET command should call back to.
             _put_callback_output_stream: The output stream a PUT command's callback should report on.
             _get_callback: Function to which GET command should call back to.
             _get_azure_callback: Function to which an Azure GET command should call back to.
             _get_callback_output_stream: The output stream a GET command's callback should report on.
             _show_progress_bar: Whether or not to show progress bar.
-            _statement_params: Extra information that should be sent to Snowflake with query.
+            _statement_params: Extra information that should be sent to Snowflake with query. This dict will not be
+                modified by the connector.
             _is_internal: This flag indicates whether the query is issued internally by the connector.
             _describe_only: If true, the query will not be executed but return the schema/description of this query.
             _no_results: This flag tells the back-end to not return the result, just fire the query and return the
                 response returned by Snowflake's server.
             _use_ijson: This flag doesn't do anything as ijson support has ended.
             _is_put_get: Force decision of this SQL query being a PUT, or GET command. This is detected otherwise.
             _raise_put_get_error: Whether to raise PUT and GET errors.
@@ -685,19 +744,22 @@
         if _do_reset:
             self.reset()
         command = command.strip(" \t\n\r") if command else None
         if not command:
             logger.warning("execute: no query is given to execute")
             return None
 
-        if _statement_params is None:
-            _statement_params = dict()
-
-        if num_statements:
-            _statement_params["MULTI_STATEMENT_COUNT"] = num_statements
+        _statement_params = _statement_params or dict()
+        # If we need to add another parameter, please consider introducing a dict for all extra params
+        # See discussion in https://github.com/snowflakedb/snowflake-connector-python/pull/1524#discussion_r1174061775
+        if num_statements is not None:
+            _statement_params = {
+                **_statement_params,
+                "MULTI_STATEMENT_COUNT": num_statements,
+            }
 
         kwargs: dict[str, Any] = {
             "timeout": timeout,
             "statement_params": _statement_params,
             "is_internal": _is_internal,
             "describe_only": _describe_only,
             "_no_results": _no_results,
@@ -782,14 +844,16 @@
 
             self._is_file_transfer = "command" in data and data["command"] in (
                 "UPLOAD",
                 "DOWNLOAD",
             )
             logger.debug("PUT OR GET: %s", self.is_file_transfer)
             if self.is_file_transfer:
+                from .file_transfer_agent import SnowflakeFileTransferAgent
+
                 # Decide whether to use the old, or new code path
                 sf_file_transfer_agent = SnowflakeFileTransferAgent(
                     self,
                     query,
                     ret,
                     put_callback=_put_callback,
                     put_azure_callback=_put_azure_callback,
@@ -1173,45 +1237,38 @@
                 seqparams
             )
 
             self.execute(query, params, _do_reset=False, **kwargs)
 
         return self
 
-    def _result_iterator(
-        self,
-    ) -> Generator[dict, None, None] | Generator[tuple, None, None]:
-        """Yields the elements from _result and raises an exception when appropriate."""
-        try:
-            for _next in self._result:
-                if isinstance(_next, Exception):
-                    Error.errorhandler_wrapper_from_ready_exception(
-                        self._connection,
-                        self,
-                        _next,
-                    )
-                self._rownumber += 1
-                yield _next
-        except TypeError as err:
-            if self._result_state == ResultState.DEFAULT:
-                raise err
-            else:
-                yield None
-
     def fetchone(self) -> dict | tuple | None:
         """Fetches one row."""
         if self._prefetch_hook is not None:
             self._prefetch_hook()
         if self._result is None and self._result_set is not None:
             self._result = iter(self._result_set)
             self._result_state = ResultState.VALID
+
         try:
-            return next(self._result_iterator())
-        except StopIteration:
-            return None
+            _next = next(self._result, None)
+            if isinstance(_next, Exception):
+                Error.errorhandler_wrapper_from_ready_exception(
+                    self._connection,
+                    self,
+                    _next,
+                )
+            if _next is not None:
+                self._rownumber += 1
+            return _next
+        except TypeError as err:
+            if self._result_state == ResultState.DEFAULT:
+                raise err
+            else:
+                return None
 
     def fetchmany(self, size: int | None = None) -> list[tuple] | list[dict]:
         """Fetches the number of specified rows."""
         if size is None:
             size = self.arraysize
 
         if size < 0:
@@ -1247,14 +1304,16 @@
 
     def nextset(self) -> SnowflakeCursor | None:
         """
         Fetches the next set of results if the previously executed query was multi-statement so that subsequent calls
         to any of the fetch*() methods will return rows from the next query's set of results. Returns None if no more
         query results are available.
         """
+        if self._prefetch_hook is not None:
+            self._prefetch_hook()
         self.reset()
         if self._multi_statement_resultIds:
             self.query_result(self._multi_statement_resultIds[0])
             logger.info(
                 f"Retrieved results for query ID: {self._multi_statement_resultIds.popleft()}"
             )
             return self
@@ -1298,19 +1357,19 @@
             self._inner_cursor = None
         self._prefetch_hook = None
         if not self.connection._reuse_results:
             self._result_set = None
 
     def __iter__(self) -> Iterator[dict] | Iterator[tuple]:
         """Iteration over the result set."""
-        # set _result if _result_set is not None
-        if self._result is None and self._result_set is not None:
-            self._result = iter(self._result_set)
-            self._result_state = ResultState.VALID
-        return self._result_iterator()
+        while True:
+            _next = self.fetchone()
+            if _next is None:
+                break
+            yield _next
 
     def __cancel_query(self, query) -> None:
         if self._sequence_counter >= 0 and not self.is_closed():
             logger.debug("canceled. %s, request_id: %s", query, self._request_id)
             with self._lock_canceling:
                 self._connection._cancel_query(query, self._request_id)
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/description.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/errors.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_transfer_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1013,42 +1013,55 @@
                             stage_location_type=self._stage_location_type,
                             encryption_material=self._encryption_material[0]
                             if len(self._encryption_material) > 0
                             else None,
                         )
                     )
         elif self._command_type == CMD_TYPE_DOWNLOAD:
+            basename_counts = dict()
             for idx, file_name in enumerate(self._src_files):
                 if not file_name:
                     continue
                 first_path_sep = file_name.find("/")
                 dst_file_name = (
                     file_name[first_path_sep + 1 :]
                     if first_path_sep >= 0
                     else file_name
                 )
                 url = None
                 if self._presigned_urls and idx < len(self._presigned_urls):
                     url = self._presigned_urls[idx]
+
+                basename = os.path.basename(file_name)
+                basename_counts[basename] = basename_counts.get(basename, 0) + 1
+
                 self._file_metadata.append(
                     SnowflakeFileMeta(
-                        name=os.path.basename(file_name),
+                        name=basename,
                         src_file_name=file_name,
                         dst_file_name=dst_file_name,
                         stage_location_type=self._stage_location_type,
                         local_location=self._local_location,
                         presigned_url=url,
                         encryption_material=self._src_file_to_encryption_material[
                             file_name
                         ]
                         if file_name in self._src_file_to_encryption_material
                         else None,
                     )
                 )
 
+            # TODO: remove this warning once we support directory structure for GET
+            duplicate_basenames = [k for k, v in basename_counts.items() if v > 1]
+            if duplicate_basenames:
+                logger.warning(
+                    f"Downloading multiple files with the same name could cause failures. "
+                    f"File names with multiple entries: {duplicate_basenames}"
+                )
+
     def _process_file_compression_type(self) -> None:
         user_specified_source_compression = None
         if self._source_compression == "auto_detect":
             auto_detect = True
         elif self._source_compression == "none":
             auto_detect = False
         else:
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/file_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/network.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,18 @@
             "msg": f"{response.status_code} {response.reason}: {method} {url}",
             "errno": ER_FAILED_TO_REQUEST,
             "sqlstate": SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED,
         },
     )
 
 
+def is_login_request(url: str) -> bool:
+    return "/session/v1/login-request" in url
+
+
 class ProxySupportAdapter(HTTPAdapter):
     """This Adapter creates proper headers for Proxy CONNECT messages."""
 
     def get_connection(
         self, url: str, proxies: OrderedDict | None = None
     ) -> HTTPConnectionPool | HTTPSConnectionPool:
         proxy = select_proxy(url, proxies)
@@ -1051,15 +1055,18 @@
                         ret = binary_data_handler.to_iterator(
                             raw_ret.raw, download_end_time - download_start_time
                         )
                     else:
                         ret = raw_ret.json()
                     return ret
 
-                if is_retryable_http_code(raw_ret.status_code):
+                if is_login_request(full_url) and raw_ret.status_code == FORBIDDEN:
+                    raise ForbiddenError
+
+                elif is_retryable_http_code(raw_ret.status_code):
                     error = get_http_retryable_error(raw_ret.status_code)
                     logger.debug(f"{error}. Retrying...")
                     # retryable server exceptions
                     raise RetryRequest(error)
 
                 elif (
                     raw_ret.status_code == UNAUTHORIZED
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/options.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     """
     try:
         pandas = importlib.import_module("pandas")
         # since we enable relative imports without dots this import gives us an issues when ran from test directory
         from pandas import DataFrame  # NOQA
 
         pyarrow = importlib.import_module("pyarrow")
+
         # Check whether we have the currently supported pyarrow installed
         installed_packages = {
             package.metadata["Name"]: package for package in distributions()
         }
         if {"pyarrow", "snowflake-connector-python"} <= installed_packages.keys():
             dependencies = installed_packages[
                 "snowflake-connector-python"
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/pandas_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,21 +218,18 @@
     # in Snowflake, all parquet data is stored in a single column, $1, so we must select columns explicitly
     # see (https://docs.snowflake.com/en/user-guide/script-data-load-transform-parquet.html)
     if quote_identifiers:
         quote = '"'
         # if the column name contains a double quote, we need to escape it by replacing with two double quotes
         # https://docs.snowflake.com/en/sql-reference/identifiers-syntax#double-quoted-identifiers
         snowflake_column_names = [str(c).replace('"', '""') for c in df.columns]
-        columns = '"' + '","'.join(snowflake_column_names) + '"'
-        parquet_columns = "$1:" + ",$1:".join(f'"{c}"' for c in snowflake_column_names)
     else:
         quote = ""
         snowflake_column_names = list(df.columns)
-        columns = ",".join(snowflake_column_names)
-        parquet_columns = "$1:" + ",$1:".join(snowflake_column_names)
+    columns = quote + f"{quote},{quote}".join(snowflake_column_names) + quote
 
     def drop_object(name: str, object_type: str) -> None:
         drop_sql = f"DROP {object_type.upper()} IF EXISTS {name} /* Python:snowflake.connector.pandas_tools.write_pandas() */"
         logger.debug(f"dropping {object_type} with '{drop_sql}'")
         cursor.execute(drop_sql, _is_internal=True)
 
     if auto_create_table or overwrite:
@@ -275,28 +272,36 @@
         create_table_sql = (
             f"CREATE {table_type.upper()} TABLE IF NOT EXISTS {target_table_location} "
             f"({create_table_columns})"
             f" /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
         )
         logger.debug(f"auto creating table with '{create_table_sql}'")
         cursor.execute(create_table_sql, _is_internal=True)
+        # need explicit casting when the underlying table schema is inferred
+        parquet_columns = "$1:" + ",$1:".join(
+            f"{quote}{snowflake_col}{quote}::{column_type_mapping[col]}"
+            for snowflake_col, col in zip(snowflake_column_names, df.columns)
+        )
     else:
         target_table_location = build_location_helper(
             database=database,
             schema=schema,
             name=table_name,
             quote_identifiers=quote_identifiers,
         )
+        parquet_columns = "$1:" + ",$1:".join(
+            f"{quote}{snowflake_col}{quote}" for snowflake_col in snowflake_column_names
+        )
 
     try:
         copy_into_sql = (
             f"COPY INTO {target_table_location} /* Python:snowflake.connector.pandas_tools.write_pandas() */ "
             f"({columns}) "
             f"FROM (SELECT {parquet_columns} FROM @{stage_location}) "
-            f"FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression_map[compression]}) "
+            f"FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression_map[compression]}{' BINARY_AS_TEXT=FALSE' if auto_create_table or overwrite else ''}) "
             f"PURGE=TRUE ON_ERROR={on_error}"
         )
         logger.debug(f"copying into with '{copy_into_sql}'")
         copy_results = cursor.execute(copy_into_sql, _is_internal=True).fetchall()
 
         if overwrite:
             original_table_location = build_location_helper(
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/proxy.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/result_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,15 @@
                 JSONResultBatch(
                     c["rowCount"],
                     chunk_headers,
                     remote_chunk_info(c),
                     schema,
                     column_converters,
                     cursor._use_dict_result,
+                    json_result_force_utf8_decoding=cursor._connection._json_result_force_utf8_decoding,
                 )
                 for c in chunks
             ]
         else:
             rest_of_chunks = [
                 ArrowResultBatch(
                     c["rowCount"],
@@ -380,22 +381,25 @@
         self,
         rowcount: int,
         chunk_headers: dict[str, str] | None,
         remote_chunk_info: RemoteChunkInfo | None,
         schema: Sequence[ResultMetadata],
         column_converters: Sequence[tuple[str, SnowflakeConverterType]],
         use_dict_result: bool,
+        *,
+        json_result_force_utf8_decoding: bool = False,
     ) -> None:
         super().__init__(
             rowcount,
             chunk_headers,
             remote_chunk_info,
             schema,
             use_dict_result,
         )
+        self._json_result_force_utf8_decoding = json_result_force_utf8_decoding
         self.column_converters = column_converters
 
     @classmethod
     def from_data(
         cls,
         data: Sequence[Sequence[Any]],
         data_len: int,
@@ -416,18 +420,29 @@
         return new_chunk
 
     def _load(self, response: Response) -> list:
         """This function loads a compressed JSON file into memory.
 
         Returns:
             Whatever ``json.loads`` return, but in a list.
-            Unfortunately there's not type hint for this.
+            Unfortunately there's no type hint for this.
             For context: https://github.com/python/typing/issues/182
         """
-        read_data = response.text
+        # if users specify how to decode the data, we decode the bytes using the specified encoding
+        if self._json_result_force_utf8_decoding:
+            try:
+                read_data = str(response.content, "utf-8", errors="strict")
+            except Exception as exc:
+                err_msg = f"failed to decode json result content due to error {exc!r}"
+                logger.error(err_msg)
+                raise Error(msg=err_msg)
+        else:
+            # note: SNOW-787480 response.apparent_encoding is unreliable, chardet.detect can be wrong which is used by
+            # response.text to decode content, check issue: https://github.com/chardet/chardet/issues/148
+            read_data = response.text
         return json.loads("".join(["[", read_data, "]"]))
 
     def _parse(
         self, downloaded_data
     ) -> list[dict | Exception] | list[tuple | Exception]:
         """Parses downloaded data into its final form."""
         logger.debug(f"parsing for result batch id: {self.id}")
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/result_set.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/test_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/time_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/url_util.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/util_text.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         major, minor, patch = chardet_version.split(".")[:3]
         major, minor, patch = int(major), int(minor), int(patch)
         # chardet_version >= 3.0.2, < 6.0.0
         assert (3, 0, 2) <= (major, minor, patch) < (6, 0, 0)
     elif charset_normalizer_version:
         major, minor, patch = charset_normalizer_version.split(".")[:3]
         major, minor, patch = int(major), int(minor), int(patch)
-        # charset_normalizer >= 2.0.0 < 3.0.0
-        assert (2, 0, 0) <= (major, minor, patch) < (3, 0, 0)
+        # charset_normalizer >= 2.0.0 < 4.0.0
+        assert (2, 0, 0) <= (major, minor, patch) < (4, 0, 0)
     else:
         raise Exception("You need either charset_normalizer or chardet installed")
 
 
 def _check_cryptography(cryptography_version):
     # cryptography < 1.3.4
     try:
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 from .compat import builtin_str
 
 _VALID_HEADER_NAME_RE_BYTE = re.compile(rb"^[^:\s][^:\r\n]*$")
 _VALID_HEADER_NAME_RE_STR = re.compile(r"^[^:\s][^:\r\n]*$")
 _VALID_HEADER_VALUE_RE_BYTE = re.compile(rb"^\S[^\r\n]*$|^$")
 _VALID_HEADER_VALUE_RE_STR = re.compile(r"^\S[^\r\n]*$|^$")
 
+_HEADER_VALIDATORS_STR = (_VALID_HEADER_NAME_RE_STR, _VALID_HEADER_VALUE_RE_STR)
+_HEADER_VALIDATORS_BYTE = (_VALID_HEADER_NAME_RE_BYTE, _VALID_HEADER_VALUE_RE_BYTE)
 HEADER_VALIDATORS = {
-    bytes: (_VALID_HEADER_NAME_RE_BYTE, _VALID_HEADER_VALUE_RE_BYTE),
-    str: (_VALID_HEADER_NAME_RE_STR, _VALID_HEADER_VALUE_RE_STR),
+    bytes: _HEADER_VALIDATORS_BYTE,
+    str: _HEADER_VALIDATORS_STR,
 }
 
 
 def to_native_string(string, encoding="ascii"):
     """Given a string object, regardless of type, returns a representation of
     that string in the native string type, encoding and decoding where
     necessary. This assumes ASCII unless told otherwise.
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     NewConnectionError,
     ProtocolError,
 )
 from ..urllib3.exceptions import ProxyError as _ProxyError
 from ..urllib3.exceptions import ReadTimeoutError, ResponseError
 from ..urllib3.exceptions import SSLError as _SSLError
 from ..urllib3.poolmanager import PoolManager, proxy_from_url
-from ..urllib3.response import HTTPResponse
 from ..urllib3.util import Timeout as TimeoutSauce
 from ..urllib3.util import parse_url
 from ..urllib3.util.retry import Retry
 
 from .auth import _basic_auth_str
 from .compat import basestring, urlparse
 from .cookies import extract_cookies_to_jar
@@ -481,71 +480,27 @@
                 )
         elif isinstance(timeout, TimeoutSauce):
             pass
         else:
             timeout = TimeoutSauce(connect=timeout, read=timeout)
 
         try:
-            if not chunked:
-                resp = conn.urlopen(
-                    method=request.method,
-                    url=url,
-                    body=request.body,
-                    headers=request.headers,
-                    redirect=False,
-                    assert_same_host=False,
-                    preload_content=False,
-                    decode_content=False,
-                    retries=self.max_retries,
-                    timeout=timeout,
-                )
-
-            # Send the request.
-            else:
-                if hasattr(conn, "proxy_pool"):
-                    conn = conn.proxy_pool
-
-                low_conn = conn._get_conn(timeout=DEFAULT_POOL_TIMEOUT)
-
-                try:
-                    skip_host = "Host" in request.headers
-                    low_conn.putrequest(
-                        request.method,
-                        url,
-                        skip_accept_encoding=True,
-                        skip_host=skip_host,
-                    )
-
-                    for header, value in request.headers.items():
-                        low_conn.putheader(header, value)
-
-                    low_conn.endheaders()
-
-                    for i in request.body:
-                        low_conn.send(hex(len(i))[2:].encode("utf-8"))
-                        low_conn.send(b"\r\n")
-                        low_conn.send(i)
-                        low_conn.send(b"\r\n")
-                    low_conn.send(b"0\r\n\r\n")
-
-                    # Receive the response from the server
-                    r = low_conn.getresponse()
-
-                    resp = HTTPResponse.from_httplib(
-                        r,
-                        pool=conn,
-                        connection=low_conn,
-                        preload_content=False,
-                        decode_content=False,
-                    )
-                except Exception:
-                    # If we hit any problems here, clean up the connection.
-                    # Then, raise so that we can handle the actual exception.
-                    low_conn.close()
-                    raise
+            resp = conn.urlopen(
+                method=request.method,
+                url=url,
+                body=request.body,
+                headers=request.headers,
+                redirect=False,
+                assert_same_host=False,
+                preload_content=False,
+                decode_content=False,
+                retries=self.max_retries,
+                timeout=timeout,
+                chunked=chunked,
+            )
 
         except (ProtocolError, OSError) as err:
             raise ConnectionError(err, request=request)
 
         except MaxRetryError as e:
             if isinstance(e.reason, ConnectTimeoutError):
                 # TODO: Remove this in 3.0.0: see #2811
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,45 +102,45 @@
 
 def post(url, data=None, json=None, **kwargs):
     r"""Sends a POST request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
-    :param json: (optional) json data to send in the body of the :class:`Request`.
+    :param json: (optional) A JSON serializable Python object to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
     return request("post", url, data=data, json=json, **kwargs)
 
 
 def put(url, data=None, **kwargs):
     r"""Sends a PUT request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
-    :param json: (optional) json data to send in the body of the :class:`Request`.
+    :param json: (optional) A JSON serializable Python object to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
     return request("put", url, data=data, **kwargs)
 
 
 def patch(url, data=None, **kwargs):
     r"""Sends a PATCH request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
-    :param json: (optional) json data to send in the body of the :class:`Request`.
+    :param json: (optional) A JSON serializable Python object to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
     return request("patch", url, data=data, **kwargs)
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
             scheme, auth, host, port, path, query, fragment = parse_url(url)
         except LocationParseError as e:
             raise InvalidURL(*e.args)
 
         if not scheme:
             raise MissingSchema(
                 f"Invalid URL {url!r}: No scheme supplied. "
-                f"Perhaps you meant http://{url}?"
+                f"Perhaps you meant https://{url}?"
             )
 
         if not host:
             raise InvalidURL(f"Invalid URL {url!r}: No host supplied")
 
         # In general, we want to try IDNA encoding the hostname if the string contains
         # non-ASCII characters. This allows users to automatically get the correct IDNA
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/requests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 
 from ..urllib3.util import make_headers, parse_url
 
 from . import certs
 from .__version__ import __version__
 
 # to_native_string is unused here, but imported here for backwards compatibility
-from ._internal_utils import HEADER_VALIDATORS, to_native_string  # noqa: F401
+from ._internal_utils import (  # noqa: F401
+    _HEADER_VALIDATORS_BYTE,
+    _HEADER_VALIDATORS_STR,
+    HEADER_VALIDATORS,
+    to_native_string,
+)
 from .compat import (
     Mapping,
     basestring,
     bytes,
     getproxies,
     getproxies_environment,
     integer_types,
@@ -1027,28 +1032,31 @@
 def check_header_validity(header):
     """Verifies that header parts don't contain leading whitespace
     reserved characters, or return characters.
 
     :param header: tuple, in the format (name, value).
     """
     name, value = header
+    _validate_header_part(header, name, 0)
+    _validate_header_part(header, value, 1)
 
-    for part in header:
-        if type(part) not in HEADER_VALIDATORS:
-            raise InvalidHeader(
-                f"Header part ({part!r}) from {{{name!r}: {value!r}}} must be "
-                f"of type str or bytes, not {type(part)}"
-            )
-
-    _validate_header_part(name, "name", HEADER_VALIDATORS[type(name)][0])
-    _validate_header_part(value, "value", HEADER_VALIDATORS[type(value)][1])
 
+def _validate_header_part(header, header_part, header_validator_index):
+    if isinstance(header_part, str):
+        validator = _HEADER_VALIDATORS_STR[header_validator_index]
+    elif isinstance(header_part, bytes):
+        validator = _HEADER_VALIDATORS_BYTE[header_validator_index]
+    else:
+        raise InvalidHeader(
+            f"Header part ({header_part!r}) from {header} "
+            f"must be of type str or bytes, not {type(header_part)}"
+        )
 
-def _validate_header_part(header_part, header_kind, validator):
     if not validator.match(header_part):
+        header_kind = "name" if header_validator_index == 0 else "value"
         raise InvalidHeader(
             f"Invalid leading whitespace, reserved character(s), or return"
             f"character(s) in header {header_kind}: {header_part!r}"
         )
 
 
 def urldefragauth(url):
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,31 @@
 from .poolmanager import PoolManager, ProxyManager, proxy_from_url
 from .response import HTTPResponse
 from .util.request import make_headers
 from .util.retry import Retry
 from .util.timeout import Timeout
 from .util.url import get_host
 
+# === NOTE TO REPACKAGERS AND VENDORS ===
+# Please delete this block, this logic is only
+# for urllib3 being distributed via PyPI.
+# See: https://github.com/urllib3/urllib3/issues/2680
+try:
+    import urllib3_secure_extra  # type: ignore # noqa: F401
+except ImportError:
+    pass
+else:
+    warnings.warn(
+        "'urllib3[secure]' extra is deprecated and will be removed "
+        "in a future release of urllib3 2.x. Read more in this issue: "
+        "https://github.com/urllib3/urllib3/issues/2680",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
+
 __author__ = "Andrey Petrov (andrey.petrov@shazow.net)"
 __license__ = "MIT"
 __version__ = __version__
 
 __all__ = (
     "HTTPConnectionPool",
     "HTTPSConnectionPool",
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,19 @@
         elif six.ensure_str(header.lower()) not in SKIPPABLE_HEADERS:
             raise ValueError(
                 "urllib3.util.SKIP_HEADER only supports '%s'"
                 % ("', '".join(map(str.title, sorted(SKIPPABLE_HEADERS))),)
             )
 
     def request(self, method, url, body=None, headers=None):
+        # Update the inner socket's timeout value to send the request.
+        # This only triggers if the connection is re-used.
+        if getattr(self, "sock", None) is not None:
+            self.sock.settimeout(self.timeout)
+
         if headers is None:
             headers = {}
         else:
             # Avoid modifying the headers passed into .request()
             headers = headers.copy()
         if "user-agent" not in (six.ensure_str(k.lower()) for k in headers):
             headers["User-Agent"] = _get_default_user_agent()
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
             :class:`urllib3.util.Timeout`, which gives you more fine-grained
             control over your timeouts.
         """
         self.num_requests += 1
 
         timeout_obj = self._get_timeout(timeout)
         timeout_obj.start_connect()
-        conn.timeout = timeout_obj.connect_timeout
+        conn.timeout = Timeout.resolve_default_timeout(timeout_obj.connect_timeout)
 
         # Trigger any extra validation we need to do.
         try:
             self._validate_conn(conn)
         except (SocketTimeout, BaseSSLError) as e:
             # Py2 raises this as a BaseSSLError, Py3 raises it as socket timeout.
             self._raise_timeout(err=e, url=url, timeout_value=conn.timeout)
@@ -858,15 +858,15 @@
                 release_conn=release_conn,
                 chunked=chunked,
                 body_pos=body_pos,
                 **response_kw
             )
 
         # Check if we should retry the HTTP response.
-        has_retry_after = bool(response.getheader("Retry-After"))
+        has_retry_after = bool(response.headers.get("Retry-After"))
         if retries.is_retry(method, response.status, has_retry_after):
             try:
                 retries = retries.increment(method, url, response=response, _pool=self)
             except MaxRetryError:
                 if retries.raise_on_status:
                     response.drain_conn()
                     raise
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                     retries=retries,
                     redirect=redirect,
                     timeout=timeout,
                     **response_kw
                 )
 
         # Check if we should retry the HTTP response.
-        has_retry_after = bool(http_response.getheader("Retry-After"))
+        has_retry_after = bool(http_response.headers.get("Retry-After"))
         if retries.is_retry(method, http_response.status, has_retry_after):
             retries = retries.increment(method, url, response=http_response, _pool=self)
             log.debug("Retry: %s", url)
             retries.sleep(http_response)
             return self.urlopen(
                 method,
                 url,
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # Send negotiation message
         headers[req_header] = "NTLM %s" % ntlm.create_NTLM_NEGOTIATE_MESSAGE(
             self.rawuser
         )
         log.debug("Request headers: %s", headers)
         conn.request("GET", self.authurl, None, headers)
         res = conn.getresponse()
-        reshdr = dict(res.getheaders())
+        reshdr = dict(res.headers)
         log.debug("Response status: %s %s", res.status, res.reason)
         log.debug("Response headers: %s", reshdr)
         log.debug("Response data: %s [...]", res.read(100))
 
         # Remove the reference to the socket, so that it can not be closed by
         # the response object (we want to keep the socket open)
         res.fp = None
@@ -97,15 +97,15 @@
             ServerChallenge, self.user, self.domain, self.pw, NegotiateFlags
         )
         headers[req_header] = "NTLM %s" % auth_msg
         log.debug("Request headers: %s", headers)
         conn.request("GET", self.authurl, None, headers)
         res = conn.getresponse()
         log.debug("Response status: %s %s", res.status, res.reason)
-        log.debug("Response headers: %s", dict(res.getheaders()))
+        log.debug("Response headers: %s", dict(res.headers))
         log.debug("Response data: %s [...]", res.read()[:100])
         if res.status != 200:
             if res.status == 401:
                 raise Exception("Server rejected request: wrong username or password")
             raise Exception("Wrong server response: %s %s" % (res.status, res.reason))
 
         res.fp = None
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 .. _crime attack: https://en.wikipedia.org/wiki/CRIME_(security_exploit)
 .. _pyopenssl: https://www.pyopenssl.org
 .. _cryptography: https://cryptography.io
 .. _idna: https://github.com/kjd/idna
 """
 from __future__ import absolute_import
 
+import OpenSSL.crypto
 import OpenSSL.SSL
 from cryptography import x509
+from cryptography.hazmat.backends.openssl import backend as openssl_backend
 
 try:
     from cryptography.x509 import UnsupportedExtension
 except ImportError:
     # UnsupportedExtension is gone in cryptography >= 2.1.0
     class UnsupportedExtension(Exception):
         pass
@@ -67,19 +69,28 @@
 except ImportError:  # Platform-specific: Python 3
     _fileobject = None
     from ..packages.backports.makefile import backport_makefile
 
 import logging
 import ssl
 import sys
+import warnings
 
 from .. import util
 from ..packages import six
 from ..util.ssl_ import PROTOCOL_TLS_CLIENT
 
+warnings.warn(
+    "'urllib3.contrib.pyopenssl' module is deprecated and will be removed "
+    "in a future release of urllib3 2.x. Read more in this issue: "
+    "https://github.com/urllib3/urllib3/issues/2680",
+    category=DeprecationWarning,
+    stacklevel=2,
+)
+
 __all__ = ["inject_into_urllib3", "extract_from_urllib3"]
 
 # SNI always works.
 HAS_SNI = True
 
 # Map from urllib3 to PyOpenSSL compatible parameter-values.
 _openssl_versions = {
@@ -209,15 +220,20 @@
     return name
 
 
 def get_subj_alt_name(peer_cert):
     """
     Given an PyOpenSSL certificate, provides all the subject alternative names.
     """
-    cert = peer_cert.to_cryptography()
+    # Pass the cert to cryptography, which has much better APIs for this.
+    if hasattr(peer_cert, "to_cryptography"):
+        cert = peer_cert.to_cryptography()
+    else:
+        der = OpenSSL.crypto.dump_certificate(OpenSSL.crypto.FILETYPE_ASN1, peer_cert)
+        cert = x509.load_der_x509_certificate(der, openssl_backend)
 
     # We want to find the SAN extension. Ask Cryptography to locate it (it's
     # faster than looping in Python)
     try:
         ext = cert.extensions.get_extension_for_class(x509.SubjectAlternativeName).value
     except x509.ExtensionNotFound:
         # No such extension, return the empty list.
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import absolute_import
 
 import io
 import logging
+import sys
+import warnings
 import zlib
 from contextlib import contextmanager
 from socket import error as SocketError
 from socket import timeout as SocketTimeout
 
 try:
     try:
         import brotlicffi as brotli
     except ImportError:
         import brotli
 except ImportError:
     brotli = None
 
+from . import util
 from ._collections import HTTPHeaderDict
 from .connection import BaseSSLError, HTTPException
 from .exceptions import (
     BodyNotHttplibCompatible,
     DecodeError,
     HTTPError,
     IncompleteRead,
@@ -477,14 +480,62 @@
                     self._connection.close()
 
             # If we hold the original response but it's closed now, we should
             # return the connection back to the pool.
             if self._original_response and self._original_response.isclosed():
                 self.release_conn()
 
+    def _fp_read(self, amt):
+        """
+        Read a response with the thought that reading the number of bytes
+        larger than can fit in a 32-bit int at a time via SSL in some
+        known cases leads to an overflow error that has to be prevented
+        if `amt` or `self.length_remaining` indicate that a problem may
+        happen.
+
+        The known cases:
+          * 3.8 <= CPython < 3.9.7 because of a bug
+            https://github.com/urllib3/urllib3/issues/2513#issuecomment-1152559900.
+          * urllib3 injected with pyOpenSSL-backed SSL-support.
+          * CPython < 3.10 only when `amt` does not fit 32-bit int.
+        """
+        assert self._fp
+        c_int_max = 2 ** 31 - 1
+        if (
+            (
+                (amt and amt > c_int_max)
+                or (self.length_remaining and self.length_remaining > c_int_max)
+            )
+            and not util.IS_SECURETRANSPORT
+            and (util.IS_PYOPENSSL or sys.version_info < (3, 10))
+        ):
+            buffer = io.BytesIO()
+            # Besides `max_chunk_amt` being a maximum chunk size, it
+            # affects memory overhead of reading a response by this
+            # method in CPython.
+            # `c_int_max` equal to 2 GiB - 1 byte is the actual maximum
+            # chunk size that does not lead to an overflow error, but
+            # 256 MiB is a compromise.
+            max_chunk_amt = 2 ** 28
+            while amt is None or amt != 0:
+                if amt is not None:
+                    chunk_amt = min(amt, max_chunk_amt)
+                    amt -= chunk_amt
+                else:
+                    chunk_amt = max_chunk_amt
+                data = self._fp.read(chunk_amt)
+                if not data:
+                    break
+                buffer.write(data)
+                del data  # to reduce peak memory usage by `max_chunk_amt`.
+            return buffer.getvalue()
+        else:
+            # StringIO doesn't like amt=None
+            return self._fp.read(amt) if amt is not None else self._fp.read()
+
     def read(self, amt=None, decode_content=None, cache_content=False):
         """
         Similar to :meth:`http.client.HTTPResponse.read`, but with two additional
         parameters: ``decode_content`` and ``cache_content``.
 
         :param amt:
             How much of the content to read. If specified, caching is skipped
@@ -509,21 +560,19 @@
         if self._fp is None:
             return
 
         flush_decoder = False
         fp_closed = getattr(self._fp, "closed", False)
 
         with self._error_catcher():
+            data = self._fp_read(amt) if not fp_closed else b""
             if amt is None:
-                # cStringIO doesn't like amt=None
-                data = self._fp.read() if not fp_closed else b""
                 flush_decoder = True
             else:
                 cache_content = False
-                data = self._fp.read(amt) if not fp_closed else b""
                 if (
                     amt != 0 and not data
                 ):  # Platform-specific: Buggy versions of Python.
                     # Close the connection when no data is returned
                     #
                     # This is redundant to what httplib/http.client _should_
                     # already do.  However, versions of python released before
@@ -611,17 +660,29 @@
             original_response=r,
             **response_kw
         )
         return resp
 
     # Backwards-compatibility methods for http.client.HTTPResponse
     def getheaders(self):
+        warnings.warn(
+            "HTTPResponse.getheaders() is deprecated and will be removed "
+            "in urllib3 v2.1.0. Instead access HTTPResponse.headers directly.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         return self.headers
 
     def getheader(self, name, default=None):
+        warnings.warn(
+            "HTTPResponse.getheader() is deprecated and will be removed "
+            "in urllib3 v2.1.0. Instead use HTTPResponse.headers.get(name, default).",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         return self.headers.get(name, default)
 
     # Backwards compatibility for http.cookiejar
     def info(self):
         return self.headers
 
     # Overrides from io.IOBase
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
             seconds = 0
 
         return seconds
 
     def get_retry_after(self, response):
         """Get the value of Retry-After in seconds."""
 
-        retry_after = response.getheader("Retry-After")
+        retry_after = response.headers.get("Retry-After")
 
         if retry_after is None:
             return None
 
         return self.parse_retry_after(retry_after)
 
     def sleep_for_retry(self, response=None):
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 
 import time
 
-# The default socket timeout, used by httplib to indicate that no timeout was
-# specified by the user
-from socket import _GLOBAL_DEFAULT_TIMEOUT
+# The default socket timeout, used by httplib to indicate that no timeout was; specified by the user
+from socket import _GLOBAL_DEFAULT_TIMEOUT, getdefaulttimeout
 
 from ..exceptions import TimeoutStateError
 
 # A sentinel value to indicate that no timeout was specified by the user in
 # urllib3
 _Default = object()
 
@@ -113,14 +112,18 @@
             self.total,
         )
 
     # __str__ provided for backwards compatibility
     __str__ = __repr__
 
     @classmethod
+    def resolve_default_timeout(cls, timeout):
+        return getdefaulttimeout() if timeout is cls.DEFAULT_TIMEOUT else timeout
+
+    @classmethod
     def _validate_timeout(cls, value, name):
         """Check that a timeout attribute is valid.
 
         :param value: The timeout value to validate
         :param name: The name of the timeout attribute to validate. This is
             used to specify in error messages.
         :return: The validated and casted version of the given value.
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     "(?:(?:%(hex)s:){0,4}%(hex)s)?::%(ls32)s",
     # [ *5( h16 ":" ) h16 ] "::"              h16
     "(?:(?:%(hex)s:){0,5}%(hex)s)?::%(hex)s",
     # [ *6( h16 ":" ) h16 ] "::"
     "(?:(?:%(hex)s:){0,6}%(hex)s)?::",
 ]
 
-UNRESERVED_PAT = r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._!\-~"
+UNRESERVED_PAT = r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._\-~"
 IPV6_PAT = "(?:" + "|".join([x % _subs for x in _variations]) + ")"
 ZONE_ID_PAT = "(?:%25|%)(?:[" + UNRESERVED_PAT + "]|%[a-fA-F0-9]{2})+"
 IPV6_ADDRZ_PAT = r"\[" + IPV6_PAT + r"(?:" + ZONE_ID_PAT + r")?\]"
 REG_NAME_PAT = r"(?:[^\[\]%:/?#]|%[a-fA-F0-9]{2})*"
 TARGET_RE = re.compile(r"^(/[^?#]*)(?:\?([^#]*))?(?:#.*)?$")
 
 IPV4_RE = re.compile("^" + IPV4_PAT + "$")
 IPV6_RE = re.compile("^" + IPV6_PAT + "$")
 IPV6_ADDRZ_RE = re.compile("^" + IPV6_ADDRZ_PAT + "$")
 BRACELESS_IPV6_ADDRZ_RE = re.compile("^" + IPV6_ADDRZ_PAT[2:-2] + "$")
 ZONE_ID_RE = re.compile("(" + ZONE_ID_PAT + r")\]$")
 
-_HOST_PORT_PAT = ("^(%s|%s|%s)(?::([0-9]{0,5}))?$") % (
+_HOST_PORT_PAT = ("^(%s|%s|%s)(?::0*?(|0|[1-9][0-9]{0,4}))?$") % (
     REG_NAME_PAT,
     IPV4_PAT,
     IPV6_ADDRZ_PAT,
 )
 _HOST_PORT_RE = re.compile(_HOST_PORT_PAT, re.UNICODE | re.DOTALL)
 
 UNRESERVED_CHARS = set(
@@ -299,15 +299,15 @@
                 return six.ensure_str(
                     b".".join([_idna_encode(label) for label in host.split(".")])
                 )
     return host
 
 
 def _idna_encode(name):
-    if name and any([ord(x) > 128 for x in name]):
+    if name and any(ord(x) >= 128 for x in name):
         try:
             import idna
         except ImportError:
             six.raise_from(
                 LocationParseError("Unable to parse URL without the 'idna' module"),
                 None,
             )
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.4.7
+Version: 2023.5.3
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.4.7/src/snowflake_connector_python_nightly.egg-info/requires.txt` & `snowflake-connector-python-nightly-2023.5.3/src/snowflake_connector_python_nightly.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 oscrypto<2.0.0
 pyOpenSSL<24.0.0,>=16.2.0
 pycryptodomex!=3.5.0,<4.0.0,>=3.2
 pyjwt<3.0.0
 pytz
 requests<3.0.0
 packaging
-charset_normalizer<3,>=2
+charset_normalizer<4,>=2
 idna<4,>=2.5
 urllib3<1.27,>=1.21.1
 certifi>=2017.4.17
 typing_extensions<5,>=4.3
 filelock<4,>=3.5
 
 [:python_version < "3.8"]
@@ -21,15 +21,15 @@
 [development]
 Cython
 coverage
 more-itertools
 numpy<1.25.0
 pendulum!=2.1.1
 pexpect
-pytest<7.3.0
+pytest<7.4.0
 pytest-cov
 pytest-rerunfailures
 pytest-timeout
 pytest-xdist
 pytzdata
 
 [pandas]
```

