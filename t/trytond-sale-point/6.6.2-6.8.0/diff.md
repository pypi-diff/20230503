# Comparing `tmp/trytond_sale_point-6.6.2.tar.gz` & `tmp/trytond_sale_point-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_point-6.6.2.tar", last modified: Wed May  3 16:42:46 2023, max compression
+gzip compressed data, was "trytond_sale_point-6.8.0.tar", last modified: Mon May  1 12:01:39 2023, max compression
```

## Comparing `trytond_sale_point-6.6.2.tar` & `trytond_sale_point-6.8.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.874240 trytond_sale_point-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-05-03 16:42:42.000000 trytond_sale_point-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-03 16:42:42.000000 trytond_sale_point-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-05-03 16:42:46.874240 trytond_sale_point-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.867573 trytond_sale_point-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.850906 trytond_sale_point-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17170 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17597 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17225 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17366 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14479 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14154 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17032 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45448 2023-04-13 17:26:18.000000 trytond_sale_point-6.6.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24915 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:42:46.874240 trytond_sale_point-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4565 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.857573 trytond_sale_point-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/scenario_sale_point.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3694 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/scenario_sale_point_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4456 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/scenario_sale_point_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5016 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/scenario_sale_point_session.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3928 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/scenario_sale_point_tax_excluded.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.870906 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-05-03 16:42:45.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2894 2023-05-03 16:42:46.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:42:45.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-03 16:42:45.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:34:34.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-03 16:42:45.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:42:45.000000 trytond_sale_point-6.6.2/trytond_sale_point.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:42:46.864240 trytond_sale_point-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_session_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_session_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_transfer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_transfer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_transfer_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/cash_transfer_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/payment_form_wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/payment_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/sale_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/sale_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-13 16:52:41.000000 trytond_sale_point-6.6.2/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.750683 trytond_sale_point-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-05-01 11:14:48.000000 trytond_sale_point-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:14:48.000000 trytond_sale_point-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-05-01 12:01:39.747349 trytond_sale_point-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.747349 trytond_sale_point-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.734016 trytond_sale_point-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17178 2023-04-30 10:46:36.000000 trytond_sale_point-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17597 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17215 2023-04-30 10:46:36.000000 trytond_sale_point-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17446 2023-04-30 10:46:36.000000 trytond_sale_point-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14479 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14154 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17042 2023-04-30 10:46:36.000000 trytond_sale_point-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-04-29 08:02:50.000000 trytond_sale_point-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45309 2023-04-28 07:46:16.000000 trytond_sale_point-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24915 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:39.750683 trytond_sale_point-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.737349 trytond_sale_point-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5832 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/scenario_sale_point.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3674 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/scenario_sale_point_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4456 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/scenario_sale_point_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4996 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/scenario_sale_point_session.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3928 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/scenario_sale_point_tax_excluded.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-05-01 11:14:42.000000 trytond_sale_point-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.747349 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-05-01 12:01:38.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2894 2023-05-01 12:01:39.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:38.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 12:01:38.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 12:01:38.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:38.000000 trytond_sale_point-6.8.0/trytond_sale_point.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:39.744016 trytond_sale_point-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_session_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_session_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_transfer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_transfer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_transfer_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/cash_transfer_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/payment_form_wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/payment_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/sale_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/sale_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_sale_point-6.8.0/view/template_tree.xml
```

### Comparing `trytond_sale_point-6.6.2/COPYRIGHT` & `trytond_sale_point-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/LICENSE` & `trytond_sale_point-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/PKG-INFO` & `trytond_sale_point-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_point
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-point/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_point
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton POS sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 #################
 Sale Point Module
 #################
```

### Comparing `trytond_sale_point-6.6.2/__init__.py` & `trytond_sale_point-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/account.py` & `trytond_sale_point-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/doc/conf.py` & `trytond_sale_point-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_point-6.6.2/doc/design.rst` & `trytond_sale_point-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/bg.po` & `trytond_sale_point-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/ca.po` & `trytond_sale_point-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 msgctxt "field:sale.point.cash.transfer,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:sale.point.cash.transfer,move:"
 msgid "Move"
-msgstr "Moviment"
+msgstr "Assentament"
 
 msgctxt "field:sale.point.cash.transfer,point:"
 msgid "Point"
 msgstr "Punt"
 
 msgctxt "field:sale.point.cash.transfer,session:"
 msgid "Session"
@@ -244,15 +244,15 @@
 
 msgctxt "field:sale.point.sale,lines:"
 msgid "Lines"
 msgstr "Línies"
 
 msgctxt "field:sale.point.sale,move:"
 msgid "Move"
-msgstr "Moviment"
+msgstr "Assentament"
 
 msgctxt "field:sale.point.sale,number:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:sale.point.sale,payments:"
 msgid "Payments"
@@ -284,15 +284,15 @@
 
 msgctxt "field:sale.point.sale.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:sale.point.sale.line,moves:"
 msgid "Moves"
-msgstr "Moviments"
+msgstr "Assentament"
 
 msgctxt "field:sale.point.sale.line,product:"
 msgid "Product"
 msgstr "Producte"
 
 msgctxt "field:sale.point.sale.line,quantity:"
 msgid "Quantity"
```

### Comparing `trytond_sale_point-6.6.2/locale/cs.po` & `trytond_sale_point-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/de.po` & `trytond_sale_point-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/es.po` & `trytond_sale_point-6.8.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 msgctxt "field:sale.point.cash.transfer,date:"
 msgid "Date"
 msgstr "Fecha"
 
 msgctxt "field:sale.point.cash.transfer,move:"
 msgid "Move"
-msgstr "Movimiento"
+msgstr "Asiento"
 
 msgctxt "field:sale.point.cash.transfer,point:"
 msgid "Point"
 msgstr "Punto"
 
 msgctxt "field:sale.point.cash.transfer,session:"
 msgid "Session"
@@ -244,15 +244,15 @@
 
 msgctxt "field:sale.point.sale,lines:"
 msgid "Lines"
 msgstr "Líneas"
 
 msgctxt "field:sale.point.sale,move:"
 msgid "Move"
-msgstr "Movimiento"
+msgstr "Asiento"
 
 msgctxt "field:sale.point.sale,number:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:sale.point.sale,payments:"
 msgid "Payments"
@@ -284,15 +284,15 @@
 
 msgctxt "field:sale.point.sale.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:sale.point.sale.line,moves:"
 msgid "Moves"
-msgstr "Movimientos"
+msgstr "Asiento"
 
 msgctxt "field:sale.point.sale.line,product:"
 msgid "Product"
 msgstr "Producto"
 
 msgctxt "field:sale.point.sale.line,quantity:"
 msgid "Quantity"
```

### Comparing `trytond_sale_point-6.6.2/locale/es_419.po` & `trytond_sale_point-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/et.po` & `trytond_sale_point-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/fa.po` & `trytond_sale_point-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/fi.po` & `trytond_sale_point-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/fr.po` & `trytond_sale_point-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -463,49 +463,50 @@
 msgid "You cannot delete sale \"%(sale)s\" because it has a number."
 msgstr ""
 "Vous ne pouvez pas supprimer la vente « %(sale)s » car elle a un numéro."
 
 msgctxt "model:ir.message,text:msg_transfer_delete_posted"
 msgid "You cannot delete transfer \"%(transfer)s\" because it is posted."
 msgstr ""
-"Vous ne pouvez pas supprimer le transfert « %(transfer)s » car il est posté."
+"Vous ne pouvez pas supprimer le transfert « %(transfer)s » car il est "
+"comptabilisé."
 
 msgctxt "model:ir.message,text:msg_transfer_delete_session_open"
 msgid "To delete transfer \"%(transfer)s\" you must re-open session \"%(session)s\"."
 msgstr ""
 "Pour supprimer le transfert « %(transfer)s » vous devez rouvrir la session "
 "« %(session)s »."
 
 msgctxt "model:ir.model.button,confirm:cash_session_post_button"
 msgid "Are you sure you want to post the sessions?"
-msgstr "Êtes-vous sûr de vouloir poster les sessions ?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser les sessions ?"
 
 msgctxt "model:ir.model.button,confirm:cash_transfer_post_button"
 msgid "Are you sure you want to post the transfer?"
-msgstr "Êtes-vous sûr de vouloir poster le transfert ?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser le transfert ?"
 
 msgctxt "model:ir.model.button,confirm:sale_post_button"
 msgid "Are you sure you want to post the sales?"
-msgstr "Êtes-vous sûr de vouloir poster les ventes ?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser les ventes ?"
 
 msgctxt "model:ir.model.button,string:cash_session_close_button"
 msgid "Close"
 msgstr "Clôturer"
 
 msgctxt "model:ir.model.button,string:cash_session_open_button"
 msgid "Re-Open"
 msgstr "Rouvrir"
 
 msgctxt "model:ir.model.button,string:cash_session_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:cash_transfer_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:sale_cancel_button"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:sale_open_button"
 msgid "Re-Open"
@@ -513,15 +514,15 @@
 
 msgctxt "model:ir.model.button,string:sale_pay_button"
 msgid "Pay"
 msgstr "Payer"
 
 msgctxt "model:ir.model.button,string:sale_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:sale_process_button"
 msgid "Process"
 msgstr "Traiter"
 
 msgctxt "model:ir.rule.group,name:rule_group_cash_session_companies"
 msgid "User in companies"
@@ -577,15 +578,15 @@
 
 msgctxt "model:res.group,name:group_sale_point"
 msgid "POS"
 msgstr "PDV"
 
 msgctxt "model:res.group,name:group_sale_point_posting"
 msgid "POS Posting"
-msgstr "Postage PDV"
+msgstr "Comptabilisation PDV"
 
 msgctxt "model:sale.point,name:"
 msgid "Point of Sale"
 msgstr "Point de vente"
 
 msgctxt "model:sale.point.cash.session,name:"
 msgid "POS Cash Session"
@@ -625,23 +626,23 @@
 
 msgctxt "selection:sale.point.cash.session,state:"
 msgid "Open"
 msgstr "Ouverte"
 
 msgctxt "selection:sale.point.cash.session,state:"
 msgid "Posted"
-msgstr "Postée"
+msgstr "Comptabilisé"
 
 msgctxt "selection:sale.point.cash.transfer,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:sale.point.cash.transfer,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Cancelled"
 msgstr "Annulée"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Done"
@@ -649,15 +650,15 @@
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Open"
 msgstr "Ouverte"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Posted"
-msgstr "Postée"
+msgstr "Comptabilisé"
 
 msgctxt "view:sale.point.sale.line:"
 msgid "General"
 msgstr "Général"
 
 msgctxt "view:sale.point.sale:"
 msgid "Other Info"
```

### Comparing `trytond_sale_point-6.6.2/locale/hu.po` & `trytond_sale_point-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/id.po` & `trytond_sale_point-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/it.po` & `trytond_sale_point-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/lo.po` & `trytond_sale_point-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/lt.po` & `trytond_sale_point-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/nl.po` & `trytond_sale_point-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:product.gross_price,gross_price:"
 msgid "Gross Price"
 msgstr "Bruto prijs"
 
 msgctxt "field:product.gross_price,template:"
 msgid "Template"
-msgstr "Sjabloon"
+msgstr "Template"
 
 msgctxt "field:product.product,gross_price:"
 msgid "Gross Price"
 msgstr "Bruto prijs"
 
 msgctxt "field:product.product,gross_prices:"
 msgid "Gross Prices"
@@ -48,15 +48,15 @@
 
 msgctxt "field:sale.point,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:sale.point,return_location:"
 msgid "Return Location"
-msgstr "Retourlocatie"
+msgstr "Retour locatie"
 
 msgctxt "field:sale.point,sequence:"
 msgid "Sequence"
 msgstr "Reeks"
 
 msgctxt "field:sale.point,storage_location:"
 msgid "Storage Location"
@@ -80,35 +80,35 @@
 
 msgctxt "field:sale.point.cash.session,next_session:"
 msgid "Next Session"
 msgstr "Volgende sessie"
 
 msgctxt "field:sale.point.cash.session,payments:"
 msgid "Payments"
-msgstr "betalingen"
+msgstr "Betalingen"
 
 msgctxt "field:sale.point.cash.session,point:"
 msgid "Point"
-msgstr "Punt"
+msgstr "Verkooppunt"
 
 msgctxt "field:sale.point.cash.session,previous_session:"
 msgid "Previous Session"
 msgstr "Vorige sessie"
 
 msgctxt "field:sale.point.cash.session,start_amount:"
 msgid "Start Amount"
 msgstr "Startbedrag"
 
 msgctxt "field:sale.point.cash.session,state:"
 msgid "State"
-msgstr "Staat"
+msgstr "Status"
 
 msgctxt "field:sale.point.cash.session,transfers:"
 msgid "Transfers"
-msgstr "Overboekingen"
+msgstr "Boekingen"
 
 msgctxt "field:sale.point.cash.session.relation,next:"
 msgid "Next"
 msgstr "Volgende"
 
 msgctxt "field:sale.point.cash.session.relation,previous:"
 msgid "Previous"
@@ -132,31 +132,31 @@
 
 msgctxt "field:sale.point.cash.transfer,move:"
 msgid "Move"
 msgstr "Boeking"
 
 msgctxt "field:sale.point.cash.transfer,point:"
 msgid "Point"
-msgstr "Punt"
+msgstr "Verkooppunt"
 
 msgctxt "field:sale.point.cash.transfer,session:"
 msgid "Session"
 msgstr "Sessie"
 
 msgctxt "field:sale.point.cash.transfer,state:"
 msgid "State"
-msgstr "Staat"
+msgstr "Status"
 
 msgctxt "field:sale.point.cash.transfer,type:"
 msgid "Type"
-msgstr "Type"
+msgstr "Soort"
 
 msgctxt "field:sale.point.cash.transfer.type,account:"
 msgid "Account"
-msgstr "Rekening"
+msgstr "Grootboekrekening"
 
 msgctxt "field:sale.point.cash.transfer.type,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:sale.point.cash.transfer.type,journal:"
 msgid "Journal"
@@ -184,15 +184,15 @@
 
 msgctxt "field:sale.point.payment,method:"
 msgid "Method"
 msgstr "Methode"
 
 msgctxt "field:sale.point.payment,point:"
 msgid "Point"
-msgstr "Punt"
+msgstr "Verkooppunt"
 
 msgctxt "field:sale.point.payment,sale:"
 msgid "Sale"
 msgstr "Verkoop"
 
 msgctxt "field:sale.point.payment,sale_state:"
 msgid "Sale State"
@@ -200,15 +200,15 @@
 
 msgctxt "field:sale.point.payment,session:"
 msgid "Session"
 msgstr "Sessie"
 
 msgctxt "field:sale.point.payment.method,account:"
 msgid "Account"
-msgstr "Rekening"
+msgstr "Grootboekrekening"
 
 msgctxt "field:sale.point.payment.method,cash:"
 msgid "Cash"
 msgstr "Contant geld"
 
 msgctxt "field:sale.point.payment.method,company:"
 msgid "Company"
@@ -220,55 +220,55 @@
 
 msgctxt "field:sale.point.sale,amount_paid:"
 msgid "Paid"
 msgstr "Betaald"
 
 msgctxt "field:sale.point.sale,amount_to_pay:"
 msgid "To Pay"
-msgstr "te betalen"
+msgstr "Te betalen"
 
 msgctxt "field:sale.point.sale,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:sale.point.sale,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:sale.point.sale,date:"
 msgid "Date"
-msgstr "datum"
+msgstr "Datum"
 
 msgctxt "field:sale.point.sale,employee:"
 msgid "Employee"
 msgstr "Werknemer"
 
 msgctxt "field:sale.point.sale,lines:"
 msgid "Lines"
 msgstr "Regels"
 
 msgctxt "field:sale.point.sale,move:"
 msgid "Move"
-msgstr "Mutatie"
+msgstr "Boeking"
 
 msgctxt "field:sale.point.sale,number:"
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:sale.point.sale,payments:"
 msgid "Payments"
-msgstr "betalingen"
+msgstr "Betalingen"
 
 msgctxt "field:sale.point.sale,point:"
 msgid "Point"
-msgstr "Punt"
+msgstr "Verkooppunt"
 
 msgctxt "field:sale.point.sale,state:"
 msgid "State"
-msgstr "Staat"
+msgstr "Status"
 
 msgctxt "field:sale.point.sale,total:"
 msgid "Total"
 msgstr "Totaal"
 
 msgctxt "field:sale.point.sale,total_tax:"
 msgid "Total Tax"
@@ -284,15 +284,15 @@
 
 msgctxt "field:sale.point.sale.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:sale.point.sale.line,moves:"
 msgid "Moves"
-msgstr "Mutaties"
+msgstr "Boekingen"
 
 msgctxt "field:sale.point.sale.line,product:"
 msgid "Product"
 msgstr "Product"
 
 msgctxt "field:sale.point.sale.line,quantity:"
 msgid "Quantity"
@@ -312,31 +312,32 @@
 
 msgctxt "field:sale.point.sale.line,unit_gross_price:"
 msgid "Unit Gross Price"
 msgstr "Brutoprijs per eenheid"
 
 msgctxt "field:sale.point.sale.line,unit_list_price:"
 msgid "Unit List Price"
-msgstr "eenheidsprijslijst"
+msgstr "Eenheidsprijslijst"
 
 msgctxt "field:sale.point.sale.line,unit_price:"
 msgid "Unit Price"
-msgstr "Eenheids- prijs"
+msgstr "Eenheidsprijs"
 
 msgctxt "help:product.product,gross_price:"
 msgid "The price with default tax included."
-msgstr "De prijs met standaard belasting inbegrepen."
+msgstr "De prijs met belasting inbegrepen."
 
 msgctxt "help:product.template,gross_price:"
 msgid "The price with default tax included."
-msgstr "De prijs met standaard belasting inbegrepen."
+msgstr "De prijs met belasting inbegrepen."
 
 msgctxt "help:sale.point,customer_location:"
 msgid "The location where goods are put when sold."
-msgstr "De locatie waar goederen worden geplaatst wanneer ze verkocht zijn."
+msgstr ""
+"De locatie waar de goederen worden geplaatst wanneer ze verkocht zijn."
 
 msgctxt "help:sale.point,return_location:"
 msgid ""
 "The location where goods are put when returned.\n"
 "If empty the storage location is used."
 msgstr ""
 "De plaats waar goederen bij terugkomst worden neergezet.\n"
@@ -349,40 +350,40 @@
 
 msgctxt "help:sale.point,tax_included:"
 msgid "Check if unit Price includes tax."
 msgstr "Vink aan als de eenheidsprijs inclusief belasting is."
 
 msgctxt "model:ir.action,name:act_cash_session_form"
 msgid "POS Cash Sessions"
-msgstr "POS Cash-sessies"
+msgstr "POS sessies"
 
 msgctxt "model:ir.action,name:act_cash_transfer_type_form"
 msgid "POS Cash Transfer Types"
-msgstr "POS kas soorten boeking"
+msgstr "POS boeking soorten"
 
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "POS Payment Methods"
-msgstr "POS-betaalmethoden"
+msgstr "POS betaalmethoden"
 
 msgctxt "model:ir.action,name:act_point_form"
 msgid "Points of Sale"
 msgstr "Verkooppunten"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "POS Sales"
-msgstr "POS-verkoop"
+msgstr "POS verkoop"
 
 msgctxt "model:ir.action,name:wizard_pay"
 msgid "Pay POS Sale"
-msgstr "Betaal POS-verkoop"
+msgstr "Betaal POS verkoop"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_cash_session_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Alles"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_cash_session_form_domain_closed"
 msgid "Closed"
 msgstr "Afgesloten"
 
 msgctxt ""
@@ -392,15 +393,15 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_all"
 msgid "All"
 msgstr "Alles"
 
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_done"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Gereed"
 
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_open"
 msgid "Opened"
 msgstr "Geopend"
 
 msgctxt "model:ir.message,text:msg_cash_session_delete_open"
 msgid "To delete session \"%(session)s\" you must re-open it."
@@ -411,15 +412,15 @@
 msgstr "Een sessie kan slechts één keer als vorige worden gebruikt."
 
 msgctxt "model:ir.message,text:msg_cash_session_wrong_end_amount"
 msgid ""
 "To close session \"%(session)s\" you must change end amount to have "
 "%(amount)s instead of %(end_amount)s."
 msgstr ""
-"Om de sessie \"%(session)s\" te sluiten, moet je het eindbedrag wijzigen om "
+"Om de sessie \"%(session)s\" te sluiten, moet u het eindbedrag wijzigen om "
 "%(amount)s te krijgen in plaats van %(end_amount)s."
 
 msgctxt "model:ir.message,text:msg_payment_delete_sale_open"
 msgid "To delete payment \"%(payment)s\" you must re-open sale \"%(sale)s\"."
 msgstr ""
 "Om de betaling \"%(payment)s\" te verwijderen, moet u de verkoop "
 "\"%(sale)s\" opnieuw openen."
@@ -439,50 +440,50 @@
 msgstr "Elk verkooppunt kan slechts één sessie open hebben."
 
 msgctxt "model:ir.message,text:msg_point_change_tax_included"
 msgid ""
 "You cannot change the point of sale's tax included flag because it has "
 "sales."
 msgstr ""
-"U kunt het vinkje inclusief btw van het verkooppunt niet wijzigen omdat deze"
-" verkopen heeft."
+"U kunt het 'inclusief belasting' van het verkooppunt niet wijzigen omdat "
+"deze verkopen heeft."
 
 msgctxt "model:ir.message,text:msg_sale_amount_paid_cancelled"
 msgid "The sale \"%(sale)s\" is cancelled so cannot have amount paid."
 msgstr ""
 "De verkoop \"%(sale)s\" is geannuleerd, er mag dus geen betaald bedrag "
 "geboekt zijn."
 
 msgctxt "model:ir.message,text:msg_sale_amount_to_pay_done_paid"
 msgid "The sale \"%(sale)s\" is done so cannot have an amount to pay."
 msgstr ""
-"De verkoop \"%(sale)s\" is gedaan en mag dus geen te betalen bedrag hebben."
+"De verkoop \"%(sale)s\" is afgerond en mag dus geen te betalen bedrag "
+"hebben."
 
 msgctxt "model:ir.message,text:msg_sale_delete_numbered"
 msgid "You cannot delete sale \"%(sale)s\" because it has a number."
 msgstr "U kunt verkoop \"%(sale)s\" niet verwijderen omdat deze een nummer heeft."
 
 msgctxt "model:ir.message,text:msg_transfer_delete_posted"
 msgid "You cannot delete transfer \"%(transfer)s\" because it is posted."
-msgstr ""
-"U kunt overboeking \"%(transfer)s\" niet verwijderen omdat deze geboekt is ."
+msgstr "U kunt boeking \"%(transfer)s\" niet verwijderen omdat deze geboekt is ."
 
 msgctxt "model:ir.message,text:msg_transfer_delete_session_open"
 msgid "To delete transfer \"%(transfer)s\" you must re-open session \"%(session)s\"."
 msgstr ""
-"Om overdracht \"%(transfer)s\" te verwijderen, moet u sessie \"%(session)s\""
-" opnieuw openen."
+"Om boeking \"%(transfer)s\" te verwijderen, moet u sessie \"%(session)s\" "
+"opnieuw openen."
 
 msgctxt "model:ir.model.button,confirm:cash_session_post_button"
 msgid "Are you sure you want to post the sessions?"
-msgstr "Weet je zeker dat je de sessies wilt boeken?"
+msgstr "Weet u zeker dat u de sessies wilt boeken?"
 
 msgctxt "model:ir.model.button,confirm:cash_transfer_post_button"
 msgid "Are you sure you want to post the transfer?"
-msgstr "Weet u zeker dat u de overboeking wilt boeken?"
+msgstr "Weet u zeker dat u de boeking wilt boeken?"
 
 msgctxt "model:ir.model.button,confirm:sale_post_button"
 msgid "Are you sure you want to post the sales?"
 msgstr "Weet u zeker dat u de verkopen wilt boeken?"
 
 msgctxt "model:ir.model.button,string:cash_session_close_button"
 msgid "Close"
@@ -490,35 +491,35 @@
 
 msgctxt "model:ir.model.button,string:cash_session_open_button"
 msgid "Re-Open"
 msgstr "Heropen"
 
 msgctxt "model:ir.model.button,string:cash_session_post_button"
 msgid "Post"
-msgstr "Boek"
+msgstr "Boeken"
 
 msgctxt "model:ir.model.button,string:cash_transfer_post_button"
 msgid "Post"
-msgstr "Boek"
+msgstr "Boeken"
 
 msgctxt "model:ir.model.button,string:sale_cancel_button"
 msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Annuleer"
 
 msgctxt "model:ir.model.button,string:sale_open_button"
 msgid "Re-Open"
 msgstr "Heropen"
 
 msgctxt "model:ir.model.button,string:sale_pay_button"
 msgid "Pay"
-msgstr "Betalen"
+msgstr "Betaal"
 
 msgctxt "model:ir.model.button,string:sale_post_button"
 msgid "Post"
-msgstr "Boek"
+msgstr "Boeken"
 
 msgctxt "model:ir.model.button,string:sale_process_button"
 msgid "Process"
 msgstr "Verwerken"
 
 msgctxt "model:ir.rule.group,name:rule_group_cash_session_companies"
 msgid "User in companies"
@@ -546,79 +547,79 @@
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale"
 msgid "POS"
 msgstr "POS"
 
 msgctxt "model:ir.ui.menu,name:menu_cash_session_form"
 msgid "POS Cash Sessions"
-msgstr "POS Cash-sessies"
+msgstr "POS sessies"
 
 msgctxt "model:ir.ui.menu,name:menu_cash_transfer_type_form"
 msgid "POS Cash Transfer Types"
-msgstr "POS kas soorten boeking"
+msgstr "POS boeking soorten"
 
 msgctxt "model:ir.ui.menu,name:menu_payment_method_form"
 msgid "POS Payment Methods"
-msgstr "POS-betaalmethoden"
+msgstr "POS betaalmethoden"
 
 msgctxt "model:ir.ui.menu,name:menu_point_form"
 msgid "Points of Sale"
 msgstr "Verkooppunten"
 
 msgctxt "model:ir.ui.menu,name:menu_sale_form"
 msgid "POS Sales"
-msgstr "POS-verkoop"
+msgstr "POS verkopen"
 
 msgctxt "model:product.gross_price,name:"
 msgid "Product Gross Price"
 msgstr "Bruto productprijs"
 
 msgctxt "model:res.group,name:group_sale_point"
 msgid "POS"
 msgstr "POS"
 
 msgctxt "model:res.group,name:group_sale_point_posting"
 msgid "POS Posting"
-msgstr "POS-boeking"
+msgstr "POS boeking"
 
 msgctxt "model:sale.point,name:"
 msgid "Point of Sale"
 msgstr "Verkooppunt"
 
 msgctxt "model:sale.point.cash.session,name:"
 msgid "POS Cash Session"
-msgstr "POS Cash-sessies"
+msgstr "POS sessies"
 
 msgctxt "model:sale.point.cash.session.relation,name:"
 msgid "POS Session Relation"
-msgstr "POS-sessierelatie"
+msgstr "POS sessie relatie"
 
 msgctxt "model:sale.point.cash.transfer,name:"
 msgid "POS Cash Transfer"
 msgstr "POS kas overboeking"
 
 msgctxt "model:sale.point.cash.transfer.type,name:"
 msgid "POS Cash Transfer Type"
 msgstr "POS kas soort boeking"
 
 msgctxt "model:sale.point.payment,name:"
 msgid "POS Payment"
-msgstr "POS-betaling"
+msgstr "POS betaling"
 
 msgctxt "model:sale.point.payment.method,name:"
 msgid "POS Payment Method"
-msgstr "POS-betaalmethoden"
+msgstr "POS betaalmethoden"
 
 msgctxt "model:sale.point.sale,name:"
 msgid "POS Sale"
-msgstr "POS-verkoop"
+msgstr "POS verkoop"
 
 msgctxt "model:sale.point.sale.line,name:"
 msgid "POS Sale Line"
-msgstr "POS-verkooplijn"
+msgstr "POS verkoopregel"
 
 msgctxt "selection:sale.point.cash.session,state:"
 msgid "Closed"
 msgstr "Afgesloten"
 
 msgctxt "selection:sale.point.cash.session,state:"
 msgid "Open"
@@ -638,15 +639,15 @@
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Cancelled"
 msgstr "Geannuleerd"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Afgerond"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Open"
 msgstr "Open"
 
 msgctxt "selection:sale.point.sale,state:"
 msgid "Posted"
@@ -658,15 +659,15 @@
 
 msgctxt "view:sale.point.sale:"
 msgid "Other Info"
 msgstr "Overige informatie"
 
 msgctxt "view:sale.point.sale:"
 msgid "Payments"
-msgstr "betalingen"
+msgstr "Betalingen"
 
 msgctxt "view:sale.point.sale:"
 msgid "Sale"
 msgstr "Verkoop"
 
 msgctxt "wizard_button:sale.point.sale.pay,payment,end:"
 msgid "Cancel"
```

### Comparing `trytond_sale_point-6.6.2/locale/pl.po` & `trytond_sale_point-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/pt.po` & `trytond_sale_point-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/ro.po` & `trytond_sale_point-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/ru.po` & `trytond_sale_point-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/sl.po` & `trytond_sale_point-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/tr.po` & `trytond_sale_point-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/uk.po` & `trytond_sale_point-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/locale/zh_CN.po` & `trytond_sale_point-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/message.xml` & `trytond_sale_point-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/product.py` & `trytond_sale_point-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/product.xml` & `trytond_sale_point-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/sale.py` & `trytond_sale_point-6.8.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,15 @@
         return True
 
     @classmethod
     def write(cls, *args):
         pool = Pool()
         Sale = pool.get('sale.point.sale')
         transaction = Transaction()
-        if (transaction.user != 0
-                and transaction.context.get('_check_access')):
+        if transaction.user and transaction.check_access:
             actions = iter(args)
             for points, values in zip(actions, actions):
                 if 'tax_included' in values:
                     for sub_points in grouped_slice(points):
                         if Sale.search([
                                     ('points', 'in',
                                         list(map(int, sub_points))),
@@ -232,16 +231,15 @@
 
     @classmethod
     def default_state(cls):
         return 'open'
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company and self.company.currency:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @fields.depends('lines')
     def on_change_with_total_tax(self, name=None):
         return sum(line.tax_amount for line in self.lines)
 
     @fields.depends('company', 'lines')
     def on_change_with_total(self, name=None):
@@ -355,15 +353,15 @@
 
     def get_account_move(self):
         'Return account move'
         pool = Pool()
         Move = pool.get('account.move')
         Period = pool.get('account.period')
 
-        period_id = Period.find(self.company.id, date=self.date)
+        period = Period.find(self.company, date=self.date)
         lines = []
         for line in self.lines:
             move_lines = line.get_account_move_lines()
             if move_lines:
                 lines.extend(move_lines)
 
         move_lines = self.get_tax_move_lines()
@@ -373,15 +371,15 @@
         for payment in self.payments:
             move_lines = payment.get_account_move_lines()
             if move_lines:
                 lines.extend(move_lines)
 
         move = Move()
         move.journal = self.point.journal
-        move.period = period_id
+        move.period = period
         move.date = self.date
         move.origin = self
         move.company = self.company
         move.lines = lines
         return move
 
     def get_tax_move_lines(self):
@@ -453,15 +451,18 @@
 
     sale = fields.Many2One(
         'sale.point.sale', "Sale", required=True, ondelete='CASCADE',
         states=_states)
     product = fields.Many2One(
         'product.product', "Product", required=True,
         domain=[
-            ('salable', '=', True),
+            If((Eval('sale_state') == 'open')
+                & ~(Eval('quantity', 0) < 0),
+                ('salable', '=', True),
+                ()),
             ],
         context={
             'company': Eval('company'),
             },
         states=_states, depends={'company'})
     quantity = fields.Float(
         "Quantity", digits='unit', required=True, states=_states)
@@ -506,16 +507,15 @@
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('sale')
 
     @fields.depends('product')
     def on_change_with_unit(self, name=None):
         # TODO packaging UOM
-        if self.product:
-            return self.product.sale_uom.id
+        return self.product.sale_uom if self.product else None
 
     @classmethod
     def get_sale_states(cls):
         pool = Pool()
         Sale = pool.get('sale.point.sale')
         return Sale.fields_get(['state'])['state']['selection']
 
@@ -570,25 +570,23 @@
             * (self.unit_price or Decimal('0')))
         if self.currency:
             return self.currency.round(amount)
         return amount
 
     @fields.depends('sale', '_parent_sale.company')
     def on_change_with_company(self, name=None):
-        if self.sale and self.sale.company:
-            return self.sale.company.id
+        return self.sale.company if self.sale else None
 
     @classmethod
     def search_company(cls, name, clause):
         return [('sale.company',) + tuple(clause[1:])]
 
     @fields.depends('sale', '_parent_sale.currency')
     def on_change_with_currency(self, name=None):
-        if self.sale and self.sale.currency:
-            return self.sale.currency.id
+        return self.sale.currency if self.sale else None
 
     @property
     def untax_amount(self):
         amount = (Decimal(str(self.quantity or 0))
             * (self.unit_list_price or Decimal('0')))
         if getattr(self, 'currency', None):
             amount = self.currency.round(amount)
@@ -871,16 +869,15 @@
 
     @classmethod
     def default_end_amount(cls):
         return Decimal(0)
 
     @fields.depends('point')
     def on_change_with_currency(self, name=None):
-        if self.point:
-            return self.point.company.currency.id
+        return self.point.company.currency if self.point else None
 
     @classmethod
     @Workflow.transition('open')
     def open(cls, sessions):
         pass
 
     @classmethod
@@ -1016,21 +1013,19 @@
     @fields.depends('sale', '_parent_sale.amount_to_pay')
     def on_change_sale(self):
         if self.sale:
             self.amount = self.sale.amount_to_pay
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company and self.company.currency:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @fields.depends('sale', '_parent_sale.company')
     def on_change_with_company(self, name=None):
-        if self.sale and self.sale.company:
-            return self.sale.company.id
+        return self.sale.company if self.sale else None
 
     @classmethod
     def search_company(cls, name, clause):
         return [('sale.company',) + tuple(clause[1:])]
 
     @classmethod
     def get_sale_states(cls):
@@ -1041,16 +1036,15 @@
     @fields.depends('sale', '_parent_sale.state')
     def on_change_with_sale_state(self, name=None):
         if self.sale:
             return self.sale.state
 
     @fields.depends('sale', '_parent_sale.point')
     def on_change_with_point(self, name=None):
-        if self.sale and self.sale.point:
-            return self.sale.point.id
+        return self.sale.point if self.sale else None
 
     @fields.depends('method')
     def on_change_with_cash(self, name=None):
         if self.method:
             return self.method.cash
 
     @classmethod
@@ -1247,21 +1241,19 @@
 
     @classmethod
     def default_date(cls):
         return Pool().get('ir.date').today()
 
     @fields.depends('point')
     def on_change_with_company(self, name=None):
-        if self.point:
-            return self.point.company.id
+        return self.point.company if self.point else None
 
     @fields.depends('point')
     def on_change_with_currency(self, name=None):
-        if self.point:
-            return self.point.company.currency.id
+        return self.point.company.currency if self.point else None
 
     @classmethod
     def delete(cls, transfers):
         for transfer in transfers:
             if transfer.state == 'posted':
                 raise AccessError(
                     gettext('sale_point.msg_transfer_delete_posted',
@@ -1296,28 +1288,28 @@
 
     def get_move(self, account):
         pool = Pool()
         Line = pool.get('account.move.line')
         Move = pool.get('account.move')
         Period = pool.get('account.period')
 
-        period_id = Period.find(self.company.id, date=self.date)
+        period = Period.find(self.company, date=self.date)
         line = Line()
         if self.amount >= 0:
             line.debit, line.credit = self.amount, Decimal(0)
         else:
             line.debit, line.credit = Decimal(0), -self.amount
         line.account = account
         counterpart = Line()
         counterpart.debit, counterpart.credit = line.credit, line.debit
         counterpart.account = self.type.account
 
         move = Move()
         move.journal = self.type.journal
-        move.period = period_id
+        move.period = period
         move.date = self.date
         move.origin = self
         move.company = self.company
         move.lines = [line, counterpart]
         return move
 
     @classmethod
```

### Comparing `trytond_sale_point-6.6.2/sale.xml` & `trytond_sale_point-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/sale_reporting.py` & `trytond_sale_point-6.8.0/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/setup.py` & `trytond_sale_point-6.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
     return content
 
 
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
@@ -37,16 +34,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_point'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
@@ -54,23 +54,23 @@
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for Point of Sales',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-sale-point/'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/sale_point',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton POS sale',
     package_dir={'trytond.modules.sale_point': '.'},
     packages=(
         ['trytond.modules.sale_point']
         + ['trytond.modules.sale_point.%s' % p for p in find_packages()]
         ),
@@ -107,24 +107,24 @@
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
         'Topic :: Office/Business :: Financial :: Accounting',
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

### Comparing `trytond_sale_point-6.6.2/tests/scenario_sale_point.rst` & `trytond_sale_point-6.8.0/tests/scenario_sale_point.rst`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     >>> sale.total
     Decimal('6036.00')
     >>> sale.total_tax
     Decimal('1047.55')
 
 Overpay by terminal::
 
-    >>> payment = Wizard('sale.point.sale.pay', [sale])
+    >>> payment = sale.click('pay')
     >>> payment.form.method = terminal_method
     >>> payment.form.amount
     Decimal('6036.00')
     >>> payment.form.amount = Decimal('6100.00')
     >>> payment.execute('pay')
 
     >>> payment.form.method == cash_method
```

### Comparing `trytond_sale_point-6.6.2/tests/scenario_sale_point_reporting.rst` & `trytond_sale_point-6.8.0/tests/scenario_sale_point_reporting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     >>> sale = Sale(point=pos)
     >>> line = sale.lines.new()
     >>> line.product = goods
     >>> line.quantity = 1
     >>> sale.save()
 
-    >>> payment = Wizard('sale.point.sale.pay', [sale])
+    >>> payment = sale.click('pay')
     >>> payment.form.method = cash_method
     >>> payment.execute('pay')
 
 Check sale reporting::
 
     >>> Reporting = Model.get('sale.reporting.main')
     >>> context = dict(
```

### Comparing `trytond_sale_point-6.6.2/tests/scenario_sale_point_return.rst` & `trytond_sale_point-6.8.0/tests/scenario_sale_point_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/tests/scenario_sale_point_session.rst` & `trytond_sale_point-6.8.0/tests/scenario_sale_point_session.rst`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     >>> line.quantity = 1
     >>> sale.save()
     >>> sale.total
     Decimal('20.00')
 
 Pay by cash::
 
-    >>> payment = Wizard('sale.point.sale.pay', [sale])
+    >>> payment = sale.click('pay')
     >>> payment.form.method = cash_method
     >>> payment.form.amount
     Decimal('20.00')
     >>> payment.execute('pay')
 
     >>> sale.state
     'done'
```

### Comparing `trytond_sale_point-6.6.2/tests/scenario_sale_point_tax_excluded.rst` & `trytond_sale_point-6.8.0/tests/scenario_sale_point_tax_excluded.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/tox.ini` & `trytond_sale_point-6.8.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/sale_point/* -m unittest discover -s tests
-    coverage report --include=./**/sale_point/* --omit=*/tests/*
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

### Comparing `trytond_sale_point-6.6.2/trytond_sale_point.egg-info/PKG-INFO` & `trytond_sale_point-6.8.0/trytond_sale_point.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-point
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-point/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_point
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton POS sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 #################
 Sale Point Module
 #################
```

### Comparing `trytond_sale_point-6.6.2/trytond_sale_point.egg-info/SOURCES.txt` & `trytond_sale_point-6.8.0/trytond_sale_point.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/view/cash_session_form.xml` & `trytond_sale_point-6.8.0/view/cash_session_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/view/cash_transfer_form.xml` & `trytond_sale_point-6.8.0/view/cash_transfer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/view/point_form.xml` & `trytond_sale_point-6.8.0/view/point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/view/sale_form.xml` & `trytond_sale_point-6.8.0/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.6.2/view/sale_line_form.xml` & `trytond_sale_point-6.8.0/view/sale_line_form.xml`

 * *Files identical despite different names*

