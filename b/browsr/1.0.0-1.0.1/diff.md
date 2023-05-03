# Comparing `tmp/browsr-1.0.0.tar.gz` & `tmp/browsr-1.0.1.tar.gz`

## Comparing `browsr-1.0.0.tar` & `browsr-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.0.0/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.0.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.0.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/__main__.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/_base.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/_version.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/code_browser.css
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 browsr-1.0.0/browsr/code_browser.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.0.0/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.0.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.0.0/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.0.0/docs/index.md
--rw-r--r--   0        0        0    58119 2020-02-02 00:00:00.000000 browsr-1.0.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 browsr-1.0.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.0.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.0.0/README.md
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 browsr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.0.1/.releaserc.js
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.0.1/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.0.1/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/__main__.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/_base.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/_version.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/code_browser.css
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 browsr-1.0.1/browsr/code_browser.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.0.1/docs/api_documentation.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.0.1/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.0.1/docs/contributing.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.0.1/docs/index.md
+-rw-r--r--   0        0        0    58119 2020-02-02 00:00:00.000000 browsr-1.0.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 browsr-1.0.1/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.0.1/README.md
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 browsr-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.0.1/PKG-INFO
```

### Comparing `browsr-1.0.0/.releaserc.js` & `browsr-1.0.1/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/mkdocs.yaml` & `browsr-1.0.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/semantic_release/package-lock.json` & `browsr-1.0.1/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/semantic_release/release_notes.hbs` & `browsr-1.0.1/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/workflows/lint.yaml` & `browsr-1.0.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/workflows/publish.yaml` & `browsr-1.0.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/workflows/release.yaml` & `browsr-1.0.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.github/workflows/tests.yaml` & `browsr-1.0.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/browsr/_base.py` & `browsr-1.0.1/browsr/_base.py`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/browsr/code_browser.py` & `browsr-1.0.1/browsr/code_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         """
         stat = file_path.stat()
         if isinstance(stat, dict):
             file_size = {key.lower(): value for key, value in stat.items()}["size"]
             file_size_mb = file_size / 1000 / 1000
         else:
             file_size_mb = stat.st_size / 1000 / 1000
-        max_file_size = 80
+        max_file_size = 8
         too_large = file_size_mb >= max_file_size
         exception = (
             True
             if not isinstance(file_path, CloudPath) and ".csv" in file_path.suffixes
             else False
         )
         if too_large is True and exception is not True:
```

### Comparing `browsr-1.0.0/docs/contributing.md` & `browsr-1.0.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/docs/index.md` & `browsr-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/requirements/requirements-dev.txt` & `browsr-1.0.1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/requirements/requirements-prod.txt` & `browsr-1.0.1/requirements/requirements-prod.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/.gitignore` & `browsr-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/LICENSE.txt` & `browsr-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/README.md` & `browsr-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/pyproject.toml` & `browsr-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsr-1.0.0/PKG-INFO` & `browsr-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.0.0
+Version: 1.0.1
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.0.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.0.1 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

