# Comparing `tmp/pytest-frappe-0.1.0.tar.gz` & `tmp/pytest-frappe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.1.0.tar", last modified: Mon Apr 17 14:52:17 2023, max compression
+gzip compressed data, was "pytest-frappe-0.1.1.tar", last modified: Wed May  3 17:02:23 2023, max compression
```

## Comparing `pytest-frappe-0.1.0.tar` & `pytest-frappe-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.1.0/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.1.0/Makefile
--rw-r--r--   0        0        0       69 2023-04-14 11:37:30.475170 pytest-frappe-0.1.0/README.md
--rw-r--r--   0        0        0     1411 2023-04-17 14:28:42.325679 pytest-frappe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-17 14:49:40.864164 pytest-frappe-0.1.0/pytest_frappe/__init__.py
--rw-r--r--   0        0        0      963 2023-04-17 14:15:25.070473 pytest-frappe-0.1.0/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      259 2023-04-17 14:35:34.965334 pytest-frappe-0.1.0/pytest_frappe/plugin.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.1.0/setup.cfg
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 pytest-frappe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.1.1/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.1.1/Makefile
+-rw-r--r--   0        0        0     1501 2023-04-17 15:11:03.689905 pytest-frappe-0.1.1/README.md
+-rw-r--r--   0        0        0     1411 2023-04-17 14:28:42.325679 pytest-frappe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-03 16:59:23.178052 pytest-frappe-0.1.1/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0     1186 2023-05-03 16:59:23.590048 pytest-frappe-0.1.1/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      408 2023-05-03 16:53:54.157466 pytest-frappe-0.1.1/pytest_frappe/plugin.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.1.1/setup.cfg
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 pytest-frappe-0.1.1/PKG-INFO
```

### Comparing `pytest-frappe-0.1.0/.gitignore` & `pytest-frappe-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.0/LICENSE` & `pytest-frappe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.0/pyproject.toml` & `pytest-frappe-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.0/pytest_frappe/fixtures.py` & `pytest-frappe-0.1.1/pytest_frappe/fixtures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import pathlib
 import frappe
 import pytest
 
 
-def get_site_configs(sites_path):
+def get_site_configs(sites_path, site=None):
     """Returns the sites path and the current site"""
     sites_path = pathlib.Path(sites_path)
-    current_site = sites_path / "currentsite.txt"
-    with open(current_site, "r") as f:
-        current_site = f.readline().strip()
-    return str(sites_path), current_site
+    if site is None:
+        current_site_file = sites_path / "currentsite.txt"
+        with open(current_site_file, "r") as f:
+            site_to_use = f.readline().strip()
+    else:
+        site_to_use = site
+    return str(sites_path), site_to_use
 
 
 @pytest.fixture(scope="session")
 def db_instance(request):
     """Returns a database instance."""
     sites_path = request.config.getoption("--sites-path")
-    sites_path, current_site = get_site_configs(sites_path)
+    site = request.config.getoption("--site")
+
+    if not sites_path:
+        raise Exception("Please provide the sites path")
+
+    sites_path, current_site = get_site_configs(sites_path, site)
 
     frappe.init(site=current_site, sites_path=sites_path)
     frappe.connect()
 
     # TODO: should we mock the commit method?
     # mock_commit = MagicMock()
     # frappe.db.commit = mock_commit
```

