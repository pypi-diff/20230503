# Comparing `tmp/trytond_purchase_request-6.6.3.tar.gz` & `tmp/trytond_purchase_request-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request-6.6.3.tar", last modified: Fri Feb 17 18:39:54 2023, max compression
+gzip compressed data, was "trytond_purchase_request-6.8.0.tar", last modified: Mon May  1 11:47:56 2023, max compression
```

## Comparing `trytond_purchase_request-6.6.3.tar` & `trytond_purchase_request-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.426252 trytond_purchase_request-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     2056 2023-02-17 18:39:50.000000 trytond_purchase_request-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-02-17 18:39:50.000000 trytond_purchase_request-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3402 2023-02-17 18:39:54.426252 trytond_purchase_request-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.422919 trytond_purchase_request-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.419586 trytond_purchase_request-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6899 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7269 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6147 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7383 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7235 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6193 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6491 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7820 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6147 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7222 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6818 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6175 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7239 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6845 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6183 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7215 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6436 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7027 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7021 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6920 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6147 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5876 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6937 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3791 2023-01-15 17:31:04.000000 trytond_purchase_request-6.6.3/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1329 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21785 2023-02-13 22:28:57.000000 trytond_purchase_request-6.6.3/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10468 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-17 18:39:54.426252 trytond_purchase_request-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.422919 trytond_purchase_request-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8597 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/tests/scenario_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-02-05 21:18:48.000000 trytond_purchase_request-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.426252 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3402 2023-02-17 18:39:53.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1988 2023-02-17 18:39:54.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-17 18:39:53.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-02-17 18:39:53.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-15 17:49:51.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-02-17 18:39:53.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-17 18:39:53.000000 trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:39:54.422919 trytond_purchase_request-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/view/handle_purchase_cancellation_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/view/purchase_request_create_purchase_ask_party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1813 2022-12-19 12:02:53.000000 trytond_purchase_request-6.6.3/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      601 2022-12-19 12:02:50.000000 trytond_purchase_request-6.6.3/view/purchase_request_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.743803 trytond_purchase_request-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1919 2023-05-01 11:05:19.000000 trytond_purchase_request-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-05-01 11:05:19.000000 trytond_purchase_request-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3393 2023-05-01 11:47:56.743803 trytond_purchase_request-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.743803 trytond_purchase_request-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.737136 trytond_purchase_request-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6899 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7269 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6147 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7383 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7235 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6193 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6491 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7820 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6147 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7222 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6818 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6175 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7239 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6845 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6183 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7215 2023-04-30 10:46:36.000000 trytond_purchase_request-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6436 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7027 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7021 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6920 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6147 2023-04-29 08:02:44.000000 trytond_purchase_request-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5876 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6937 2023-04-29 08:02:45.000000 trytond_purchase_request-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1329 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    21936 2023-04-22 15:53:52.000000 trytond_purchase_request-6.8.0/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10472 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:56.743803 trytond_purchase_request-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4404 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.740469 trytond_purchase_request-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8541 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/tests/scenario_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-05-01 11:05:14.000000 trytond_purchase_request-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.743803 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3393 2023-05-01 11:47:55.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1988 2023-05-01 11:47:56.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:55.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 11:47:55.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-05-01 11:47:55.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:55.000000 trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:56.740469 trytond_purchase_request-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/view/handle_purchase_cancellation_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 trytond_purchase_request-6.8.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-01-16 14:00:21.000000 trytond_purchase_request-6.8.0/view/purchase_request_create_purchase_ask_party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1813 2023-04-22 15:53:49.000000 trytond_purchase_request-6.8.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      601 2023-04-15 07:12:15.000000 trytond_purchase_request-6.8.0/view/purchase_request_tree.xml
```

### Comparing `trytond_purchase_request-6.6.3/CHANGELOG` & `trytond_purchase_request-6.8.0/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-Version 6.6.3 - 2023-02-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
 
-Version 6.6.1 - 2023-01-15
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_purchase_request-6.6.3/COPYRIGHT` & `trytond_purchase_request-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2016-2022 Nicolas Évrard.
+Copyright (C) 2016-2023 Nicolas Évrard.
 Copyright (C) 2013-2015 NaN-tic.
 Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
 Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
```

### Comparing `trytond_purchase_request-6.6.3/LICENSE` & `trytond_purchase_request-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/PKG-INFO` & `trytond_purchase_request-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_request
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase request
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Purchase Request Module
 #######################
 
 The Purchase Request module introduces the concept of Purchase Requests which
```

### Comparing `trytond_purchase_request-6.6.3/README.rst` & `trytond_purchase_request-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/__init__.py` & `trytond_purchase_request-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/doc/conf.py` & `trytond_purchase_request-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
```

### Comparing `trytond_purchase_request-6.6.3/doc/index.rst` & `trytond_purchase_request-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/bg.po` & `trytond_purchase_request-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/ca.po` & `trytond_purchase_request-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/cs.po` & `trytond_purchase_request-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/de.po` & `trytond_purchase_request-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/es.po` & `trytond_purchase_request-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/es_419.po` & `trytond_purchase_request-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/et.po` & `trytond_purchase_request-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/fa.po` & `trytond_purchase_request-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/fi.po` & `trytond_purchase_request-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/fr.po` & `trytond_purchase_request-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/hu.po` & `trytond_purchase_request-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/id.po` & `trytond_purchase_request-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/it.po` & `trytond_purchase_request-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/lo.po` & `trytond_purchase_request-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/lt.po` & `trytond_purchase_request-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/nl.po` & `trytond_purchase_request-6.8.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 msgctxt "model:ir.action,name:act_open_request_form"
 msgid "Purchase Requests"
 msgstr "Aankoopverzoeken"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "Aankoopverzoeken"
+msgstr "Inkoop Aanvragen"
 
 msgctxt "model:ir.action,name:wizard_create_purchase"
 msgid "Create Purchase"
 msgstr "Inkooporder maken"
 
 msgctxt "model:ir.action,name:wizard_purchase_cancellation_handle_exception"
 msgid "Handle Purchase Cancellation"
```

### Comparing `trytond_purchase_request-6.6.3/locale/pl.po` & `trytond_purchase_request-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/pt.po` & `trytond_purchase_request-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/ro.po` & `trytond_purchase_request-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/ru.po` & `trytond_purchase_request-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/sl.po` & `trytond_purchase_request-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/tr.po` & `trytond_purchase_request-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/uk.po` & `trytond_purchase_request-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/locale/zh_CN.po` & `trytond_purchase_request-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/message.xml` & `trytond_purchase_request-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/purchase.py` & `trytond_purchase_request-6.8.0/purchase.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
-from trytond.transaction import Transaction
+from trytond.transaction import without_check_access
 
 from .exceptions import PurchaseWarehouseWarning
 
 
 def process_request(func):
+    # Must be run after the purchase transition
+    # such as purchase has the proper state
     @wraps(func)
     def wrapper(cls, purchases):
         pool = Pool()
         Request = pool.get('purchase.request')
         func(cls, purchases)
         requests = [r for p in purchases for l in p.lines for r in l.requests]
         Request.update_state(requests)
@@ -28,17 +30,16 @@
 
     @classmethod
     def delete(cls, purchases):
         cls.check_delete_purchase_request(purchases)
         super(Purchase, cls).delete(purchases)
 
     @classmethod
+    @without_check_access
     def check_delete_purchase_request(cls, purchases):
-        with Transaction().set_context(_check_access=False):
-            purchases = cls.browse(purchases)
         for purchase in purchases:
             for line in purchase.lines:
                 if line.requests:
                     raise AccessError(
                         gettext('purchase_request.msg_purchase_delete_request',
                             purchase=purchase.rec_name))
 
@@ -66,22 +67,22 @@
                                 purchase=self.rec_name,
                                 purchase_warehouse=self.warehouse.rec_name,
                                 request=request.rec_name,
                                 request_warehouse=request.warehouse.rec_name))
 
     @classmethod
     @ModelView.button
-    @Workflow.transition('cancelled')
     @process_request
+    @Workflow.transition('cancelled')
     def cancel(cls, purchases):
         super(Purchase, cls).cancel(purchases)
 
     @classmethod
-    @Workflow.transition('done')
     @process_request
+    @Workflow.transition('done')
     def do(cls, purchases):
         super(Purchase, cls).do(purchases)
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'purchase.line'
 
@@ -97,12 +98,12 @@
         default.setdefault('requests')
         return super().copy(lines, default=default)
 
     @classmethod
     def delete(cls, lines):
         pool = Pool()
         Request = pool.get('purchase.request')
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             requests = [r for l in cls.browse(lines) for r in l.requests]
         super().delete(lines)
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             Request.update_state(requests)
```

### Comparing `trytond_purchase_request-6.6.3/purchase.xml` & `trytond_purchase_request-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/purchase_request.py` & `trytond_purchase_request-6.8.0/purchase_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 
 class PurchaseRequest(ModelSQL, ModelView):
     'Purchase Request'
     __name__ = 'purchase.request'
 
     product = fields.Many2One(
         'product.product', "Product", readonly=True,
-        domain=[('purchasable', '=', True)],
+        domain=[
+            If((Eval('state') == 'draft')
+                & ~(Eval('quantity', 0) < 0),
+                ('purchasable', '=', True),
+                ()),
+            ],
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     description = fields.Text('Description', readonly=True, states=STATES)
     summary = fields.Function(fields.Char('Summary'), 'on_change_with_summary')
     party = fields.Many2One(
@@ -282,21 +287,19 @@
     def on_change_with_uom_digits(self, name=None):
         if self.uom:
             return self.uom.digits
         return 2
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends('product')
     def on_change_with_default_uom(self, name=None):
-        if self.product:
-            return self.product.default_uom.id
+        return self.product.default_uom if self.product else None
 
     @fields.depends('product')
     def on_change_with_default_uom_digits(self, name=None):
         if self.product:
             return self.product.default_uom.digits
         return 2
 
@@ -322,15 +325,15 @@
         return super().view_attributes() + [
             ('/tree', 'visual', If(Eval('state') == 'cancelled', 'muted', '')),
             ]
 
     @classmethod
     def create(cls, vlist):
         transaction = Transaction()
-        if transaction.user != 0 and transaction.context.get('_check_access'):
+        if transaction.user and transaction.check_access:
             raise AccessError(
                 gettext('purchase_request.msg_request_no_create'))
         return super(PurchaseRequest, cls).create(vlist)
 
     @classmethod
     def delete(cls, requests):
         for request in requests:
@@ -552,14 +555,17 @@
         Uom = pool.get('product.uom')
         unit = line.unit
         compute_qty = Uom.compute_qty
         return sum(
             compute_qty(r.uom, r.quantity, unit, round=False)
             for r in requests)
 
+    def end(self):
+        return 'reload'
+
 
 class HandlePurchaseCancellationException(Wizard):
     'Handle Purchase Cancellation Exception'
     __name__ = 'purchase.request.handle.purchase.cancellation'
 
     start = StateView('purchase.request.handle.purchase.cancellation.start',
         'purchase_request.handle_purchase_cancellation_start', [
```

### Comparing `trytond_purchase_request-6.6.3/purchase_request.xml` & `trytond_purchase_request-6.8.0/purchase_request.xml`

 * *Files 0% similar despite different names*

#### Comparing `trytond_purchase_request-6.6.3/purchase_request.xml` & `trytond_purchase_request-6.8.0/purchase_request.xml`

```diff
@@ -118,15 +118,15 @@
     <record model="ir.model.access" id="access_purchase_request">
       <field name="model" search="[('model', '=', 'purchase.request')]"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
-    <record model="ir.model.access" id="access_purchase_request_sale">
+    <record model="ir.model.access" id="access_purchase_request_purchase">
       <field name="model" search="[('model', '=', 'purchase.request')]"/>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
```

### Comparing `trytond_purchase_request-6.6.3/setup.py` & `trytond_purchase_request-6.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 def read(fname):
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_request'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -51,22 +51,22 @@
     get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for purchase requests',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/purchase_request',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase request',
     package_dir={'trytond.modules.purchase_request': '.'},
     packages=(
         ['trytond.modules.purchase_request']
         + ['trytond.modules.purchase_request.%s' % p for p in find_packages()]
         ),
@@ -103,23 +103,23 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_purchase_request-6.6.3/tests/scenario_purchase_request.rst` & `trytond_purchase_request-6.8.0/tests/scenario_purchase_request.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 =========================
 Purchase Request Scenario
 =========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (create_chart,
     ...     get_accounts)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['purchase_request', 'stock_supply'])
 
 Create company::
```

### Comparing `trytond_purchase_request-6.6.3/tox.ini` & `trytond_purchase_request-6.8.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/purchase_request/* -m unittest discover -s tests
-    coverage report --include=./**/purchase_request/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/PKG-INFO` & `trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-purchase-request
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_request
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase request
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Purchase Request Module
 #######################
 
 The Purchase Request module introduces the concept of Purchase Requests which
```

### Comparing `trytond_purchase_request-6.6.3/trytond_purchase_request.egg-info/SOURCES.txt` & `trytond_purchase_request-6.8.0/trytond_purchase_request.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/view/purchase_request_form.xml` & `trytond_purchase_request-6.8.0/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-6.6.3/view/purchase_request_tree.xml` & `trytond_purchase_request-6.8.0/view/purchase_request_tree.xml`

 * *Files identical despite different names*

