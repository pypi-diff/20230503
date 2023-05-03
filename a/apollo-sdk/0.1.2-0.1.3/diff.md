# Comparing `tmp/apollo-sdk-0.1.2.tar.gz` & `tmp/apollo-sdk-0.1.3.macosx-13-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.1.2.tar", last modified: Sun Apr 30 05:04:52 2023, max compression
+gzip compressed data, was "apollo-sdk-0.1.3.macosx-13-arm64.tar", last modified: Wed May  3 17:45:54 2023, max compression
```

## Comparing `apollo-sdk-0.1.2.tar` & `apollo-sdk-0.1.3.macosx-13-arm64.tar`

### file list

```diff
@@ -1,58 +1,109 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.850677 apollo-sdk-0.1.2/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.1.2/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)      632 2023-04-30 05:04:52.850828 apollo-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     5509 2023-04-29 17:42:09.000000 apollo-sdk-0.1.2/README.md
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.846342 apollo-sdk-0.1.2/apollo/
--rw-r--r--   0 abpyguru   (501) staff       (20)     1403 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3608 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/client.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.846472 apollo-sdk-0.1.2/apollo/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847013 apollo-sdk-0.1.2/apollo/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847175 apollo-sdk-0.1.2/apollo/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847333 apollo-sdk-0.1.2/apollo/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847460 apollo-sdk-0.1.2/apollo/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848002 apollo-sdk-0.1.2/apollo/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1375 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848154 apollo-sdk-0.1.2/apollo/models/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848281 apollo-sdk-0.1.2/apollo/models/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848414 apollo-sdk-0.1.2/apollo/models/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/google/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848561 apollo-sdk-0.1.2/apollo/models/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848708 apollo-sdk-0.1.2/apollo/models/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1194 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848846 apollo-sdk-0.1.2/apollo/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848967 apollo-sdk-0.1.2/apollo/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.849516 apollo-sdk-0.1.2/apollo/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1155 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.849745 apollo-sdk-0.1.2/apollo/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.850537 apollo-sdk-0.1.2/apollo_sdk.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)      632 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1087 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-04-30 05:04:52.851122 apollo-sdk-0.1.2/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1899 2023-04-30 05:04:44.000000 apollo-sdk-0.1.2/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316428 ./
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316488 ./Users/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316546 ./Users/abpyguru/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316605 ./Users/abpyguru/Desktop/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316668 ./Users/abpyguru/Desktop/2023/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316735 ./Users/abpyguru/Desktop/2023/apollo/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316807 ./Users/abpyguru/Desktop/2023/apollo/backend/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316881 ./Users/abpyguru/Desktop/2023/apollo/backend/env/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.316958 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.317028 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.354203 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.340689 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1403 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.348398 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1447 2023-05-03 17:45:54.344255 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4511 2023-05-03 17:45:54.340855 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1123 2023-05-03 17:45:54.347538 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/const.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     8698 2023-05-03 17:45:54.345007 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2203 2023-05-03 17:45:54.347117 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1454 2023-05-03 17:45:54.343206 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__pycache__/resource.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3608 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332295 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332506 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      215 2023-05-03 17:45:54.332435 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332646 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332802 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/aws/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      219 2023-05-03 17:45:54.332749 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/aws/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.325263 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.325463 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/google/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      222 2023-05-03 17:45:54.325383 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/google/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.325607 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332017 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/microsoft/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      225 2023-05-03 17:45:54.325710 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/microsoft/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.332920 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/openai/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.333136 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/openai/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      222 2023-05-03 17:45:54.333055 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/openai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1450 2023-05-03 17:36:48.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.333484 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.333699 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      213 2023-05-03 17:45:54.333610 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.337563 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.339439 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      382 2023-05-03 17:45:54.338711 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1950 2023-05-03 17:45:54.339376 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4843 2023-05-03 17:45:54.337798 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__pycache__/cloud.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2060 2023-05-03 17:45:54.338302 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__pycache__/local.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.339807 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.339955 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mongo/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      219 2023-05-03 17:45:54.339894 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mongo/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.339566 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.339704 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mysql/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      219 2023-05-03 17:45:54.339652 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mysql/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.336853 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.337120 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/postgres/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      222 2023-05-03 17:45:54.337057 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/postgres/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.334075 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.336458 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      382 2023-05-03 17:45:54.335467 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      637 2023-05-03 17:45:54.336265 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2119 2023-05-03 17:45:54.334239 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__pycache__/cloud.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      706 2023-05-03 17:45:54.335137 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__pycache__/local.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1375 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/manager.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1194 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.345188 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.345333 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      212 2023-05-03 17:45:54.345278 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.346512 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.346731 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/graphql/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      220 2023-05-03 17:45:54.346650 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/graphql/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.345514 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.346377 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      369 2023-05-03 17:45:54.346057 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      835 2023-05-03 17:45:54.346296 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1287 2023-05-03 17:45:54.345606 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__pycache__/cloud.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      880 2023-05-03 17:45:54.345847 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__pycache__/local.cpython-311.pyc
+-rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1154 2023-05-03 17:37:51.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.341889 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.342103 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/tests/__pycache__/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      210 2023-05-03 17:45:54.342014 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/tests/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-03 17:45:54.355638 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      632 2023-05-03 17:45:54.250451 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1107 2023-05-03 17:45:54.259144 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-03 17:45:54.250650 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-05-03 17:45:54.250853 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-03 17:45:54.250968 ./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/top_level.txt
```

### Comparing `apollo-sdk-0.1.2/PKG-INFO` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo_sdk-0.1.3-py3.11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Build automated decision making workflows. Aggregate your LLMs all into one place and build from there using one api.
 Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API, Inc.
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apollo-sdk-0.1.2/apollo/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/client.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/client.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/const.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     "all_tables": "select table_name from information_schema.tables where table_schema='public'",
 }
 
 # Test account for firebase
 TEST_ACCOUNT = os.environ.get("test_account", None)
 
 # Service SDK test token, THIS IS PUBLIC
-test_token = os.environ.get("test_token", "81ecfd535e2d0c402bc84be64f31edcbed643d3e")
+test_token = os.environ.get("test_token", None)
```

### Comparing `apollo-sdk-0.1.2/apollo/database/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/firebase/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/firebase/base.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/firebase/cloud.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/firebase/local.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/mongo/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/mysql/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/postgres/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/supabase/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/supabase/base.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/supabase/cloud.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/database/supabase/local.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/exceptions.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/manager.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/manager.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/models/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/models/aws/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/models/google/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/models/microsoft/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/models/openai/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/resource.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/resource.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/service/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/service/graphql/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/service/json/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/service/json/base.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/service/json/cloud.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/cloud.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     @staticmethod
     def make_http_request():
         return None
 
     @staticmethod
     def make_https_request(body):
         response = requests.post(
-            "https://api.apolloapi.io/api/v1/content/",
+            "https://api.apolloapi.io/api/v1/apollo/",
             headers={"Authorization": f"Token {test_token}"},
             json=body,
             timeout=10,
         )
         return response.json()
```

### Comparing `apollo-sdk-0.1.2/apollo/service/json/local.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/service/json/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.2/apollo/tests/__init__.py` & `./Users/abpyguru/Desktop/2023/apollo/backend/env/lib/python3.11/site-packages/apollo/tests/__init__.py`

 * *Files identical despite different names*

