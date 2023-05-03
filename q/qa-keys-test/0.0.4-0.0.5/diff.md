# Comparing `tmp/qa-keys-test-0.0.4.tar.gz` & `tmp/qa-keys-test-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa-keys-test-0.0.4.tar", last modified: Wed May  3 11:08:41 2023, max compression
+gzip compressed data, was "qa-keys-test-0.0.5.tar", last modified: Wed May  3 11:29:43 2023, max compression
```

## Comparing `qa-keys-test-0.0.4.tar` & `qa-keys-test-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.531649 qa-keys-test-0.0.4/
--rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      233 2023-05-03 11:08:41.527103 qa-keys-test-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.478230 qa-keys-test-0.0.4/automation/
--rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.4/automation/__init__.py
--rw-rw-rw-   0        0        0      234 2023-05-03 10:42:08.000000 qa-keys-test-0.0.4/automation/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.483149 qa-keys-test-0.0.4/config/
--rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.4/config/qa_key.json
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.492450 qa-keys-test-0.0.4/python/
--rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.4/python/__init__.py
--rw-rw-rw-   0        0        0      203 2023-05-03 10:39:49.000000 qa-keys-test-0.0.4/python/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.521834 qa-keys-test-0.0.4/qa_keys_test.egg-info/
--rw-rw-rw-   0        0        0      233 2023-05-03 11:08:40.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-03 11:08:41.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:08:40.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-03 11:08:41.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:08:41.531649 qa-keys-test-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      415 2023-05-03 11:07:45.000000 qa-keys-test-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:43.965212 qa-keys-test-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:29:43.960049 qa-keys-test-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:43.919728 qa-keys-test-0.0.5/automation_qa_key/
+-rw-rw-rw-   0        0        0       36 2023-05-03 11:29:12.000000 qa-keys-test-0.0.5/automation_qa_key/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-05-03 10:42:08.000000 qa-keys-test-0.0.5/automation_qa_key/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:43.923558 qa-keys-test-0.0.5/config/
+-rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.5/config/qa_key.json
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:43.932918 qa-keys-test-0.0.5/python/
+-rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.5/python/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-05-03 10:39:49.000000 qa-keys-test-0.0.5/python/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:43.957017 qa-keys-test-0.0.5/qa_keys_test.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:29:43.000000 qa-keys-test-0.0.5/qa_keys_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-03 11:29:43.000000 qa-keys-test-0.0.5/qa_keys_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:29:43.000000 qa-keys-test-0.0.5/qa_keys_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.5/qa_keys_test.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-05-03 11:29:43.000000 qa-keys-test-0.0.5/qa_keys_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:29:43.965212 qa-keys-test-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-05-03 11:28:49.000000 qa-keys-test-0.0.5/setup.py
```

### Comparing `qa-keys-test-0.0.4/LICENSE` & `qa-keys-test-0.0.5/LICENSE`

 * *Files identical despite different names*

