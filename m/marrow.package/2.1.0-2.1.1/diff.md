# Comparing `tmp/marrow.package-2.1.0.tar.gz` & `tmp/marrow.package-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marrow.package-2.1.0.tar", last modified: Tue Nov 29 19:04:34 2022, max compression
+gzip compressed data, was "marrow.package-2.1.1.tar", last modified: Wed May  3 16:37:41 2023, max compression
```

## Comparing `marrow.package-2.1.0.tar` & `marrow.package-2.1.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.955361 marrow.package-2.1.0/
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.944333 marrow.package-2.1.0/.github/
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.947553 marrow.package-2.1.0/.github/workflows/
--rw-r--r--   0 amcgregor   (502) staff       (20)      935 2022-11-29 18:55:09.000000 marrow.package-2.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 amcgregor   (502) staff       (20)      374 2022-06-16 15:02:25.000000 marrow.package-2.1.0/.gitignore
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.944790 marrow.package-2.1.0/.packaging/
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.947807 marrow.package-2.1.0/.packaging/dist/
--rw-r--r--   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:30.000000 marrow.package-2.1.0/.packaging/dist/.keep
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.948013 marrow.package-2.1.0/.packaging/release/
--rw-r--r--   0 amcgregor   (502) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.0/.packaging/release/.keep
--rw-r--r--   0 amcgregor   (502) staff       (20)      982 2022-06-16 15:02:25.000000 marrow.package-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 amcgregor   (502) staff       (20)     1095 2022-11-29 18:55:09.000000 marrow.package-2.1.0/LICENSE.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)       61 2022-06-16 15:02:25.000000 marrow.package-2.1.0/MANIFEST.in
--rw-r--r--   0 amcgregor   (502) staff       (20)     1887 2022-11-29 18:55:09.000000 marrow.package-2.1.0/Makefile
--rw-r--r--   0 amcgregor   (502) staff       (20)     1385 2022-11-29 19:04:34.955593 marrow.package-2.1.0/PKG-INFO
--rw-r--r--   0 amcgregor   (502) staff       (20)    13322 2022-11-29 19:01:44.000000 marrow.package-2.1.0/README.rst
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.945159 marrow.package-2.1.0/marrow/
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.952497 marrow.package-2.1.0/marrow/package/
--rw-r--r--   0 amcgregor   (502) staff       (20)      107 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/__init__.py
--rw-r--r--   0 amcgregor   (502) staff       (20)      766 2022-10-27 20:20:00.000000 marrow.package-2.1.0/marrow/package/cache.py
--rw-r--r--   0 amcgregor   (502) staff       (20)      449 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/canonical.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     3024 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/disport.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     5770 2022-11-29 18:55:09.000000 marrow.package-2.1.0/marrow/package/host.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     2296 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/lazy.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     4064 2022-11-29 18:55:09.000000 marrow.package-2.1.0/marrow/package/loader.py
--rw-r--r--   0 amcgregor   (502) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/py.typed
--rw-r--r--   0 amcgregor   (502) staff       (20)      812 2022-11-29 18:55:55.000000 marrow.package-2.1.0/marrow/package/release.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     2565 2022-06-16 15:02:25.000000 marrow.package-2.1.0/marrow/package/tarjan.py
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.949810 marrow.package-2.1.0/marrow.package.egg-info/
--rw-r--r--   0 amcgregor   (502) staff       (20)     1385 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/PKG-INFO
--rw-r--r--   0 amcgregor   (502) staff       (20)      880 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/SOURCES.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)        1 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/dependency_links.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)      113 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/entry_points.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)        1 2022-10-27 18:35:56.000000 marrow.package-2.1.0/marrow.package.egg-info/not-zip-safe
--rw-r--r--   0 amcgregor   (502) staff       (20)      148 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/requires.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)        7 2022-11-29 19:04:34.000000 marrow.package-2.1.0/marrow.package.egg-info/top_level.txt
--rw-r--r--   0 amcgregor   (502) staff       (20)     2985 2022-11-29 19:04:34.956734 marrow.package-2.1.0/setup.cfg
--rwxr-xr-x   0 amcgregor   (502) staff       (20)      152 2022-06-16 15:02:25.000000 marrow.package-2.1.0/setup.py
-drwxr-xr-x   0 amcgregor   (502) staff       (20)        0 2022-11-29 19:04:34.955084 marrow.package-2.1.0/test/
--rw-r--r--   0 amcgregor   (502) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/__init__.py
--rw-r--r--   0 amcgregor   (502) staff       (20)      168 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/conftest.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     3281 2022-11-29 18:55:09.000000 marrow.package-2.1.0/test/helper.py
--rw-r--r--   0 amcgregor   (502) staff       (20)      745 2022-11-29 18:55:09.000000 marrow.package-2.1.0/test/test_cache.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     2933 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/test_canonical.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     2650 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/test_host.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     1219 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/test_lazy.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     2126 2022-11-29 18:55:09.000000 marrow.package-2.1.0/test/test_loader.py
--rw-r--r--   0 amcgregor   (502) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/test_registry.py
--rw-r--r--   0 amcgregor   (502) staff       (20)     1755 2022-06-16 15:02:25.000000 marrow.package-2.1.0/test/test_tarjan.py
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.243944 marrow.package-2.1.1/
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.234670 marrow.package-2.1.1/.github/
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.237664 marrow.package-2.1.1/.github/workflows/
+-rw-r--r--   0 amcgregor   (501) staff       (20)      935 2023-05-03 15:27:31.000000 marrow.package-2.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0 amcgregor   (501) staff       (20)      374 2022-06-16 15:02:25.000000 marrow.package-2.1.1/.gitignore
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.234994 marrow.package-2.1.1/.packaging/
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.237952 marrow.package-2.1.1/.packaging/dist/
+-rw-r--r--   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:29:32.000000 marrow.package-2.1.1/.packaging/dist/.keep
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.238098 marrow.package-2.1.1/.packaging/release/
+-rw-r--r--   0 amcgregor   (501) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.1/.packaging/release/.keep
+-rw-r--r--   0 amcgregor   (501) staff       (20)      982 2022-06-16 15:02:25.000000 marrow.package-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1095 2023-05-03 15:27:31.000000 marrow.package-2.1.1/LICENSE.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)       61 2022-06-16 15:02:25.000000 marrow.package-2.1.1/MANIFEST.in
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1930 2023-05-03 16:34:20.000000 marrow.package-2.1.1/Makefile
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1385 2023-05-03 16:37:41.244065 marrow.package-2.1.1/PKG-INFO
+-rw-r--r--   0 amcgregor   (501) staff       (20)    14181 2023-05-03 15:39:30.000000 marrow.package-2.1.1/README.rst
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.235299 marrow.package-2.1.1/marrow/
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.241490 marrow.package-2.1.1/marrow/package/
+-rw-r--r--   0 amcgregor   (501) staff       (20)      107 2022-06-16 15:02:25.000000 marrow.package-2.1.1/marrow/package/__init__.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)      739 2023-05-03 15:47:11.000000 marrow.package-2.1.1/marrow/package/cache.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1080 2023-05-03 15:27:31.000000 marrow.package-2.1.1/marrow/package/canonical.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     2952 2023-05-03 15:47:11.000000 marrow.package-2.1.1/marrow/package/disport.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     5701 2023-05-03 15:51:29.000000 marrow.package-2.1.1/marrow/package/host.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     2246 2023-05-03 15:47:11.000000 marrow.package-2.1.1/marrow/package/lazy.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     4018 2023-05-03 15:52:11.000000 marrow.package-2.1.1/marrow/package/loader.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.1/marrow/package/py.typed
+-rw-r--r--   0 amcgregor   (501) staff       (20)      812 2023-05-03 15:27:31.000000 marrow.package-2.1.1/marrow/package/release.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     2485 2023-05-03 16:11:02.000000 marrow.package-2.1.1/marrow/package/tarjan.py
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.239640 marrow.package-2.1.1/marrow.package.egg-info/
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1385 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/PKG-INFO
+-rw-r--r--   0 amcgregor   (501) staff       (20)      895 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/SOURCES.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)        1 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/dependency_links.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)      137 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/entry_points.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)        1 2023-05-03 15:50:35.000000 marrow.package-2.1.1/marrow.package.egg-info/not-zip-safe
+-rw-r--r--   0 amcgregor   (501) staff       (20)      160 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/requires.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)        7 2023-05-03 16:37:41.000000 marrow.package-2.1.1/marrow.package.egg-info/top_level.txt
+-rw-r--r--   0 amcgregor   (501) staff       (20)       88 2023-05-03 16:25:17.000000 marrow.package-2.1.1/pyproject.toml
+-rw-r--r--   0 amcgregor   (501) staff       (20)     3022 2023-05-03 16:37:41.244754 marrow.package-2.1.1/setup.cfg
+-rwxr-xr-x   0 amcgregor   (501) staff       (20)      152 2022-06-16 15:02:25.000000 marrow.package-2.1.1/setup.py
+drwxr-xr-x   0 amcgregor   (501) staff       (20)        0 2023-05-03 16:37:41.243723 marrow.package-2.1.1/test/
+-rw-r--r--   0 amcgregor   (501) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/__init__.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)      168 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/conftest.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     3281 2023-05-03 15:27:31.000000 marrow.package-2.1.1/test/helper.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)      745 2023-05-03 15:27:31.000000 marrow.package-2.1.1/test/test_cache.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     3278 2023-05-03 15:27:31.000000 marrow.package-2.1.1/test/test_canonical.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     2650 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/test_host.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1219 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/test_lazy.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     2126 2023-05-03 15:27:31.000000 marrow.package-2.1.1/test/test_loader.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)        0 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/test_registry.py
+-rw-r--r--   0 amcgregor   (501) staff       (20)     1755 2022-06-16 15:02:25.000000 marrow.package-2.1.1/test/test_tarjan.py
```

### Comparing `marrow.package-2.1.0/.github/workflows/pytest.yml` & `marrow.package-2.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/.pre-commit-config.yaml` & `marrow.package-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/LICENSE.txt` & `marrow.package-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/Makefile` & `marrow.package-2.1.1/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,34 @@
 	@echo "Usage: make <command>\n\033[36m\033[0m"
 	@awk 'BEGIN {FS = ":.*##"} /^[a-zA-Z_-]+:.*?##/ { printf "\033[36m%-18s\033[0m %s\n", $$1, $$2 } /^##@/ { printf "\n\033[1m%s\033[0m\n", substr($$0, 5) } ' $(MAKEFILE_LIST) | sort
 
 clean:  ## Remove executable caches and ephemeral collections.
 	find . -name __pycache__ -exec rm -rfv {} +
 	find . -iname \*.pyc -exec rm -fv {} +
 	find . -iname \*.pyo -exec rm -fv {} +
-	rm -rvf build htmlcov
+	rm -rvf .packaging/* htmlcov dist
 
 veryclean: clean  ## Remove all project metadata, executable caches, and sensitive collections.
-	rm -rvf *.egg-info .packaging/{build,dist,release}/*
+	rm -rvf *.egg-info
 
 lint:  ## Execute pylint across the project.
 	pylint --rcfile=setup.cfg marrow
 
 test: develop
 	pytest
 
 testloop:  ## Automatically execute the test suite limited to one failure.
 	find marrow test -name \*.py | entr -c pytest --ff --maxfail=1 -q
 
-release:  ## Package up and utilize Twine to issue a release.
-	./setup.py sdist bdist_wheel ${RELEASE_OPTIONS}
-	python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+release: test  ## Package up and utilize Twine to issue a release.
+	rm -vf dist/*
+	pip3 install -U build twine
+	python3 -m build
+	#python3 -m twine upload --repository-url https://test.pypi.org/legacy/ .packaging/release/*
+	python3 -m twine upload dist/*
 
 ${PROJECT}.egg-info/PKG-INFO: setup.py setup.cfg
 	@mkdir -p ${VIRTUAL_ENV}/lib/pip-cache
 	
 	@# General
 	@[ ! -e /private ] && pip install --cache-dir "${VIRTUAL_ENV}/lib/pip-cache" -e ".[${USE}]" || true
```

### Comparing `marrow.package-2.1.0/PKG-INFO` & `marrow.package-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marrow.package
-Version: 2.1.0
+Version: 2.1.1
 Summary: Plugin discovery and management, dependency graphing, and object import path canonicalization.
 Home-page: https://github.com/marrow/package
 Author: Alice Bevan-McGregor
 Author-email: alice@gothcandy.com
 License: MIT
 Project-URL: Source code, https://github.com/marrow/package
 Project-URL: Issue tracker, https://github.com/marrow/package/issues
```

### Comparing `marrow.package-2.1.0/README.rst` & `marrow.package-2.1.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==============
 Marrow Package
 ==============
 
-    © 2014-2022 Alice Bevan-McGregor and contributors.
+    © 2014-2023 Alice Bevan-McGregor and contributors.
 
 ..
 
     https://github.com/marrow/package
 
 ..
 
@@ -93,14 +93,28 @@
 	* instance classmethod
 	* instance method
 	* instance staticmethod
 * nested classes and methods
 * closures
 
 
+3.1. Resolving Plugin References
+================================
+
+The ``load`` utility can optionally be provided a plugin namespace to search. If the target object is found within the
+namespace, the name of the plugin entry will be returned. By default, if a named plugin can **not** be found, a
+``LookupError`` will be raised. If a direct reference is acceptable, the boolean ``direct`` argument (third positional)
+can be made truthy to permit direct references.
+
+    from marrow.package.canonical import name
+
+    assert name(name, 'marrow.package.sample') == 'name'
+
+
+
 4. Resolving Object References
 ==============================
 
 Two utilities are provided which allow you resolve string path references to objects.  The first is quite simple::
 
     from marrow.package.loader import traverse
     
@@ -137,14 +151,15 @@
     
     # Load the "pip" command-line interface.
     assert load('pip', 'console_scripts') is main
 
 Providing a namespace does not prevent explicit object lookup (dot-colon notation) from working.
 
 
+
 4.2. Caching Import References
 ------------------------------
 
 An attribute-access dictionary is provided that acts as an import cache::
 
     from marrow.package.cache import PackageCache
     from pip import main
@@ -260,24 +275,31 @@
 * **Implement package-relative path lookup.** The `load` utility function can now resolve the path to a file relative
   to a package. This is particularly useful for looking up the path to template files or on-disk static assets.
 * **Protected attribute access now fails.** Underscore-prefixed attributes are assumed to be "protected", with the
   technical note that Python adds new internal "double underscore" attributes which must not spontaneously exist, or
   generate errors other than `AttributeError`.
 * **Tests are now independent of third-party plugin registration.**
 
+Version 2.1.1
+-------------
+
+* **Update type hinting validation.** The ``typeguard`` package has removed a functional utility; decoration now used.
+* **Canonical plugin name resolution.** The ``name()`` utility can now resolve the plugin name if given a plugin
+  namespace to check.
+
 
 7. License
 ==========
 
 Marrow Package has been released under the MIT Open Source license.
 
 7.1. The MIT License
 --------------------
 
-Copyright © 2014-2022 Alice Bevan-McGregor and contributors.
+Copyright © 2014-2023 Alice Bevan-McGregor and contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
 persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
```

### Comparing `marrow.package-2.1.0/marrow/package/cache.py` & `marrow.package-2.1.1/marrow/package/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from collections import defaultdict
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from .loader import load
 
 
 class PluginCache(defaultdict):
 	"""Lazily load plugins from the given namespace.
 	
 	Supports read-only dictionary-like and attribute access.
 	"""
 	
+	@typechecked
 	def __init__(self,  namespace: str):
 		"""You must specify an entry point namespace."""
 		
-		assert check_argument_types()
-		
 		super().__init__()
+		
 		self.namespace =  namespace
 	
 	def __missing__(self,  key):
 		"""If not already loaded, attempt to load the reference."""
 		
 		self[key] = load(key, self.namespace)
 		return self[key]
```

### Comparing `marrow.package-2.1.0/marrow/package/disport.py` & `marrow.package-2.1.1/marrow/package/disport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Import redirector registry utility.
 
 Disport; noun: diversion from work or serious matters; recreation or amusement.
 """
 
 from collections import deque
-from typeguard import check_argument_types
+from typeguard import typechecked
 from typing import Deque, Sequence, Iterable, Optional
 
 from .loader import load, nodefault
 
 
 class Importer:
 	"""A helper class to redirect imports and plugin loading.
@@ -29,46 +29,43 @@
 	
 	redirects: Deque[str]
 	namespace: str
 	separators: Iterable[str]
 	executable: bool
 	protect: bool
 	
+	@typechecked
 	def __init__(self, redirect:Optional[Iterable[str]]=None, namespace:str=None,
 				separators:Iterable[str]=('.', ':'), executable:bool=False, protect:bool=True):
 		"""Configure the disport Importer.
 		
 		The arguments are essentially the same as those for the load or lazyload utilities, with the addition of the
 		ability to specify an initial iterable of overrides through the `redirect` argument. This should be an
 		iterable of tuples (or tuple-alikes) in the form `(source, destination)`.
 		"""
 		
-		assert check_argument_types()
-		
 		super().__init__()
 		
 		self.redirects = deque()
 		self.namespace = namespace
 		self.separators = separators
 		self.executable = executable
 		self.protect = protect
 		
 		# Initial redirects processing.
 		if redirect:
 			for source, destination in redirect:
 				self.redirect(source, destination)
 	
+	@typechecked
 	def redirect(self, source:str, destination:str):
-		assert check_argument_types()
-		
 		self.redirects.appendleft((source, destination))
 	
+	@typechecked
 	def __call__(self, target:str, default=nodefault):
-		assert check_argument_types()
-		
 		for candidate, destination in self.redirects:
 			if candidate == target:  # Plugin reference.
 				pass
 				return
 			
 			if not target.startswith(candidate):
 				continue
```

### Comparing `marrow.package-2.1.0/marrow/package/host.py` & `marrow.package-2.1.1/marrow/package/host.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pkg_resources
 
-from typeguard import check_argument_types
+from typeguard import typechecked
 from typing import Any, Dict, Iterable, List, Set, cast
 from pkg_resources import Distribution
 from logging import getLogger as _logger
 
 from .canonical import name as _name
 from .cache import PluginCache
 from .loader import traverse
@@ -21,17 +21,16 @@
 	namespace:str
 	folders:Iterable[str]
 	plugins:List[Plugin]
 	named:PluginCache
 	
 	__wrapped__ = None  # Python decorator protocol bypass.
 	
+	@typechecked
 	def __init__(self, namespace:str, folders:Iterable[str]=None):
-		assert check_argument_types()
-		
 		self.namespace = namespace
 		self.folders = folders if folders else []
 		self.plugins = []
 		self.named = PluginCache(namespace)
 		
 		self.ws = ws = pkg_resources.working_set
 		
@@ -42,24 +41,23 @@
 			env = pkg_resources.Environment([path])
 			ws.require(*env)
 		
 		ws.subscribe(self._register)
 		
 		super(PluginManager, self).__init__()
 	
+	@typechecked
 	def register(self, name:str, plugin:object) -> None:
-		assert check_argument_types()
-		
 		log.info("Registering plugin" + name + " in namespace " + self.namespace + ".",
 				extra = dict(plugin_name=name, namespace=self.namespace, plugin=_name(plugin)))
 		self.named[name] = plugin
 		self.plugins.append(plugin)
 	
+	@typechecked
 	def _register(self, dist:Distribution) -> None:
-		assert check_argument_types()
 		entries = dist.get_entry_map(self.namespace)
 		
 		if not entries:
 			return
 		
 		try:
 			for name in entries:
```

### Comparing `marrow.package-2.1.0/marrow/package/lazy.py` & `marrow.package-2.1.1/marrow/package/lazy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from threading import RLock
 from collections.abc import MutableMapping
-from typeguard import check_argument_types
+from typeguard import typechecked
 from typing import Any, Callable
 
 from .loader import traverse, load
 
 
 sentinel = object()
 
@@ -25,17 +25,16 @@
 				return 42
 		
 		obj = MyClass()
 		assert obj.myattr == 42 # Executed!
 		assert obj.myattr == 42 # Not.
 	"""
 	
+	@typechecked
 	def __init__(self, func:Callable[[Any], None], name:str=None, doc:str=None):
-		assert check_argument_types()
-		
 		self.__name__ = name or func.__name__
 		self.__module__ = func.__module__
 		self.__doc__ = func.__doc__
 		self.lock = RLock()
 		self.func = func
 	
 	def __repr__(self):
@@ -50,14 +49,15 @@
 			
 			if value is sentinel:
 				value = instance.__dict__[self.__name__] = self.func(instance)
 		
 		return value
 
 
+@typechecked
 def lazyload(reference: str, *args, **kw):
 	"""Lazily load and cache an object reference upon dereferencing.
 	
 	Assign the result of calling this function with either an object reference passed in positionally:
 	
 		class MyClass:
 			debug = lazyload('logging:debug')
@@ -67,16 +67,14 @@
 		class AnotherClass:
 			target = 'logging:info'
 			log = lazyload('.target')
 	
 	Additional arguments are passed to the eventual call to `load()`.
 	"""
 	
-	assert check_argument_types()
-	
 	def lazily_load_reference(self):
 		ref = reference
 		
 		if ref.startswith('.'):
 			ref = traverse(self, ref[1:])
 		
 		return load(ref, *args, **kw)
```

### Comparing `marrow.package-2.1.0/marrow/package/loader.py` & `marrow.package-2.1.1/marrow/package/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 from pkg_resources import iter_entry_points, resource_filename
 from typing import Sequence, Optional
 
-from typeguard import check_argument_types
-
+from typeguard import typechecked
 
 nodefault = object()
 
 
+@typechecked
 def traverse(obj, target:str, default=nodefault, executable:bool=False, separator:str='.', protect:bool=True):
 	"""Traverse down an object, using getattr or getitem.
 	
 	If ``executable`` is ``True`` any executable function encountered will be, with no arguments. Traversal will
 	continue on the result of that call.  You can change the separator as desired, i.e. to a '/'.
 	
 	By default attributes (but not array elements) prefixed with an underscore are taboo.  They will not resolve,
@@ -20,15 +20,14 @@
 	
 	Certain allowances are made: if a 'path segment' is numerical, it's treated as an array index. If attribute
 	lookup fails, it will re-try on that object using array notation and continue from there.  This makes lookup
 	very flexible.
 	"""
 	
 	# TODO: Support numerical slicing, i.e. ``1:4``, or even just ``:-1`` and things.
-	assert check_argument_types()
 	
 	value = obj
 	remainder = target
 	
 	if not target:
 		return obj
 	
@@ -54,14 +53,15 @@
 					raise LookupError("Could not resolve '" + target + "' on: " + repr(obj))
 				
 				return default
 		
 	return value
 
 
+@typechecked
 def load(target:str, namespace:str=None, default=nodefault, executable:bool=False, separators:Sequence[str]=('.', ':', '/'),
 		protect:bool=True):
 	"""This helper function loads an object identified by a dotted-notation string.
 	
 	For example::
 	
 		# Load class Foo from example.objects.
@@ -82,15 +82,14 @@
 	will retrieve a named attribute, forward-slash notation will retrieve the path to a file relative to the dot-
 	notation package:
 	
 		# Where is master.html relative to example.template?
 		load('example.template/master.html')
 	"""
 	
-	assert check_argument_types()
 	path:Optional[str] = None
 	
 	if separators[1] in target and separators[2] in target:
 		raise LookupError("Can not target an attribute from a file on-disk.")
 	
 	if namespace and separators[1] not in target:
 		allowable = dict((i.name,  i) for i in iter_entry_points(namespace))
```

### Comparing `marrow.package-2.1.0/marrow/package/release.py` & `marrow.package-2.1.1/marrow/package/release.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/marrow/package/tarjan.py` & `marrow.package-2.1.1/marrow/package/tarjan.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 
 by Paul Harrison
 
 Public domain, do with it as you will.
 
 From a blog post by Paul Harrison: http://www.logarithmic.net/pfh/blog/01208083168
 
-Somee cleanup was applied, and Python 3 function annotations (typing module, typeguard validation) supplied.
+Some cleanup was applied, and Python 3 function annotations (typing module, typeguard validation) supplied.
 """
 
 from collections import defaultdict
-from typeguard import check_argument_types
+from typeguard import typechecked
 from typing import List, Mapping, MutableMapping, Sequence, Tuple, Iterable
 
 Graph = Mapping[str, Iterable[str]]
 
 
-def strongly_connected_components(graph: Graph) -> List[Tuple[str, ...]]:
+@typechecked
+def strongly_connected_components(graph: Graph) -> List[Tuple]:
 	"""Find the strongly connected components in a graph using Tarjan's algorithm.
 	
 	The `graph` argument should be a dictionary mapping node names to sequences of successor nodes.
 	"""
 	
-	assert check_argument_types()
-	
 	result: List[Tuple[str, ...]] = []
 	stack: List[str] = []
 	low: MutableMapping[str, int] = {}
 	
 	def visit(node: str):
 		if node in low: return
 		
@@ -51,17 +50,16 @@
 	
 	for node in graph:
 		visit(node)
 	
 	return result
 
 
+@typechecked
 def topological_sort(graph:Graph) -> list:
-	assert check_argument_types()
-	
 	count: MutableMapping[str, int] = defaultdict(lambda: 0)
 	
 	for node in graph:
 		for successor in graph[node]:
 			count[successor] += 1
 	
 	result = []
@@ -75,19 +73,18 @@
 			count[successor] -= 1
 			if count[successor] == 0:
 				ready.append(successor)
 	
 	return result
 
 
+@typechecked
 def robust_topological_sort(graph: Graph) -> list:
 	"""Identify strongly connected components then perform a topological sort of those components."""
 	
-	assert check_argument_types()
-	
 	components = strongly_connected_components(graph)
 	
 	node_component = {}
 	component_graph: Graph = {}
 	
 	for component in components:
 		for node in component:
```

### Comparing `marrow.package-2.1.0/marrow.package.egg-info/PKG-INFO` & `marrow.package-2.1.1/marrow.package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marrow.package
-Version: 2.1.0
+Version: 2.1.1
 Summary: Plugin discovery and management, dependency graphing, and object import path canonicalization.
 Home-page: https://github.com/marrow/package
 Author: Alice Bevan-McGregor
 Author-email: alice@gothcandy.com
 License: MIT
 Project-URL: Source code, https://github.com/marrow/package
 Project-URL: Issue tracker, https://github.com/marrow/package/issues
```

### Comparing `marrow.package-2.1.0/marrow.package.egg-info/SOURCES.txt` & `marrow.package-2.1.1/marrow.package.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/pytest.yml
 .packaging/dist/.keep
 .packaging/release/.keep
 marrow.package.egg-info/PKG-INFO
 marrow.package.egg-info/SOURCES.txt
```

### Comparing `marrow.package-2.1.0/setup.cfg` & `marrow.package-2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 packages = marrow.package
 include_package_data = True
 python_requires = >=3.8
 zip_safe = False
 setup_requires = 
 	setuptools-scm >= 1.7.0
 install_requires = 
-	typeguard
+	typeguard ~=2.3.0,<3.0
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flakes
 	pytest-isort
 	pytest-mypy
 
@@ -71,17 +71,17 @@
 
 [options.package_data]
 * = *.txt, *.md, *.rst
 marrow/package = py.typed
 
 [options.entry_points]
 marrow.package.sample = 
-	name = marrow.package:name
-	load = marrow.package:load
-	traverse = marrow.package:traverse
+	name = marrow.package.canonical:name
+	load = marrow.package.loader:load
+	traverse = marrow.package.loader:traverse
 
 [check]
 metadata = 1
 strict = 1
 
 [clean]
 build-base = .packaging/build
```

### Comparing `marrow.package-2.1.0/test/helper.py` & `marrow.package-2.1.1/test/helper.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/test/test_cache.py` & `marrow.package-2.1.1/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/test/test_canonical.py` & `marrow.package-2.1.1/test/test_canonical.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,7 +70,18 @@
 		assert name(helper.decorated_deep) == 'test.helper:decorated_deep'
 	
 	def test__resolve__of_a_module_level_decorated_method(self):
 		assert name(helper.Example.decorated_shallow) == 'test.helper:Example.decorated_shallow'
 		
 	def test__resolve__of_a_module_level_decorated_decorated_method(self):
 		assert name(helper.Example.decorated_deep) == 'test.helper:Example.decorated_deep'
+	
+	def test__resolve__plugin_name(self):
+		assert name(name, 'marrow.package.sample') == 'name'
+	
+	def test__resolve__plugin_missing(self):
+		with pytest.raises(LookupError):
+			name(TestCase, 'marrow.package.sample')
+	
+	def test__resolve__plugin_direct(self):
+		assert name(TestCase, 'marrow.package.sample', True) == 'unittest.case:TestCase'
+
```

### Comparing `marrow.package-2.1.0/test/test_host.py` & `marrow.package-2.1.1/test/test_host.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/test/test_lazy.py` & `marrow.package-2.1.1/test/test_lazy.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/test/test_loader.py` & `marrow.package-2.1.1/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `marrow.package-2.1.0/test/test_tarjan.py` & `marrow.package-2.1.1/test/test_tarjan.py`

 * *Files identical despite different names*

