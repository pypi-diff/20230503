# Comparing `tmp/module-utilities-0.2.0.tar.gz` & `tmp/module-utilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.2.0.tar", last modified: Wed May  3 02:37:04 2023, max compression
+gzip compressed data, was "module-utilities-0.3.0.tar", last modified: Wed May  3 20:30:10 2023, max compression
```

## Comparing `module-utilities-0.2.0.tar` & `module-utilities-0.3.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.917237 module-utilities-0.2.0/
--rw-r--r--   0 wpk      (42033)    36681     1358 2023-05-03 02:36:13.000000 module-utilities-0.2.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.846022 module-utilities-0.2.0/.github/
--rw-r--r--   0 wpk      (42033)    36681      368 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1307 2023-05-02 03:09:02.000000 module-utilities-0.2.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3581 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-04-27 23:45:36.000000 module-utilities-0.2.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-27 23:45:36.000000 module-utilities-0.2.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      388 2023-05-03 02:36:13.000000 module-utilities-0.2.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9267 2023-05-03 02:36:13.000000 module-utilities-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-27 23:45:36.000000 module-utilities-0.2.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-04-27 23:45:36.000000 module-utilities-0.2.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11367 2023-05-03 02:36:13.000000 module-utilities-0.2.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     5953 2023-05-03 02:37:04.917642 module-utilities-0.2.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2844 2023-05-03 02:36:13.000000 module-utilities-0.2.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.846597 module-utilities-0.2.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.847078 module-utilities-0.2.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.847948 module-utilities-0.2.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-04-27 23:45:36.000000 module-utilities-0.2.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033)    36681      204 2023-04-27 23:45:36.000000 module-utilities-0.2.0/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.856969 module-utilities-0.2.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.832060 module-utilities-0.2.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.857729 module-utilities-0.2.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.859312 module-utilities-0.2.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.864844 module-utilities-0.2.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.869159 module-utilities-0.2.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.871899 module-utilities-0.2.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14793 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.874793 module-utilities-0.2.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681     1675 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/example-usage-1.rst
--rw-r--r--   0 wpk      (42033)    36681     1667 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       89 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.876991 module-utilities-0.2.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033)    36681    15671 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      937 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.877987 module-utilities-0.2.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      192 2023-05-03 02:36:13.000000 module-utilities-0.2.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.2.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.887416 module-utilities-0.2.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      232 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      349 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       64 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      136 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      116 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-04-27 23:45:36.000000 module-utilities-0.2.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 03:09:02.000000 module-utilities-0.2.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.888226 module-utilities-0.2.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-04-27 23:45:36.000000 module-utilities-0.2.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.889973 module-utilities-0.2.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.2.0/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033)    36681    15671 2023-05-03 02:36:13.000000 module-utilities-0.2.0/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6202 2023-05-03 02:36:13.000000 module-utilities-0.2.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.895228 module-utilities-0.2.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      403 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-27 23:45:36.000000 module-utilities-0.2.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 03:09:02.000000 module-utilities-0.2.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-04-27 23:45:36.000000 module-utilities-0.2.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681      297 2023-05-03 02:37:04.919251 module-utilities-0.2.0/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-27 23:45:36.000000 module-utilities-0.2.0/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.835442 module-utilities-0.2.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.902294 module-utilities-0.2.0/src/module_utilities/
--rw-r--r--   0 wpk      (42033)    36681      683 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2646 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033)    36681    23552 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_docscrape.py
--rw-r--r--   0 wpk      (42033)    36681      382 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033)    36681     5927 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033)    36681     9989 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033)    36681    19277 2023-05-03 02:36:13.000000 module-utilities-0.2.0/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-05-02 03:09:02.000000 module-utilities-0.2.0/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.910342 module-utilities-0.2.0/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     5953 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2670 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 12:55:39.000000 module-utilities-0.2.0/src/module_utilities.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033)    36681       48 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       17 2023-05-03 02:37:04.000000 module-utilities-0.2.0/src/module_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 02:37:04.916456 module-utilities-0.2.0/tests/
--rw-r--r--   0 wpk      (42033)    36681       46 2023-04-27 23:45:36.000000 module-utilities-0.2.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.2.0/tests/conftest.py
--rw-r--r--   0 wpk      (42033)    36681    10864 2023-05-02 03:09:02.000000 module-utilities-0.2.0/tests/test_cached.py
--rw-r--r--   0 wpk      (42033)    36681     7467 2023-05-03 02:36:13.000000 module-utilities-0.2.0/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033)    36681      169 2023-05-02 03:09:02.000000 module-utilities-0.2.0/tests/test_module_utilities.py
--rw-r--r--   0 wpk      (42033)    36681     4013 2023-05-03 02:36:13.000000 module-utilities-0.2.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.798253 module-utilities-0.3.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1358 2023-05-03 02:36:13.000000 module-utilities-0.3.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.741254 module-utilities-0.3.0/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1307 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3581 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.3.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      495 2023-05-03 20:28:18.000000 module-utilities-0.3.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9267 2023-05-03 02:36:13.000000 module-utilities-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-27 23:45:36.000000 module-utilities-0.3.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.3.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11367 2023-05-03 02:36:13.000000 module-utilities-0.3.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6060 2023-05-03 20:30:10.798663 module-utilities-0.3.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2844 2023-05-03 02:36:13.000000 module-utilities-0.3.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.742133 module-utilities-0.3.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.742900 module-utilities-0.3.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.743970 module-utilities-0.3.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.3.0/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.749812 module-utilities-0.3.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.728433 module-utilities-0.3.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.750500 module-utilities-0.3.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.752436 module-utilities-0.3.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.758369 module-utilities-0.3.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.763003 module-utilities-0.3.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.765680 module-utilities-0.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.767992 module-utilities-0.3.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1675 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/example-usage-1.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1667 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       89 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.769562 module-utilities-0.3.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      937 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.770407 module-utilities-0.3.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.780300 module-utilities-0.3.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      232 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      349 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.781523 module-utilities-0.3.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.3.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.783594 module-utilities-0.3.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.0/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.0/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6202 2023-05-03 02:36:13.000000 module-utilities-0.3.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.788777 module-utilities-0.3.0/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      403 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-27 23:45:36.000000 module-utilities-0.3.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-27 23:45:36.000000 module-utilities-0.3.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      297 2023-05-03 20:30:10.799712 module-utilities-0.3.0/setup.cfg
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-27 23:45:36.000000 module-utilities-0.3.0/setup.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.732011 module-utilities-0.3.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.792346 module-utilities-0.3.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      683 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23552 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_docscrape.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20974 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.795136 module-utilities-0.3.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6060 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2670 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-25 12:55:39.000000 module-utilities-0.3.0/src/module_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       48 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.797558 module-utilities-0.3.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.3.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.3.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.3.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-05-02 03:09:02.000000 module-utilities-0.3.0/tests/test_module_utilities.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4013 2023-05-03 02:36:13.000000 module-utilities-0.3.0/tox.ini
```

### Comparing `module-utilities-0.2.0/.cruft.json` & `module-utilities-0.3.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/.editorconfig` & `module-utilities-0.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/.gitignore` & `module-utilities-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/.pre-commit-config.yaml` & `module-utilities-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/CONTRIBUTING.md` & `module-utilities-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/LICENSE` & `module-utilities-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/Makefile` & `module-utilities-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/PKG-INFO` & `module-utilities-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of utilities to aid working with python modules.
 Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
@@ -132,14 +132,20 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.3.0 — 2023-05-03
+
+### Added
+
+- Added `DocFiller.assign_param` to more easily add a new parameter.
+
 ## v0.2.0 — 2023-05-02
 
 ### Added
 
 - Added method `assign_keys` to `DocFiller`.
 
 ## v0.1.0 — 2023-05-01
```

### Comparing `module-utilities-0.2.0/README.md` & `module-utilities-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.3.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/Makefile` & `module-utilities-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_static/css/nist-combined.css` & `module-utilities-0.3.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_static/js/leave_notice.js` & `module-utilities-0.3.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_static/js/nist-header-footer.js` & `module-utilities-0.3.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/autosummary/class.rst` & `module-utilities-0.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/autosummary/module.rst` & `module-utilities-0.3.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/class-individual-pages.rst` & `module-utilities-0.3.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/class-single-page.rst` & `module-utilities-0.3.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/custom-module-template.rst` & `module-utilities-0.3.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/module-custom-imported.rst` & `module-utilities-0.3.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/module-custom.rst` & `module-utilities-0.3.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/module-single.rst` & `module-utilities-0.3.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/_templates/module-template.rst` & `module-utilities-0.3.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/conf.py` & `module-utilities-0.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     "Series": "~pandas.Series",
     "DataFrame": "~pandas.DataFrame",
     "Categorical": "~pandas.Categorical",
     "Path": "~~pathlib.Path",
     # objects with abbreviated namespace (from pandas)
     "pd.Index": "~pandas.Index",
     "pd.NaT": "~pandas.NaT",
+    "DocFiller": "~module_utilities.docfiller.DocFiller",
 }
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
```

### Comparing `module-utilities-0.2.0/docs/examples/example-usage-1.rst` & `module-utilities-0.3.0/docs/examples/example-usage-1.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/examples/example-usage.md` & `module-utilities-0.3.0/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/examples/usage/cached.ipynb` & `module-utilities-0.3.0/docs/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/examples/usage/docfiller.ipynb` & `module-utilities-0.3.0/docs/examples/usage/docfiller.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9816478058014517%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, ':::\\n'), (5, '\\n'), (6, '\\n'), (7, ':::{note}\\n'), "*

 * *            "(8, '{mod}`~module_utilities.docfiller` assumes Numpy style docstrings\\n'), (10, "*

 * *            "'\\n')]}}, 6: {'outputs': {0: {'text': {insert: [(4, '\\n'), (14, '\\n'), (25, "*

 * *            "'\\n'), (35, '\\n')]}}}}, 9: {'source': {insert: [(0, '@ (\\n'), (1, '    "*

 * *            'd.update(\\n\'), (2, \'        summary="A function.",\\n\'), (3, \'        '*

 * *            'extended_summary="""\\n\'), ( […]*

```diff
@@ -7,14 +7,20 @@
             "source": [
                 "# docfiller\n",
                 "\n",
                 ":::{eval-rst}\n",
                 ".. currentmodule:: module_utilities.docfiller\n",
                 ":::\n",
                 "\n",
+                "\n",
+                ":::{note}\n",
+                "{mod}`~module_utilities.docfiller` assumes Numpy style docstrings\n",
+                ":::\n",
+                "\n",
+                "\n",
                 "It is common to want to share documentation information across functions/methods.  The module {mod}`~module_utilities.docfiller` provides a way to do this:\n",
                 "\n",
                 "For example, if you have these function:"
             ]
         },
         {
             "cell_type": "code",
@@ -156,42 +162,46 @@
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "A function.\n",
                         "\n",
                         "A longer description\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    An x param\n",
                         "y : int\n",
                         "    A y param\n",
                         "z : str\n",
                         "    A z param\n",
                         "\n",
+                        "\n",
                         "Returns\n",
                         "-------\n",
                         "output : float\n",
                         "    An output\n",
                         "\n",
                         "\n",
                         "A different function.\n",
                         "\n",
                         "A longer description of b_function\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    An x param\n",
                         "y : float\n",
                         "    A different y param\n",
                         "z : str\n",
                         "    A z param\n",
                         "\n",
+                        "\n",
                         "Returns\n",
                         "-------\n",
                         "output : float\n",
                         "    An different output\n",
                         "\n"
                     ]
                 }
@@ -272,27 +282,23 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "95067163",
             "metadata": {},
             "outputs": [],
             "source": [
-                "@d.update(\n",
-                "    summary=\"A function.\",\n",
-                "    extended_summary=\"\"\"\n",
-                "    A longer description\n",
-                "    \"\"\",\n",
-                "    y=\"\"\"\n",
-                "    y : int\n",
-                "        A y param\n",
-                "    \"\"\",\n",
-                "    output=\"\"\"\n",
-                "    output : float\n",
-                "        An output\n",
-                "    \"\"\",\n",
+                "@ (\n",
+                "    d.update(\n",
+                "        summary=\"A function.\",\n",
+                "        extended_summary=\"\"\"\n",
+                "        A longer description\n",
+                "        \"\"\",\n",
+                "    )\n",
+                "    .assign_param(\"y\", \"int\", \"A y param\")\n",
+                "    .assign_param(\"output\", \"float\", \"An output\")\n",
                 ").dedent().decorate\n",
                 "def a_function3(x, y, z):\n",
                 "    \"\"\"\n",
                 "    {summary}\n",
                 "\n",
                 "    {extended_summary}\n",
                 "\n",
@@ -309,40 +315,36 @@
                 "    {output}\n",
                 "    \"\"\"\n",
                 "\n",
                 "\n",
                 "assert a_function3.__doc__ == a_function2.__doc__\n",
                 "\n",
                 "\n",
-                "@d.update(\n",
-                "    summary=\"A different function.\",\n",
-                "    extended_summary=\"A longer description of b_function\",\n",
-                "    y=\"\"\"\n",
-                "    y : float\n",
-                "        A different y param\n",
-                "    \"\"\",\n",
-                "    output=\"\"\"\n",
-                "    output : float\n",
-                "        An different output\n",
-                "    \"\"\",\n",
+                "@ (\n",
+                "    d.update(\n",
+                "        summary=\"A different function.\",\n",
+                "        extended_summary=\"A longer description of b_function\",\n",
+                "    )\n",
+                "    .assign_param(\"y\", \"float\", \"A different y param\")\n",
+                "    .assign_param(\"output\", \"float\", \"An different output\")\n",
                 ").dedent()(a_function3)\n",
                 "def b_function3(x, y, z):\n",
                 "    pass\n",
                 "\n",
                 "\n",
                 "assert b_function3.__doc__ == b_function2.__doc__"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4fd7eb47",
             "metadata": {},
             "source": [
-                "Note that for `b_function3`, we used the template/docstring from `a_function3`.  {class}`docfiller.DocFiller` defaults to using\n",
-                "the functions docstring for replacement.  But you can pass a string or function to use as the template to be filled."
+                "Note that for `b_function3`, we used the template/docstring from `a_function3`.  {class}`DocFiller` defaults to using\n",
+                "the functions docstring for replacement.  But you can pass a string or function to use as the template to be filled.  Above, we also used {meth}`DocFiller.assign_param` to create a correctly formatted parameter."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6fcd8202",
             "metadata": {},
             "source": [
@@ -443,26 +445,28 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "A thing\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    x parameter\n",
                         "y : float\n",
                         "    y parameter\n",
                         "beta : float\n",
                         "    A float value for beta\n",
                         "\n",
                         "\n",
                         "An array thing\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    x parameter\n",
                         "y : float\n",
                         "    y parameter\n",
                         "beta : array-like\n",
@@ -535,14 +539,16 @@
             "cell_type": "code",
             "execution_count": 9,
             "id": "6db66b94",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# back to call because passing parameters\n",
+                "\n",
+                "\n",
                 "@d(beta=d[\"beta_float\"], summary=\"A thing\")\n",
                 "def func_float2(x, y, beta):\n",
                 "    \"\"\"\n",
                 "    {summary}\n",
                 "\n",
                 "\n",
                 "    Parameters\n",
@@ -563,20 +569,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0a5a4821",
             "metadata": {},
             "source": [
-                "Better still, you can use {meth}`docfiller.Docfiller.assign_keys`:"
+                "Better still, you can use {meth}`DocFiller.assign_keys`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "id": "4fee935c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "@d.assign_keys(beta=\"beta_float\")(summary=\"A thing\")\n",
                 "def func_float3(x, y, beta):\n",
                 "    \"\"\"\n",
@@ -598,15 +604,15 @@
                 "\n",
                 "assert func_float3.__doc__ == func_float.__doc__\n",
                 "assert func_array3.__doc__ == func_array.__doc__"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 11,
             "id": "68fcb14e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -652,14 +658,126 @@
                 "    {y}\n",
                 "    {z0}\n",
                 "    \"\"\"\n",
                 "\n",
                 "\n",
                 "print(func0.__doc__)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "7c7039c5",
+            "metadata": {},
+            "source": [
+                "## Works with classes\n",
+                "\n",
+                "This also works with classes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "id": "bf6b8405",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "expected = \"\"\"\n",
+                "A summary\n",
+                "\n",
+                "A longer summary\n",
+                "\n",
+                "Parameters\n",
+                "----------\n",
+                "x : float\n",
+                "    x param\n",
+                "    some other stuff\n",
+                "y : float\n",
+                "    y param\n",
+                "\n",
+                "Returns\n",
+                "-------\n",
+                "out : float\n",
+                "    output\n",
+                "\"\"\"\n",
+                "\n",
+                "d = DocFiller.from_docstring(expected, combine_keys=\"parameters\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
+            "id": "2eb1580a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class hello in module __main__:\n",
+                        "\n",
+                        "class hello(builtins.object)\n",
+                        " |  A summary\n",
+                        " |  \n",
+                        " |  A longer summary\n",
+                        " |  \n",
+                        " |  Parameters\n",
+                        " |  ----------\n",
+                        " |  x : float\n",
+                        " |      x param\n",
+                        " |      some other stuff\n",
+                        " |  y : float\n",
+                        " |      y param\n",
+                        " |  \n",
+                        " |  Returns\n",
+                        " |  -------\n",
+                        " |  out : float\n",
+                        " |      output\n",
+                        " |  \n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d()\n",
+                "class hello:\n",
+                "    \"\"\"\n",
+                "    {summary}\n",
+                "\n",
+                "    {extended_summary}\n",
+                "\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    {x}\n",
+                "    {y}\n",
+                "\n",
+                "    Returns\n",
+                "    -------\n",
+                "    {returns.out}\n",
+                "    \"\"\"\n",
+                "\n",
+                "\n",
+                "assert hello.__doc__ == expected\n",
+                "\n",
+                "\n",
+                "@d(hello)\n",
+                "class hello2(hello):\n",
+                "    pass\n",
+                "\n",
+                "\n",
+                "assert hello2.__doc__ == expected\n",
+                "\n",
+                "help(hello)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "module-utilities-dev [conda env:dev-3]",
             "language": "python",
             "name": "conda-env-dev-3-py"
```

### Comparing `module-utilities-0.2.0/docs/installation.md` & `module-utilities-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/docs/make.bat` & `module-utilities-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/environment/dev-extras.yaml` & `module-utilities-0.3.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/environment/docs-extras.yaml` & `module-utilities-0.3.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/examples/usage/cached.ipynb` & `module-utilities-0.3.0/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/examples/usage/docfiller.ipynb` & `module-utilities-0.3.0/examples/usage/docfiller.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9816478058014517%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, ':::\\n'), (5, '\\n'), (6, '\\n'), (7, ':::{note}\\n'), "*

 * *            "(8, '{mod}`~module_utilities.docfiller` assumes Numpy style docstrings\\n'), (10, "*

 * *            "'\\n')]}}, 6: {'outputs': {0: {'text': {insert: [(4, '\\n'), (14, '\\n'), (25, "*

 * *            "'\\n'), (35, '\\n')]}}}}, 9: {'source': {insert: [(0, '@ (\\n'), (1, '    "*

 * *            'd.update(\\n\'), (2, \'        summary="A function.",\\n\'), (3, \'        '*

 * *            'extended_summary="""\\n\'), ( […]*

```diff
@@ -7,14 +7,20 @@
             "source": [
                 "# docfiller\n",
                 "\n",
                 ":::{eval-rst}\n",
                 ".. currentmodule:: module_utilities.docfiller\n",
                 ":::\n",
                 "\n",
+                "\n",
+                ":::{note}\n",
+                "{mod}`~module_utilities.docfiller` assumes Numpy style docstrings\n",
+                ":::\n",
+                "\n",
+                "\n",
                 "It is common to want to share documentation information across functions/methods.  The module {mod}`~module_utilities.docfiller` provides a way to do this:\n",
                 "\n",
                 "For example, if you have these function:"
             ]
         },
         {
             "cell_type": "code",
@@ -156,42 +162,46 @@
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "A function.\n",
                         "\n",
                         "A longer description\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    An x param\n",
                         "y : int\n",
                         "    A y param\n",
                         "z : str\n",
                         "    A z param\n",
                         "\n",
+                        "\n",
                         "Returns\n",
                         "-------\n",
                         "output : float\n",
                         "    An output\n",
                         "\n",
                         "\n",
                         "A different function.\n",
                         "\n",
                         "A longer description of b_function\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    An x param\n",
                         "y : float\n",
                         "    A different y param\n",
                         "z : str\n",
                         "    A z param\n",
                         "\n",
+                        "\n",
                         "Returns\n",
                         "-------\n",
                         "output : float\n",
                         "    An different output\n",
                         "\n"
                     ]
                 }
@@ -272,27 +282,23 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "95067163",
             "metadata": {},
             "outputs": [],
             "source": [
-                "@d.update(\n",
-                "    summary=\"A function.\",\n",
-                "    extended_summary=\"\"\"\n",
-                "    A longer description\n",
-                "    \"\"\",\n",
-                "    y=\"\"\"\n",
-                "    y : int\n",
-                "        A y param\n",
-                "    \"\"\",\n",
-                "    output=\"\"\"\n",
-                "    output : float\n",
-                "        An output\n",
-                "    \"\"\",\n",
+                "@ (\n",
+                "    d.update(\n",
+                "        summary=\"A function.\",\n",
+                "        extended_summary=\"\"\"\n",
+                "        A longer description\n",
+                "        \"\"\",\n",
+                "    )\n",
+                "    .assign_param(\"y\", \"int\", \"A y param\")\n",
+                "    .assign_param(\"output\", \"float\", \"An output\")\n",
                 ").dedent().decorate\n",
                 "def a_function3(x, y, z):\n",
                 "    \"\"\"\n",
                 "    {summary}\n",
                 "\n",
                 "    {extended_summary}\n",
                 "\n",
@@ -309,40 +315,36 @@
                 "    {output}\n",
                 "    \"\"\"\n",
                 "\n",
                 "\n",
                 "assert a_function3.__doc__ == a_function2.__doc__\n",
                 "\n",
                 "\n",
-                "@d.update(\n",
-                "    summary=\"A different function.\",\n",
-                "    extended_summary=\"A longer description of b_function\",\n",
-                "    y=\"\"\"\n",
-                "    y : float\n",
-                "        A different y param\n",
-                "    \"\"\",\n",
-                "    output=\"\"\"\n",
-                "    output : float\n",
-                "        An different output\n",
-                "    \"\"\",\n",
+                "@ (\n",
+                "    d.update(\n",
+                "        summary=\"A different function.\",\n",
+                "        extended_summary=\"A longer description of b_function\",\n",
+                "    )\n",
+                "    .assign_param(\"y\", \"float\", \"A different y param\")\n",
+                "    .assign_param(\"output\", \"float\", \"An different output\")\n",
                 ").dedent()(a_function3)\n",
                 "def b_function3(x, y, z):\n",
                 "    pass\n",
                 "\n",
                 "\n",
                 "assert b_function3.__doc__ == b_function2.__doc__"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4fd7eb47",
             "metadata": {},
             "source": [
-                "Note that for `b_function3`, we used the template/docstring from `a_function3`.  {class}`docfiller.DocFiller` defaults to using\n",
-                "the functions docstring for replacement.  But you can pass a string or function to use as the template to be filled."
+                "Note that for `b_function3`, we used the template/docstring from `a_function3`.  {class}`DocFiller` defaults to using\n",
+                "the functions docstring for replacement.  But you can pass a string or function to use as the template to be filled.  Above, we also used {meth}`DocFiller.assign_param` to create a correctly formatted parameter."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6fcd8202",
             "metadata": {},
             "source": [
@@ -443,26 +445,28 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "A thing\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    x parameter\n",
                         "y : float\n",
                         "    y parameter\n",
                         "beta : float\n",
                         "    A float value for beta\n",
                         "\n",
                         "\n",
                         "An array thing\n",
                         "\n",
+                        "\n",
                         "Parameters\n",
                         "----------\n",
                         "x : float\n",
                         "    x parameter\n",
                         "y : float\n",
                         "    y parameter\n",
                         "beta : array-like\n",
@@ -535,14 +539,16 @@
             "cell_type": "code",
             "execution_count": 9,
             "id": "6db66b94",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# back to call because passing parameters\n",
+                "\n",
+                "\n",
                 "@d(beta=d[\"beta_float\"], summary=\"A thing\")\n",
                 "def func_float2(x, y, beta):\n",
                 "    \"\"\"\n",
                 "    {summary}\n",
                 "\n",
                 "\n",
                 "    Parameters\n",
@@ -563,20 +569,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0a5a4821",
             "metadata": {},
             "source": [
-                "Better still, you can use {meth}`docfiller.Docfiller.assign_keys`:"
+                "Better still, you can use {meth}`DocFiller.assign_keys`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "id": "4fee935c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "@d.assign_keys(beta=\"beta_float\")(summary=\"A thing\")\n",
                 "def func_float3(x, y, beta):\n",
                 "    \"\"\"\n",
@@ -598,15 +604,15 @@
                 "\n",
                 "assert func_float3.__doc__ == func_float.__doc__\n",
                 "assert func_array3.__doc__ == func_array.__doc__"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 11,
             "id": "68fcb14e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -652,14 +658,126 @@
                 "    {y}\n",
                 "    {z0}\n",
                 "    \"\"\"\n",
                 "\n",
                 "\n",
                 "print(func0.__doc__)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "7c7039c5",
+            "metadata": {},
+            "source": [
+                "## Works with classes\n",
+                "\n",
+                "This also works with classes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "id": "bf6b8405",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "expected = \"\"\"\n",
+                "A summary\n",
+                "\n",
+                "A longer summary\n",
+                "\n",
+                "Parameters\n",
+                "----------\n",
+                "x : float\n",
+                "    x param\n",
+                "    some other stuff\n",
+                "y : float\n",
+                "    y param\n",
+                "\n",
+                "Returns\n",
+                "-------\n",
+                "out : float\n",
+                "    output\n",
+                "\"\"\"\n",
+                "\n",
+                "d = DocFiller.from_docstring(expected, combine_keys=\"parameters\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
+            "id": "2eb1580a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class hello in module __main__:\n",
+                        "\n",
+                        "class hello(builtins.object)\n",
+                        " |  A summary\n",
+                        " |  \n",
+                        " |  A longer summary\n",
+                        " |  \n",
+                        " |  Parameters\n",
+                        " |  ----------\n",
+                        " |  x : float\n",
+                        " |      x param\n",
+                        " |      some other stuff\n",
+                        " |  y : float\n",
+                        " |      y param\n",
+                        " |  \n",
+                        " |  Returns\n",
+                        " |  -------\n",
+                        " |  out : float\n",
+                        " |      output\n",
+                        " |  \n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d()\n",
+                "class hello:\n",
+                "    \"\"\"\n",
+                "    {summary}\n",
+                "\n",
+                "    {extended_summary}\n",
+                "\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    {x}\n",
+                "    {y}\n",
+                "\n",
+                "    Returns\n",
+                "    -------\n",
+                "    {returns.out}\n",
+                "    \"\"\"\n",
+                "\n",
+                "\n",
+                "assert hello.__doc__ == expected\n",
+                "\n",
+                "\n",
+                "@d(hello)\n",
+                "class hello2(hello):\n",
+                "    pass\n",
+                "\n",
+                "\n",
+                "assert hello2.__doc__ == expected\n",
+                "\n",
+                "help(hello)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "module-utilities-dev [conda env:dev-3]",
             "language": "python",
             "name": "conda-env-dev-3-py"
```

### Comparing `module-utilities-0.2.0/pyproject.toml` & `module-utilities-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/scripts/docs-examples-symlinks.sh` & `module-utilities-0.3.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/src/module_utilities/__init__.py` & `module-utilities-0.3.0/src/module_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/src/module_utilities/_doc.py` & `module-utilities-0.3.0/src/module_utilities/_doc.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/src/module_utilities/_docscrape.py` & `module-utilities-0.3.0/src/module_utilities/_docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/src/module_utilities/attributedict.py` & `module-utilities-0.3.0/src/module_utilities/attributedict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Attribute dictionary (:mod:`~module_utilities.attibutedict`)
-============================================================
+Attribute dictionary (:mod:`~module_utilities.attributedict`)
+=============================================================
 """
 from __future__ import annotations
 
 from collections.abc import Mapping, MutableMapping
 from typing import Any
 
 # from typing import TypeVar, Type
@@ -35,15 +35,15 @@
     `{name.property}` in a nested manner.
 
     Parameters
     ----------
     entries : dict
     recursive : bool, default=True
         If True, recursively return ``AttributeDict`` for nested dicts.
-    allow_missing : bool, defualt=True
+    allow_missing : bool, default=True
         If True, allow missing keys.
 
     Example
     -------
     >>> d = AttributeDict({"a": 1, "b": {"c": 2}})
     >>> d.a
     1
@@ -169,15 +169,15 @@
     @classmethod
     def from_dict(
         cls, params: Mapping, max_level: int = 1, recursive: bool = True
     ) -> AttributeDict:
         """
         Create AttributeDict recursively for nested dictionaries.
 
-        To be used in cases where need to apply AttibuteDict to parameters
+        To be used in cases where need to apply AttributeDict to parameters
         passed with ``func(**params)``.
 
 
         Parameters
         ----------
         params : mapping
             Mapping to apply cls to.
```

### Comparing `module-utilities-0.2.0/src/module_utilities/cached.py` & `module-utilities-0.3.0/src/module_utilities/cached.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Cached class properties/methods (:mod:`~module_utilites.cached`)
-================================================================
+Cached class properties/methods (:mod:`~module_utilities.cached`)
+=================================================================
 
 Routines to define cached properties/methods in a class.
 """
 from __future__ import annotations
 
 from functools import wraps
 from inspect import signature
```

### Comparing `module-utilities-0.2.0/src/module_utilities/docfiller.py` & `module-utilities-0.3.0/src/module_utilities/docfiller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Fill and share documentation (:mod:`module_utilities.doc_decorate`)
+Fill and share documentation (:mod:`module_utilities.docfiller`)
 ================================================================
 """
 from __future__ import annotations
 
 import inspect
 import os
 from textwrap import dedent
@@ -101,14 +101,17 @@
 
     if isinstance(desc, str):
         if desc == "":
             desc = []
         else:
             desc = [desc]
 
+    elif len(desc) == 1 and desc[0] == "":
+        desc = []
+
     if len(desc) > 0:
         desc = "\n    ".join(desc)
         s += f"\n    {desc}"
     return s
 
 
 def _params_to_string(params, key_char: str = "|") -> str | dict[str, Any]:
@@ -309,77 +312,153 @@
             self.data = params
         else:
             self.data = dict(params)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self.data)})"
 
+    def new_like(self, data: dict | None = None) -> DocFiller:
+        """Create new object with optional data."""
+        if data is None:
+            data = self.data.copy()
+        return type(self)(data)
+
     def __getitem__(self, key: str):
         val = self.data[key]
         if isinstance(val, dict):
-            return type(self)(val)
+            return self.new_like(val)
         else:
             return val
 
     def dedent(self) -> DocFiller:
         """Recursively dedent params"""
-        return type(self)(dedent_recursive(self.data))
+        return self.new_like(dedent_recursive(self.data))
 
     @cached.meth
     def keys(self) -> list[str]:
         """List of keys"""
         return _recursive_keys(self.data)
 
     def assign_combined_key(self, new_key: str, keys: Sequence[str]) -> DocFiller:
         """Combine multiple keys into single key"""
-        data = self.data.copy()
-        data[new_key] = "\n".join([self.data[k] for k in keys])
-        return type(self)(data)
+        new = self.new_like()
+        new.data[new_key] = "\n".join([self.data[k] for k in keys])
+        return new
 
     def _gen_get_val(self, key):
         from operator import attrgetter
 
         f = attrgetter(key)
-
         return f(self.params)
 
     def assign_keys(self, **kwargs: str | Sequence[str]) -> DocFiller:
         """
         Create new key from other keys.
 
         Parameters
         ----------
         **kwargs
             new_key=old_key or new_key=[old_key0, old_key1, ...]
             Note that dot notation is accepted.
+
+
+        Examples
+        --------
+        >>> d = DocFiller({'a0': 'a0', 'a1': 'a1', 'b': 'b'})
+        >>> dn = d.assign_keys(a='a0', c=['a0','b']).data
+        >>> print(dn['a'])
+        a0
+
+        >>> print(dn['c'])
+        a0
+        b
+
+
         """
-        data = self.data.copy()
+        new = self.new_like()
         for new_key, old_keys in kwargs.items():
             if isinstance(old_keys, str):
                 keys = [old_keys]
             else:
                 keys = list(old_keys)
 
-            data[new_key] = "\n".join([self._gen_get_val(k) for k in keys])
+            new.data[new_key] = "\n".join([self._gen_get_val(k) for k in keys])
 
-        return type(self)(data)
+        return new
+
+    def assign_param(
+        self,
+        name: str,
+        ptype: str = "",
+        desc: str | list[str] = [],
+        key: str | None = None,
+    ):
+        """
+        Add in a new parameter
+
+        Parameters
+        ----------
+        name : str
+            Parameters name
+        key : str, optional
+            Optional key for placement in `self`.  This is like using `key | name`.
+        ptype : str, default=''
+            Optional type.
+        desc : str or list of str, default=''
+            Parameter description.
+
+        Returns
+        -------
+        output : DocFiller
+            New DocFiller instance.
+
+        Examples
+        --------
+        >>> d = DocFiller()
+        >>> dn = d.assign_param(
+        ...     name='x',
+        ...     ptype='float',
+        ...     desc='''
+        ...     A parameter
+        ...     with multiple levels
+        ...     ''',
+        ... )
+        >>> print(dn['x'])
+        x : float
+            A parameter
+            with multiple levels
+        """
+
+        new = self.new_like()
+
+        # cleanup desc
+        if isinstance(desc, str):
+            desc = dedent(desc).strip().split("\n")
+
+        key = name if key is None else key
+
+        new.data[key] = _build_param_docstring(name=name, ptype=ptype, desc=desc)
+
+        return new
 
     @classmethod
     def concat(
         cls,
         *args: Mapping[str, Any] | DocFiller,
         **kwargs: Mapping[str, Any] | DocFiller,
     ) -> DocFiller:
         """
         Create new object from multiple DocFiller or dict objects.
 
         Parameters
         ----------
-        *args : dict or Docfiller objects
-        **kwargs : dict or Docfiller objects
+        *args
+            dict or Docfiller
+        **kwargs
+            dict or Docfiller objects
             The passed name will be used as the top level.
 
         Returns
         -------
         DocFiller
             combined DocFiller object.
 
@@ -420,31 +499,31 @@
     def insert_level(self, name: str) -> DocFiller:
         """Insert a level/namespace."""
         return type(self)({name: self.data})
 
     def levels_to_top(self, *names: str) -> DocFiller:
         """Make a level top level accessible"""
 
-        params = dict(self.data)
+        new = self.new_like()
         for name in names:
             d = self.data[name]
             if isinstance(d, str):
                 raise ValueError(f"level {name} is not a dict")
             else:
                 for k, v in self.data[name].items():
-                    params[k] = v
-        return type(self)(params)
+                    new.data[k] = v
+        return new
 
     def rename_levels(self, **kws: str) -> DocFiller:
         """Rename a keys at top level."""
         params = {}
         for k, v in self.data.items():
             key = kws.get(k, k)
             params[key] = v
-        return type(self)(params)
+        return self.new_like(params)
 
     # def rename(self, mapping: Mapping[Any, Hashable] | None = None, **kwargs) -> DocFiller:
     #     """
     #     New DocFiller with new names at top level.
     #     """
 
     #     if mapping is not None:
@@ -465,17 +544,21 @@
 
     @cached.prop
     def _default_decorator(self) -> Callable[[F], F]:
         return doc_decorate(**self.params)
 
     def update(self, *args, **kwargs) -> DocFiller:
         """Update parameters"""
-        data = self.data.copy()
-        data.update(*args, **kwargs)
-        return type(self)(params=data)
+        new = self.new_like()
+        new.data.update(*args, **kwargs)
+        return new
+
+    def assign(self, **kwargs) -> DocFiller:
+        """Assign new key/value pairs"""
+        return self.update(**kwargs)
 
     def decorate(self, func: F) -> F:
         """
         Default decorator.
 
         This uses `self.params` and the decorated funciton docstring as a template.
         """
@@ -501,20 +584,14 @@
         if ntemplates == nparams == 0:
             return self.decorate
         elif nparams == 0:
             return doc_decorate(*templates, **self.params)
         else:
             return self.update(params)(*templates)
 
-        # if nparams > 0:
-        #     params = AttributeDict.from_dict({**self.data, **params}, max_level=1)
-        # else:
-        #     params = self.params
-        # return doc_decorate(*templates, **params)
-
     # NOTE: This is dangerous.
     # if you pass a function as a template, but forget to explicitly pass it,
     # you overwrite the docstring for that function.  Just really confusing
     # def dec(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
     #     """
     #     General decorator.
 
@@ -577,15 +654,15 @@
         Create a Docfiller instance from a dictionary.
 
         Parameters
         ----------
         params : mapping
         namespace : str, optional
             Top level namespace for DocFiller.
-        combine_keys : str, sequence of str, mapping, optional.
+        combine_keys : str, sequence of str, mapping, optional
             If str or sequence of str, Keys of ``params`` to at the top level.
             If mapping, should be of form {namespace: key(s)}
 
         keep_keys : str, sequence of str, bool
             If False, then don't keep any keys at top level.  This is useful with the ``combine_keys`` parameter.
             If True, keep all keys, regardless of combine_keys.
             If str or sequence of str, keep these keys in output.
@@ -651,15 +728,15 @@
 
         Parameters
         ----------
         func_or_doc : str or callable
             Docstring to parse to get parameters.
         namespace : str, optional
             Top level namespace for DocFiller.
-        combine_keys : str, sequence of str, mapping, optional.
+        combine_keys : str, sequence of str, mapping, optional
             If str or sequence of str, Keys of ``params`` to at the top level.
             If mapping, should be of form {namespace: key(s)}
         key_char : str, default="|"
             Character to split names.  By default, for parameters, the key will be parsed from
             The docstring. If you want to override this, you can use
             `key | name : ....` in the definition (where `'|'` is the value of `key_char`).
         keep_keys : str, sequence of str, bool
```

### Comparing `module-utilities-0.2.0/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.3.0/src/module_utilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of utilities to aid working with python modules.
 Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
@@ -132,14 +132,20 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.3.0 — 2023-05-03
+
+### Added
+
+- Added `DocFiller.assign_param` to more easily add a new parameter.
+
 ## v0.2.0 — 2023-05-02
 
 ### Added
 
 - Added method `assign_keys` to `DocFiller`.
 
 ## v0.1.0 — 2023-05-01
```

### Comparing `module-utilities-0.2.0/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.3.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/tests/test_cached.py` & `module-utilities-0.3.0/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.2.0/tests/test_docfiller.py` & `module-utilities-0.3.0/tests/test_docfiller.py`

 * *Files 5% similar despite different names*

```diff
@@ -444,7 +444,108 @@
             x array
         y : int
             y val
         """
     )
 
     assert test2.__doc__ == expected
+
+
+def test_DocFiller_assign_param():
+    expected = dedent(
+        """
+    A summary
+
+    A longer summary
+
+    Parameters
+    ----------
+    x : float
+        x param
+        With an extra line
+    y : int
+        y param
+    z : float
+    """
+    )
+
+    d = DocFiller()
+
+    dd = (
+        d.assign_param(
+            "x",
+            ptype="float",
+            desc="""
+            x param
+            With an extra line
+            """,
+        )
+        .assign_param("y", ptype="int", desc="y param")
+        .assign_param("z", ptype="float")
+    )
+
+    @dd()
+    def func():
+        """
+        A summary
+
+        A longer summary
+
+        Parameters
+        ----------
+        {x}
+        {y}
+        {z}
+        """
+        pass
+
+    assert func.__doc__ == expected
+
+
+def test_DocFiller_on_class():
+    expected = """
+    A summary
+
+    A longer summary
+
+    Parameters
+    ----------
+    x : float
+        x param
+        some other stuff
+    y : float
+        y param
+
+    Returns
+    -------
+    out : float
+        output
+    """
+
+    expected = dedent(expected)
+
+    d = DocFiller.from_docstring(expected, combine_keys="parameters")
+
+    @d()
+    class hello:
+        """
+        {summary}
+
+        {extended_summary}
+
+        Parameters
+        ----------
+        {x}
+        {y}
+
+        Returns
+        -------
+        {returns.out}
+        """
+
+    assert hello.__doc__ == expected
+
+    @d(hello)
+    class hello2(hello):
+        pass
+
+    assert hello.__doc__ == expected
```

### Comparing `module-utilities-0.2.0/tox.ini` & `module-utilities-0.3.0/tox.ini`

 * *Files identical despite different names*

