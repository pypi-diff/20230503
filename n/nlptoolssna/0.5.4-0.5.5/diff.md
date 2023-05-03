# Comparing `tmp/nlptoolssna-0.5.4.tar.gz` & `tmp/nlptoolssna-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.5.4.tar", last modified: Wed May  3 18:56:10 2023, max compression
+gzip compressed data, was "nlptoolssna-0.5.5.tar", last modified: Wed May  3 18:59:40 2023, max compression
```

## Comparing `nlptoolssna-0.5.4.tar` & `nlptoolssna-0.5.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.858030 nlptoolssna-0.5.4/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-03 18:56:10.858226 nlptoolssna-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.749827 nlptoolssna-0.5.4/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.713945 nlptoolssna-0.5.4/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.714944 nlptoolssna-0.5.4/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.751898 nlptoolssna-0.5.4/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.4/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.760987 nlptoolssna-0.5.4/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.4/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.4/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.4/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.4/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.771922 nlptoolssna-0.5.4/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.773917 nlptoolssna-0.5.4/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.4/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.778952 nlptoolssna-0.5.4/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.781417 nlptoolssna-0.5.4/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.4/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.4/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.783431 nlptoolssna-0.5.4/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.4/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.4/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.4/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.4/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.4/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.4/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.4/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.790432 nlptoolssna-0.5.4/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.794445 nlptoolssna-0.5.4/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.4/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.4/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.807259 nlptoolssna-0.5.4/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.4/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.4/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.4/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.4/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.4/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.4/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.808203 nlptoolssna-0.5.4/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.4/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.814268 nlptoolssna-0.5.4/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.4/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.4/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.827333 nlptoolssna-0.5.4/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.4/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.4/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     8145 2023-05-03 18:56:01.000000 nlptoolssna-0.5.4/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.4/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.4/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.831399 nlptoolssna-0.5.4/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.4/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.4/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.836393 nlptoolssna-0.5.4/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.4/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.4/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.4/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.851236 nlptoolssna-0.5.4/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 18:56:10.000000 nlptoolssna-0.5.4/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-03 18:56:10.860307 nlptoolssna-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:56:10.855226 nlptoolssna-0.5.4/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.4/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.820450 nlptoolssna-0.5.5/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-03 18:59:40.821447 nlptoolssna-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.713316 nlptoolssna-0.5.5/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.667505 nlptoolssna-0.5.5/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.668635 nlptoolssna-0.5.5/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.715471 nlptoolssna-0.5.5/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.5/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.724272 nlptoolssna-0.5.5/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.5/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.5/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.5/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.5/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.737226 nlptoolssna-0.5.5/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.740228 nlptoolssna-0.5.5/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.5/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.745221 nlptoolssna-0.5.5/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.747278 nlptoolssna-0.5.5/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.5/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.5/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.749314 nlptoolssna-0.5.5/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.5/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.5/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.5/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.5/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.5/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.755301 nlptoolssna-0.5.5/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.759302 nlptoolssna-0.5.5/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.5/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.5/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.771589 nlptoolssna-0.5.5/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.5/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.5/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.5/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.5/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.5/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.5/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.774560 nlptoolssna-0.5.5/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.5/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.778562 nlptoolssna-0.5.5/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.5/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.5/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.788639 nlptoolssna-0.5.5/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.5/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.5/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     8147 2023-05-03 18:59:15.000000 nlptoolssna-0.5.5/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.5/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.5/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.793636 nlptoolssna-0.5.5/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.5/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.5/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.800524 nlptoolssna-0.5.5/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.5/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.5/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.5/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.815449 nlptoolssna-0.5.5/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 18:59:40.000000 nlptoolssna-0.5.5/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-03 18:59:40.823694 nlptoolssna-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:59:40.818446 nlptoolssna-0.5.5/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.5/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.5.4/CONTRIBUTING.rst` & `nlptoolssna-0.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/LICENSE` & `nlptoolssna-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/PKG-INFO` & `nlptoolssna-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.4/README.rst` & `nlptoolssna-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/Makefile` & `nlptoolssna-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/build/html/_images/download.png` & `nlptoolssna-0.5.5/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/build/html/_static/download.png` & `nlptoolssna-0.5.5/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/make.bat` & `nlptoolssna-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/source/_static/download.png` & `nlptoolssna-0.5.5/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/source/conf.py` & `nlptoolssna-0.5.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/docs/source/installation.rst` & `nlptoolssna-0.5.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.5.5/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/arabiner/data.py` & `nlptoolssna-0.5.5/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/arabiner/datasets.py` & `nlptoolssna-0.5.5/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/arabiner/helpers.py` & `nlptoolssna-0.5.5/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/arabiner/infer.py` & `nlptoolssna-0.5.5/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/arabiner/transforms.py` & `nlptoolssna-0.5.5/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/data/my_data.pickle` & `nlptoolssna-0.5.5/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.5.5/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/morphology/charsets.py` & `nlptoolssna-0.5.5/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.5.5/nlptools/morphology/morph_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         
    return filter_results(task, output_list)
 
 def filter_results(task, lst):
     if task == 'lemmatizer':
         return remove_items_by_index(lst, [2])
     elif task == 'pos':
-        return remove_items_by_index(lst, [0])
+        return remove_items_by_index(lst, [0,1])
     else: 
         return lst
 
 
 def remove_items_by_index(lst, index_list):
     for inner_list in lst:
         for index in sorted(index_list, reverse=True):
```

### Comparing `nlptoolssna-0.5.4/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.5.5/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/parse/parser.py` & `nlptoolssna-0.5.5/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/salma/implication.py` & `nlptoolssna-0.5.5/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.5.5/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.5.5/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.4/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.5.5/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/setup.cfg` & `nlptoolssna-0.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.4/setup.py` & `nlptoolssna-0.5.5/setup.py`

 * *Files identical despite different names*

