# Comparing `tmp/module-utilities-0.1.0.tar.gz` & `tmp/module-utilities-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.1.0.tar", last modified: Tue May  2 03:10:13 2023, max compression
+gzip compressed data, was "module-utilities-0.2.0.tar", last modified: Wed May  3 02:37:04 2023, max compression
```

## Comparing `module-utilities-0.1.0.tar` & `module-utilities-0.2.0.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.105541 module-utilities-0.1.0/
--rw-r--r--   0 wpk      (42033)    36681     1361 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.011827 module-utilities-0.1.0/.github/
--rw-r--r--   0 wpk      (42033)    36681      368 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1307 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3581 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-27 23:45:36.000000 module-utilities-0.1.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      271 2023-05-02 03:09:02.000000 module-utilities-0.1.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9273 2023-05-02 03:09:02.000000 module-utilities-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-27 23:45:36.000000 module-utilities-0.1.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-04-27 23:45:36.000000 module-utilities-0.1.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11231 2023-05-02 03:09:02.000000 module-utilities-0.1.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     5914 2023-05-02 03:10:13.106029 module-utilities-0.1.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2916 2023-04-27 23:45:36.000000 module-utilities-0.1.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.012488 module-utilities-0.1.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.013278 module-utilities-0.1.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.014974 module-utilities-0.1.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033)    36681      204 2023-04-27 23:45:36.000000 module-utilities-0.1.0/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.022045 module-utilities-0.1.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1406 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:12.996629 module-utilities-0.1.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.022550 module-utilities-0.1.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.024544 module-utilities-0.1.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.034680 module-utilities-0.1.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.041479 module-utilities-0.1.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.044400 module-utilities-0.1.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14799 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.048983 module-utilities-0.1.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      887 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/create-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.050652 module-utilities-0.1.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1787 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      943 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.053297 module-utilities-0.1.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      144 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.067973 module-utilities-0.1.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      232 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      349 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       64 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      136 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      116 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.069105 module-utilities-0.1.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-04-27 23:45:36.000000 module-utilities-0.1.0/examples/README.md
--rw-r--r--   0 wpk      (42033)    36681     6200 2023-05-02 03:09:02.000000 module-utilities-0.1.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.074828 module-utilities-0.1.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      403 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-27 23:45:36.000000 module-utilities-0.1.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-04-27 23:45:36.000000 module-utilities-0.1.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681      300 2023-05-02 03:10:13.108394 module-utilities-0.1.0/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-27 23:45:36.000000 module-utilities-0.1.0/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:12.999548 module-utilities-0.1.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.088628 module-utilities-0.1.0/src/module_utilities/
--rw-r--r--   0 wpk      (42033)    36681      683 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2646 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033)    36681    23552 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_docscrape.py
--rw-r--r--   0 wpk      (42033)    36681      382 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033)    36681     5824 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033)    36681     9856 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033)    36681    18093 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.099900 module-utilities-0.1.0/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     5914 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2572 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 12:55:39.000000 module-utilities-0.1.0/src/module_utilities.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033)    36681       48 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       17 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.104771 module-utilities-0.1.0/tests/
--rw-r--r--   0 wpk      (42033)    36681       46 2023-04-27 23:45:36.000000 module-utilities-0.1.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.1.0/tests/conftest.py
--rw-r--r--   0 wpk      (42033)    36681    10864 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_cached.py
--rw-r--r--   0 wpk      (42033)    36681     6176 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033)    36681      169 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_module_utilities.py
--rw-r--r--   0 wpk      (42033)    36681     3950 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.917237 module-utilities-0.2.0/
+-rw-r--r--   0 wpk      (42033)    36681     1358 2023-05-03 02:36:13.000000 module-utilities-0.2.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.846022 module-utilities-0.2.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      368 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1307 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3581 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-27 23:45:36.000000 module-utilities-0.2.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      388 2023-05-03 02:36:13.000000 module-utilities-0.2.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9267 2023-05-03 02:36:13.000000 module-utilities-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-27 23:45:36.000000 module-utilities-0.2.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-27 23:45:36.000000 module-utilities-0.2.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11367 2023-05-03 02:36:13.000000 module-utilities-0.2.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     5953 2023-05-03 02:37:04.917642 module-utilities-0.2.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2844 2023-05-03 02:36:13.000000 module-utilities-0.2.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.846597 module-utilities-0.2.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.847078 module-utilities-0.2.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.847948 module-utilities-0.2.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033)    36681      204 2023-04-27 23:45:36.000000 module-utilities-0.2.0/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.856969 module-utilities-0.2.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.832060 module-utilities-0.2.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.857729 module-utilities-0.2.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.859312 module-utilities-0.2.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.864844 module-utilities-0.2.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.869159 module-utilities-0.2.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.871899 module-utilities-0.2.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14793 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.874793 module-utilities-0.2.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681     1675 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/example-usage-1.rst
+-rw-r--r--   0 wpk      (42033)    36681     1667 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033)    36681       89 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.876991 module-utilities-0.2.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    15671 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      241 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      937 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.877987 module-utilities-0.2.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      192 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.887416 module-utilities-0.2.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      232 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      574 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      349 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      136 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      116 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.888226 module-utilities-0.2.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-27 23:45:36.000000 module-utilities-0.2.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.889973 module-utilities-0.2.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.2.0/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    15671 2023-05-03 02:36:13.000000 module-utilities-0.2.0/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     6202 2023-05-03 02:36:13.000000 module-utilities-0.2.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.895228 module-utilities-0.2.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      403 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-27 23:45:36.000000 module-utilities-0.2.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-04-27 23:45:36.000000 module-utilities-0.2.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681      297 2023-05-03 02:37:04.919251 module-utilities-0.2.0/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-27 23:45:36.000000 module-utilities-0.2.0/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.835442 module-utilities-0.2.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.902294 module-utilities-0.2.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033)    36681      683 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     2646 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033)    36681    23552 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_docscrape.py
+-rw-r--r--   0 wpk      (42033)    36681      382 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681     5927 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033)    36681     9989 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033)    36681    19277 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.910342 module-utilities-0.2.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     5953 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2670 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 12:55:39.000000 module-utilities-0.2.0/src/module_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033)    36681       48 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       17 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.916456 module-utilities-0.2.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       46 2023-04-27 23:45:36.000000 module-utilities-0.2.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.2.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033)    36681    10864 2023-05-02 03:09:02.000000 module-utilities-0.2.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033)    36681     7467 2023-05-03 02:36:13.000000 module-utilities-0.2.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-05-02 03:09:02.000000 module-utilities-0.2.0/tests/test_module_utilities.py
+-rw-r--r--   0 wpk      (42033)    36681     4013 2023-05-03 02:36:13.000000 module-utilities-0.2.0/tox.ini
```

### Comparing `module-utilities-0.1.0/.cruft.json` & `module-utilities-0.2.0/.cruft.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8986842105263158%*

 * *Differences: {"'commit'": "'cb20a32f67dadb4142be54898a87de1efdce6bd6'",*

 * * "'context'": "{'cookiecutter': {'github_username': 'usnistgov'}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/markdown",
-    "commit": "38e14cd6d21fdc444081dcb1e34c15d0ebdc3683",
+    "commit": "cb20a32f67dadb4142be54898a87de1efdce6bd6",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
@@ -15,15 +15,15 @@
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
-            "github_username": "wpk-nist-gov",
+            "github_username": "usnistgov",
             "open_source_license": "NIST license",
             "project_name": "module-utilities",
             "project_short_description": "Collection of utilities to aid working with python modules.",
             "project_slug": "module_utilities",
             "pypi_username": "wpk-nist",
             "sphinx_auto": "automodule",
             "sphinx_theme": "sphinx_book_theme",
```

### Comparing `module-utilities-0.1.0/.editorconfig` & `module-utilities-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/.gitignore` & `module-utilities-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/.pre-commit-config.yaml` & `module-utilities-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/CONTRIBUTING.md` & `module-utilities-0.2.0/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 You can contribute in many ways:
 
 ## Types of Contributions
 
 ### Report Bugs
 
-Report bugs at <https://github.com/wpk-nist-gov/module-utilities/issues>.
+Report bugs at <https://github.com/usnistgov/module-utilities/issues>.
 
 If you are reporting a bug, please include:
 
 - Your operating system name and version.
 - Any details about your local setup that might be helpful in troubleshooting.
 - Detailed steps to reproduce the bug.
 
@@ -32,15 +32,15 @@
 `module-utilities` could always use more documentation, whether as part of the
 official `module-utilities` docs, in docstrings, or even on the web in blog
 posts, articles, and such.
 
 ### Submit Feedback
 
 The best way to send feedback is to file an issue at
-<https://github.com/wpk-nist-gov/module-utilities/issues>.
+<https://github.com/usnistgov/module-utilities/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
   welcome :)
```

### Comparing `module-utilities-0.1.0/LICENSE` & `module-utilities-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/Makefile` & `module-utilities-0.2.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
 .PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
 	$(TOX) -e $@-py$(py) -- $(posargs)
 testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
 testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
```

### Comparing `module-utilities-0.1.0/PKG-INFO` & `module-utilities-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.1.0
+Version: 0.2.0
 Summary: Collection of utilities to aid working with python modules.
-Home-page: https://github.com/wpk-nist-gov/module-utilities
+Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
-Project-URL: homepage, https://github.com/wpk-nist-gov/module-utilities
+Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -43,20 +43,19 @@
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/module-utilities
 [pypi-link]: https://pypi.org/project/module-utilities
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/module-utilities/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
-[repo-link]: https://github.com/wpk-nist-gov/module-utilities
+[repo-link]: https://github.com/usnistgov/module-utilities
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/module-utilities
 [conda-link]: https://anaconda.org/wpk-nist/module-utilities
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]:
-  https://github.com/wpk-nist-gov/module-utilities/blob/main/LICENSE
+[license-link]: https://github.com/usnistgov/module-utilities/blob/main/LICENSE
 
 <!-- other links -->
 
 [cachetools]: https://github.com/tkem/cachetools/
 
 # `module-utilities`
 
@@ -92,21 +91,14 @@
 
 or
 
 ```bash
 conda install -c wpk-nist module-utilities
 ```
 
-## Example usage
-
-```python
-import module_utilities
-
-```
-
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
 -->
@@ -123,29 +115,37 @@
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
-[wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
+[usnistgov/cookiecutter-pypackage](https://github.com/usnistgov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `module-utilities`
 
 ## Unreleased
 
 See the fragment files in
-[changelog.d](https://github.com/wpk-nist-gov/module-utilities)
+[changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.2.0 — 2023-05-02
+
+### Added
+
+- Added method `assign_keys` to `DocFiller`.
+
 ## v0.1.0 — 2023-05-01
 
 ### Added
 
 - Add typing support. Passing mypy, pyright, pytype.
 
 This software was developed by employees of the National Institute of Standards
```

### Comparing `module-utilities-0.1.0/README.md` & `module-utilities-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/module-utilities
 [pypi-link]: https://pypi.org/project/module-utilities
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/module-utilities/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
-[repo-link]: https://github.com/wpk-nist-gov/module-utilities
+[repo-link]: https://github.com/usnistgov/module-utilities
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/module-utilities
 [conda-link]: https://anaconda.org/wpk-nist/module-utilities
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]:
-  https://github.com/wpk-nist-gov/module-utilities/blob/main/LICENSE
+[license-link]: https://github.com/usnistgov/module-utilities/blob/main/LICENSE
 
 <!-- other links -->
 
 [cachetools]: https://github.com/tkem/cachetools/
 
 # `module-utilities`
 
@@ -65,21 +64,14 @@
 
 or
 
 ```bash
 conda install -c wpk-nist module-utilities
 ```
 
-## Example usage
-
-```python
-import module_utilities
-
-```
-
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
 -->
@@ -96,10 +88,10 @@
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
-[wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
+[usnistgov/cookiecutter-pypackage](https://github.com/usnistgov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
```

### Comparing `module-utilities-0.1.0/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.2.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/Makefile` & `module-utilities-0.2.0/docs/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,14 @@
 
 livehtml:
 	$(SPHINXAUTOBUILD) "$(SOURCEDIR)" "$(BUILDDIR)/html" $(ALLSPHINXAUTOOPTS) $(O)
 
 showlinks:
 	python -m sphinx.ext.intersphinx $(BUILDDIR)/html/objects.inv
 
-release_args ?= '-m "update docs" -b nist-pages'
+release_args ?= -m "update docs" -b nist-pages
 release:
-	ghp-import -o -n -m $(release_args) $(BUILDDIR)/html
+	ghp-import -o -n $(release_args) $(BUILDDIR)/html
 
 command ?= @echo pass "command=..."
 command:
 	$(command)
```

### Comparing `module-utilities-0.1.0/docs/_static/css/nist-combined.css` & `module-utilities-0.2.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_static/js/leave_notice.js` & `module-utilities-0.2.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_static/js/nist-header-footer.js` & `module-utilities-0.2.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/autosummary/class.rst` & `module-utilities-0.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/autosummary/module.rst` & `module-utilities-0.2.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/class-individual-pages.rst` & `module-utilities-0.2.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/class-single-page.rst` & `module-utilities-0.2.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/custom-module-template.rst` & `module-utilities-0.2.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/module-custom-imported.rst` & `module-utilities-0.2.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/module-custom.rst` & `module-utilities-0.2.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/module-single.rst` & `module-utilities-0.2.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/_templates/module-template.rst` & `module-utilities-0.2.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/docs/conf.py` & `module-utilities-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,18 @@
 nb_kernel_rgx_aliases = {"module_utilities.*": "python3", "conda.*": "python3"}
 
 nb_execution_allow_errors = True
 
 # - top level variables --------------------------------------------------------
 # set github_username variable to be subbed later.
 # this makes it easy to switch from wpk -> usnistgov later
-github_username = "wpk-nist-gov"
+github_username = "usnistgov"
 
 html_context = {
-    "github_user": "wpk-nist-gov",
+    "github_user": "usnistgov",
     "github_repo": "module-utilities",
     "github_version": "main",
     "doc_path": "docs",
 }
 
 # -- python3 ---------------------------------------------------------------
 autosummary_generate = True
```

### Comparing `module-utilities-0.1.0/docs/installation.md` & `module-utilities-0.2.0/docs/installation.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## From sources
 
 The sources for module-utilities can be downloaded from the [Github repo].
 
 You can either clone the public repository:
 
 ```bash
-git clone git://github.com/wpk-nist-gov/module-utilities.git
+git clone git://github.com/usnistgov/module-utilities.git
 ```
 
 Once you have a copy of the source, you can install it with:
 
 ```bash
 pip install .
 ```
@@ -40,8 +40,8 @@
 conda activate {name}
 pip install [-e] --no-deps .
 ```
 
 where options in brackets are options (for environment name, and editable
 install, repectively).
 
-[github repo]: https://github.com/wpk-nist-gov/module-utilities
+[github repo]: https://github.com/usnistgov/module-utilities
```

### Comparing `module-utilities-0.1.0/docs/make.bat` & `module-utilities-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/environment/dev-extras.yaml` & `module-utilities-0.2.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/environment/docs-extras.yaml` & `module-utilities-0.2.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/pyproject.toml` & `module-utilities-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["readme", "version"]
 requires-python = ">=3.8"
 dependencies = ["typing-extensions"]
 
 [project.urls]
-homepage = "https://github.com/wpk-nist-gov/module-utilities"
+homepage = "https://github.com/usnistgov/module-utilities"
 documentation = "https://pages.nist.gov/module-utilities/"
 
 [project.optional-dependencies]
 test = ["pytest"]
 attrs = ["attrs"]
 
 # dev = []
@@ -174,15 +174,15 @@
 known-first-party = ["module_utilities"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.nbqa.addopts]
-ruff = ["--fix", "--extend-ignore=D100,B018"]
+ruff = ["--fix", "--extend-ignore=D100,B018,D101"]
 
 [tool.flake8]
 docstring-convention = "numpy"
 ignore = [
     # # whitespace before ':' - doesn't work well with black
     "E203",
     # module level import not at top of file
```

### Comparing `module-utilities-0.1.0/scripts/docs-examples-symlinks.sh` & `module-utilities-0.2.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/src/module_utilities/__init__.py` & `module-utilities-0.2.0/src/module_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/src/module_utilities/_doc.py` & `module-utilities-0.2.0/src/module_utilities/_doc.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/src/module_utilities/_docscrape.py` & `module-utilities-0.2.0/src/module_utilities/_docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/src/module_utilities/attributedict.py` & `module-utilities-0.2.0/src/module_utilities/attributedict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""AttributeDict module"""
+"""
+Attribute dictionary (:mod:`~module_utilities.attibutedict`)
+============================================================
+"""
 from __future__ import annotations
 
 from collections.abc import Mapping, MutableMapping
 from typing import Any
 
 # from typing import TypeVar, Type
```

### Comparing `module-utilities-0.1.0/src/module_utilities/cached.py` & `module-utilities-0.2.0/src/module_utilities/cached.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-"""Routines to define cached properties/methods in a class."""
+"""
+Cached class properties/methods (:mod:`~module_utilites.cached`)
+================================================================
+
+Routines to define cached properties/methods in a class.
+"""
 from __future__ import annotations
 
 from functools import wraps
 from inspect import signature
 from typing import Any, Callable, TypeVar, cast, overload
 
 from typing_extensions import ParamSpec
```

### Comparing `module-utilities-0.1.0/src/module_utilities/docfiller.py` & `module-utilities-0.2.0/src/module_utilities/docfiller.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,20 +325,48 @@
         return type(self)(dedent_recursive(self.data))
 
     @cached.meth
     def keys(self) -> list[str]:
         """List of keys"""
         return _recursive_keys(self.data)
 
-    def assign_combined_key(self, new_key: str, keys: Sequence[str]):
+    def assign_combined_key(self, new_key: str, keys: Sequence[str]) -> DocFiller:
         """Combine multiple keys into single key"""
         data = self.data.copy()
         data[new_key] = "\n".join([self.data[k] for k in keys])
         return type(self)(data)
 
+    def _gen_get_val(self, key):
+        from operator import attrgetter
+
+        f = attrgetter(key)
+
+        return f(self.params)
+
+    def assign_keys(self, **kwargs: str | Sequence[str]) -> DocFiller:
+        """
+        Create new key from other keys.
+
+        Parameters
+        ----------
+        **kwargs
+            new_key=old_key or new_key=[old_key0, old_key1, ...]
+            Note that dot notation is accepted.
+        """
+        data = self.data.copy()
+        for new_key, old_keys in kwargs.items():
+            if isinstance(old_keys, str):
+                keys = [old_keys]
+            else:
+                keys = list(old_keys)
+
+            data[new_key] = "\n".join([self._gen_get_val(k) for k in keys])
+
+        return type(self)(data)
+
     @classmethod
     def concat(
         cls,
         *args: Mapping[str, Any] | DocFiller,
         **kwargs: Mapping[str, Any] | DocFiller,
     ) -> DocFiller:
         """
@@ -410,14 +438,30 @@
         """Rename a keys at top level."""
         params = {}
         for k, v in self.data.items():
             key = kws.get(k, k)
             params[key] = v
         return type(self)(params)
 
+    # def rename(self, mapping: Mapping[Any, Hashable] | None = None, **kwargs) -> DocFiller:
+    #     """
+    #     New DocFiller with new names at top level.
+    #     """
+
+    #     if mapping is not None:
+    #         m = dict(mapping)
+    #     else:
+    #         m = {}
+
+    #     m = dict(m, **kwargs)
+
+    #     data = self.data.copy()
+    #     for old_name, v in m.items():
+    #         data[]
+
     @cached.prop
     def params(self) -> AttributeDict:
         """An AttributeDict view of parameters."""
         return AttributeDict.from_dict(self.data, max_level=1)
 
     @cached.prop
     def _default_decorator(self) -> Callable[[F], F]:
```

### Comparing `module-utilities-0.1.0/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.2.0/src/module_utilities.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.1.0
+Version: 0.2.0
 Summary: Collection of utilities to aid working with python modules.
-Home-page: https://github.com/wpk-nist-gov/module-utilities
+Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
-Project-URL: homepage, https://github.com/wpk-nist-gov/module-utilities
+Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -43,20 +43,19 @@
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/module-utilities
 [pypi-link]: https://pypi.org/project/module-utilities
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/module-utilities/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
-[repo-link]: https://github.com/wpk-nist-gov/module-utilities
+[repo-link]: https://github.com/usnistgov/module-utilities
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/module-utilities
 [conda-link]: https://anaconda.org/wpk-nist/module-utilities
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]:
-  https://github.com/wpk-nist-gov/module-utilities/blob/main/LICENSE
+[license-link]: https://github.com/usnistgov/module-utilities/blob/main/LICENSE
 
 <!-- other links -->
 
 [cachetools]: https://github.com/tkem/cachetools/
 
 # `module-utilities`
 
@@ -92,21 +91,14 @@
 
 or
 
 ```bash
 conda install -c wpk-nist module-utilities
 ```
 
-## Example usage
-
-```python
-import module_utilities
-
-```
-
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
 -->
@@ -123,29 +115,37 @@
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
-[wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
+[usnistgov/cookiecutter-pypackage](https://github.com/usnistgov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `module-utilities`
 
 ## Unreleased
 
 See the fragment files in
-[changelog.d](https://github.com/wpk-nist-gov/module-utilities)
+[changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.2.0 — 2023-05-02
+
+### Added
+
+- Added method `assign_keys` to `DocFiller`.
+
 ## v0.1.0 — 2023-05-01
 
 ### Added
 
 - Add typing support. Passing mypy, pyright, pytype.
 
 This software was developed by employees of the National Institute of Standards
```

### Comparing `module-utilities-0.1.0/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.2.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -47,31 +47,34 @@
 docs/_templates/autodocsumm/class.rst
 docs/_templates/autodocsumm/module-inherit.rst
 docs/_templates/autodocsumm/module-noindex.rst
 docs/_templates/autodocsumm/module.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
-docs/examples/create-symlinks.sh
+docs/examples/example-usage-1.rst
 docs/examples/example-usage.md
 docs/examples/index.md
-docs/examples/usage/demo.ipynb
+docs/examples/usage/cached.ipynb
+docs/examples/usage/docfiller.ipynb
 docs/reference/index.md
 environment/dev-extras.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
 environment/docs-extras.yaml
 environment/docs.yaml
 environment/lint-extras.yaml
 environment/lint.yaml
 environment/test-extras.yaml
 environment/test.yaml
 environment/tools.yaml
 examples/README.md
+examples/usage/cached.ipynb
+examples/usage/docfiller.ipynb
 scripts/dist-conda.mk
 scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
 scripts/lint.mk
 scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/module_utilities/__init__.py
```

### Comparing `module-utilities-0.1.0/tests/test_cached.py` & `module-utilities-0.2.0/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.1.0/tests/test_docfiller.py` & `module-utilities-0.2.0/tests/test_docfiller.py`

 * *Files 11% similar despite different names*

```diff
@@ -363,7 +363,88 @@
         """
 
         return a, b
 
     assert func2.__doc__ == expected
 
     assert func2(1, 1) == (1, 1)
+
+
+def test_assign_key():
+    d = DocFiller.from_docstring(
+        """
+        Parameters
+        ----------
+        x_float | x : float
+            x float
+        x_array | x : array-like
+            x array
+        y : int
+            y val
+        """,
+        combine_keys="parameters",
+    )
+
+    dd = d.assign_keys(x="x_float")
+
+    @dd.decorate
+    def test0():
+        """
+        Parameters
+        ----------
+        {x}
+        """
+
+    expected = dedent(
+        """
+        Parameters
+        ----------
+        x : float
+            x float
+        """
+    )
+
+    assert test0.__doc__ == expected
+
+    dd = d.assign_keys(x="x_array")
+
+    @dd.decorate
+    def test1():
+        """
+        Parameters
+        ----------
+        {x}
+        """
+
+    expected = dedent(
+        """
+        Parameters
+        ----------
+        x : array-like
+            x array
+        """
+    )
+
+    assert test1.__doc__ == expected
+
+    dd = d.assign_keys(x=["x_array", "y"])
+
+    @dd.decorate
+    def test2():
+        """
+        Parameters
+        ----------
+        {x}
+        """
+
+    expected = dedent(
+        """
+        Parameters
+        ----------
+        x : array-like
+            x array
+        y : int
+            y val
+        """
+    )
+
+    assert test2.__doc__ == expected
```

### Comparing `module-utilities-0.1.0/tox.ini` & `module-utilities-0.2.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         SETUPTOOLS_SCM_PRETEND_VERSION
         command
         mypy_args
         pyright_args
         pytype_args
         release_args
         project_name
+        TEST_VERSION
 usedevelop =
     test: True
 conda_env =
     test: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
@@ -116,18 +117,18 @@
     local: local
     remote: remote
     versions.
 usedevelop = False
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote: {[base]package_name}
+    conda-remote: {[base]package_name}{env:TEST_VERSION:''}
     conda-local: {posargs}
 deps =
-    pypi-remote: {[base]package_name}
+    pypi-remote: {[base]package_name}{env:TEST_VERSION:''}
     pypi-local: {posargs}
 
 [testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
```

