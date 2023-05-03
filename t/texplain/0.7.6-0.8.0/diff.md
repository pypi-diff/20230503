# Comparing `tmp/texplain-0.7.6.tar.gz` & `tmp/texplain-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplain-0.7.6.tar", last modified: Tue Apr  4 09:41:46 2023, max compression
+gzip compressed data, was "texplain-0.8.0.tar", last modified: Wed May  3 15:26:23 2023, max compression
```

## Comparing `texplain-0.7.6.tar` & `texplain-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.582376 texplain-0.7.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.574376 texplain-0.7.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.578376 texplain-0.7.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-04 09:41:28.000000 texplain-0.7.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-04 09:41:28.000000 texplain-0.7.6/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-04 09:41:28.000000 texplain-0.7.6/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-04 09:41:28.000000 texplain-0.7.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-04 09:41:28.000000 texplain-0.7.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 09:41:28.000000 texplain-0.7.6/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-04 09:41:28.000000 texplain-0.7.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-04 09:41:28.000000 texplain-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-04 09:41:46.582376 texplain-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-04 09:41:28.000000 texplain-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.578376 texplain-0.7.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 09:41:28.000000 texplain-0.7.6/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-04 09:41:28.000000 texplain-0.7.6/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 09:41:28.000000 texplain-0.7.6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:41:46.582376 texplain-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-04 09:41:28.000000 texplain-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.578376 texplain-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.578376 texplain-0.7.6/tests/input1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/example.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.578376 texplain-0.7.6/tests/input1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/figures/Diverging.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/figures/Sequential.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/input1/unsrtnat.bst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.582376 texplain-0.7.6/tests/output1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/figure_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/figure_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/library.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/output1/unsrtnat.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_find_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_indent_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-04 09:41:28.000000 texplain-0.7.6/tests/test_texplain_example1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.582376 texplain-0.7.6/texplain/
--rw-r--r--   0 runner    (1001) docker     (123)    81164 2023-04-04 09:41:28.000000 texplain-0.7.6/texplain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:41:46.582376 texplain-0.7.6/texplain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 09:41:46.000000 texplain-0.7.6/texplain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.844694 texplain-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-03 15:26:07.000000 texplain-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-03 15:26:07.000000 texplain-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-03 15:26:07.000000 texplain-0.8.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 15:26:07.000000 texplain-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:26:07.000000 texplain-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 15:26:23.852695 texplain-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-03 15:26:07.000000 texplain-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/pre-commit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 15:26:07.000000 texplain-0.8.0/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 15:26:07.000000 texplain-0.8.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:26:23.852695 texplain-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-03 15:26:07.000000 texplain-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/input1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/example.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/input1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/figures/Diverging.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/figures/Sequential.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/unsrtnat.bst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/tests/output1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/figure_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/figure_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/library.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/unsrtnat.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_find_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_texindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_texplain_example1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/texplain/
+-rw-r--r--   0 runner    (1001) docker     (123)    87026 2023-05-03 15:26:07.000000 texplain-0.8.0/texplain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/texplain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/top_level.txt
```

### Comparing `texplain-0.7.6/.github/workflows/ci.yml` & `texplain-0.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/.github/workflows/pythonpublish.yml` & `texplain-0.8.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/.gitignore` & `texplain-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/.pre-commit-config.yaml` & `texplain-0.8.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
     args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
@@ -22,23 +22,33 @@
   - id: autoflake
     args: [--in-place, --remove-unused-variable, --remove-all-unused-imports]
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.9.0
   hooks:
   - id: reorder-python-imports
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.3.2
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
     args: [--max-line-length=100, --ignore=E203, --per-file-ignore=tests/test_one_sentence_per_line.py:E501, --per-file-ignore=tests/test_indent_long.py:E501]
+- repo: https://github.com/pre-commit/pygrep-hooks
+  rev: v1.10.0
+  hooks:
+  - id: python-check-blanket-noqa
+  - id: python-check-blanket-type-ignore
+  - id: python-no-log-warn
+  - id: python-use-type-annotations
+  - id: rst-backticks
+  - id: rst-directive-colons
+  - id: rst-inline-touching-normal
 - repo: https://github.com/asottile/setup-cfg-fmt
   rev: v2.2.0
   hooks:
   - id: setup-cfg-fmt
 - repo: https://github.com/tdegeus/conda_envfile
   rev: v0.4.2
   hooks:
```

### Comparing `texplain-0.7.6/LICENSE` & `texplain-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/PKG-INFO` & `texplain-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.7.6
+Version: 0.8.0
 Summary: Create directory with TeX-file and only dependencies.
 Home-page: https://github.com/tdegeus/texplain
 Author: Tom de Geus
 Author-email: tom@geus.me
 License: MIT
 Keywords: LaTeX
 Description-Content-Type: text/markdown
@@ -18,50 +18,50 @@
 
 **Documentation: [https://texplain.readthedocs.io](texplain.readthedocs.io)**
 
 # Usage
 
 ## command-line
 
+*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
+    Automatic indentation and formatting of a TeX-file.
+
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
     Apply any of the following options to a TeX-file:
 
     -   Remove all comments or comment-lines.
     -   Modify all occurrences of a command, for example to change `\TG{deleted}{inserted}` to `inserted`.
     -   Rename a label.
     -   Ensure common prefixes for all labels.
     -   Ensure usage of `\cref` instead of `\ref`.
 
-*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
-    Wrapper around [latexindent.pl](https://github.com/cmhughes/latexindent.pl) with augmented rules to make especially `oneSentencePerLine` more robust.
-
 *   [texplain](https://texplain.readthedocs.io/en/latest/tools.html#texplain):
     Create a directory with a TeX-file and only its dependencies
     (those figure-files and references that are actually included).
     This is particularly useful to create a clean version to submit to a journal.
 
 ## pre-commit
 
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texcleanup
         args: [--format-labels, --use-cleveref]
     ```
 
 *   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texindent
         args: []
     ```
 
 ## Python
```

### Comparing `texplain-0.7.6/README.md` & `texplain-0.8.0/texplain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,67 @@
+Metadata-Version: 2.1
+Name: texplain
+Version: 0.8.0
+Summary: Create directory with TeX-file and only dependencies.
+Home-page: https://github.com/tdegeus/texplain
+Author: Tom de Geus
+Author-email: tom@geus.me
+License: MIT
+Keywords: LaTeX
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![ci](https://github.com/tdegeus/texplain/workflows/CI/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![Documentation Status](https://readthedocs.org/projects/texplain/badge/?version=latest)](https://texplain.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://github.com/tdegeus/texplain/workflows/pre-commit/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/texplain.svg)](https://anaconda.org/conda-forge/texplain)
 
 **Documentation: [https://texplain.readthedocs.io](texplain.readthedocs.io)**
 
 # Usage
 
 ## command-line
 
+*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
+    Automatic indentation and formatting of a TeX-file.
+
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
     Apply any of the following options to a TeX-file:
 
     -   Remove all comments or comment-lines.
     -   Modify all occurrences of a command, for example to change `\TG{deleted}{inserted}` to `inserted`.
     -   Rename a label.
     -   Ensure common prefixes for all labels.
     -   Ensure usage of `\cref` instead of `\ref`.
 
-*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
-    Wrapper around [latexindent.pl](https://github.com/cmhughes/latexindent.pl) with augmented rules to make especially `oneSentencePerLine` more robust.
-
 *   [texplain](https://texplain.readthedocs.io/en/latest/tools.html#texplain):
     Create a directory with a TeX-file and only its dependencies
     (those figure-files and references that are actually included).
     This is particularly useful to create a clean version to submit to a journal.
 
 ## pre-commit
 
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texcleanup
         args: [--format-labels, --use-cleveref]
     ```
 
 *   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texindent
         args: []
     ```
 
 ## Python
```

### Comparing `texplain-0.7.6/docs/Makefile` & `texplain-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/docs/make.bat` & `texplain-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/docs/module.rst` & `texplain-0.8.0/docs/module.rst`

 * *Files 23% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     texplain.bib_select
 
 Indent LaTeX files
 ------------------
 
 .. autosummary::
 
-    texplain.texindent
+    texplain.indent
 
 Support functions
 -----------------
 
 .. autosummary::
 
     texplain.environments
     texplain.Placeholder
     texplain.text_to_placeholders
     texplain.text_from_placeholders
     texplain.find_commented
     texplain.is_commented
     texplain.remove_comments
 
-Documentation
-=============
+Details
+=======
 
 .. automodule:: texplain
     :members:
     :undoc-members: PlacholderType
```

### Comparing `texplain-0.7.6/setup.py` & `texplain-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="LaTeX",
     url=f"https://github.com/tdegeus/{project_name:s}",
     packages=find_packages(),
     use_scm_version={"write_to": f"{project_name}/_version.py"},
     setup_requires=["setuptools_scm"],
-    install_requires=["click", "numpy", "typing_extensions>=4.5.0"],
+    install_requires=["click", "numpy"],
     entry_points={
         "console_scripts": [
             f"texplain = {project_name}:_texplain_cli",
             f"texcleanup = {project_name}:_texcleanup_cli",
             f"texindent = {project_name}:_texindent_cli",
         ]
     },
```

### Comparing `texplain-0.7.6/tests/input1/apalike.bst` & `texplain-0.8.0/tests/input1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/example.tex` & `texplain-0.8.0/tests/input1/example.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/figures/Diverging.pdf` & `texplain-0.8.0/tests/input1/figures/Diverging.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/figures/Sequential.pdf` & `texplain-0.8.0/tests/input1/figures/Sequential.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/goose-article.cls` & `texplain-0.8.0/tests/input1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/refs.bib` & `texplain-0.8.0/tests/input1/refs.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/input1/unsrtnat.bst` & `texplain-0.8.0/tests/input1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/apalike.bst` & `texplain-0.8.0/tests/output1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/figure_1.pdf` & `texplain-0.8.0/tests/output1/figure_1.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/figure_2.pdf` & `texplain-0.8.0/tests/output1/figure_2.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/goose-article.cls` & `texplain-0.8.0/tests/output1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/library.bib` & `texplain-0.8.0/tests/output1/library.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/main.tex` & `texplain-0.8.0/tests/output1/main.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/output1/unsrtnat.bst` & `texplain-0.8.0/tests/output1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_align.py` & `texplain-0.8.0/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_classify.py` & `texplain-0.8.0/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_find_command.py` & `texplain-0.8.0/tests/test_find_command.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_indent.py` & `texplain-0.8.0/tests/test_indent.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_indent_long.py` & `texplain-0.8.0/tests/test_indent_long.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_placeholders.py` & `texplain-0.8.0/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_simple.py` & `texplain-0.8.0/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/tests/test_texplain_example1.py` & `texplain-0.8.0/tests/test_texplain_example1.py`

 * *Files identical despite different names*

### Comparing `texplain-0.7.6/texplain/__init__.py` & `texplain-0.8.0/texplain/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,89 +8,68 @@
 import textwrap
 from copy import deepcopy
 from shutil import copyfile
 
 import numpy as np
 from numpy.typing import ArrayLike
 from numpy.typing import NDArray
-from typing_extensions import deprecated
 
 from ._version import version  # noqa: F401
 from ._version import version_tuple  # noqa: F401
 
 
 class PlaceholderType(enum.Enum):
     r"""
     Type of placeholder.
-    The placeholders' practical definition is in :py:func:`text_to_placeholder`.
+    The placeholders' practical definition is in :py:func:`text_to_placeholders`.
     The intended use is:
 
-    :py:attr:`line`: A single line of content (1 line).
-    :py:attr:`inline_comment`: A comment that is preceded by some content.
-    :py:attr:`comment`: A comment that is the only content on that line.
-    :py:attr:`tabular`: Entire block ``\begin{tabular} ... \end{tabular}``.
-    :py:attr:`math`: Entire block of displaystyle math. E.g. ``\begin{equation} ... \end{equation}``
-    :py:attr:`inline_math`: Entire block of inline math. E.g. ``$ ... $``.
-    :py:attr:`math_line`: A single line of content in math mode.
-    :py:attr:`environment`: Entire block of environment: ``\begin{...} ... \end{...}``.
-    :py:attr:`command`: Entire block of command: ``\command[...]{...}``.
-    :py:attr:`curly_braced`: Entire block of curly braced content: ``{...}``.
-    :py:attr:`command_like`: Entire block of :py:attr:`command` or :py:attr:`curly_braced`.
-    :py:attr:`noindent_block`: Entire block of ``% \begin{noindent} ... % \end{noindent}``.
-    :py:attr:`verbatim`: Entire block of ``\begin{verbatim} ... \end{verbatim}``.
-    :py:attr:`let_command`: Definition ``\let...``.
-    :py:attr:`newif_command`: Definition ``\newif...``.
+    -   :py:attr:`line`: A single line of content (no newline).
+    -   :py:attr:`inline_comment`: A comment that is preceded by some content (no newline).
+    -   :py:attr:`comment`: A comment that is the only content on that line (no newline).
+    -   :py:attr:`tabular`: Block ``\begin{tabular} ... \end{tabular}``.
+    -   :py:attr:`math`: Block of displaymath. E.g. ``\begin{equation} ... \end{equation}``.
+    -   :py:attr:`inline_math`: Block of inline math. E.g. ``$ ... $``.
+    -   :py:attr:`math_line`: A single line of content in math mode (no newline).
+    -   :py:attr:`environment`: Block of environment: ``\begin{...} ... \end{...}``.
+    -   :py:attr:`command`: Block of command: ``\command[...]{...}``.
+    -   :py:attr:`curly_braced`: Block of curly braced content: ``{...}``.
+    -   :py:attr:`command_like`: Block of :py:attr:`command` or :py:attr:`curly_braced`.
+    -   :py:attr:`texindent_block`: Block of ``% \begin{texindent} ... % \end{texindent}``.
+    -   :py:attr:`noindent_block`: Block of ``% \begin{noindent} ... % \end{noindent}``.
+    -   :py:attr:`verbatim`: Block of ``\begin{verbatim} ... \end{verbatim}``.
+    -   :py:attr:`let_command`: Definition ``\let...``.
+    -   :py:attr:`newif_command`: Definition ``\newif...``.
 
-    Except for :py:attr:`line`, :py:attr:`math_line`, :py:attr:`comment`, :py:attr:`inline_comment`
-    all placeholders can span more than one line.
+    Except for :py:attr:`line`, :py:attr:`math_line`, :py:attr:`comment`, :py:attr:`inline_comment`,
+    and :py:attr:`math_line` all placeholders can span more than one line.
     """
 
     line = enum.auto()
     inline_comment = enum.auto()
     comment = enum.auto()
     tabular = enum.auto()
     math = enum.auto()
     inline_math = enum.auto()
     math_line = enum.auto()
     environment = enum.auto()
     command = enum.auto()
     curly_braced = enum.auto()
     command_like = enum.auto()
+    texindent_block = enum.auto()
     noindent_block = enum.auto()
     verbatim = enum.auto()
     let_command = enum.auto()
     newif_command = enum.auto()
 
 
-@deprecated("Use regex directly")
-def find_opening(
-    text: str,
-    opening: str,
-    ignore_escaped: bool = True,
-) -> list[int]:
-    r"""
-    Find opening 'bracket'.
-
-    :param text: The string to consider.
-    :param opening: The opening 'bracket' (e.g. "(", "[", "{", but also "%").
-    :param ignore_escaped: Ignore escaped 'bracket' (e.g. "\(", "\[", "\{", "\%").
-    :return: List of indices of opening 'brackets' (sorted by definition).
-    """
-
-    o = re.escape(opening)
-
-    if ignore_escaped:
-        o = r"(?<!\\)" + o
-
-    return [i.span()[0] for i in re.finditer(o, text)]
-
-
 def find_commented(text: str) -> list[list[int]]:
     """
-    Find comments bits of text.
+    Find comments.
+
     The output is such that one can find the comments text as follows::
 
         for i, j in find_commented(text):
             print(text[i : j]) # i is the index of "%"
 
     :param text: Text.
     :return: List of of indices of the beginning and end of the comments.
@@ -107,15 +86,15 @@
         newlines = newlines[j + 1 :]  # noqa: E203
 
     return ret
 
 
 def is_commented(text: str) -> NDArray[np.bool_]:
     """
-    Return array that lists per character if it corresponds to commented text.
+    Per character if it corresponds to commented text.
 
     :param text: Text.
     :return: Array of booleans of size ``len(text)``.
     """
 
     comments = find_commented(text)
     ret = np.zeros(len(text), dtype=bool)
@@ -417,15 +396,16 @@
     for i in range(len(text)):
         text[i] = re.sub(r"([^%]*)(?<!\\)(%)(.*)$", r"\1", text[i])
     return "\n".join(text)
 
 
 def environments(text: str) -> list[str]:
     r"""
-    Return list with present environments (between ``\begin{...} ... \end{...}``).
+    Return list with present environments.
+    This corresponds to the text between ``\begin{...}`` and ``\end{...}``.
     """
 
     ret = []
     curly_braces = find_matching(text, "{", "}", ignore_escaped=True)
 
     for i in re.finditer(r"\\begin{.*}", text):
         opening = i.span(0)[0] + 6
@@ -442,15 +422,15 @@
     This class stores the text to be replaced by a placeholder and the placeholder itself.
     In addition, it can store the whitespace before and after the placeholder.
 
     :param placeholder: The placeholder to use.
     :param content: The text replaced by the placeholder.
     :param space_front: The whitespace before the placeholder.
     :param space_back: The whitespace after the placeholder.
-    :param ptype: The type of placeholder.
+    :param ptype: The type of placeholder, see :py:class:`PlaceholderType`.
     :param search_placeholder:
         The regex used to search for the placeholder
         (optional, but speeds up greatly for batch searches).
     """
 
     def __init__(
         self,
@@ -486,15 +466,15 @@
             placeholder, text = Placeholder.from_text(placeholder, text, start, end)
             text = placeholder.to_text(text)
 
         :param placeholder: The placeholder to use.
         :param text: The text to consider.
         :param start: The start index of ``text`` to be replaced by the placeholder.
         :param end: The end index of ``text`` to be replaced by the placeholder.
-        :param ptype: The type of placeholder.
+        :param ptype: The type of placeholder, see :py:class:`PlaceholderType`.
         :param search_placeholder: The regex used to search the placeholder.
         :return: ``(Placeholder, text)`` where in ``text`` the placeholder is inserted.
         """
         pre = text[:start][::-1]
         post = text[end:]
         front = re.search(r"\s*", pre).end()
         back = re.search(r"\ *\n?", post).end()
@@ -513,15 +493,15 @@
     def to_text(self, text: str, index: int = None, keep_placeholder: bool = False) -> str:
         """
         Replace placeholder with content.
         If the whitespace before and after the placeholder is stored, it is restored.
 
         :param text: Text.
         :param index: The index of the placeholder.
-        :param keep_placeholder: If ``True`` the placeholder is kept (it is merely positioned).
+        :param keep_placeholder: If ``True`` keep the placeholder, change only the whitespace.
         :return: Text with placeholder replaced by content.
         """
 
         if index is None:
             index = text.find(self.placeholder)
 
         # placeholder not found
@@ -678,14 +658,25 @@
             r"%\s*\\end{noindent}",
             escape=False,
             closing_match=1,
             return_array=True,
         )
         return _apply_placeholders(text, indices, base, "noindent".upper(), ptype)
 
+    if ptype == PlaceholderType.texindent_block:
+        indices = find_matching(
+            text,
+            r"%\s*\\begin{texindent}",
+            r"%\s*\\end{texindent}",
+            escape=False,
+            closing_match=1,
+            return_array=True,
+        )
+        return _apply_placeholders(text, indices, base, "texindent".upper(), ptype)
+
     if ptype == PlaceholderType.verbatim:
         indices = find_matching(
             text,
             r"\\begin{verbatim}",
             r"\\end{verbatim}",
             escape=False,
             closing_match=1,
@@ -858,14 +849,28 @@
 
         is replaced with
 
         .. code-block:: latex
 
             -BASE-NOINDENT-1-
 
+    -   :py:class:`PlaceholderType.texindent_block`:
+
+        .. code-block:: latex
+
+            % \begin{texindent}
+            ...
+            % \end{texindent}
+
+        is replaced with
+
+        .. code-block:: latex
+
+            -BASE-TEXINDENT-1-
+
     -   :py:class:`PlaceholderType.verbatim`:
 
         .. code-block:: latex
 
             \begin{verbatim}
             ...
             \end{verbatim}
@@ -1049,16 +1054,16 @@
 
     :param text: Text.
     :param ptypes: List of placeholder types to replace
     :param base: Base string for placeholders
     :param placeholders_comments: List of placeholders that are comments (needed to search commands)
     :return:
         ``(text, placeholders)`` with
-        -  ``text``: Text with placeholders
-        -  ``placeholders``: List of placeholders
+            -  ``text``: Text with placeholders
+            -  ``placeholders``: List of placeholders
     """
 
     ret = []
 
     for ptype in ptypes:
         text, placeholders = _detail_text_to_placholders(text, ptype, base, placeholders_comments)
         ret += placeholders
@@ -1193,35 +1198,14 @@
             lines[i] = fmt.format(*(lines[i] + [""] * (len(width) - len(lines[i])))).rstrip()
         else:
             lines[i] = " ".join(lines[i])
 
     return "\n".join(lines)
 
 
-@deprecated("Use ``indent`` instead.")
-def align(
-    text: str,
-    environment: str,
-    align: str = "<",
-    base: str = "TEXINDENT-ALIGN",
-):
-    r"""
-    For all occurrences of an environment:
-    -   Place ``\begin{...}[...]{...}`` and ``\end{...}`` on own line.
-    -   Align ``&`` and ``\\`` of all lines that contain those alignment characters.
-
-    :param text: Text.
-    :param environment: Name of the environment.
-    :param align: Alignment of columns (``"<"``, ``">"`` or ``"^"``).
-    :param base: Base for temporary placeholders.
-    :return: Formatted text.
-    """
-    return indent(text, indent="")
-
-
 def _is_placeholder(text: str, placeholders: list[Placeholder]) -> list[bool]:
     """
     Check per character if it is a placeholder.
 
     :param text: Text.
     :param placeholders: List of placeholders.
     :return: List of booleans.
@@ -1245,18 +1229,20 @@
         is_comment[ret[i] : ret[i] + len(i)] = True
 
     return is_comment
 
 
 def _begin_end_one_separate_line(text: str, comment_placeholders: list[Placeholder]) -> str:
     r"""
-    Put :
+    Put:
+
     -   ``\begin{...}`` and ``\\end{...}``
     -   ``\[`` and ``\]``
     -   ``\if`` and ``\else`` and ``\fi``
+
     on separate lines.
 
     :param text: Text.
     :param comment_placeholder:
         List of :py:class:`Placeholder` for comments.
         Assumes that all comments are replaced by placeholders.
 
@@ -1305,186 +1291,356 @@
             ]
 
         text = "".join(split)
 
     return text
 
 
-def indent(text: str, indent: str = "    ") -> str:
-    """
+def _placeholders_lrsquash(placeholders: list[Placeholder]) -> list[Placeholder]:
+    for placeholder in placeholders:
+        placeholder.space_front = re.sub(r"\n\n+\ *", r"\n\n", placeholder.space_front)
+        placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
+        placeholder.space_back = re.sub(r"\n\n+\ *", r"\n\n", placeholder.space_back)
+        placeholder.space_back = re.sub(r"\ +", r" ", placeholder.space_back)
+    return placeholders
+
+
+def _placeholders_indent(placeholders: list[Placeholder]) -> list[Placeholder]:
+    for placeholder in placeholders:
+        content = placeholder.content.splitlines()
+        header = content[0]
+        footer = content[-1]
+        content = content[1:-1]
+        assert re.match(r"%\s*\\begin{texindent}", header)
+        assert re.match(r"%\s*\\end{texindent}", footer)
+        opts = re.split(r"(%\s*\\begin{texindent}{)(.*)(})", header)[2]
+        opts = {i.split("=")[0]: i.split("=")[1] for i in opts.split(",")}
+        for key in opts:
+            if key not in ["indentation"]:
+                opts[key] = opts[key].lower() in ("yes", "true", "t", "1")
+        placeholder.content = "\n".join([header, indent("\n".join(content), **opts), footer])
+    return placeholders
+
+
+def indent(
+    text: str,
+    indentation: str = "    ",
+    rstrip: bool = True,
+    lstrip: bool = True,
+    squashlines: bool = True,
+    squashspaces: bool = True,
+    symbols: bool = True,
+    environment: bool = True,
+    argument: bool = True,
+    inlinemath: bool = True,
+    linebreak: bool = True,
+    sentence: bool = True,
+    alignment: bool = True,
+    texindent: bool = True,
+    noindent: bool = True,
+) -> str:
+    r"""
     Indent text.
 
     :param text: The text to indent.
-    :param indent: The indentation to use.
+
+    :param indentation:
+        Set indentation of lines between:
+
+        -   ``\begin{...}[...]{...}`` and ``\end{...}``.
+        -   ``\[`` and ``\]``.
+        -   ``{`` and ``}``.
+        -   ``[`` and ``]`` (as command option).
+
+        Comment lines follow indentation.
+        Requires: ``lstrip``, ``inlinemath``, ```environment``.
+        To switch off indentation, set ``indentation=""``.
+
+    :param rstrip: Remove trailing spaces on all lines.
+    :param lstrip: Remove all leading spaces before applying indentation.
+    :param squashlines: Reduce the maximum number of consecutive blank lines to 2.
+    :param squashspaces: Reduce the maximum number of consecutive spaces to 1.
+    :param symbols: In math-mode: all symbols are separated by a space.
+
+    :param environment:
+        ``\begin{...}[...]{...}`` and ``\end{...}`` (and ``\[`` and ``\]``)
+        are placed on separate lines.
+
+    :param argument:
+        Any option or argument that spans more than one line is placed on separate lines.
+        For example:
+
+        .. code-block:: tex
+
+            xxx { This is a very long argument
+            that is more than one line long. } yyy
+
+        is formatted to:
+
+        .. code-block:: tex
+
+            xxx {
+                This is a very long argument
+                that is more than one line long.
+            } yyy
+
+    :param inlinemath: Inline math is placed on one line.
+    :param linebreak: ``\\`` is followed by a newline.
+
+    :param sentence:
+        One sentence per line.
+        Every sentence should start on a new line,
+        and it should be (as much as possible) on a single line.
+        The following rules of thumb are followed:
+
+        -   A sentence ends with:
+
+            -   A period, question mark, or exclamation mark.
+            -   ``\begin{...}`` or ``\end{...}``.
+            -   Two white lines.
+            -   ``\\``
+            -   The end of an argument (``}`` or ``]``), see below.
+            -   A command on the next line.
+
+        -   Commands and inline math are treated as a single word.
+            Formatting is applied on the arguments of commands.
+
+        Requires: ``rstrip``, ``lstrip``, ``squashspaces``.
+
+    :param alignment:
+
+        -   If the resulting line is less that 100 characters
+            columns in tabular environments are aligned at ``&`` and also ``\\`` are aligned.
+
+        -   In other cases single spaces are placed around ``&`` and before ``\\``.
+
+        Requires: ``environment``.
+
+    :param texindent:
+        Custom formatting in blocks:
+
+        .. code-block:: tex
+
+            % \begin{texindent}{...}
+            ...
+            % \end{texindent}
+
+        where the ``{...}`` argument is a comma-separated list of options of this function;
+        for example:
+
+        .. code-block:: tex
+
+            % \begin{texindent}{sentence=False, inlinemath=False}
+            ...
+            % \end{texindent}
+
+    :param noindent:
+        Verbatim environments and everything between
+
+        .. code-block:: tex
+
+            % \begin{noindent}
+            ...
+            % \end{noindent}
+
+        is not formatted.
+
     :return: The indented text.
     """
 
     if len(text) == 0:
         return text
 
     # check for known limitation
     if re.match(r"(?<!\\)(\$)(?<!\\)(\$)", text):
         raise NotImplementedError("Panic: don't know to deal with double dollar signs")
 
     # remove leading/trailing newlines, and trailing whitespace on each line
-    text = _rstrip_lines(text.strip())
+    if rstrip:
+        text = _rstrip_lines(text.strip())
+
+    # custom formatting
+    if texindent:
+        text, placeholders_texindent = text_to_placeholders(text, [PlaceholderType.texindent_block])
+        placeholders_texindent = _placeholders_lrsquash(placeholders_texindent)
+        placeholders_texindent = _placeholders_indent(placeholders_texindent)
+    else:
+        placeholders_texindent = []
 
     # "noindent" blocks are kept exactly as they are
-    text, placeholders_noindent = text_to_placeholders(
-        text, [PlaceholderType.noindent_block, PlaceholderType.verbatim]
-    )
-    # remove leading/trailing duplicate newlines
-    for placeholder in placeholders_noindent:
-        placeholder.space_front = re.sub(r"\n\n+\ *", r"\n\n", placeholder.space_front)
-        placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
-        placeholder.space_back = re.sub(r"\n\n+\ *", r"\n\n", placeholder.space_back)
-        placeholder.space_back = re.sub(r"\ +", r" ", placeholder.space_back)
+    if noindent:
+        text, placeholders_noindent = text_to_placeholders(
+            text, [PlaceholderType.noindent_block, PlaceholderType.verbatim]
+        )
+        placeholders_noindent = _placeholders_lrsquash(placeholders_noindent)
+    else:
+        placeholders_noindent = []
+    placeholders_noindent += placeholders_texindent
 
     # comments: exclude from formatting
     text, placeholders_comment = text_to_placeholders(text, [PlaceholderType.comment])
     text, placeholders_rcomment = text_to_placeholders(text, [PlaceholderType.inline_comment])
 
-    # line comments: remove leading whitespace
-    for placeholder in placeholders_comment:
-        placeholder.space_front = re.sub(r"(\n*)(\ *)", r"\1", placeholder.space_front)
-        placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
-
-    # inline comments: remove duplicate leading spaces
-    for placeholder in placeholders_rcomment:
-        placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
+    if lstrip:
+        # line comments: remove leading whitespace
+        for placeholder in placeholders_comment:
+            placeholder.space_front = re.sub(r"(\n*)(\ *)", r"\1", placeholder.space_front)
+            placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
+
+        # inline comments: remove duplicate leading spaces
+        for placeholder in placeholders_rcomment:
+            placeholder.space_front = re.sub(r"\ +", r" ", placeholder.space_front)
 
     # all comments are equal for the remainder of the implementation
     placeholders_comments = placeholders_comment + placeholders_rcomment
 
     # remove multiple newlines, duplicate spaces, and any leading whitespace
-    text = _lstrip_lines(text)
-    text = re.sub(r"(\n\n+)", r"\n\n", text)
-    text = re.sub(r"(\ +)", r" ", text)
+    if lstrip:
+        text = _lstrip_lines(text)
+    if squashlines:
+        text = re.sub(r"(\n\n+)", r"\n\n", text)
+    if squashspaces:
+        text = re.sub(r"(\ +)", r" ", text)
 
     # fold inline math
     text, placeholders_inline_math = text_to_placeholders(text, [PlaceholderType.inline_math])
     # inline math: always on one line
-    for placeholder in placeholders_inline_math:
-        placeholder.content = placeholder.content.replace("\n", " ")
-        placeholder.content = re.sub(r"(\ +)", r" ", placeholder.content)
-        placeholder.space_front = None
-        placeholder.space_back = None
+    if inlinemath:
+        for placeholder in placeholders_inline_math:
+            placeholder.content = placeholder.content.replace("\n", " ")
+            placeholder.content = re.sub(r"(\ +)", r" ", placeholder.content)
+            placeholder.space_front = None
+            placeholder.space_back = None
 
     # put ``\begin{...}``/ ``\end{...}`` and ``\[`` / ``\]`` on a newline
-    text, placeholders_let = text_to_placeholders(
-        text, [PlaceholderType.let_command, PlaceholderType.newif_command]
-    )
-    text = _begin_end_one_separate_line(text, placeholders_comments)
-    text = text_from_placeholders(text, placeholders_let)
+    if environment:
+        text, placeholders_let = text_to_placeholders(
+            text, [PlaceholderType.let_command, PlaceholderType.newif_command]
+        )
+        text = _begin_end_one_separate_line(text, placeholders_comments)
+        text = text_from_placeholders(text, placeholders_let)
 
     # \\ ends on line
-    text = re.sub(r"(?<!\\)(\\\\)(\ *\n?)", r"\1\n", text)
+    if linebreak:
+        text = re.sub(r"(?<!\\)(\\\\)(\ *\n?)", r"\1\n", text)
 
     # format tables: align if possible
-    text, placeholders_table = text_to_placeholders(text, [PlaceholderType.tabular])
-    for placeholder in placeholders_table:
-        placeholder.content = _align(placeholder.content)
-    text = text_from_placeholders(text, placeholders_table)
+    if alignment:
+        text, placeholders_table = text_to_placeholders(text, [PlaceholderType.tabular])
+        for placeholder in placeholders_table:
+            placeholder.content = _align(placeholder.content)
+        text = text_from_placeholders(text, placeholders_table)
 
     # apply one sentence per line
-    text, placeholders_ignore = text_to_placeholders(
-        text, [PlaceholderType.math, PlaceholderType.tabular]
-    )
-    text, placeholders_commands = text_to_placeholders(
-        text, [PlaceholderType.command_like], placeholders_comments=placeholders_comments
-    )
-    text = _one_sentence_per_line(text)
-    for placeholder in placeholders_commands:
-        placeholder.content = _format_command(placeholder.content, placeholders_comments)
-    text = text_from_placeholders(text, placeholders_ignore + placeholders_commands)
+    if sentence or argument:
+        assert lstrip
+        assert rstrip
+
+        text, placeholders_ignore = text_to_placeholders(
+            text, [PlaceholderType.math, PlaceholderType.tabular]
+        )
+        text, placeholders_commands = text_to_placeholders(
+            text, [PlaceholderType.command_like], placeholders_comments=placeholders_comments
+        )
+        if sentence:
+            text = _one_sentence_per_line(text)
+        if argument:
+            for pl in placeholders_commands:
+                pl.content = _format_command(pl.content, placeholders_comments, sentence)
+        text = text_from_placeholders(text, placeholders_ignore + placeholders_commands)
 
     # place placeholders where they belong to do indentation
     # thereafter they should not be repositioned
     text = text_from_placeholders(
         text, placeholders_noindent + placeholders_comments, keep_placeholders=True
     )
     for placeholder in placeholders_comments + placeholders_inline_math:
         placeholder.space_front = None
         placeholder.space_back = None
     placeholders = placeholders_noindent + placeholders_comments + placeholders_inline_math
 
-    # get line number of each character
-    lineno = np.empty(len(text), dtype=int)
-    i = 0
-    line = 0
-    for line, match in enumerate(re.finditer(r"\n", text)):
-        lineno[i : match.span()[0]] = line
-        i = match.span()[0]
-        lineno[i] = line
-        i += 1
-    lineno[i:] = line + 1
-    lineno = np.append(lineno, line + 2)
-
-    # initialize indentation level
-    indent_level = np.zeros(lineno[-1] + 1, dtype=int)
-
-    # add indentation to all lines between ``\begin{...}`` and ``\end{...}``
-    for env in environments(text) + [PlaceholderType.math]:
-        if env == PlaceholderType.math:
-            opening = r"\\\["
-            closing = r"\\\]"
-        elif env == "document":
-            continue
-        else:
-            opening = r"\\begin{" + env + r"}"
-            closing = r"\\end{" + env + r"}"
+    if indentation:
+        assert lstrip
+        assert environment
+        assert inlinemath
+
+        # get line number of each character
+        lineno = np.empty(len(text), dtype=int)
+        i = 0
+        line = 0
+        for line, match in enumerate(re.finditer(r"\n", text)):
+            lineno[i : match.span()[0]] = line
+            i = match.span()[0]
+            lineno[i] = line
+            i += 1
+        lineno[i:] = line + 1
+        lineno = np.append(lineno, line + 2)
+
+        # initialize indentation level
+        indent_level = np.zeros(lineno[-1] + 1, dtype=int)
+
+        # add indentation to all lines between ``\begin{...}`` and ``\end{...}``
+        for env in environments(text) + [PlaceholderType.math]:
+            if env == PlaceholderType.math:
+                opening = r"\\\["
+                closing = r"\\\]"
+            elif env == "document":
+                continue
+            else:
+                opening = r"\\begin{" + env + r"}"
+                closing = r"\\end{" + env + r"}"
+            indices = find_matching(
+                text,
+                opening,
+                closing,
+                escape=False,
+                opening_match=1,
+                closing_match=0,
+                ignore_escaped=True,
+            )
+            for opening, closing in indices.items():
+                indent_level[np.unique(lineno[opening:closing])[1:]] += 1
+
+        # add indentation to all lines between ``{`` and ``}`` containing at least one ``\n``
+        indices = find_matching(text, "{", "}", ignore_escaped=True, return_array=True)
+        for i in np.argwhere(lineno[indices[:, 0]] != lineno[indices[:, 1]]).ravel():
+            indent_level[lineno[indices[i, 0]] + 1 : lineno[indices[i, 1]]] += 1
+
+        # add indentation to all command options ``[`` and ``]`` containing at least one ``\n``
+        commands = find_command(text, is_comment=_is_placeholder(text, placeholders_comments))
+        indices = []
+        for command in commands:
+            if len(command) < 2:
+                continue
+            if text[command[1][0]] == "[":
+                indices += [command[1]]
+        indices = np.array(indices, dtype=int).reshape(-1, 2)
+        for i in np.argwhere(lineno[indices[:, 0]] != lineno[indices[:, 1]]).ravel():
+            indent_level[lineno[indices[i, 0]] + 1 : lineno[indices[i, 1]]] += 1
+
+        # add indentation for ``\if``, ``\else``, ``\fi``
         indices = find_matching(
             text,
-            opening,
-            closing,
+            r"(^|\n)(?<!\\)(\\if)([\@\w]*)(?=\n|$)",
+            r"(^|\n)(?<!\\)(\\fi)(?=\n|$)",
             escape=False,
             opening_match=1,
             closing_match=0,
             ignore_escaped=True,
         )
         for opening, closing in indices.items():
-            indent_level[np.unique(lineno[opening:closing])[1:]] += 1
-
-    # add indentation to all lines between ``{`` and ``}`` containing at least one ``\n``
-    indices = find_matching(text, "{", "}", ignore_escaped=True, return_array=True)
-    for i in np.argwhere(lineno[indices[:, 0]] != lineno[indices[:, 1]]).ravel():
-        indent_level[lineno[indices[i, 0]] + 1 : lineno[indices[i, 1]]] += 1
-
-    # add indentation to all command options ``[`` and ``]`` containing at least one ``\n``
-    commands = find_command(text, is_comment=_is_placeholder(text, placeholders_comments))
-    indices = []
-    for command in commands:
-        if len(command) < 2:
-            continue
-        if text[command[1][0]] == "[":
-            indices += [command[1]]
-    indices = np.array(indices, dtype=int).reshape(-1, 2)
-    for i in np.argwhere(lineno[indices[:, 0]] != lineno[indices[:, 1]]).ravel():
-        indent_level[lineno[indices[i, 0]] + 1 : lineno[indices[i, 1]]] += 1
-
-    # add indentation for ``\if``, ``\else``, ``\fi``
-    indices = find_matching(
-        text,
-        r"(^|\n)(?<!\\)(\\if)([\@\w]*)(?=\n|$)",
-        r"(^|\n)(?<!\\)(\\fi)(?=\n|$)",
-        escape=False,
-        opening_match=1,
-        closing_match=0,
-        ignore_escaped=True,
-    )
-    for opening, closing in indices.items():
-        indent_level[np.unique(lineno[opening - 1 : closing])[1:]] += 1
-    for match in re.finditer(r"(^|\n)(?<!\\)(\\else)(\n|$)", text):
-        indent_level[lineno[match.span(2)[0]]] -= 1
-
-    # apply indentation
-    text = text.splitlines()
-    for i in range(len(text)):
-        text[i] = indent_level[i] * indent + text[i]
-    text = "\n".join(text)
+            indent_level[np.unique(lineno[opening - 1 : closing])[1:]] += 1
+        for match in re.finditer(r"(^|\n)(?<!\\)(\\else)(\n|$)", text):
+            indent_level[lineno[match.span(2)[0]]] -= 1
+
+        # apply indentation
+        text = text.splitlines()
+        for i in range(len(text)):
+            text[i] = indent_level[i] * indentation + text[i]
+        text = "\n".join(text)
 
     text = text_from_placeholders(text, placeholders)
     return _rstrip_lines(text)
 
 
 def _detail_one_sentence_per_line(text: str) -> str:
     """
@@ -1566,14 +1722,15 @@
 
     return text_from_placeholders(ret, placeholders)
 
 
 def _format_command(
     text: str,
     placeholders_comments: list[Placeholder],
+    sentence: bool = True,
     level: int = 0,
 ) -> str:
     """
     Format a command.
     This function loops over all options and arguments and places them on a separate line if
     they contain at least one ``\n``.
     In that case :py:func:`_one_sentence_per_line` is applied to the option/argument.
@@ -1587,15 +1744,15 @@
 
         \foo[bar]{
             This is sentence.
         }
 
     :param text: Text.
     :param placeholders_comments: List of placeholders for comments.
-    :param ptype: Placeholder type.
+    :param sentence: Apply one sentence per line formatting.
     :param level: Level of nested-ness, used to define unique placeholder names.
     :return: Formatted text.
     """
     if not re.match(r".*\n.*", text):
         return text
 
     if text[0] == "{":
@@ -1627,20 +1784,22 @@
                 continue
             body = part[1:-1].strip()
             body, placeholders_cmd = text_to_placeholders(
                 body,
                 [PlaceholderType.command_like],
                 f"TEXONEPERLINE-L{level}",
             )
-            body = _one_sentence_per_line(body, [], command=True)
+            if sentence:
+                body = _one_sentence_per_line(body, [], command=True)
 
             for placeholder in placeholders_cmd:
                 placeholder.content = _format_command(
                     placeholder.content,
                     placeholders_comments,
+                    sentence,
                     level + 1,
                 )
             body = text_from_placeholders(body, placeholders_cmd)
             parts[i] = "\n".join([parts[i][0], body, parts[i][-1]])
 
     return "".join(parts)
 
@@ -1792,15 +1951,16 @@
     # ---
 
     return categories, np.where(classification < 0, categories.index("misc"), classification)
 
 
 class TeX:
     """
-    Simple TeX file manipulations.
+    Interpret TeX file to allow simple manipulations.
+    The manipulations are the member functions.
 
     :param text: LaTeX code.
     """
 
     def __init__(self, text: str):
         self.dirname = None
         self.filename = None
@@ -2092,34 +2252,46 @@
         if re.search(re.escape(cmd) + "{", test):
             return self._replace_command_impl(cmd, nargs, replace, ignore_commented)
 
     def replace_command(self, cmd: str, replace: str, ignore_commented: bool = False):
         r"""
         Replace command. For example:
 
-        *   Remove the command::
+        *   Remove the command:
+
+            .. code-block:: python
 
                 replace_command(r"{\TG}[1]", "")
 
-                    >>> This is a \TG{I would replace this} text.
-                    <<< This is a  text.
+            .. code-block:: none
 
-        *   Select a part of the command::
+                >>> This is a \TG{I would replace this} text.
+                <<< This is a  text.
+
+        *   Select a part of the command:
+
+            .. code-block:: python
 
                 replace_command(r"{\TG}[2]", "#1")
 
-                    >>> This is a \TG{text}{test}.
-                    <<< This is a test.
+            .. code-block:: none
+
+                >>> This is a \TG{text}{test}.
+                <<< This is a test.
+
+        *   Change the command:
 
-        *   Change the command::
+            .. code-block:: python
 
                 replace_command(r"{\TG}[2]", "\mycomment{#1}{#2}")
 
-                    >>> This is a \TG{text}{test}.
-                    <<< This is a \mycomment{text}{test}.
+            .. code-block:: none
+
+                >>> This is a \TG{text}{test}.
+                <<< This is a \mycomment{text}{test}.
 
         :param cmd:
             The command's definition. Given ``\newcommand{cmd}[args]{def}`` you should specify
             ``{cmd}[args]``, or ``{cmd}`` (or even ``cmd``) which defaults to ``{cmd}[1]``
 
         :param replace:
             The ``def`` part (curly braces around are optional). As in LaTeX replacement is
@@ -2373,22 +2545,26 @@
         formatter_class=argparse.RawTextHelpFormatter,
         description=textwrap.dedent(
             """\
             Apply some simple clean-up rules.
             Most of the options are fully self explanatory, except for:
 
             --replace-command
-                It can replace a command by another command, or simply 'remove' it,
-                keeping just a sequence of arguments.
+                Replace a command by another command.
+                This can also be 'removing' the command and keeping just a sequence of arguments.
                 This option is very much like a LaTeX command, but applied to the source.
-                For example::
+                For example:
+
+                .. code-block:: none
 
                     --replace-command "{\\TG}[2]" "#1"
 
-                Applied a change as follows::
+                Applies a change as follows:
+
+                .. code-block:: none
 
                     >>> This is a \\TG{text}{test}.
                     <<< This is a test.
 
                 Note that the number of arguments defaults to 1 (above ``[2]`` fixes 2 arguments).
                 Finally, commented text is ignored.
             """
@@ -2436,36 +2612,39 @@
         help='Automatically prepend labels with "fig:", "eq:", "tab:", "sec:", "ch:" (if needed).',
     )
 
     parser.add_argument(
         "-F",
         "--prepend-format-labels",
         type=str,
-        help='Automatically prepend labels with "fig:ARG", "eq:ARG", ...; see --format-labels.',
+        help='Add ARG to labels (e.g. "fig:ARG:...", "eq:ARG:..."; see ``--format-labels``).',
     )
 
     parser.add_argument(
         "-s",
         "--use-cleveref",
         action="store_true",
         help=r'Change "Fig.~\ref{...}" etc. to "\\cref{...}".',
     )
 
     parser.add_argument("-v", "--version", action="version", version=version)
-    parser.add_argument("files", nargs="+", type=str, help="TeX file")
+    parser.add_argument("files", nargs="+", type=str, help="TeX file(s) (changed in-place).")
 
     return parser
 
 
 def texcleanup(args: list[str]):
     """
     Command-line tool to copy to clean output directory, see ``--help``.
     """
 
     parser = _texcleanup_parser()
+    parser.description = re.sub(
+        r"(.*)(:\s*)(\.\. code-block:: none)(.*)", r"\1::\4", parser.description, re.MULTILINE
+    )
     args = parser.parse_args(args)
     assert all([os.path.isfile(file) for file in args.files])
 
     for file in args.files:
         tex = TeX.from_file(file)
 
         if args.remove_commentlines or args.remove_comments:
@@ -2505,37 +2684,37 @@
     Return parser for :py:func:`texplain`.
     """
 
     desc = "Create a clean output directory with only included files/citations."
     parser = argparse.ArgumentParser(description=desc)
     parser.add_argument("-c", "--keep-comments", action="store_true", help="Keep comments")
     parser.add_argument("-v", "--version", action="version", version=version)
-    parser.add_argument("input", type=str, help="TeX file")
-    parser.add_argument("outdir", type=str, help="Output directory")
+    parser.add_argument("file", type=str, help="Main TeX file.")
+    parser.add_argument("outdir", type=str, help="Output directory for formatted/included files.")
     return parser
 
 
 def texplain(args: list[str]):
     """
     Command-line tool to copy to clean output directory, see ``--help``.
     """
 
     parser = _texplain_parser()
     args = parser.parse_args(args)
 
-    if not os.path.isfile(args.input):
-        raise OSError(f'"{args.input:s}" does not exist')
+    if not os.path.isfile(args.file):
+        raise OSError(f'"{args.file:s}" does not exist')
 
     if os.path.isdir(args.outdir):
         if os.listdir(args.outdir):
             raise OSError(f'"{args.outdir:s}" is not empty, provide a new or empty directory')
     else:
         os.makedirs(args.outdir)
 
-    old = TeX.from_file(args.input)
+    old = TeX.from_file(args.file)
     new = deepcopy(old)
     new.dirname = args.outdir
 
     if not args.keep_comments:
         new.remove_commentlines()
         new.remove_comments()
 
@@ -2599,26 +2778,26 @@
 
 
 def _texindent_parser():
     """
     Return parser for :py:func:`texindent`.
     """
 
-    desc = "Wrapper around ``latexindent.pl`` with some additional rules. ``texplain.texindent``."
+    desc = "Indent code using :py:func:`texplain.indent`."
     parser = argparse.ArgumentParser(description=desc)
 
     parser.add_argument("-v", "--version", action="version", version=version)
-    parser.add_argument("files", nargs="+", type=str, help="TeX file")
+    parser.add_argument("files", nargs="+", type=str, help="TeX file(s) (changed in-place).")
 
     return parser
 
 
 def texindent_cli(args: list[str]):
     """
-    Wrapper around latexindent.pl, see ``--help``.
+    Indent TeX file, see ``--help``.
     """
 
     parser = _texindent_parser()
     args = parser.parse_args(args)
     assert all([os.path.isfile(file) for file in args.files])
 
     for filepath in args.files:
```

### Comparing `texplain-0.7.6/texplain.egg-info/PKG-INFO` & `texplain-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,55 @@
-Metadata-Version: 2.1
-Name: texplain
-Version: 0.7.6
-Summary: Create directory with TeX-file and only dependencies.
-Home-page: https://github.com/tdegeus/texplain
-Author: Tom de Geus
-Author-email: tom@geus.me
-License: MIT
-Keywords: LaTeX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![ci](https://github.com/tdegeus/texplain/workflows/CI/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![Documentation Status](https://readthedocs.org/projects/texplain/badge/?version=latest)](https://texplain.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://github.com/tdegeus/texplain/workflows/pre-commit/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/texplain.svg)](https://anaconda.org/conda-forge/texplain)
 
 **Documentation: [https://texplain.readthedocs.io](texplain.readthedocs.io)**
 
 # Usage
 
 ## command-line
 
+*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
+    Automatic indentation and formatting of a TeX-file.
+
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
     Apply any of the following options to a TeX-file:
 
     -   Remove all comments or comment-lines.
     -   Modify all occurrences of a command, for example to change `\TG{deleted}{inserted}` to `inserted`.
     -   Rename a label.
     -   Ensure common prefixes for all labels.
     -   Ensure usage of `\cref` instead of `\ref`.
 
-*   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
-    Wrapper around [latexindent.pl](https://github.com/cmhughes/latexindent.pl) with augmented rules to make especially `oneSentencePerLine` more robust.
-
 *   [texplain](https://texplain.readthedocs.io/en/latest/tools.html#texplain):
     Create a directory with a TeX-file and only its dependencies
     (those figure-files and references that are actually included).
     This is particularly useful to create a clean version to submit to a journal.
 
 ## pre-commit
 
 *   [texcleanup](https://texplain.readthedocs.io/en/latest/tools.html#texcleanup):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texcleanup
         args: [--format-labels, --use-cleveref]
     ```
 
 *   [texindent](https://texplain.readthedocs.io/en/latest/tools.html#texindent):
 
     ```yaml
     repos:
     - repo: https://github.com/tdegeus/texplain
-      rev: v0.7.0
+      rev: v0.8.0
       hooks:
       - id: texindent
         args: []
     ```
 
 ## Python
```

### Comparing `texplain-0.7.6/texplain.egg-info/SOURCES.txt` & `texplain-0.8.0/texplain.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 .github/workflows/pythonpublish.yml
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/module.rst
+docs/pre-commit.rst
 docs/tools.rst
 tests/__init__.py
 tests/test_align.py
 tests/test_classify.py
 tests/test_find_command.py
 tests/test_indent.py
 tests/test_indent_long.py
+tests/test_indent_options.py
+tests/test_indent_texindent.py
 tests/test_placeholders.py
 tests/test_simple.py
 tests/test_texplain_example1.py
 tests/input1/apalike.bst
 tests/input1/example.tex
 tests/input1/goose-article.cls
 tests/input1/refs.bib
```

