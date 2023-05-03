# Comparing `tmp/slippy_api-0.1.tar.gz` & `tmp/slippy_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippy_api-0.1.tar", last modified: Wed May  3 21:29:30 2023, max compression
+gzip compressed data, was "slippy_api-0.2.tar", last modified: Wed May  3 21:46:07 2023, max compression
```

## Comparing `slippy_api-0.1.tar` & `slippy_api-0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 21:29:30.927223 slippy_api-0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-03 21:18:14.000000 slippy_api-0.1/LICENSE
--rw-rw-rw-   0        0        0      486 2023-05-03 21:29:30.927223 slippy_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-05-03 21:14:37.000000 slippy_api-0.1/README.md
--rw-rw-rw-   0        0        0       88 2023-05-03 21:18:46.000000 slippy_api-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 21:29:30.927223 slippy_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-05-03 21:06:16.000000 slippy_api-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:29:30.916222 slippy_api-0.1/slippi/
--rw-rw-rw-   0        0        0        0 2023-04-18 00:49:17.000000 slippy_api-0.1/slippi/__init__.py
--rw-rw-rw-   0        0        0      522 2023-05-03 20:50:52.000000 slippy_api-0.1/slippi/main.py
--rw-rw-rw-   0        0        0     4170 2023-05-01 22:57:10.000000 slippy_api-0.1/slippi/slippi_api.py
--rw-rw-rw-   0        0        0     2240 2023-05-01 22:01:29.000000 slippy_api-0.1/slippi/slippi_characters.py
--rw-rw-rw-   0        0        0     1500 2023-05-01 21:31:57.000000 slippy_api-0.1/slippi/slippi_ranks.py
--rw-rw-rw-   0        0        0     4096 2023-05-01 23:08:27.000000 slippy_api-0.1/slippi/slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:29:30.920222 slippy_api-0.1/slippi/tests/
--rw-rw-rw-   0        0        0        0 2023-05-01 22:44:38.000000 slippy_api-0.1/slippi/tests/__init__.py
--rw-rw-rw-   0        0        0     2039 2023-05-01 22:58:46.000000 slippy_api-0.1/slippi/tests/test_slippi_api.py
--rw-rw-rw-   0        0        0      671 2023-05-01 22:51:54.000000 slippy_api-0.1/slippi/tests/test_slippi_characters.py
--rw-rw-rw-   0        0        0      885 2023-05-01 22:52:07.000000 slippy_api-0.1/slippi/tests/test_slippi_ranks.py
--rw-rw-rw-   0        0        0     4628 2023-05-01 22:51:39.000000 slippy_api-0.1/slippi/tests/test_slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:29:30.926222 slippy_api-0.1/slippy_api.egg-info/
--rw-rw-rw-   0        0        0      486 2023-05-03 21:29:30.000000 slippy_api-0.1/slippy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-03 21:29:30.000000 slippy_api-0.1/slippy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 21:29:30.000000 slippy_api-0.1/slippy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 21:29:30.000000 slippy_api-0.1/slippy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 21:46:07.352158 slippy_api-0.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-03 21:18:14.000000 slippy_api-0.2/LICENSE
+-rw-rw-rw-   0        0        0      142 2023-05-03 21:43:44.000000 slippy_api-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      486 2023-05-03 21:46:07.351161 slippy_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-05-03 21:14:37.000000 slippy_api-0.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-03 21:18:46.000000 slippy_api-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2023-05-01 22:45:43.000000 slippy_api-0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 21:46:07.352158 slippy_api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-05-03 21:44:58.000000 slippy_api-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:46:07.333157 slippy_api-0.2/slippi/
+-rw-rw-rw-   0        0        0        0 2023-04-18 00:49:17.000000 slippy_api-0.2/slippi/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-05-03 20:50:52.000000 slippy_api-0.2/slippi/main.py
+-rw-rw-rw-   0        0        0     4170 2023-05-01 22:57:10.000000 slippy_api-0.2/slippi/slippi_api.py
+-rw-rw-rw-   0        0        0     2240 2023-05-01 22:01:29.000000 slippy_api-0.2/slippi/slippi_characters.py
+-rw-rw-rw-   0        0        0     1500 2023-05-01 21:31:57.000000 slippy_api-0.2/slippi/slippi_ranks.py
+-rw-rw-rw-   0        0        0     4096 2023-05-01 23:08:27.000000 slippy_api-0.2/slippi/slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:46:07.337160 slippy_api-0.2/slippi/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-01 22:44:38.000000 slippy_api-0.2/slippi/tests/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-05-01 22:58:46.000000 slippy_api-0.2/slippi/tests/test_slippi_api.py
+-rw-rw-rw-   0        0        0      671 2023-05-01 22:51:54.000000 slippy_api-0.2/slippi/tests/test_slippi_characters.py
+-rw-rw-rw-   0        0        0      885 2023-05-01 22:52:07.000000 slippy_api-0.2/slippi/tests/test_slippi_ranks.py
+-rw-rw-rw-   0        0        0     4628 2023-05-01 22:51:39.000000 slippy_api-0.2/slippi/tests/test_slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:46:07.350159 slippy_api-0.2/slippy_api.egg-info/
+-rw-rw-rw-   0        0        0      486 2023-05-03 21:46:07.000000 slippy_api-0.2/slippy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-05-03 21:46:07.000000 slippy_api-0.2/slippy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 21:46:07.000000 slippy_api-0.2/slippy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 21:46:07.000000 slippy_api-0.2/slippy_api.egg-info/top_level.txt
```

### Comparing `slippy_api-0.1/LICENSE` & `slippy_api-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/main.py` & `slippy_api-0.2/slippi/main.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/slippi_api.py` & `slippy_api-0.2/slippi/slippi_api.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/slippi_characters.py` & `slippy_api-0.2/slippi/slippi_characters.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/slippi_ranks.py` & `slippy_api-0.2/slippi/slippi_ranks.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/slippi_user.py` & `slippy_api-0.2/slippi/slippi_user.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/tests/test_slippi_api.py` & `slippy_api-0.2/slippi/tests/test_slippi_api.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/tests/test_slippi_characters.py` & `slippy_api-0.2/slippi/tests/test_slippi_characters.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/tests/test_slippi_ranks.py` & `slippy_api-0.2/slippi/tests/test_slippi_ranks.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.1/slippi/tests/test_slippi_user.py` & `slippy_api-0.2/slippi/tests/test_slippi_user.py`

 * *Files identical despite different names*

