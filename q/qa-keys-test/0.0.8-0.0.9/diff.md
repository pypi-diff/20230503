# Comparing `tmp/qa-keys-test-0.0.8.tar.gz` & `tmp/qa-keys-test-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa-keys-test-0.0.8.tar", last modified: Wed May  3 12:08:05 2023, max compression
+gzip compressed data, was "qa-keys-test-0.0.9.tar", last modified: Wed May  3 15:16:09 2023, max compression
```

## Comparing `qa-keys-test-0.0.8.tar` & `qa-keys-test-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:08:05.244415 qa-keys-test-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      233 2023-05-03 12:08:05.239476 qa-keys-test-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 12:08:05.199589 qa-keys-test-0.0.8/automation_qa_key_helper/
--rw-rw-rw-   0        0        0       45 2023-05-03 11:56:12.000000 qa-keys-test-0.0.8/automation_qa_key_helper/__init__.py
--rw-rw-rw-   0        0        0      413 2023-05-03 12:07:33.000000 qa-keys-test-0.0.8/automation_qa_key_helper/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:08:05.204564 qa-keys-test-0.0.8/config/
--rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.8/config/qa_key.json
-drwxrwxrwx   0        0        0        0 2023-05-03 12:08:05.236030 qa-keys-test-0.0.8/qa_keys_test.egg-info/
--rw-rw-rw-   0        0        0      233 2023-05-03 12:08:04.000000 qa-keys-test-0.0.8/qa_keys_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-03 12:08:05.000000 qa-keys-test-0.0.8/qa_keys_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:08:04.000000 qa-keys-test-0.0.8/qa_keys_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.8/qa_keys_test.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-05-03 12:08:04.000000 qa-keys-test-0.0.8/qa_keys_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 12:08:05.245025 qa-keys-test-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-05-03 12:07:48.000000 qa-keys-test-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:16:09.811065 qa-keys-test-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-03 15:16:02.000000 qa-keys-test-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      233 2023-05-03 15:16:09.806688 qa-keys-test-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 15:16:09.769416 qa-keys-test-0.0.9/automation_qa_key_helper/
+-rw-rw-rw-   0        0        0       45 2023-05-03 11:56:12.000000 qa-keys-test-0.0.9/automation_qa_key_helper/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-05-03 12:07:33.000000 qa-keys-test-0.0.9/automation_qa_key_helper/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:16:09.773673 qa-keys-test-0.0.9/config/
+-rw-rw-rw-   0        0        0      144 2023-05-03 15:12:02.000000 qa-keys-test-0.0.9/config/qa_key.json
+drwxrwxrwx   0        0        0        0 2023-05-03 15:16:09.802192 qa-keys-test-0.0.9/qa_keys_test.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-05-03 15:16:08.000000 qa-keys-test-0.0.9/qa_keys_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-03 15:16:09.000000 qa-keys-test-0.0.9/qa_keys_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:16:09.000000 qa-keys-test-0.0.9/qa_keys_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.9/qa_keys_test.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-05-03 15:16:09.000000 qa-keys-test-0.0.9/qa_keys_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 15:16:09.812069 qa-keys-test-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      440 2023-05-03 12:15:06.000000 qa-keys-test-0.0.9/setup.py
```

### Comparing `qa-keys-test-0.0.8/LICENSE` & `qa-keys-test-0.0.9/LICENSE`

 * *Files identical despite different names*

