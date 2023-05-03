# Comparing `tmp/textdescriptives-2.6.0.tar.gz` & `tmp/textdescriptives-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.6.0.tar", last modified: Fri Apr 28 08:37:10 2023, max compression
+gzip compressed data, was "textdescriptives-2.6.1.tar", last modified: Wed May  3 07:18:23 2023, max compression
```

## Comparing `textdescriptives-2.6.0.tar` & `textdescriptives-2.6.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.759298 textdescriptives-2.6.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2254 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)     8145 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23971 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9640 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3548 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2784 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96689 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    17211 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/sklearn_integration.ipynb
--rw-r--r--   0 root         (0) root         (0)     7465 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     3074 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:37:10.759298 textdescriptives-2.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.739297 textdescriptives-2.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     7504 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5515 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22254 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10426 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6126 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/extractors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/src/textdescriptives/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/integrations/sklearn_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23971 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.860781 textdescriptives-2.6.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)     8642 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23729 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/readability.md
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    13090 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-03 07:18:13.000000 textdescriptives-2.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.860781 textdescriptives-2.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22254 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6126 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23729 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_utils.py
```

### Comparing `textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/dependabot.yml` & `textdescriptives-2.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.6.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/documentation.yml` & `textdescriptives-2.6.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/draft-pdf.yml` & `textdescriptives-2.6.1/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/release.yml` & `textdescriptives-2.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/stale.yml` & `textdescriptives-2.6.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.github/workflows/tests.yml` & `textdescriptives-2.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.gitignore` & `textdescriptives-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/.pre-commit-config.yaml` & `textdescriptives-2.6.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         #args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.262
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
```

### Comparing `textdescriptives-2.6.0/.zenodo.json` & `textdescriptives-2.6.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/CHANGELOG.md` & `textdescriptives-2.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.6.1 (2023-05-03)
+### Fix
+* Updated dev. dependencies to not include upper bounds ([`48bedec`](https://github.com/HLasse/TextDescriptives/commit/48bedecfb9565b23c1cb11f52b0fd414d2554d01))
+
+### Documentation
+* Removed error from notebook ([`708d9d7`](https://github.com/HLasse/TextDescriptives/commit/708d9d72ed9f90e9da2840261173c6d6609fff3e))
+* Added description of readability scores ([`16cda18`](https://github.com/HLasse/TextDescriptives/commit/16cda18ce2742fd403822387a14ac10d109d649f))
+
 ## v2.6.0 (2023-04-28)
 ### Feature
 * Add sklearn transformer ([`be733c6`](https://github.com/HLasse/TextDescriptives/commit/be733c6161993deb6e284475224d6363c99a8962))
 
 ### Documentation
 * Add sklearn to requirements in docs ([`33194c9`](https://github.com/HLasse/TextDescriptives/commit/33194c937803acdd2abb4198b97ead3981958fd1))
 * Minor docstring changes ([`375d3e0`](https://github.com/HLasse/TextDescriptives/commit/375d3e03a8792b54f5dfd6080e27ca34925628c3))
```

### Comparing `textdescriptives-2.6.0/CITATION.cff` & `textdescriptives-2.6.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/CODE_OF_CONDUCT.md` & `textdescriptives-2.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/CONTRIBUTING.md` & `textdescriptives-2.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/LICENSE` & `textdescriptives-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/PKG-INFO` & `textdescriptives-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.6.0
+Version: 2.6.1
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -236,19 +236,18 @@
 
 
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
-[![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
-A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
+A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
```

### Comparing `textdescriptives-2.6.0/README.md` & `textdescriptives-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
-[![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
-A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
+A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
```

#### html2text {}

```diff
@@ -1,35 +1,31 @@
  [https://github.com/HLasse/TextDescriptives/raw/main/docs/_static/icon.png] #
 TextDescriptives [![spacy](https://img.shields.io/badge/built%20with-spaCy-
 09a3d5.svg)](https://spacy.io) [![github actions pytest](https://github.com/
 hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://
 github.com/hlasse/textdescriptives/actions) [![github actions docs](https://
 github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/
-badge.svg)](https://hlasse.github.io/TextDescriptives/) [![arXiv](https://
-img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/
-2301.02057) [![status](https://joss.theoj.org/papers/
-06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/
-06447337ee61969b5a64de484199df24) [![Open in Streamlit](https://
-static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://
+badge.svg)](https://hlasse.github.io/TextDescriptives/) [![status](https://
+joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://
+joss.theoj.org/papers/06447337ee61969b5a64de484199df24) [![Open in Streamlit]
+(https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://
 huggingface.co/spaces/HLasse/textdescriptives) A Python library for calculating
 a large variety of metrics from text(s) using spaCy v.3 pipeline components and
-extensions. TextDescriptives can be used to calculate several descriptive
-statistics, readability metrics, and metrics related to dependency distance. #
-ð§ Installation `pip install textdescriptives` # ð° News * We now have a
-TextDescriptives-powered web-app so you can extract and downloads metrics
-without a single line of code! Check it out [here](https://huggingface.co/
-spaces/HLasse/textdescriptives) * Version 2.0 out with a new API, a new
-component, updated documentation, and tutorials! Components are now called by
-"`textdescriptives/{metric_name}`. New `coherence` component for calculating
-the semantic coherence between sentences. See the [documentation](https://
-github.com/HLasse/TextDescriptives) for tutorials and more information! # â¡
-Quick Start Use `extract_metrics` to quickly extract your desired metrics. To
-see available methods you can simply run: ```python import textdescriptives as
-td td.get_valid_metrics() # {'quality', 'readability', 'all',
-'descriptive_stats', 'dependency_distance', 'pos_proportions',
+extensions. # ð§ Installation `pip install textdescriptives` # ð° News * We
+now have a TextDescriptives-powered web-app so you can extract and downloads
+metrics without a single line of code! Check it out [here](https://
+huggingface.co/spaces/HLasse/textdescriptives) * Version 2.0 out with a new
+API, a new component, updated documentation, and tutorials! Components are now
+called by "`textdescriptives/{metric_name}`. New `coherence` component for
+calculating the semantic coherence between sentences. See the [documentation]
+(https://github.com/HLasse/TextDescriptives) for tutorials and more
+information! # â¡ Quick Start Use `extract_metrics` to quickly extract your
+desired metrics. To see available methods you can simply run: ```python import
+textdescriptives as td td.get_valid_metrics() # {'quality', 'readability',
+'all', 'descriptive_stats', 'dependency_distance', 'pos_proportions',
 'information_theory', 'coherence'} ``` Set the `spacy_model` parameter to
 specify which spaCy model to use, otherwise, TextDescriptives will auto-
 download an appropriate one based on `lang`. If `lang` is set, `spacy_model` is
 not necessary and vice versa. Specify which metrics to extract in the `metrics`
 argument. `None` extracts all metrics. ```py import textdescriptives as td text
 = "The world is changed. I feel it in the water. I feel it in the earth. I
 smell it in the air. Much that once was is lost, for none now live who remember
```

### Comparing `textdescriptives-2.6.0/docs/Makefile` & `textdescriptives-2.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/_static/icon.png` & `textdescriptives-2.6.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/_static/icon_dark_old.png` & `textdescriptives-2.6.1/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/_static/icon_old.png` & `textdescriptives-2.6.1/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/coherence.rst` & `textdescriptives-2.6.1/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/conf.py` & `textdescriptives-2.6.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 html_show_sourcelink = True
 
-source_suffix = {".rst": "restructuredtext", ".md": "markdown", ".ipynb": "myst-nb"}
+source_suffix = {".rst": "restructuredtext", ".md": "myst-nb", ".ipynb": "myst-nb"}
 
 html_context = {
     "display_github": True,  # Add 'Edit on Github' link instead of 'View page source'
     "github_user": "HLasse",
     "github_repo": project,
     "github_version": "main",
     "conf_py_path": "/docs/",
```

### Comparing `textdescriptives-2.6.0/docs/dependencydistance.rst` & `textdescriptives-2.6.1/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/descriptivestats.rst` & `textdescriptives-2.6.1/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/faq.rst` & `textdescriptives-2.6.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/index.rst` & `textdescriptives-2.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/information_theory.rst` & `textdescriptives-2.6.1/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/installation.rst` & `textdescriptives-2.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/make.bat` & `textdescriptives-2.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/news.rst` & `textdescriptives-2.6.1/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/posstats.rst` & `textdescriptives-2.6.1/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/quality.rst` & `textdescriptives-2.6.1/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.6.1/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.6.1/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/docs/usingthepackage.rst` & `textdescriptives-2.6.1/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/paper/paper.bib` & `textdescriptives-2.6.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/paper/paper.md` & `textdescriptives-2.6.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/paper/paper_quarto.pdf` & `textdescriptives-2.6.1/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/paper/paper_quarto.qmd` & `textdescriptives-2.6.1/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/pyproject.toml` & `textdescriptives-2.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.6.0"
+version = "2.6.1"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"},
              {name = "Kenneth Enevoldsen"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -45,37 +45,38 @@
 homepage = "https://hlasse.github.io/TextDescriptives/"
 repository = "https://github.com/HLasse/textdescriptives"
 documentation = "https://hlasse.github.io/TextDescriptives/"
 
 [project.optional-dependencies]
 style = [
     "black==23.3.0",
-    "pre-commit==3.1.1",
-    "ruff==0.0.260",
+    "pre-commit==3.2.2",
+    "ruff==0.0.263",
     "mypy==1.1.1"
 ]
 tests = [
-    "pytest>=7.1.3,<7.3.0",
-    "pytest-cov>=3.0.0,<3.0.1",
+    "pytest>=7.1.3",
+    "pytest-cov>=3.0.0",
 ]
 docs = [
-    "sphinx>=5.3.0,<6.2.0",
-    "furo==2023.3.27",
-    "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.8.2",
-    "myst-nb>=0.6.0,<1.17.0",
-    "sphinx_design>=0.3.0,<0.3.1",
-    "autodoc_pydantic>=1.1.0,<1.9.0",
+    "sphinx>=5.3.0",
+    "furo>=2023.3.27",
+    "sphinx-copybutton>=0.5.1",
+    "sphinxext-opengraph>=0.7.3",
+    "myst-nb>=0.6.0",
+    "sphinx_design>=0.3.0",
+    "autodoc_pydantic>=1.1.0",
 ]
 tutorials = [
     "jupyter",
     "seaborn",
     "matplotlib",
     "datasets>=2.8.0",
     "scikit-learn>=1.1.1",
+    "ipython<=8.12",
 ]
 sklearn = [
     "scikit-learn>=1.1.1",
 ]
 
 [project.readme]
 file = "README.md"
```

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/coherence.py` & `textdescriptives-2.6.1/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.6.1/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.6.1/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.6.1/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.6.1/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/quality.py` & `textdescriptives-2.6.1/src/textdescriptives/components/quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.6.1/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/readability.py` & `textdescriptives-2.6.1/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/components/utils.py` & `textdescriptives-2.6.1/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/data/spam.csv` & `textdescriptives-2.6.1/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/extractors.py` & `textdescriptives-2.6.1/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/integrations/sklearn_featurizer.py` & `textdescriptives-2.6.1/src/textdescriptives/integrations/sklearn_featurizer.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/load_components.py` & `textdescriptives-2.6.1/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives/utils.py` & `textdescriptives-2.6.1/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.6.1/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.6.0
+Version: 2.6.1
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -236,19 +236,18 @@
 
 
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
-[![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
-A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
+A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
 * We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
```

### Comparing `textdescriptives-2.6.0/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.6.1/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 docs/index.rst
 docs/information_theory.rst
 docs/installation.rst
 docs/make.bat
 docs/news.rst
 docs/posstats.rst
 docs/quality.rst
-docs/readability.rst
+docs/readability.md
 docs/tutorial.rst
 docs/usingthepackage.rst
 docs/_static/icon.png
 docs/_static/icon_dark_old.png
 docs/_static/icon_old.png
 docs/tutorials/filter_corpus_using_quality.ipynb
 docs/tutorials/introductory_tutorial.ipynb
```

### Comparing `textdescriptives-2.6.0/tests/books.py` & `textdescriptives-2.6.1/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_coherence.py` & `textdescriptives-2.6.1/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_dependency_distance.py` & `textdescriptives-2.6.1/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_descriptive_stats.py` & `textdescriptives-2.6.1/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_extractors.py` & `textdescriptives-2.6.1/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_information.py` & `textdescriptives-2.6.1/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_load_components.py` & `textdescriptives-2.6.1/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_pos_proportions.py` & `textdescriptives-2.6.1/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_quality.py` & `textdescriptives-2.6.1/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_readability.py` & `textdescriptives-2.6.1/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.0/tests/test_utils.py` & `textdescriptives-2.6.1/tests/test_utils.py`

 * *Files identical despite different names*

