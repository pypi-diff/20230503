# Comparing `tmp/iqm-client-9.7.tar.gz` & `tmp/iqm-client-9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-client-9.7.tar", last modified: Tue Dec 20 14:08:34 2022, max compression
+gzip compressed data, was "iqm-client-9.8.tar", last modified: Tue Dec 20 15:30:27 2022, max compression
```

## Comparing `iqm-client-9.7.tar` & `iqm-client-9.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.806888 iqm-client-9.7/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-20 14:07:40.000000 iqm-client-9.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.798888 iqm-client-9.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.802888 iqm-client-9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2022-12-20 14:07:40.000000 iqm-client-9.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2022-12-20 14:07:40.000000 iqm-client-9.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-20 14:07:40.000000 iqm-client-9.7/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-20 14:07:40.000000 iqm-client-9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-20 14:07:40.000000 iqm-client-9.7/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-20 14:07:40.000000 iqm-client-9.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-20 14:07:40.000000 iqm-client-9.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2022-12-20 14:07:40.000000 iqm-client-9.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-20 14:07:40.000000 iqm-client-9.7/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-20 14:07:40.000000 iqm-client-9.7/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2022-12-20 14:07:40.000000 iqm-client-9.7/INTEGRATION_GUIDE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-20 14:07:40.000000 iqm-client-9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-20 14:08:34.806888 iqm-client-9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-20 14:07:40.000000 iqm-client-9.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.802888 iqm-client-9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.798888 iqm-client-9.7/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.802888 iqm-client-9.7/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.802888 iqm-client-9.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/integration_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-20 14:07:40.000000 iqm-client-9.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-20 14:07:40.000000 iqm-client-9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-20 14:08:34.806888 iqm-client-9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-20 14:07:40.000000 iqm-client-9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.798888 iqm-client-9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.806888 iqm-client-9.7/src/iqm_client/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-20 14:07:40.000000 iqm-client-9.7/src/iqm_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34346 2022-12-20 14:07:40.000000 iqm-client-9.7/src/iqm_client/iqm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 14:07:40.000000 iqm-client-9.7/src/iqm_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.806888 iqm-client-9.7/src/iqm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-20 14:08:34.000000 iqm-client-9.7/src/iqm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-20 14:08:34.000000 iqm-client-9.7/src/iqm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:08:34.000000 iqm-client-9.7/src/iqm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:08:11.000000 iqm-client-9.7/src/iqm_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-20 14:08:34.000000 iqm-client-9.7/src/iqm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 14:08:34.000000 iqm-client-9.7/src/iqm_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-20 14:07:40.000000 iqm-client-9.7/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.806888 iqm-client-9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:08:34.806888 iqm-client-9.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/resources/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2022-12-20 14:07:40.000000 iqm-client-9.7/tests/test_iqm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2022-12-20 14:07:40.000000 iqm-client-9.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.283018 iqm-client-9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-20 15:29:32.000000 iqm-client-9.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.263019 iqm-client-9.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.271019 iqm-client-9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2022-12-20 15:29:32.000000 iqm-client-9.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2022-12-20 15:29:32.000000 iqm-client-9.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-20 15:29:32.000000 iqm-client-9.8/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-20 15:29:32.000000 iqm-client-9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-20 15:29:32.000000 iqm-client-9.8/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-20 15:29:32.000000 iqm-client-9.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-20 15:29:32.000000 iqm-client-9.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2022-12-20 15:29:32.000000 iqm-client-9.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-20 15:29:32.000000 iqm-client-9.8/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-20 15:29:32.000000 iqm-client-9.8/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2022-12-20 15:29:32.000000 iqm-client-9.8/INTEGRATION_GUIDE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-20 15:29:32.000000 iqm-client-9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-20 15:30:27.283018 iqm-client-9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-20 15:29:32.000000 iqm-client-9.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.275019 iqm-client-9.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.267019 iqm-client-9.8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.275019 iqm-client-9.8/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.279018 iqm-client-9.8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/integration_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-20 15:29:32.000000 iqm-client-9.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-20 15:29:32.000000 iqm-client-9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-20 15:30:27.283018 iqm-client-9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-20 15:29:32.000000 iqm-client-9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.267019 iqm-client-9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.279018 iqm-client-9.8/src/iqm_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-20 15:29:32.000000 iqm-client-9.8/src/iqm_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34347 2022-12-20 15:29:32.000000 iqm-client-9.8/src/iqm_client/iqm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:32.000000 iqm-client-9.8/src/iqm_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.279018 iqm-client-9.8/src/iqm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-20 15:30:27.000000 iqm-client-9.8/src/iqm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-20 15:30:27.000000 iqm-client-9.8/src/iqm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:30:27.000000 iqm-client-9.8/src/iqm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:30:04.000000 iqm-client-9.8/src/iqm_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-20 15:30:27.000000 iqm-client-9.8/src/iqm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 15:30:27.000000 iqm-client-9.8/src/iqm_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-20 15:29:32.000000 iqm-client-9.8/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.283018 iqm-client-9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:27.283018 iqm-client-9.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/resources/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2022-12-20 15:29:32.000000 iqm-client-9.8/tests/test_iqm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2022-12-20 15:29:32.000000 iqm-client-9.8/tox.ini
```

### Comparing `iqm-client-9.7/.coveragerc` & `iqm-client-9.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/.github/workflows/ci.yml` & `iqm-client-9.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/.github/workflows/publish.yml` & `iqm-client-9.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/.github/workflows/tag_and_release.yml` & `iqm-client-9.8/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/CHANGELOG.rst` & `iqm-client-9.8/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 9.8
+===========
+
+* Bugfix: ``Circuit.metadata`` Pydantic field needs default value. `#64 <https://github.com/iqm-finland/iqm-client/pull/64>`_
+
 Version 9.7
 ===========
 
 * Add optional ``metadata`` field to ``Circuit``. `#63 <https://github.com/iqm-finland/iqm-client/pull/63>`_
 
 Version 9.6
 ===========
```

### Comparing `iqm-client-9.7/DEVELOPMENT.rst` & `iqm-client-9.8/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/INTEGRATION_GUIDE.rst` & `iqm-client-9.8/INTEGRATION_GUIDE.rst`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/LICENSE` & `iqm-client-9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/PKG-INFO` & `iqm-client-9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-client
-Version: 9.7
+Version: 9.8
 Summary: A client library for accessing an IQM quantum computer
 Home-page: https://github.com/iqm-finland/iqm-client
 Author: IQM developers
 Author-email: developers@meetiqm.com
 License: Apache 2.0
 Project-URL: Documentation, https://iqm-finland.github.io/iqm-client
 Platform: any
```

### Comparing `iqm-client-9.7/README.rst` & `iqm-client-9.8/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/Makefile` & `iqm-client-9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_static/images/favicon.ico` & `iqm-client-9.8/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_static/images/logo.png` & `iqm-client-9.8/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_templates/autosummary-class-template.rst` & `iqm-client-9.8/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_templates/autosummary-module-template.rst` & `iqm-client-9.8/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_templates/page.html` & `iqm-client-9.8/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/_templates/versioning.html` & `iqm-client-9.8/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/docs/conf.py` & `iqm-client-9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/pyproject.toml` & `iqm-client-9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/setup.cfg` & `iqm-client-9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/setup.py` & `iqm-client-9.8/setup.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/src/iqm_client/__init__.py` & `iqm-client-9.8/src/iqm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/src/iqm_client/iqm_client.py` & `iqm-client-9.8/src/iqm_client/iqm_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 class Circuit(BaseModel):
     """Quantum circuit to be executed."""
 
     name: str = Field(..., description='name of the circuit', example='test circuit')
     """name of the circuit"""
     instructions: tuple[Instruction, ...] = Field(..., description='instructions comprising the circuit')
     """instructions comprising the circuit"""
-    metadata: Optional[dict[str, Any]] = Field(..., description='arbitrary metadata associated with the circuit')
+    metadata: Optional[dict[str, Any]] = Field(None, description='arbitrary metadata associated with the circuit')
     """arbitrary metadata associated with the circuit"""
 
     def all_qubits(self) -> set[str]:
         """Return the names of all qubits in the circuit."""
         qubits: set[str] = set()
         for instruction in self.instructions:
             qubits.update(instruction.qubits)
```

### Comparing `iqm-client-9.7/src/iqm_client.egg-info/PKG-INFO` & `iqm-client-9.8/src/iqm_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-client
-Version: 9.7
+Version: 9.8
 Summary: A client library for accessing an IQM quantum computer
 Home-page: https://github.com/iqm-finland/iqm-client
 Author: IQM developers
 Author-email: developers@meetiqm.com
 License: Apache 2.0
 Project-URL: Documentation, https://iqm-finland.github.io/iqm-client
 Platform: any
```

### Comparing `iqm-client-9.7/src/iqm_client.egg-info/SOURCES.txt` & `iqm-client-9.8/src/iqm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tag-from-pipeline.sh` & `iqm-client-9.8/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tests/conftest.py` & `iqm-client-9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tests/resources/tokens.json` & `iqm-client-9.8/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tests/test_authentication.py` & `iqm-client-9.8/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tests/test_iqm_client.py` & `iqm-client-9.8/tests/test_iqm_client.py`

 * *Files identical despite different names*

### Comparing `iqm-client-9.7/tox.ini` & `iqm-client-9.8/tox.ini`

 * *Files identical despite different names*

