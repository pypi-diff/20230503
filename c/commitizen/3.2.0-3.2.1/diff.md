# Comparing `tmp/commitizen-3.2.0.tar.gz` & `tmp/commitizen-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.2.0.tar", max compression
+gzip compressed data, was "commitizen-3.2.1.tar", max compression
```

## Comparing `commitizen-3.2.0.tar` & `commitizen-3.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-05-01 18:45:22.914135 commitizen-3.2.0/LICENSE
--rw-r--r--   0        0        0      609 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__version__.py
--rw-r--r--   0        0        0     8609 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/bump.py
--rw-r--r--   0        0        0    11956 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16927 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13932 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7266 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12929 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1575 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7114 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3125 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3327 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/version_types.py
--rw-r--r--   0        0        0     5748 2023-05-01 18:45:22.918135 commitizen-3.2.0/docs/README.md
--rw-r--r--   0        0        0     3929 2023-05-01 18:45:22.930135 commitizen-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 commitizen-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-03 07:33:34.924081 commitizen-3.2.1/LICENSE
+-rw-r--r--   0        0        0      609 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     8609 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/bump.py
+-rw-r--r--   0        0        0    11956 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16927 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13932 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7266 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12929 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-03 07:33:34.924081 commitizen-3.2.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1575 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7114 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3125 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3327 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-05-03 07:33:34.928081 commitizen-3.2.1/commitizen/version_types.py
+-rw-r--r--   0        0        0     5748 2023-05-03 07:33:34.928081 commitizen-3.2.1/docs/README.md
+-rw-r--r--   0        0        0     3938 2023-05-03 07:33:34.940081 commitizen-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 commitizen-3.2.1/PKG-INFO
```

### Comparing `commitizen-3.2.0/LICENSE` & `commitizen-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/__init__.py` & `commitizen-3.2.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/bump.py` & `commitizen-3.2.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/changelog.py` & `commitizen-3.2.1/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/changelog_parser.py` & `commitizen-3.2.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cli.py` & `commitizen-3.2.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cmd.py` & `commitizen-3.2.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/bump.py` & `commitizen-3.2.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/changelog.py` & `commitizen-3.2.1/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/check.py` & `commitizen-3.2.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/commit.py` & `commitizen-3.2.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/init.py` & `commitizen-3.2.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/commands/version.py` & `commitizen-3.2.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/config/__init__.py` & `commitizen-3.2.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/config/base_config.py` & `commitizen-3.2.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/config/json_config.py` & `commitizen-3.2.1/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/config/toml_config.py` & `commitizen-3.2.1/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/config/yaml_config.py` & `commitizen-3.2.1/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/__init__.py` & `commitizen-3.2.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/base.py` & `commitizen-3.2.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.2.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.2.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/customize/customize.py` & `commitizen-3.2.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/jira/jira.py` & `commitizen-3.2.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.2.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/defaults.py` & `commitizen-3.2.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/exceptions.py` & `commitizen-3.2.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/factory.py` & `commitizen-3.2.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/git.py` & `commitizen-3.2.1/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/hooks.py` & `commitizen-3.2.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/out.py` & `commitizen-3.2.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/providers.py` & `commitizen-3.2.1/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/commitizen/version_types.py` & `commitizen-3.2.1/commitizen/version_types.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/docs/README.md` & `commitizen-3.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.0/pyproject.toml` & `commitizen-3.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.2.0"
+version = "3.2.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.2.0"
+version = "3.2.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -42,16 +42,16 @@
 packaging = ">=19"
 tomlkit = ">=0.5.3,<1.0.0"
 jinja2 = ">=2.10.3"
 pyyaml = ">=3.08"
 argcomplete = ">=1.12.1,<3.1"
 typing-extensions = { version = "^4.0.1", python = "<3.8" }
 charset-normalizer = ">=2.1.0,<4"
-# Use the Python 3.11 compatible API: https://github.com/python/importlib_metadata#compatibility
-importlib_metadata = { version = ">=4.13,<5"}
+# Use the Python 3.11 and 3.12 compatible API: https://github.com/python/importlib_metadata#compatibility
+importlib_metadata = { version = ">=4.13,<7"}
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.34"
 # test
 pytest = "^7.2.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.10"
```

### Comparing `commitizen-3.2.0/PKG-INFO` & `commitizen-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.2.0
+Version: 3.2.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: argcomplete (>=1.12.1,<3.1)
 Requires-Dist: charset-normalizer (>=2.1.0,<4)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
 Requires-Dist: decli (>=0.6.0,<0.7.0)
-Requires-Dist: importlib_metadata (>=4.13,<5)
+Requires-Dist: importlib_metadata (>=4.13,<7)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: packaging (>=19)
 Requires-Dist: pyyaml (>=3.08)
 Requires-Dist: questionary (>=1.4.0,<2.0.0)
 Requires-Dist: termcolor (>=1.1,<3)
 Requires-Dist: tomlkit (>=0.5.3,<1.0.0)
 Requires-Dist: typing-extensions (>=4.0.1,<5.0.0) ; python_version < "3.8"
```

