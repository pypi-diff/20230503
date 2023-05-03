# Comparing `tmp/types-regex-2023.3.23.1.tar.gz` & `tmp/types-regex-2023.5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2023.3.23.1.tar", last modified: Tue Mar 28 12:32:41 2023, max compression
+gzip compressed data, was "types-regex-2023.5.4.0.tar", last modified: Wed May  3 01:15:30 2023, max compression
```

## Comparing `types-regex-2023.3.23.1.tar` & `types-regex-2023.5.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:41.421576 types-regex-2023.3.23.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-28 12:32:40.000000 types-regex-2023.3.23.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:32:40.000000 types-regex-2023.3.23.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-28 12:32:41.417576 types-regex-2023.3.23.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:41.417576 types-regex-2023.3.23.1/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-28 12:32:40.000000 types-regex-2023.3.23.1/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:32:25.000000 types-regex-2023.3.23.1/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-28 12:32:25.000000 types-regex-2023.3.23.1/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-28 12:32:25.000000 types-regex-2023.3.23.1/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-03-28 12:32:25.000000 types-regex-2023.3.23.1/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:32:41.421576 types-regex-2023.3.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-28 12:32:40.000000 types-regex-2023.3.23.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:41.417576 types-regex-2023.3.23.1/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-28 12:32:41.000000 types-regex-2023.3.23.1/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-28 12:32:41.000000 types-regex-2023.3.23.1/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:32:41.000000 types-regex-2023.3.23.1/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 12:32:41.000000 types-regex-2023.3.23.1/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:15:30.750081 types-regex-2023.5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-03 01:15:28.000000 types-regex-2023.5.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 01:15:28.000000 types-regex-2023.5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 01:15:30.750081 types-regex-2023.5.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:15:30.750081 types-regex-2023.5.4.0/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 01:15:28.000000 types-regex-2023.5.4.0/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 01:15:14.000000 types-regex-2023.5.4.0/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-03 01:15:14.000000 types-regex-2023.5.4.0/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 01:15:14.000000 types-regex-2023.5.4.0/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-03 01:15:14.000000 types-regex-2023.5.4.0/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:15:30.750081 types-regex-2023.5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-03 01:15:28.000000 types-regex-2023.5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:15:30.750081 types-regex-2023.5.4.0/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 01:15:30.000000 types-regex-2023.5.4.0/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 01:15:30.000000 types-regex-2023.5.4.0/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:15:30.000000 types-regex-2023.5.4.0/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 01:15:30.000000 types-regex-2023.5.4.0/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2023.3.23.1/CHANGELOG.md` & `types-regex-2023.5.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 2023.5.4.0 (2023-05-03)
+
+[stubsabot] Bump regex to 2023.5.4 (#10131)
+
+Release: https://pypi.org/pypi/regex/2023.5.4
+Homepage: https://github.com/mrabarnett/mrab-regex
+Diff: https://github.com/mrabarnett/mrab-regex/compare/2023.3.23...2023.5.4
+
+Stubsabot analysis of the diff between the two releases:
+ - Total lines of Python code added: 8.
+ - Total lines of Python code deleted: 3.
+
 ## 2023.3.23.1 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 2023.3.23.0 (2023-03-24)
 
 [stubsabot] Bump regex to 2023.3.23 (#9933)
```

### Comparing `types-regex-2023.3.23.1/PKG-INFO` & `types-regex-2023.5.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.3.23.1
+Version: 2023.5.4.0
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `06878a98be134ac9f10446980b03903301ec845e`.
```

### Comparing `types-regex-2023.3.23.1/regex-stubs/_regex.pyi` & `types-regex-2023.5.4.0/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.3.23.1/regex-stubs/_regex_core.pyi` & `types-regex-2023.5.4.0/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.3.23.1/regex-stubs/regex.pyi` & `types-regex-2023.5.4.0/regex-stubs/regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.3.23.1/setup.py` & `types-regex-2023.5.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `06878a98be134ac9f10446980b03903301ec845e`.
 '''.lstrip()
 
 setup(name=name,
-      version="2023.3.23.1",
+      version="2023.5.4.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2023.3.23.1/types_regex.egg-info/PKG-INFO` & `types-regex-2023.5.4.0/types_regex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.3.23.1
+Version: 2023.5.4.0
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `06878a98be134ac9f10446980b03903301ec845e`.
```

