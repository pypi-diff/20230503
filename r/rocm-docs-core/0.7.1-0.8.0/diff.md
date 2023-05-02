# Comparing `tmp/rocm-docs-core-0.7.1.tar.gz` & `tmp/rocm-docs-core-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm-docs-core-0.7.1.tar", last modified: Wed Apr 26 17:05:25 2023, max compression
+gzip compressed data, was "rocm-docs-core-0.8.0.tar", last modified: Tue May  2 21:56:15 2023, max compression
```

## Comparing `rocm-docs-core-0.7.1.tar` & `rocm-docs-core-0.8.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.354876 rocm-docs-core-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-26 17:05:25.354876 rocm-docs-core-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:05:25.358876 rocm-docs-core-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.326876 rocm-docs-core-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.330876 rocm-docs-core-0.7.1/src/rocm_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.326876 rocm-docs-core-0.7.1/src/rocm_docs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.330876 rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/
--rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/doxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.330876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.334876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/article-info.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/social-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.334876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.334876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.326876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.354876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.354876 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-26 17:05:07.000000 rocm-docs-core-0.7.1/src/rocm_docs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:05:25.354876 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 17:05:25.000000 rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.793553 rocm-docs-core-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.797554 rocm-docs-core-0.8.0/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.793553 rocm-docs-core-0.8.0/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.797554 rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/doxygen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.797554 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.797554 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/article-info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/social-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.801554 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.801554 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.793553 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-02 21:56:00.000000 rocm-docs-core-0.8.0/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:15.813555 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 21:56:15.000000 rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/top_level.txt
```

### Comparing `rocm-docs-core-0.7.1/LICENSE.txt` & `rocm-docs-core-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/PKG-INFO` & `rocm-docs-core-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.7.1
+Version: 0.8.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm-docs-core-0.7.1/README.md` & `rocm-docs-core-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/pyproject.toml` & `rocm-docs-core-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,64 +3,63 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'rocm-docs-core'
-version = "0.7.1"
+version = "0.8.0"
 authors=[
   {name="Lauren Wrubleski", email="Lauren.Wrubleski@amd.com"}
 ]
 description ='Core utilities for all ROCm documentation on RTD'
 readme="README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent"
 ]
 dependencies = [
-  "GitPython>=3.1.30,<3.2",
-  'importlib_resources>=5.10.2,<5.11;python_version<"3.9"',
+  "GitPython>=3.1.30",
+  'importlib_resources>=5.10.2;python_version<"3.9"',
   "PyGithub>=1.58.1",
-  "docutils>=0.18.1",
   "sphinx>=5.3.0",
-  "breathe==4.34.0",
-  "sphinx-design==0.4.1",
-  "sphinx-copybutton==0.5.1",
-  "sphinx_external_toc==0.3.1",
+  "breathe>=4.34.0",
+  "sphinx-design>=0.3.0",
+  "sphinx-copybutton>=0.5.1",
+  "sphinx_external_toc>=0.3.1",
   "sphinx-book-theme>=1.0.1",
-  "myst_nb==0.17.1",
-  "myst-parser[linkify]==0.18.1",
-  "sphinx-notfound-page==0.8.3",
-  "pydata-sphinx-theme>=0.13.3,<14"
+  "myst_nb>=0.17.1",
+  "myst-parser[linkify]>=0.18.1",
+  "sphinx-notfound-page>=0.8.3",
+  "pydata-sphinx-theme>=0.13.3"
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 repository="https://github.com/RadeonOpenCompute/rocm-docs-core"
 documentation="https://docs.amd.com"
 
 [project.optional-dependencies]
 api_reference = [
-  "doxysphinx>=3.2.1,<4"
+  "doxysphinx>=3.2.1,!=3.3.0,!=3.3.1"
 ]
 development = [
-  "commitizen>=2.42,<3"
+  "commitizen>=2.42"
 ]
 
 [project.entry-points."sphinx.html_themes"]
 rocm_docs_theme = "rocm_docs.theme"
 
 [tool.setuptools.packages.find]
 where=["src"]
 
 [tool.setuptools.package-data]
 rocm_docs = ["data/**/*", "rocm_docs_theme/**/*"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.1"
+version = "0.8.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 annotated_tag = true
 major_version_zero = true
```

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/__init__.py` & `rocm-docs-core-0.8.0/src/rocm_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/core.py` & `rocm-docs-core-0.8.0/src/rocm_docs/core.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/header.html` & `rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm-docs-core-0.8.0/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/doxygen.py` & `rocm-docs-core-0.8.0/src/rocm_docs/doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/article-info.html` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/article-info.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/components/social-links.html` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/components/social-links.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div class="rocm-footer">
     {%- include "components/social-links.html" with context -%}
     <div class="rocm-footer-links">
         <ul>
             <li><a href="https://www.amd.com/en/corporate/copyright" target="_blank">Terms and Conditions</a></li>
-            <li><a href="https://rocmdocs.amd.com/projects/alpha/en/develop/release/licensing.html">ROCm Licenses and Disclaimers</a></li>
+            <li><a href="https://rocm.docs.amd.com/en/latest/release/licensing.html">ROCm Licenses and Disclaimers</a></li>
             <li><a href="https://www.amd.com/en/corporate/privacy" target="_blank">Privacy</a></li>
             <li><a href="https://www.amd.com/en/corporate/trademarks" target="_blank">Trademarks</a></li>
             <li><a href="https://www.amd.com/system/files/documents/statement-human-trafficking-forced-labor.pdf" target="_blank">Statement on Forced Labor</a></li>
             <li><a href="https://www.amd.com/en/corporate/competition" target="_blank">Fair and Open Competition</a></li>
             <li><a href="https://www.amd.com/system/files/documents/amd-uk-tax-strategy.pdf" target="_blank">UK Tax Strategy</a></li>
             <li><a href="https://www.amd.com/en/corporate/cookies" target="_blank">Cookie Policy</a></li>
             <!-- OneTrust Cookies Settings button start -->
```

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/sections/header.html` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/custom.css` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/custom.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css` & `rocm-docs-core-0.8.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/theme.py` & `rocm-docs-core-0.8.0/src/rocm_docs/theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 def setup(app: Sphinx) -> Dict[str, Any]:
     app.add_js_file(
         "https://download.amd.com/js/analytics/analyticsinit.js",
         priority=999_999,
         loading_method="async",
     )
     app.add_js_file("code_word_breaks.js", loading_method="async")
+    app.add_js_file("renameVersionLinks.js", loading_method="async")
     here = Path(__file__).parent.resolve()
     theme_path = here / "rocm_docs_theme"
     app.add_html_theme("rocm_docs_theme", str(theme_path))
     for css in [
         "custom.css",
         "rocm_header.css",
         "rocm_footer.css",
```

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs/util.py` & `rocm-docs-core-0.8.0/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.7.1
+Version: 0.8.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm-docs-core-0.7.1/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm-docs-core-0.8.0/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/rocm_docs/rocm_docs_theme/sections/footer.html
 src/rocm_docs/rocm_docs_theme/sections/header.html
 src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
 src/rocm_docs/rocm_docs_theme/static/custom.css
 src/rocm_docs/rocm_docs_theme/static/fonts.css
 src/rocm_docs/rocm_docs_theme/static/fonts.css.map
 src/rocm_docs/rocm_docs_theme/static/fonts.scss
+src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
 src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
 src/rocm_docs/rocm_docs_theme/static/rocm_header.css
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
```

