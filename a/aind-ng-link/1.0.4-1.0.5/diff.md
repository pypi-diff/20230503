# Comparing `tmp/aind-ng-link-1.0.4.tar.gz` & `tmp/aind-ng-link-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-ng-link-1.0.4.tar", last modified: Fri Apr 28 18:02:14 2023, max compression
+gzip compressed data, was "aind-ng-link-1.0.5.tar", last modified: Wed May  3 16:28:12 2023, max compression
```

## Comparing `aind-ng-link-1.0.4.tar` & `aind-ng-link-1.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.931219 aind-ng-link-1.0.4/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      170 2023-04-27 22:23:53.000000 aind-ng-link-1.0.4/.flake8
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.773700 aind-ng-link-1.0.4/.github/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.810050 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.823229 aind-ng-link-1.0.4/.github/workflows/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.github/workflows/tag.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2199 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/.gitignore
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/LICENSE
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 18:02:14.930206 aind-ng-link-1.0.4/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 00:41:21.000000 aind-ng-link-1.0.4/README.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.836497 aind-ng-link-1.0.4/doc_template/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/Makefile
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/make.bat
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.844325 aind-ng-link-1.0.4/doc_template/source/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/source/conf.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/doc_template/source/index.rst
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1610 2023-04-28 17:53:08.000000 aind-ng-link-1.0.4/pyproject.toml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2269 2023-04-28 16:05:38.000000 aind-ng-link-1.0.4/requirements.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-04-28 18:02:14.931500 aind-ng-link-1.0.4/setup.cfg
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      256 2023-04-28 15:26:22.000000 aind-ng-link-1.0.4/setup.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.775862 aind-ng-link-1.0.4/src/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.854281 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      961 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      137 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/requires.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-04-28 18:02:14.000000 aind-ng-link-1.0.4/src/aind_ng_link.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.899747 aind-ng-link-1.0.4/src/ng_link/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      183 2023-04-28 18:01:35.000000 aind-ng-link-1.0.4/src/ng_link/__init__.py
--rw-------   0 jonathan.wong   (502) staff       (20)     6457 2023-04-28 16:50:07.000000 aind-ng-link-1.0.4/src/ng_link/dispim_link.py
--rw-------   0 jonathan.wong   (502) staff       (20)     3704 2023-04-28 16:50:21.000000 aind-ng-link-1.0.4/src/ng_link/exaspim_link.py
--rw-------   0 jonathan.wong   (502) staff       (20)     4403 2023-04-28 16:48:59.000000 aind-ng-link-1.0.4/src/ng_link/link_utils.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.4/src/ng_link/ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-27 22:17:45.000000 aind-ng-link-1.0.4/src/ng_link/ng_state.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.913012 aind-ng-link-1.0.4/src/ng_link/scripts/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.4/src/ng_link/scripts/ccf_ref.csv
--rw-------   0 jonathan.wong   (502) staff       (20)      894 2023-04-28 16:43:46.000000 aind-ng-link-1.0.4/src/ng_link/scripts/create_links.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     6945 2023-04-27 22:24:18.000000 aind-ng-link-1.0.4/src/ng_link/scripts/generate_cff_cell_count.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.918990 aind-ng-link-1.0.4/src/ng_link/utils/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/src/ng_link/utils/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.4/src/ng_link/utils/utils.py
--rw-------   0 jonathan.wong   (502) staff       (20)     2545 2023-04-28 16:51:41.000000 aind-ng-link-1.0.4/src/ng_link/xml_parsing.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-04-28 18:02:14.928197 aind-ng-link-1.0.4/tests/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/tests/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.4/tests/test_ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.4/tests/test_ng_state.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.339367 aind-ng-link-1.0.5/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      170 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/.flake8
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.088622 aind-ng-link-1.0.5/.github/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.141366 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.169923 aind-ng-link-1.0.5/.github/workflows/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/workflows/ci.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/workflows/tag.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2199 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.gitignore
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/LICENSE
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-03 16:28:12.338487 aind-ng-link-1.0.5/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/README.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.179018 aind-ng-link-1.0.5/doc_template/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/Makefile
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/make.bat
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.189262 aind-ng-link-1.0.5/doc_template/source/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/source/conf.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/source/index.rst
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1610 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/pyproject.toml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2269 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/requirements.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-05-03 16:28:12.339589 aind-ng-link-1.0.5/setup.cfg
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      256 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/setup.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.091113 aind-ng-link-1.0.5/src/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.200680 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      961 2023-05-03 16:28:12.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      137 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/requires.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.249569 aind-ng-link-1.0.5/src/ng_link/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      181 2023-05-03 16:24:50.000000 aind-ng-link-1.0.5/src/ng_link/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     6444 2023-05-02 17:25:23.000000 aind-ng-link-1.0.5/src/ng_link/dispim_link.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     3691 2023-05-03 16:22:24.000000 aind-ng-link-1.0.5/src/ng_link/exaspim_link.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     4403 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/link_utils.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.5/src/ng_link/ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/ng_state.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.282405 aind-ng-link-1.0.5/src/ng_link/scripts/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.5/src/ng_link/scripts/ccf_ref.csv
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      909 2023-05-02 17:27:04.000000 aind-ng-link-1.0.5/src/ng_link/scripts/create_links.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     6945 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/scripts/generate_cff_cell_count.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.299290 aind-ng-link-1.0.5/src/ng_link/utils/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/src/ng_link/utils/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.5/src/ng_link/utils/utils.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2545 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/xml_parsing.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.337280 aind-ng-link-1.0.5/tests/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/tests/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.5/tests/test_ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/tests/test_ng_state.py
```

### Comparing `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/.github/ISSUE_TEMPLATE/user-story.md` & `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/.github/workflows/ci.yml` & `aind-ng-link-1.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/.github/workflows/tag.yml` & `aind-ng-link-1.0.5/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/.gitignore` & `aind-ng-link-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/LICENSE` & `aind-ng-link-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/PKG-INFO` & `aind-ng-link-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.4/README.md` & `aind-ng-link-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/doc_template/Makefile` & `aind-ng-link-1.0.5/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/doc_template/make.bat` & `aind-ng-link-1.0.5/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/doc_template/source/conf.py` & `aind-ng-link-1.0.5/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/pyproject.toml` & `aind-ng-link-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/requirements.txt` & `aind-ng-link-1.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/aind_ng_link.egg-info/PKG-INFO` & `aind-ng-link-1.0.5/src/aind_ng_link.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.4/src/aind_ng_link.egg-info/SOURCES.txt` & `aind-ng-link-1.0.5/src/aind_ng_link.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/dispim_link.py` & `aind-ng-link-1.0.5/src/ng_link/dispim_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 Library for generating dispim link.
 """
 import numpy as np
 
-from ng_link import NgState
-
-import xml_parsing
-import link_utils
+from ng_link import NgState, xml_parsing, link_utils
 
 
 def apply_deskewing(matrix_3x4: np.ndarray, theta: float = 45) -> np.ndarray:
     """
     Compounds deskewing transform to input 3x4 matrix:
         Deskewing @ Input_3x4_Matrix.
```

### Comparing `aind-ng-link-1.0.4/src/ng_link/exaspim_link.py` & `aind-ng-link-1.0.5/src/ng_link/exaspim_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 Library for generating exaspim link.
 """
 import numpy as np
 
-from ng_link import NgState
-
-import xml_parsing
-import link_utils
+from ng_link import NgState, xml_parsing, link_utils
 
 def omit_initial_offsets(view_transforms: dict[int, list[dict]]) -> None:
     """
     For OME-Zarr datasets, inital offsets are
     already encoded in the metadata and extracted my neuroglancer.
     This function removes the duplicate transform.
```

### Comparing `aind-ng-link-1.0.4/src/ng_link/link_utils.py` & `aind-ng-link-1.0.5/src/ng_link/link_utils.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/ng_layer.py` & `aind-ng-link-1.0.5/src/ng_link/ng_layer.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/ng_state.py` & `aind-ng-link-1.0.5/src/ng_link/ng_state.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/scripts/ccf_ref.csv` & `aind-ng-link-1.0.5/src/ng_link/scripts/ccf_ref.csv`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/scripts/create_links.py` & `aind-ng-link-1.0.5/src/ng_link/scripts/create_links.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # from ng_link import exaspim_link
 from ng_link import dispim_link
 
 def main():
     # Fill in your own data
     base_channel_path = (
-        "/Users/jonathan.wong/Projects/aind-ng-link/dispim_new.xml"
+        "/Users/jonathan.wong/Projects/aind-ng-link/registered_tester.xml"
     )
     cross_channel_path = (
-        "/Users/jonathan.wong/Projects/aind-ng-link/dispim_new_coreg.xml"
+        "/Users/jonathan.wong/Projects/aind-ng-link/registered_tester_coreg.xml"
     )
     s3_path = (
         "s3://aind-open-data/diSPIM_647459_2022-12-21_00-39-00/diSPIM.zarr"
     )
 
     # exaspim_link.generate_exaspim_link(
     #     base_channel_path,
@@ -24,14 +24,14 @@
     dispim_link.generate_dispim_link(
         base_channel_path,
         cross_channel_path,
         s3_path,
         max_dr=800,
         opacity=0.5,
         blend="additive",
-        deskew_angle=45,
+        deskew_angle=-45,
         output_json_path=".",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aind-ng-link-1.0.4/src/ng_link/scripts/generate_cff_cell_count.py` & `aind-ng-link-1.0.5/src/ng_link/scripts/generate_cff_cell_count.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/utils/utils.py` & `aind-ng-link-1.0.5/src/ng_link/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.4/src/ng_link/xml_parsing.py` & `aind-ng-link-1.0.5/src/ng_link/xml_parsing.py`

 * *Files identical despite different names*

