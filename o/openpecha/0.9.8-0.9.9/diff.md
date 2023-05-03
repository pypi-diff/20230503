# Comparing `tmp/openpecha-0.9.8.tar.gz` & `tmp/openpecha-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpecha-0.9.8.tar", last modified: Mon Nov  7 09:41:36 2022, max compression
+gzip compressed data, was "openpecha-0.9.9.tar", last modified: Tue Nov 22 08:35:35 2022, max compression
```

## Comparing `openpecha-0.9.8.tar` & `openpecha-0.9.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.928547 openpecha-0.9.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-07 09:41:33.000000 openpecha-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3150 2022-11-07 09:41:36.928547 openpecha-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2725 2022-11-07 09:41:33.000000 openpecha-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.912546 openpecha-0.9.8/openpecha/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-07 09:41:34.000000 openpecha-0.9.8/openpecha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.912546 openpecha-0.9.8/openpecha/alignment/
--rw-r--r--   0 root         (0) root         (0)     3399 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.912546 openpecha-0.9.8/openpecha/alignment/exporter/
--rw-r--r--   0 root         (0) root         (0)     2800 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/exporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/exporter/bitext.py
--rw-r--r--   0 root         (0) root         (0)     3064 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/exporter/po.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.916547 openpecha-0.9.8/openpecha/alignment/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12702 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/integrations/tx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.916547 openpecha-0.9.8/openpecha/alignment/parsers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4173 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/parsers/po.py
--rw-r--r--   0 root         (0) root         (0)     2135 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/parsers/tmx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.916547 openpecha-0.9.8/openpecha/alignment/segmenters/
--rw-r--r--   0 root         (0) root         (0)       75 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/segmenters/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/segmenters/basic.py
--rw-r--r--   0 root         (0) root         (0)      587 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/segmenters/sentence.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/segmenters/tmx.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/segmenters/transfer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.916547 openpecha-0.9.8/openpecha/alignment/tmx/
--rw-r--r--   0 root         (0) root         (0)     7810 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/tmx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5607 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/tmx/create_opf.py
--rw-r--r--   0 root         (0) root         (0)     3291 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/alignment/tmx/translated_po_to_opf.py
--rw-r--r--   0 root         (0) root         (0)    12366 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/blupdate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.916547 openpecha-0.9.8/openpecha/buda/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/buda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7365 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/buda/api.py
--rw-r--r--   0 root         (0) root         (0)     2893 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/buda/chunker.py
--rw-r--r--   0 root         (0) root         (0)      267 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/buda/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/catalog/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      128 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/config.py
--rw-r--r--   0 root         (0) root         (0)      968 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/filter.py
--rw-r--r--   0 root         (0) root         (0)     3866 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/manager.py
--rw-r--r--   0 root         (0) root         (0)     2374 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/storage.py
--rw-r--r--   0 root         (0) root         (0)      120 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/catalog/utils.py
--rw-r--r--   0 root         (0) root         (0)     8833 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/collated/
--rw-r--r--   0 root         (0) root         (0)      159 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collated/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collated/base.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collated/diffs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/collection/
--rw-r--r--   0 root         (0) root         (0)      173 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collection/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/collection/import/
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collection/import/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/collection/import/plugins/
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/collection/import/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      524 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/annotation.py
--rw-r--r--   0 root         (0) root         (0)     2110 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/annotations.py
--rw-r--r--   0 root         (0) root         (0)      654 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/ids.py
--rw-r--r--   0 root         (0) root         (0)     4451 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/layer.py
--rw-r--r--   0 root         (0) root         (0)     3109 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/metadata.py
--rw-r--r--   0 root         (0) root         (0)    16753 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/core/pecha.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.920547 openpecha-0.9.8/openpecha/corpus/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/corpus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/corpus/download.py
--rw-r--r--   0 root         (0) root         (0)     1493 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/corpus/quality.py
--rw-r--r--   0 root         (0) root         (0)       41 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.924547 openpecha-0.9.8/openpecha/formatters/
--rw-r--r--   0 root         (0) root         (0)      212 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6493 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/editor.py
--rw-r--r--   0 root         (0) root         (0)     1588 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/empty.py
--rw-r--r--   0 root         (0) root         (0)    12636 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/formatter.py
--rw-r--r--   0 root         (0) root         (0)    50014 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/hfml.py
--rw-r--r--   0 root         (0) root         (0)     4437 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/layers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.924547 openpecha-0.9.8/openpecha/formatters/ocr/
--rw-r--r--   0 root         (0) root         (0)      133 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8835 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/ocr/google_vision.py
--rw-r--r--   0 root         (0) root         (0)    10911 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/ocr/hocr.py
--rw-r--r--   0 root         (0) root         (0)    28306 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/ocr/ocr.py
--rw-r--r--   0 root         (0) root         (0)     7409 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/pedurma.py
--rw-r--r--   0 root         (0) root         (0)    23766 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/formatters/tsadra.py
--rw-r--r--   0 root         (0) root         (0)     6677 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/github_utils.py
--rw-r--r--   0 root         (0) root         (0)    12705 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/proofreading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.928547 openpecha-0.9.8/openpecha/serializers/
--rw-r--r--   0 root         (0) root         (0)      210 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14918 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/docx.py
--rw-r--r--   0 root         (0) root         (0)     9498 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/editor.py
--rw-r--r--   0 root         (0) root         (0)    25181 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/epub.py
--rw-r--r--   0 root         (0) root         (0)     4632 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/hfml.py
--rw-r--r--   0 root         (0) root         (0)     5746 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/pedurma.py
--rw-r--r--   0 root         (0) root         (0)    12435 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/rdf.py
--rw-r--r--   0 root         (0) root         (0)    13902 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     5882 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/storages.py
--rw-r--r--   0 root         (0) root         (0)     5764 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.928547 openpecha-0.9.8/openpecha/work/
--rw-r--r--   0 root         (0) root         (0)     3817 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2684 2022-11-07 09:41:33.000000 openpecha-0.9.8/openpecha/work/bdrc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 09:41:36.912546 openpecha-0.9.8/openpecha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3150 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2610 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      420 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-07 09:41:36.000000 openpecha-0.9.8/openpecha.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      457 2022-11-07 09:41:36.928547 openpecha-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1806 2022-11-07 09:41:33.000000 openpecha-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.485978 openpecha-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-22 08:35:32.000000 openpecha-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3150 2022-11-22 08:35:35.485978 openpecha-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2725 2022-11-22 08:35:32.000000 openpecha-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.469977 openpecha-0.9.9/openpecha/
+-rw-r--r--   0 root         (0) root         (0)       61 2022-11-22 08:35:33.000000 openpecha-0.9.9/openpecha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.469977 openpecha-0.9.9/openpecha/alignment/
+-rw-r--r--   0 root         (0) root         (0)     3399 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.469977 openpecha-0.9.9/openpecha/alignment/exporter/
+-rw-r--r--   0 root         (0) root         (0)     2800 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/exporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/exporter/bitext.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/exporter/po.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.469977 openpecha-0.9.9/openpecha/alignment/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12702 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/integrations/tx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.473977 openpecha-0.9.9/openpecha/alignment/parsers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/parsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/parsers/po.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/parsers/tmx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.473977 openpecha-0.9.9/openpecha/alignment/segmenters/
+-rw-r--r--   0 root         (0) root         (0)       75 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/segmenters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/segmenters/basic.py
+-rw-r--r--   0 root         (0) root         (0)      587 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/segmenters/sentence.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/segmenters/tmx.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/segmenters/transfer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.473977 openpecha-0.9.9/openpecha/alignment/tmx/
+-rw-r--r--   0 root         (0) root         (0)     7810 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/tmx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5607 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/tmx/create_opf.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/alignment/tmx/translated_po_to_opf.py
+-rw-r--r--   0 root         (0) root         (0)    12366 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/blupdate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.473977 openpecha-0.9.9/openpecha/buda/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/buda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/buda/api.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/buda/chunker.py
+-rw-r--r--   0 root         (0) root         (0)      267 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/buda/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/catalog/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      128 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/config.py
+-rw-r--r--   0 root         (0) root         (0)      968 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/manager.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/storage.py
+-rw-r--r--   0 root         (0) root         (0)      120 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/catalog/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/collated/
+-rw-r--r--   0 root         (0) root         (0)      159 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collated/base.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collated/diffs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/collection/
+-rw-r--r--   0 root         (0) root         (0)      173 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collection/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/collection/import/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collection/import/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/collection/import/plugins/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/collection/import/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      524 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.477978 openpecha-0.9.9/openpecha/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/annotation.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/annotations.py
+-rw-r--r--   0 root         (0) root         (0)      654 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/ids.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/layer.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    16753 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/core/pecha.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.481978 openpecha-0.9.9/openpecha/corpus/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/corpus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/corpus/download.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/corpus/quality.py
+-rw-r--r--   0 root         (0) root         (0)       41 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.481978 openpecha-0.9.9/openpecha/formatters/
+-rw-r--r--   0 root         (0) root         (0)      212 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6493 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/editor.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/empty.py
+-rw-r--r--   0 root         (0) root         (0)    12636 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/formatter.py
+-rw-r--r--   0 root         (0) root         (0)    50014 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/hfml.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.481978 openpecha-0.9.9/openpecha/formatters/ocr/
+-rw-r--r--   0 root         (0) root         (0)      133 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/ocr/google_vision.py
+-rw-r--r--   0 root         (0) root         (0)    10911 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/ocr/hocr.py
+-rw-r--r--   0 root         (0) root         (0)    28306 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/ocr/ocr.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/pedurma.py
+-rw-r--r--   0 root         (0) root         (0)    23766 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/formatters/tsadra.py
+-rw-r--r--   0 root         (0) root         (0)     6677 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/github_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12705 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/proofreading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.485978 openpecha-0.9.9/openpecha/serializers/
+-rw-r--r--   0 root         (0) root         (0)      210 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/docx.py
+-rw-r--r--   0 root         (0) root         (0)     9498 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/editor.py
+-rw-r--r--   0 root         (0) root         (0)    25181 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/epub.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/hfml.py
+-rw-r--r--   0 root         (0) root         (0)     5746 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/pedurma.py
+-rw-r--r--   0 root         (0) root         (0)    12435 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/rdf.py
+-rw-r--r--   0 root         (0) root         (0)    13902 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/storages.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.485978 openpecha-0.9.9/openpecha/work/
+-rw-r--r--   0 root         (0) root         (0)     3817 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2022-11-22 08:35:32.000000 openpecha-0.9.9/openpecha/work/bdrc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 08:35:35.469977 openpecha-0.9.9/openpecha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3150 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      420 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-11-22 08:35:35.000000 openpecha-0.9.9/openpecha.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2022-11-22 08:35:35.485978 openpecha-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1806 2022-11-22 08:35:32.000000 openpecha-0.9.9/setup.py
```

### Comparing `openpecha-0.9.8/LICENSE` & `openpecha-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/PKG-INFO` & `openpecha-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpecha
-Version: 0.9.8
+Version: 0.9.9
 Summary: OpenPecha Toolkit allows state of the art for distributed standoff annotations on moving texts
 Home-page: https://github.com/OpenPoti/openpecha-toolkit
 Author: Esukhia developers
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openpecha Version: 0.9.8 Summary: OpenPecha Toolkit
+Metadata-Version: 2.1 Name: openpecha Version: 0.9.9 Summary: OpenPecha Toolkit
 allows state of the art for distributed standoff annotations on moving texts
 Home-page: https://github.com/OpenPoti/openpecha-toolkit Author: Esukhia
 developers Author-email: esukhiadev@gmail.com License: Apache2 Platform:
 UNKNOWN Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: transifex License-File: LICENSE
                                     ******
                                  [OpenPecha]
```

### Comparing `openpecha-0.9.8/README.md` & `openpecha-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/__init__.py` & `openpecha-0.9.9/openpecha/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/exporter/__init__.py` & `openpecha-0.9.9/openpecha/alignment/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/exporter/bitext.py` & `openpecha-0.9.9/openpecha/alignment/exporter/bitext.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/exporter/po.py` & `openpecha-0.9.9/openpecha/alignment/exporter/po.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/integrations/tx.py` & `openpecha-0.9.9/openpecha/alignment/integrations/tx.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/parsers/po.py` & `openpecha-0.9.9/openpecha/alignment/parsers/po.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/parsers/tmx.py` & `openpecha-0.9.9/openpecha/alignment/parsers/tmx.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/segmenters/sentence.py` & `openpecha-0.9.9/openpecha/alignment/segmenters/sentence.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/tmx/__init__.py` & `openpecha-0.9.9/openpecha/alignment/tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/tmx/create_opf.py` & `openpecha-0.9.9/openpecha/alignment/tmx/create_opf.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/alignment/tmx/translated_po_to_opf.py` & `openpecha-0.9.9/openpecha/alignment/tmx/translated_po_to_opf.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/blupdate.py` & `openpecha-0.9.9/openpecha/blupdate.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/buda/api.py` & `openpecha-0.9.9/openpecha/buda/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,16 @@
                             if l.language == "bo-x-ewts":
                                 res["source_metadata"]["author"] = CONVERTER.toUnicode(l.value)
                                 break
                             else:
                                 res["source_metadata"]["author"] = l.value
         res["source_metadata"]["languages"] = list(res["source_metadata"]["languages"])
         for _, _, ig in g.triples((wres, BDO.instanceHasVolume, None)):
+            if g.value(ig, BDO.volumeNumber) is None or g.value(ig, BDO.volumePagesTotal) is None:
+                continue
             iglname = str(ig)[str(ig).rfind('/')+1:]
             res["image_groups"][iglname] = {}
             iginfo = res["image_groups"][iglname]
             iginfo["id"] = str(ig)
             iginfo["total_pages"] = int(g.value(ig, BDO.volumePagesTotal))
             iginfo["volume_number"] = int(g.value(ig, BDO.volumeNumber))
             iginfo["volume_pages_bdrc_intro"] = int(g.value(ig, BDO.volumePagesTbrcIntro))
```

### Comparing `openpecha-0.9.8/openpecha/buda/chunker.py` & `openpecha-0.9.9/openpecha/buda/chunker.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/catalog/filter.py` & `openpecha-0.9.9/openpecha/catalog/filter.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/catalog/manager.py` & `openpecha-0.9.9/openpecha/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/catalog/storage.py` & `openpecha-0.9.9/openpecha/catalog/storage.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/cli.py` & `openpecha-0.9.9/openpecha/cli.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/config.py` & `openpecha-0.9.9/openpecha/config.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/annotation.py` & `openpecha-0.9.9/openpecha/core/annotation.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/annotations.py` & `openpecha-0.9.9/openpecha/core/annotations.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/ids.py` & `openpecha-0.9.9/openpecha/core/ids.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/layer.py` & `openpecha-0.9.9/openpecha/core/layer.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/metadata.py` & `openpecha-0.9.9/openpecha/core/metadata.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/core/pecha.py` & `openpecha-0.9.9/openpecha/core/pecha.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/corpus/download.py` & `openpecha-0.9.9/openpecha/corpus/download.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/corpus/quality.py` & `openpecha-0.9.9/openpecha/corpus/quality.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/editor.py` & `openpecha-0.9.9/openpecha/formatters/editor.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/empty.py` & `openpecha-0.9.9/openpecha/formatters/empty.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/formatter.py` & `openpecha-0.9.9/openpecha/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/hfml.py` & `openpecha-0.9.9/openpecha/formatters/hfml.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/layers.py` & `openpecha-0.9.9/openpecha/formatters/layers.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/ocr/google_vision.py` & `openpecha-0.9.9/openpecha/formatters/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/ocr/hocr.py` & `openpecha-0.9.9/openpecha/formatters/ocr/hocr.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/ocr/ocr.py` & `openpecha-0.9.9/openpecha/formatters/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/pedurma.py` & `openpecha-0.9.9/openpecha/formatters/pedurma.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/formatters/tsadra.py` & `openpecha-0.9.9/openpecha/formatters/tsadra.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/github_utils.py` & `openpecha-0.9.9/openpecha/github_utils.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/proofreading.py` & `openpecha-0.9.9/openpecha/proofreading.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/docx.py` & `openpecha-0.9.9/openpecha/serializers/docx.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/editor.py` & `openpecha-0.9.9/openpecha/serializers/editor.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/epub.py` & `openpecha-0.9.9/openpecha/serializers/epub.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/hfml.py` & `openpecha-0.9.9/openpecha/serializers/hfml.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/pedurma.py` & `openpecha-0.9.9/openpecha/serializers/pedurma.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/rdf.py` & `openpecha-0.9.9/openpecha/serializers/rdf.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/serializers/serialize.py` & `openpecha-0.9.9/openpecha/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/storages.py` & `openpecha-0.9.9/openpecha/storages.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/utils.py` & `openpecha-0.9.9/openpecha/utils.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/work/__init__.py` & `openpecha-0.9.9/openpecha/work/__init__.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha/work/bdrc.py` & `openpecha-0.9.9/openpecha/work/bdrc.py`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/openpecha.egg-info/PKG-INFO` & `openpecha-0.9.9/openpecha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpecha
-Version: 0.9.8
+Version: 0.9.9
 Summary: OpenPecha Toolkit allows state of the art for distributed standoff annotations on moving texts
 Home-page: https://github.com/OpenPoti/openpecha-toolkit
 Author: Esukhia developers
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openpecha Version: 0.9.8 Summary: OpenPecha Toolkit
+Metadata-Version: 2.1 Name: openpecha Version: 0.9.9 Summary: OpenPecha Toolkit
 allows state of the art for distributed standoff annotations on moving texts
 Home-page: https://github.com/OpenPoti/openpecha-toolkit Author: Esukhia
 developers Author-email: esukhiadev@gmail.com License: Apache2 Platform:
 UNKNOWN Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: transifex License-File: LICENSE
                                     ******
                                  [OpenPecha]
```

### Comparing `openpecha-0.9.8/openpecha.egg-info/SOURCES.txt` & `openpecha-0.9.9/openpecha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpecha-0.9.8/setup.py` & `openpecha-0.9.9/setup.py`

 * *Files identical despite different names*

