# Comparing `tmp/types-docutils-0.19.1.8.tar.gz` & `tmp/types-docutils-0.19.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docutils-0.19.1.8.tar", last modified: Sat Apr 29 15:14:09 2023, max compression
+gzip compressed data, was "types-docutils-0.19.1.9.tar", last modified: Wed May  3 12:29:52 2023, max compression
```

## Comparing `types-docutils-0.19.1.8.tar` & `types-docutils-0.19.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/docutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/examples.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/frontend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/io.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/nodes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/recommonmark_wrapper.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/admonitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/body.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/images.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/parts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/references.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/states.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/doctree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/pep.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/standalone.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/statemachine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/transforms/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/docutils_xml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/html4css1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/html5_polyglot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/latex2e.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/manpage.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/odf_odt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/pep_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/pseudoxml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/s5_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/xetex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/types_docutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/docutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/examples.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/frontend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/io.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/nodes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/recommonmark_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/admonitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/parts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/references.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/states.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/doctree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/pep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/standalone.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/statemachine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/transforms/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/docutils_xml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/html4css1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/html5_polyglot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/latex2e.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/manpage.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/odf_odt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/pep_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/pseudoxml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/s5_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/xetex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/types_docutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/top_level.txt
```

### Comparing `types-docutils-0.19.1.8/CHANGELOG.md` & `types-docutils-0.19.1.9/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 0.19.1.9 (2023-05-03)
+
+[docutils] Add items to docutils.node (#10102)
+
+* Add class paragraph
+* Add class TextElement
+* Add Element.index(), .remove(), and .insert()
+
 ## 0.19.1.8 (2023-04-29)
 
 docutils: Input can take bytearray (#10108)
 
 Part of #9006
 
 docutils: add nodes.General; make Element iterable (#10099)
```

### Comparing `types-docutils-0.19.1.8/PKG-INFO` & `types-docutils-0.19.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.8
+Version: 0.19.1.9
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
```

### Comparing `types-docutils-0.19.1.8/docutils-stubs/__init__.pyi` & `types-docutils-0.19.1.9/docutils-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/frontend.pyi` & `types-docutils-0.19.1.9/docutils-stubs/frontend.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/io.pyi` & `types-docutils-0.19.1.9/docutils-stubs/io.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/nodes.pyi` & `types-docutils-0.19.1.9/docutils-stubs/nodes.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import sys
 import xml.dom.minidom
 from _typeshed import Incomplete
 from abc import abstractmethod
 from collections.abc import Callable, Generator, Iterable, Iterator, Sequence
 from typing import Any, ClassVar, Protocol, TypeVar, overload
-from typing_extensions import Literal, Self
+from typing_extensions import Literal, Self, SupportsIndex
 
 from docutils.transforms import Transformer
 
 _N = TypeVar("_N", bound=Node)
 
 class _DomModule(Protocol):
     Document: type[xml.dom.minidom.Document]
@@ -75,14 +76,15 @@
         siblings: bool = False,
         ascend: bool = False,
     ) -> Node: ...
     def previous_sibling(self) -> Node | None: ...
 
 class Element(Node):
     children: list[Node]
+    rawsource: str
     def __init__(self, rawsource: str = "", *children: Node, **attributes): ...
     def __len__(self) -> int: ...
     def __contains__(self, key: str | Node) -> bool: ...
     # '__iter__' is added as workaround, since mypy doesn't support classes that are iterable via '__getitem__'
     # see https://github.com/python/typeshed/pull/10099#issuecomment-1528789395
     def __iter__(self) -> Iterator[Node]: ...
     @overload
@@ -101,16 +103,22 @@
     def __add__(self, other: list[Node]) -> list[Node]: ...
     def __radd__(self, other: list[Node]) -> list[Node]: ...
     def __iadd__(self, other: Node | Iterable[Node]) -> Self: ...
     def copy(self) -> Self: ...
     def deepcopy(self) -> Self: ...
     def pformat(self, indent: str = "    ", level: int = 0) -> str: ...
     def astext(self) -> str: ...
+    def index(self, item: Node, start: int = 0, stop: int = sys.maxsize) -> int: ...
+    def remove(self, item: Node) -> None: ...
+    def insert(self, index: SupportsIndex, item: Node | Iterable[Node] | None) -> None: ...
     def __getattr__(self, __name: str) -> Incomplete: ...
 
+class TextElement(Element):
+    def __init__(self, rawsource: str = "", text: str = "", *children: Node, **attributes) -> None: ...
+
 class Text(Node, str):
     tagname: ClassVar[str]
     children: tuple[()]
 
     # we omit the rawsource parameter because it has been deprecated and is ignored
     def __new__(cls, data: str) -> Self: ...
     def __init__(self, data: str) -> None: ...
@@ -131,12 +139,14 @@
     transformer: Transformer
     def copy(self) -> Self: ...
     def deepcopy(self) -> Self: ...
     def pformat(self, indent: str = "    ", level: int = 0) -> str: ...
     def astext(self) -> str: ...
     def __getattr__(self, __name: str) -> Incomplete: ...
 
+class paragraph(General, TextElement): ...
+
 class NodeVisitor:
     def __init__(self, document: document): ...
     def __getattr__(self, __name: str) -> Incomplete: ...
 
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-docutils-0.19.1.8/docutils-stubs/parsers/__init__.pyi` & `types-docutils-0.19.1.9/docutils-stubs/parsers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/parsers/rst/__init__.pyi` & `types-docutils-0.19.1.9/docutils-stubs/parsers/rst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/parsers/rst/roles.pyi` & `types-docutils-0.19.1.9/docutils-stubs/parsers/rst/roles.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/transforms/__init__.pyi` & `types-docutils-0.19.1.9/docutils-stubs/transforms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/docutils-stubs/utils/__init__.pyi` & `types-docutils-0.19.1.9/docutils-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.8/setup.py` & `types-docutils-0.19.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.19.1.8",
+      version="0.19.1.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md",
```

### Comparing `types-docutils-0.19.1.8/types_docutils.egg-info/PKG-INFO` & `types-docutils-0.19.1.9/types_docutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.8
+Version: 0.19.1.9
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
```

### Comparing `types-docutils-0.19.1.8/types_docutils.egg-info/SOURCES.txt` & `types-docutils-0.19.1.9/types_docutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

