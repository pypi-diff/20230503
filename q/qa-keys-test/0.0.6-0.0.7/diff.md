# Comparing `tmp/qa-keys-test-0.0.6.tar.gz` & `tmp/qa-keys-test-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa-keys-test-0.0.6.tar", last modified: Wed May  3 11:53:48 2023, max compression
+gzip compressed data, was "qa-keys-test-0.0.7.tar", last modified: Wed May  3 11:56:40 2023, max compression
```

## Comparing `qa-keys-test-0.0.6.tar` & `qa-keys-test-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:53:48.111180 qa-keys-test-0.0.6/
--rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      233 2023-05-03 11:53:48.106189 qa-keys-test-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:53:48.077185 qa-keys-test-0.0.6/automation_qa_key_helper/
--rw-rw-rw-   0        0        0       35 2023-05-03 11:53:39.000000 qa-keys-test-0.0.6/automation_qa_key_helper/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-03 11:52:10.000000 qa-keys-test-0.0.6/automation_qa_key_helper/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:53:48.081843 qa-keys-test-0.0.6/config/
--rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.6/config/qa_key.json
-drwxrwxrwx   0        0        0        0 2023-05-03 11:53:48.103217 qa-keys-test-0.0.6/qa_keys_test.egg-info/
--rw-rw-rw-   0        0        0      233 2023-05-03 11:53:47.000000 qa-keys-test-0.0.6/qa_keys_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-03 11:53:47.000000 qa-keys-test-0.0.6/qa_keys_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:53:47.000000 qa-keys-test-0.0.6/qa_keys_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.6/qa_keys_test.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-05-03 11:53:47.000000 qa-keys-test-0.0.6/qa_keys_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:53:48.111180 qa-keys-test-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      415 2023-05-03 11:46:41.000000 qa-keys-test-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:56:40.401096 qa-keys-test-0.0.7/
+-rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:56:40.396180 qa-keys-test-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:56:40.362040 qa-keys-test-0.0.7/automation_qa_key_helper/
+-rw-rw-rw-   0        0        0       45 2023-05-03 11:56:12.000000 qa-keys-test-0.0.7/automation_qa_key_helper/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-03 11:52:10.000000 qa-keys-test-0.0.7/automation_qa_key_helper/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:56:40.366321 qa-keys-test-0.0.7/config/
+-rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.7/config/qa_key.json
+drwxrwxrwx   0        0        0        0 2023-05-03 11:56:40.392355 qa-keys-test-0.0.7/qa_keys_test.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:56:39.000000 qa-keys-test-0.0.7/qa_keys_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-03 11:56:40.000000 qa-keys-test-0.0.7/qa_keys_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:56:39.000000 qa-keys-test-0.0.7/qa_keys_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.7/qa_keys_test.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-05-03 11:56:40.000000 qa-keys-test-0.0.7/qa_keys_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:56:40.401096 qa-keys-test-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-05-03 11:55:35.000000 qa-keys-test-0.0.7/setup.py
```

### Comparing `qa-keys-test-0.0.6/LICENSE` & `qa-keys-test-0.0.7/LICENSE`

 * *Files identical despite different names*

