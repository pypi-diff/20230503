# Comparing `tmp/osm_easy_api-0.3.0.tar.gz` & `tmp/osm_easy_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-0.3.0.tar", last modified: Tue Mar 14 14:32:25 2023, max compression
+gzip compressed data, was "osm_easy_api-0.4.0.tar", last modified: Wed May  3 18:27:08 2023, max compression
```

## Comparing `osm_easy_api-0.3.0.tar` & `osm_easy_api-0.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.805922 osm_easy_api-0.3.0/
--rw-rw-rw-   0        0        0     1564 2023-03-14 14:29:44.000000 osm_easy_api-0.3.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0    42753 2023-03-14 14:32:25.806920 osm_easy_api-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2023-03-14 14:28:57.000000 osm_easy_api-0.3.0/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-03-14 14:32:25.808287 osm_easy_api-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.736043 osm_easy_api-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.756205 osm_easy_api-0.3.0/src/osm_easy_api/
--rw-rw-rw-   0        0        0      161 2023-03-14 14:29:32.000000 osm_easy_api-0.3.0/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.777605 osm_easy_api-0.3.0/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.787022 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    13815 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     3759 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    16106 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5426 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    10841 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     6799 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.798790 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     4271 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      282 2023-03-08 21:13:45.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1183 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     1465 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-03-14 14:12:31.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     1016 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     1534 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0      945 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.801156 osm_easy_api-0.3.0/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-03-08 21:21:55.000000 osm_easy_api-0.3.0/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-0.3.0/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.804912 osm_easy_api-0.3.0/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-0.3.0/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-03-14 14:32:25.772472 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    42753 2023-03-14 14:32:25.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-03-14 14:32:25.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 14:32:25.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-03-14 14:32:25.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-14 14:32:25.000000 osm_easy_api-0.3.0/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.301620 osm_easy_api-0.4.0/
+-rw-rw-rw-   0        0        0     2741 2023-05-03 18:26:26.000000 osm_easy_api-0.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/LICENSE.md
+-rw-rw-rw-   0        0        0    44021 2023-05-03 18:27:08.301620 osm_easy_api-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4542 2023-03-23 20:46:05.000000 osm_easy_api-0.4.0/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-05-03 18:27:08.308134 osm_easy_api-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.242055 osm_easy_api-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.254380 osm_easy_api-0.4.0/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-05-03 18:26:45.000000 osm_easy_api-0.4.0/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.276668 osm_easy_api-0.4.0/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.284231 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14405 2023-04-02 18:15:22.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4369 2023-04-02 18:15:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17037 2023-04-02 18:17:01.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5540 2023-04-02 18:17:21.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-04-02 18:18:10.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.295442 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     4381 2023-03-23 20:30:50.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1183 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2683 2023-05-03 17:59:51.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1707 2023-05-03 17:48:59.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.297624 osm_easy_api-0.4.0/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.300625 osm_easy_api-0.4.0/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.272122 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    44021 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-0.3.0/CHANGELOG.md` & `osm_easy_api-0.4.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0]
+### Added
+- `to_dict()` method and `from_dict()` class method to `Note`.  
+- `to_dict()` method and `from_dict()` class method to `Comment`.
+- `to_dict()` method and `from_dict()` class method to `User`.
+- Documentation about `Meta` and `Action` class.
+- Assert error (with information to report it on github) when api returns an error code not described on the wiki.
+- `to_dict()` method and `from_dict()` class method to `(relation) Member`.
+
+### Fixed
+- `Note` can now be imported from package.
+- `Comment` can now be imported from package.
+- `User` can now be imported from package.
+- `Member` can now be imported from package.
+- Pdoc command in `README.md`.
+- `Relation.to_dict()` method now recursively serialises members.
+- `Way.to_dict()` method now recursively serialises nodes.
+
+### Changed
+- Changed imports in `Relation.py` to use importing through a module rather than directly from a file.
+- Added `sample_dataclasses.py` file in tests fixtures to reduce code duplication.
+- Changed function name and deleted unnecessary argument in `append_elements_to_master_element()` nested inside private method `_to_xml()` in `OsmChange`.
+
 ## [0.3.0] - 2023-03-14
 
 ### Added
 - `to_dict()` method and `from_dict()` class method to Changeset. [#7](https://github.com/docentYT/osm_easy_api/issues/7)
 - Ability to set user_agent in `Diff` and `Api` class. [#5](https://github.com/docentYT/osm_easy_api/issues/5)
 - `osm_object_primitive` `from_dict()` class method now raises `ValueError` if the `type` key is not found.
```

### Comparing `osm_easy_api-0.3.0/LICENSE.md` & `osm_easy_api-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/PKG-INFO` & `osm_easy_api-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -22,17 +22,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 # osm_easy_api
 
 ![Tests](https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg)
-![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/0ccbb839a128ad6f69f7e0d160c4eb32d273389a/coverage-badge.svg)
+![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg)
 [![PyPI version](https://badge.fury.io/py/osm_easy_api.svg)](https://badge.fury.io/py/osm_easy_api)
 
+[Me on openstreetmap](https://www.openstreetmap.org/user/kwiatek_123)
+
 Python package for parsing osm diffs and communicating with the osm api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
 ## What next?
@@ -48,15 +50,15 @@
 ``` 
 
 # Documentation
 
 You can view documentation on [github-pages](https://docentyt.github.io/osm_easy_api/osm_easy_api.html).
 
 Documentation is build using [pdoc](https://pdoc.dev).
-To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source src !src.utils`.
+To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source osm_easy_api !osm_easy_api.utils`.
 
 # Examples
 
 ## DIFF
 
 ### Print trees
 
@@ -160,14 +162,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0]
+### Added
+- `to_dict()` method and `from_dict()` class method to `Note`.  
+- `to_dict()` method and `from_dict()` class method to `Comment`.
+- `to_dict()` method and `from_dict()` class method to `User`.
+- Documentation about `Meta` and `Action` class.
+- Assert error (with information to report it on github) when api returns an error code not described on the wiki.
+- `to_dict()` method and `from_dict()` class method to `(relation) Member`.
+
+### Fixed
+- `Note` can now be imported from package.
+- `Comment` can now be imported from package.
+- `User` can now be imported from package.
+- `Member` can now be imported from package.
+- Pdoc command in `README.md`.
+- `Relation.to_dict()` method now recursively serialises members.
+- `Way.to_dict()` method now recursively serialises nodes.
+
+### Changed
+- Changed imports in `Relation.py` to use importing through a module rather than directly from a file.
+- Added `sample_dataclasses.py` file in tests fixtures to reduce code duplication.
+- Changed function name and deleted unnecessary argument in `append_elements_to_master_element()` nested inside private method `_to_xml()` in `OsmChange`.
+
 ## [0.3.0] - 2023-03-14
 
 ### Added
 - `to_dict()` method and `from_dict()` class method to Changeset. [#7](https://github.com/docentYT/osm_easy_api/issues/7)
 - Ability to set user_agent in `Diff` and `Api` class. [#5](https://github.com/docentYT/osm_easy_api/issues/5)
 - `osm_object_primitive` `from_dict()` class method now raises `ValueError` if the `type` key is not found.
```

### Comparing `osm_easy_api-0.3.0/README.md` & `osm_easy_api-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # osm_easy_api
 
 ![Tests](https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg)
-![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/0ccbb839a128ad6f69f7e0d160c4eb32d273389a/coverage-badge.svg)
+![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg)
 [![PyPI version](https://badge.fury.io/py/osm_easy_api.svg)](https://badge.fury.io/py/osm_easy_api)
 
+[Me on openstreetmap](https://www.openstreetmap.org/user/kwiatek_123)
+
 Python package for parsing osm diffs and communicating with the osm api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
 ## What next?
@@ -23,15 +25,15 @@
 ``` 
 
 # Documentation
 
 You can view documentation on [github-pages](https://docentyt.github.io/osm_easy_api/osm_easy_api.html).
 
 Documentation is build using [pdoc](https://pdoc.dev).
-To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source src !src.utils`.
+To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source osm_easy_api !osm_easy_api.utils`.
 
 # Examples
 
 ## DIFF
 
 ### Print trees
```

### Comparing `osm_easy_api-0.3.0/setup.cfg` & `osm_easy_api-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/api.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             url=join_url(self.outer._url.changeset["get"], param),
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
 
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_changeset(generator, include_discussion)[0] # type: ignore
 
     def get_query(self, left: float | None = None, bottom: float | None = None, right: float | None = None, top: float | None = None,
     user_id: str | None = None, display_name: str | None = None,
     time_one: str | None = None, time_two: str | None = None,
     open: bool = False, closed: bool = False,
@@ -164,14 +165,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
 
         match status_code:
             case 200: pass
             case 400: raise ValueError("Invalid arguments. See https://wiki.openstreetmap.org/wiki/API_v0.6#Query:_GET_/api/0.6/changesets for more info.")
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_changeset(generator) # type: ignore
     
     def update(self, id: int, comment: str | None = None, tags: Tags | None = None) -> Changeset:
         """Updates the changeset with new comment or tags or both.
 
         Args:
@@ -211,14 +213,15 @@
         response = self.outer._request(self.outer._RequestMethods.PUT,
             self.outer._url.changeset["update"].format(id=id), self.outer._Requirement.YES, body=xml_str, stream=True, auto_status_code_handling = False)
 
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.text)
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
         response.raw.decode_content = True
         return self._xml_to_changeset(self.outer._raw_stream_parser(response.raw), True)[0]
 
     def close(self, id: int) -> None:
         """Close changeset by ID.
 
@@ -230,14 +233,15 @@
             exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor: The changeset was already closer or you are not the author.
         """
         response = self.outer._request(self.outer._RequestMethods.PUT, self.outer._url.changeset["close"].format(id = id), self.outer._Requirement.YES, auto_status_code_handling = False)
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.text)
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
     def download(self, id: int) -> Generator[Tuple['Action', 'Node | Way | Relation'], None, None]:
         """Download changes made in changeset. Like in 'diff' module.
 
         Args:
             id (int): Changeset ID.
 
@@ -248,14 +252,15 @@
             Generator: Diff generator like in 'diff' module.
         """
         stream = self.outer._request(self.outer._RequestMethods.GET, self.outer._url.changeset["download"].format(id=id), self.outer._Requirement.NO, stream=True, auto_status_code_handling = False)
 
         match stream.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {stream.status_code}. Please report it on github."
         
         stream.raw.decode_content = True
         def generator() -> Generator[tuple['Action', 'Node | Way | Relation'], None, None]:   
             gen = OsmChange_parser_generator(stream.raw, None)
             next(gen) # for meta data
             for action, element in gen: # type: ignore
                 assert isinstance(action, Action), "ERROR::API::ENDPOINTS::CHANGESET::download action TYPE IS NOT EQUAL TO ACTION"
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             exceptions.ChangesetNotClosed: Changeset must be closed to add comment.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["comment"].format(id=changeset_id, text=text), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 409: raise exceptions.ChangesetNotClosed()
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
     def subscribe(self, changeset_id: int) -> None:
         """Subscribe to the discussion to receive notifications for new comments.
 
         Args:
             changeset_id (int): Changeset id.
 
@@ -34,14 +35,15 @@
             exceptions.AlreadySubscribed: You are already subscribed to this changeset.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["subscribe"].format(id=changeset_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 409: raise exceptions.AlreadySubscribed()
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
     def unsubscribe(self, changeset_id: int) -> None:
         """Unsubscribe from discussion to stop receiving notifications.
 
         Args:
             changeset_id (int): Changeset id.
 
@@ -49,14 +51,15 @@
             exceptions.NotSubscribed: You are not subscribed to this changeset.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["unsubscribe"].format(id=changeset_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.NotSubscribed()
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
     def hide(self, comment_id: int) -> None:
         """Set visible flag on changeset comment to false. MODERATOR ONLY!
 
         Args:
             comment_id (int): Comment id.
 
@@ -66,14 +69,15 @@
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["hide"].format(comment_id=comment_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 403: raise exceptions.NotAModerator()
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
 
     def unhide(self, comment_id: int) -> None:
         """Set visible flag on changeset comment to true. MODERATOR ONLY!
 
         Args:
             comment_id (int): Comment id.
 
@@ -82,8 +86,9 @@
             exceptions.IdNotFoundError: Comment with provided id not found.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["unhide"].format(comment_id=comment_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 403: raise exceptions.NotAModerator()
-            case 404: raise exceptions.IdNotFoundError()
+            case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/elements.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         response = self.outer._request(self.outer._RequestMethods.PUT, self.outer._url.elements["create"].format(element_type=element_name), self.outer._Requirement.YES, body=body, auto_status_code_handling=False)
 
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.content)
             case 412: raise ValueError(response.content)
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
         
         return int(response.text)
 
     def get(self, element: type[Node_Way_Relation], id: int) -> Node_Way_Relation :
         """""Get element by id
 
         Args:
@@ -65,14 +66,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 410: raise exceptions.ElementDeleted()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
         
         for event, elem in generator:
             if elem.tag in ("node", "way", "relation") and event == "start":
                 object = _element_to_osm_object(elem)
                 return object
             
         return object
@@ -100,14 +102,15 @@
 
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 409: raise ValueError(response.content)
             case 404: raise exceptions.IdNotFoundError()
             case 412: raise exceptions.IdNotFoundError(response.content)
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
         return int(response.content)
     
     def delete(self, element: Node | Way | Relation, changeset_id: int) -> int:
         """Deletes element. 
 
         Args:
             element (Node | Way | Relation): Element object which you want to delete. Id is not sufficient.
@@ -131,14 +134,15 @@
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.content)
             case 410: raise exceptions.ElementDeleted()
             case 412: raise ValueError(response.content)
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
         return int(response.content)
     
     def history(self, element: type[Node_Way_Relation], id: int) -> list[Node_Way_Relation]:
         """Returns all old versions of element.
 
         Args:
             element (type[Node_Way_Relation]): Element type to search for.
@@ -156,14 +160,15 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
         
         objects_list = []
         for event, elem in generator:
             if elem.tag == element_name and event == "start":
                 objects_list.append(_element_to_osm_object(elem))
             
         return objects_list
@@ -190,14 +195,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 403: raise exceptions.IdNotFoundError("This version of the element is not available (due to redaction)")
             case 404: raise exceptions.IdNotFoundError()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
         
         for event, elem in generator:
             if elem.tag in ("node", "way", "relation"):
                 object = _element_to_osm_object(elem)
                 return object
         assert False, "[ERROR::API::ENDPOINTS::ELEMENTS::version] Cannot create an element."
     
@@ -227,14 +233,15 @@
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError()
             case 404: raise exceptions.IdNotFoundError()
             case 414: raise ValueError("URL too long (too many ids)")
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
         
         objects_list = []
         for event, elem in generator:
             if elem.tag == element.__name__.lower() and event == "start":
                 objects_list.append(_element_to_osm_object(elem))
             
         return objects_list
@@ -306,14 +313,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 410: raise exceptions.ElementDeleted()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
         
         nodes_dict: dict[int, Node] = {}
         ways_dict:  dict[int, Way]  = {}
         relations_dict: dict[int, Relation] = {}
         for event, elem in generator:
             if event == "start":
                 if elem.tag == "node":
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,16 @@
                 auto_status_code_handling=False
             )
 
             match response.status_code:
                 case 200: pass
                 case 400: raise exceptions.LimitsExceeded("You are trying to download too much data.")
                 case 509: raise exceptions.LimitsExceeded("You have downloaded too much data. Please try again later. See https://wiki.openstreetmap.org/wiki/Developer_FAQ#I've_been_blocked_from_the_API_for_downloading_too_much._Now_what?")
-            
+                case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+
             response.raw.decode_content = True
             def generator():
                 gen = OsmChange_parser_generator(response.raw, None)
                 next(gen) # for meta data
                 for action, element in gen: # type: ignore
                     yield element           # type: ignore
             return generator()
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError("Limits exceeded")
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_note(generator)
     
     def create(self, latitude: str, longitude: str, text: str) -> Note:
         """Creates new note.
 
         Args:
@@ -150,14 +151,15 @@
             auth_requirement=self.outer._Requirement.YES,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyClosed()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_note(generator)[0]
     
     def close(self, id: int, text: str | None = None) -> Note:
         """Close a note as fixed.
 
         Args:
@@ -179,14 +181,15 @@
             auth_requirement=self.outer._Requirement.YES,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyClosed()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_note(generator)[0]
     
     def reopen(self, id: int, text: str | None = None) -> Note:
         """Close a note as fixed.
 
         Args:
@@ -209,14 +212,15 @@
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyOpen()
             case 410: raise exceptions.ElementDeleted()
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         return self._xml_to_note(generator)[0]
     
     def search(self, text: str, limit: int = 100, closed_days: int = 7, user_id: int | None = None, from_date: str | None = None, to_date: str | None = None, sort: str = "updated_at", order: str = "newest") -> list[Note]:
         """Search for notes with initial text and comments.
 
         Args:
@@ -247,12 +251,13 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError("Limits exceeded")
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
 
         try:
             return self._xml_to_note(generator)
         except:
             return []
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         url = self.outer._url.user["preferences"]
         if key:
             url += f"/{key}"
             response = self.outer._request(self.outer._RequestMethods.GET, url, self.outer._Requirement.YES, auto_status_code_handling=False)
             match response.status_code:
                 case 200: pass
                 case 404: raise ValueError("Preference not found")
+                case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
             return {key: response.text}
         generator = self.outer._get_generator(
             url=url,
             auth_requirement=self.outer._Requirement.YES,
             auto_status_code_handling=True)
         
         preferences = {}
@@ -160,8 +161,9 @@
             ValueError: Preference not found.
         """
         url = self.outer._url.user["preferences"]
         url += f"/{key}"
         response = self.outer._request(self.outer._RequestMethods.DELETE, url, self.outer._Requirement.YES, auto_status_code_handling=False)
         match response.status_code:
             case 200: pass
-            case 404: raise ValueError("Preference not found")
+            case 404: raise ValueError("Preference not found")
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-0.4.0/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from typing import NamedTuple
 
 from ..data_classes.node import Node
 from ..data_classes.way import Way
 from ..data_classes.relation import Relation
 
 Meta = NamedTuple("Meta", [("version", str), ("generator", str), ("sequence_number", str)])
+Meta.__doc__ = """\
+    Namedtuple, which stores information about OsmChange.
+    """
 
 class Action(Enum):
+    """Enum that represents the actions performed on an element in a given OsmChange."""
     CREATE = 0
     MODIFY = 1
     DELETE = 2
     NONE = 3
 
 class OsmChange():
     meta: Meta
@@ -47,32 +51,32 @@
     def _to_xml(self, changeset_id):
         root = minidom.Document()
         xml = root.createElement("osmChange")
         xml.setAttribute("version", self.meta.version)
         xml.setAttribute("generator", self.meta.generator)
         root.appendChild(xml)
 
-        def append_elements__to_master_element(main_element, master_name, elements):
+        def append_elements_to_master_element(master_name, elements):
             if not elements: return
             master = root.createElement(master_name)
             for element in elements:
                 master.appendChild(element._to_xml(changeset_id))
             xml.appendChild(master)
             
-        append_elements__to_master_element(xml, "create", self.get(Node, Action.CREATE))
-        append_elements__to_master_element(xml, "modify", self.get(Node, Action.MODIFY))
-        append_elements__to_master_element(xml, "delete", self.get(Node, Action.DELETE))
-
-        append_elements__to_master_element(xml, "create", self.get(Way, Action.CREATE))
-        append_elements__to_master_element(xml, "modify", self.get(Way, Action.MODIFY))
-        append_elements__to_master_element(xml, "delete", self.get(Way, Action.DELETE))
-
-        append_elements__to_master_element(xml, "create", self.get(Relation, Action.CREATE))
-        append_elements__to_master_element(xml, "modify", self.get(Relation, Action.MODIFY))
-        append_elements__to_master_element(xml, "delete", self.get(Relation, Action.DELETE))
+        append_elements_to_master_element("create", self.get(Node, Action.CREATE))
+        append_elements_to_master_element("modify", self.get(Node, Action.MODIFY))
+        append_elements_to_master_element("delete", self.get(Node, Action.DELETE))
+
+        append_elements_to_master_element("create", self.get(Way, Action.CREATE))
+        append_elements_to_master_element("modify", self.get(Way, Action.MODIFY))
+        append_elements_to_master_element("delete", self.get(Way, Action.DELETE))
+
+        append_elements_to_master_element("create", self.get(Relation, Action.CREATE))
+        append_elements_to_master_element("modify", self.get(Relation, Action.MODIFY))
+        append_elements_to_master_element("delete", self.get(Relation, Action.DELETE))
 
         xml_str = root.toprettyxml(indent="\t")
         return xml_str
 
     def get(self, type: type[Node | Way | Relation], action: Action = Action.NONE) -> list[Node | Way | Relation]:
         """Gets list of elements with provided type and action.
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/diff/diff.py` & `osm_easy_api-0.4.0/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-0.4.0/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-0.4.0/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-easy-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -22,17 +22,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 # osm_easy_api
 
 ![Tests](https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg)
-![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/0ccbb839a128ad6f69f7e0d160c4eb32d273389a/coverage-badge.svg)
+![coverage](https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg)
 [![PyPI version](https://badge.fury.io/py/osm_easy_api.svg)](https://badge.fury.io/py/osm_easy_api)
 
+[Me on openstreetmap](https://www.openstreetmap.org/user/kwiatek_123)
+
 Python package for parsing osm diffs and communicating with the osm api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
 ## What next?
@@ -48,15 +50,15 @@
 ``` 
 
 # Documentation
 
 You can view documentation on [github-pages](https://docentyt.github.io/osm_easy_api/osm_easy_api.html).
 
 Documentation is build using [pdoc](https://pdoc.dev).
-To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source src !src.utils`.
+To run docs on your machine use preferred command: `pdoc --docformat google --no-show-source osm_easy_api !osm_easy_api.utils`.
 
 # Examples
 
 ## DIFF
 
 ### Print trees
 
@@ -160,14 +162,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0]
+### Added
+- `to_dict()` method and `from_dict()` class method to `Note`.  
+- `to_dict()` method and `from_dict()` class method to `Comment`.
+- `to_dict()` method and `from_dict()` class method to `User`.
+- Documentation about `Meta` and `Action` class.
+- Assert error (with information to report it on github) when api returns an error code not described on the wiki.
+- `to_dict()` method and `from_dict()` class method to `(relation) Member`.
+
+### Fixed
+- `Note` can now be imported from package.
+- `Comment` can now be imported from package.
+- `User` can now be imported from package.
+- `Member` can now be imported from package.
+- Pdoc command in `README.md`.
+- `Relation.to_dict()` method now recursively serialises members.
+- `Way.to_dict()` method now recursively serialises nodes.
+
+### Changed
+- Changed imports in `Relation.py` to use importing through a module rather than directly from a file.
+- Added `sample_dataclasses.py` file in tests fixtures to reduce code duplication.
+- Changed function name and deleted unnecessary argument in `append_elements_to_master_element()` nested inside private method `_to_xml()` in `OsmChange`.
+
 ## [0.3.0] - 2023-03-14
 
 ### Added
 - `to_dict()` method and `from_dict()` class method to Changeset. [#7](https://github.com/docentYT/osm_easy_api/issues/7)
 - Ability to set user_agent in `Diff` and `Api` class. [#5](https://github.com/docentYT/osm_easy_api/issues/5)
 - `osm_object_primitive` `from_dict()` class method now raises `ValueError` if the `type` key is not found.
```

### Comparing `osm_easy_api-0.3.0/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-0.4.0/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

