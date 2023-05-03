# Comparing `tmp/nvm-0.0.1.tar.gz` & `tmp/nvm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-0.0.1.tar", last modified: Wed May  3 19:20:16 2023, max compression
+gzip compressed data, was "nvm-0.0.2.tar", last modified: Wed May  3 19:28:10 2023, max compression
```

## Comparing `nvm-0.0.1.tar` & `nvm-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.0.1/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.0.1/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/.github/
--rw-------   0 jiko      (1000) jiko      (1000)      314 2023-05-03 18:32:02.000000 nvm-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-03 18:32:02.000000 nvm-0.0.1/.gitignore
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.0.1/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.0.1/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.0.1/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.0.1/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.0.1/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     2990 2023-05-03 19:15:50.000000 nvm-0.0.1/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:20:16.327937 nvm-0.0.1/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)      748 2023-05-03 18:44:59.000000 nvm-0.0.1/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.1/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.0.1/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.1/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.0.1/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.0.1/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.323937 nvm-0.0.1/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.323937 nvm-0.0.1/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-03 15:23:48.000000 nvm-0.0.1/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-03 15:23:48.000000 nvm-0.0.1/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.323937 nvm-0.0.1/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-03 15:23:49.000000 nvm-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-03 15:23:35.000000 nvm-0.0.1/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.1/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.1/docs/build/html/_static/plus.png
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5202 2023-05-03 19:00:16.000000 nvm-0.0.1/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-03 19:00:19.000000 nvm-0.0.1/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      265 2023-05-03 19:00:19.000000 nvm-0.0.1/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.0.1/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      338 2023-05-03 18:32:02.000000 nvm-0.0.1/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-03 19:20:16.327937 nvm-0.0.1/nvm/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.0.1/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1108 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-03 19:20:16.000000 nvm-0.0.1/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.0.1/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      414 2023-05-03 18:32:02.000000 nvm-0.0.1/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      546 2023-05-03 19:20:16.327937 nvm-0.0.1/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.0.1/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:20:16.327937 nvm-0.0.1/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.0.1/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-03 18:32:02.000000 nvm-0.0.1/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.0.1/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.0.1/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.0.2/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.0.2/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/.github/
+-rw-------   0 jiko      (1000) jiko      (1000)      314 2023-05-03 18:32:02.000000 nvm-0.0.2/.github/ISSUE_TEMPLATE.md
+-rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-03 18:32:02.000000 nvm-0.0.2/.gitignore
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.0.2/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.0.2/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.0.2/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.0.2/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.0.2/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     2990 2023-05-03 19:15:50.000000 nvm-0.0.2/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:28:10.041162 nvm-0.0.2/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)      748 2023-05-03 18:44:59.000000 nvm-0.0.2/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/bin/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/bin/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.0.2/bin/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.0.2/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.0.2/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-03 15:23:48.000000 nvm-0.0.2/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-03 15:23:48.000000 nvm-0.0.2/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-03 15:23:49.000000 nvm-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      526 2023-05-03 19:24:06.000000 nvm-0.0.2/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5202 2023-05-03 19:00:16.000000 nvm-0.0.2/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-03 19:00:19.000000 nvm-0.0.2/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      265 2023-05-03 19:00:19.000000 nvm-0.0.2/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      338 2023-05-03 18:32:02.000000 nvm-0.0.2/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm/_version.py
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.0.2/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1130 2023-05-03 19:28:10.000000 nvm-0.0.2/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.0.2/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      414 2023-05-03 18:32:02.000000 nvm-0.0.2/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      546 2023-05-03 19:28:10.041162 nvm-0.0.2/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.0.2/setup.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.0.2/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-03 18:32:02.000000 nvm-0.0.2/tests/test_nvm.py
+-rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.0.2/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.0.2/versioneer.py
```

### Comparing `nvm-0.0.1/.gitignore` & `nvm-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/CONTRIBUTING.rst` & `nvm-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/LICENSE` & `nvm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/Makefile` & `nvm-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/PKG-INFO` & `nvm-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.0.1/README.rst` & `nvm-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/data/emacs-logo/emacs-128x128.png` & `nvm-0.0.2/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/data/emacs-logo/emacs.svg` & `nvm-0.0.2/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/docs/Makefile` & `nvm-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/docs/source/conf.py` & `nvm-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/docs/source/installation.rst` & `nvm-0.0.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/nvm.egg-info/PKG-INFO` & `nvm-0.0.2/nvm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.0.1/nvm.egg-info/SOURCES.txt` & `nvm-0.0.2/nvm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .github/ISSUE_TEMPLATE.md
 bin/.gitkeep
 bin/nvm.py
 data/.gitkeep
 data/emacs-logo/emacs-128x128.png
 data/emacs-logo/emacs.svg
 docs/Makefile
+docs/requirements.txt
 docs/build/html/_static/check-solid.svg
 docs/build/html/_static/copy-button.svg
 docs/build/html/_static/file.png
 docs/build/html/_static/minus.png
 docs/build/html/_static/plus.png
 docs/build/html/_static/css/fonts/fontawesome-webfont.svg
 docs/source/authors.rst
```

### Comparing `nvm-0.0.1/nvm.egg-info/requires.txt` & `nvm-0.0.2/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/pyproject.toml` & `nvm-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/setup.cfg` & `nvm-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/setup.py` & `nvm-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/tests/test_nvm.py` & `nvm-0.0.2/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/tox.ini` & `nvm-0.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `nvm-0.0.1/versioneer.py` & `nvm-0.0.2/versioneer.py`

 * *Files identical despite different names*

