# Comparing `tmp/qa-keys-test-0.0.3.tar.gz` & `tmp/qa-keys-test-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa-keys-test-0.0.3.tar", last modified: Wed May  3 10:53:44 2023, max compression
+gzip compressed data, was "qa-keys-test-0.0.4.tar", last modified: Wed May  3 11:08:41 2023, max compression
```

## Comparing `qa-keys-test-0.0.3.tar` & `qa-keys-test-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:53:44.418328 qa-keys-test-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      233 2023-05-03 10:53:44.413936 qa-keys-test-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 10:53:44.371265 qa-keys-test-0.0.3/automation/
--rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.3/automation/__init__.py
--rw-rw-rw-   0        0        0      234 2023-05-03 10:42:08.000000 qa-keys-test-0.0.3/automation/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:53:44.375013 qa-keys-test-0.0.3/config/
--rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.3/config/qa_key.json
-drwxrwxrwx   0        0        0        0 2023-05-03 10:53:44.381298 qa-keys-test-0.0.3/python/
--rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.3/python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:53:44.409298 qa-keys-test-0.0.3/qa_keys_test.egg-info/
--rw-rw-rw-   0        0        0      233 2023-05-03 10:53:43.000000 qa-keys-test-0.0.3/qa_keys_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-03 10:53:44.000000 qa-keys-test-0.0.3/qa_keys_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:53:43.000000 qa-keys-test-0.0.3/qa_keys_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.3/qa_keys_test.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-03 10:53:43.000000 qa-keys-test-0.0.3/qa_keys_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 10:53:44.418328 qa-keys-test-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      373 2023-05-03 10:52:39.000000 qa-keys-test-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.531649 qa-keys-test-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-03 06:35:35.000000 qa-keys-test-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:08:41.527103 qa-keys-test-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-03 06:35:35.000000 qa-keys-test-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.478230 qa-keys-test-0.0.4/automation/
+-rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.4/automation/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-05-03 10:42:08.000000 qa-keys-test-0.0.4/automation/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.483149 qa-keys-test-0.0.4/config/
+-rw-rw-rw-   0        0        0      144 2023-05-03 09:23:52.000000 qa-keys-test-0.0.4/config/qa_key.json
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.492450 qa-keys-test-0.0.4/python/
+-rw-rw-rw-   0        0        0        0 2023-05-03 08:44:02.000000 qa-keys-test-0.0.4/python/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-05-03 10:39:49.000000 qa-keys-test-0.0.4/python/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:41.521834 qa-keys-test-0.0.4/qa_keys_test.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-05-03 11:08:40.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-03 11:08:41.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:08:40.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 09:25:49.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-03 11:08:41.000000 qa-keys-test-0.0.4/qa_keys_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:08:41.531649 qa-keys-test-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-05-03 11:07:45.000000 qa-keys-test-0.0.4/setup.py
```

### Comparing `qa-keys-test-0.0.3/LICENSE` & `qa-keys-test-0.0.4/LICENSE`

 * *Files identical despite different names*

