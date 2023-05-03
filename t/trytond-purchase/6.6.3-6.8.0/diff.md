# Comparing `tmp/trytond_purchase-6.6.3.tar.gz` & `tmp/trytond_purchase-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-6.6.3.tar", last modified: Wed May  3 16:50:11 2023, max compression
+gzip compressed data, was "trytond_purchase-6.8.0.tar", last modified: Mon May  1 11:45:48 2023, max compression
```

## Comparing `trytond_purchase-6.6.3.tar` & `trytond_purchase-6.8.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.037030 trytond_purchase-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     6311 2023-05-03 16:50:07.000000 trytond_purchase-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-03 16:50:06.000000 trytond_purchase-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2737 2023-05-03 16:50:11.037030 trytond_purchase-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4665 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.033696 trytond_purchase-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_purchase-6.6.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.033696 trytond_purchase-6.6.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/doc/usage/prepurchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4855 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.033696 trytond_purchase-6.6.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5669 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.017029 trytond_purchase-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    35592 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35328 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30883 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35743 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35471 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30371 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32518 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37533 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30870 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35601 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34532 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31521 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34043 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35508 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33653 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35638 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32124 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33812 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30149 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36104 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33482 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30861 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    29262 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33860 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3533 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2177 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19384 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-08 09:35:50.000000 trytond_purchase-6.6.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    78119 2023-04-22 21:24:47.000000 trytond_purchase-6.6.3/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28088 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11493 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:50:11.037030 trytond_purchase-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4565 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9675 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5694 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.020363 trytond_purchase-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19258 2023-04-08 09:35:50.000000 trytond_purchase-6.6.3/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3145 2023-04-08 09:35:50.000000 trytond_purchase-6.6.3/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.037030 trytond_purchase-6.6.3/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2737 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4734 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-15 18:00:51.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:50:10.000000 trytond_purchase-6.6.3/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:50:11.030363 trytond_purchase-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      785 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3483 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1630 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      569 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2022-12-19 12:02:50.000000 trytond_purchase-6.6.3/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-04-08 09:35:50.000000 trytond_purchase-6.6.3/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-13 16:52:41.000000 trytond_purchase-6.6.3/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.248875 trytond_purchase-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6583 2023-05-01 11:03:55.000000 trytond_purchase-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:03:55.000000 trytond_purchase-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-01 11:45:48.245541 trytond_purchase-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/prepurchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4855 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.232208 trytond_purchase-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37471 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37513 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32682 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38008 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37693 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32179 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34342 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39508 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32669 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37860 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36612 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33346 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35879 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37467 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35472 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37911 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33939 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35630 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31956 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37996 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35318 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32660 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30987 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35757 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19452 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    82990 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32163 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11720 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:48.248875 trytond_purchase-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9634 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.235541 trytond_purchase-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19171 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1676 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3009 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3025 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-05-01 11:03:49.000000 trytond_purchase-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.245541 trytond_purchase-6.8.0/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4760 2023-05-01 11:45:48.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.238875 trytond_purchase-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3481 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-28 07:46:16.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-28 07:46:16.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/template_tree.xml
```

### Comparing `trytond_purchase-6.6.3/CHANGELOG` & `trytond_purchase-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
-Version 6.6.3 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.2 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-01-15
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Fill taxes from default account for line without product
+* Add partially shipped to shipment state
+* Add pending, awaiting payment and partially paid to invoice state
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Add related stock moves and invoice lines on purchase line
+* Add relate to purchase lines from party and product
+* Simplify relate to purchases
+* Prevent creation of lines for non draft purchases
+* Allow searching reporting records by name
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add reporting
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_purchase-6.6.3/COPYRIGHT` & `trytond_purchase-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/LICENSE` & `trytond_purchase-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/PKG-INFO` & `trytond_purchase-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 ###############
 Purchase Module
 ###############
```

### Comparing `trytond_purchase-6.6.3/__init__.py` & `trytond_purchase-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/configuration.py` & `trytond_purchase-6.8.0/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # this repository contains the full copyright notices and license terms.
 from trytond import backend
 from trytond.model import (
     ModelSingleton, ModelSQL, ModelView, ValueMixin, fields)
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.pool import Pool
-from trytond.pyson import Eval, Id
+from trytond.pyson import Eval, Id, TimeDelta
 from trytond.tools.multivalue import migrate_property
 
 purchase_invoice_method = fields.Selection(
     'get_purchase_invoice_method', "Invoice Method")
 
 
 def get_purchase_methods(field_name):
@@ -32,15 +32,20 @@
                 ('company', 'in',
                     [Eval('context', {}).get('company', -1), None]),
                 ('sequence_type', '=',
                     Id('purchase', 'sequence_type_purchase')),
                 ]))
     purchase_invoice_method = fields.MultiValue(purchase_invoice_method)
     get_purchase_invoice_method = get_purchase_methods('invoice_method')
-    purchase_process_after = fields.TimeDelta("Process Purchase after",
+    purchase_process_after = fields.TimeDelta(
+        "Process Purchase after",
+        domain=['OR',
+            ('purchase_process_after', '=', None),
+            ('purchase_process_after', '>=', TimeDelta()),
+            ],
         help="The grace period during which confirmed purchase "
         "can still be reset to draft.\n"
         "Applied only if a worker queue is activated.")
 
     @classmethod
     def multivalue_model(cls, field):
         pool = Pool()
```

### Comparing `trytond_purchase-6.6.3/configuration.xml` & `trytond_purchase-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/doc/conf.py` & `trytond_purchase-6.8.0/doc/conf.py`

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

### Comparing `trytond_purchase-6.6.3/doc/design.rst` & `trytond_purchase-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/doc/usage/prepurchase.rst` & `trytond_purchase-6.8.0/doc/usage/prepurchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/doc/usage/process.rst` & `trytond_purchase-6.8.0/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/doc/usage/returns.rst` & `trytond_purchase-6.8.0/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/icons/LICENSE` & `trytond_purchase-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/invoice.py` & `trytond_purchase-6.8.0/invoice.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # this repository contains the full copyright notices and license terms.
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
-from trytond.transaction import Transaction
+from trytond.pyson import Eval
+from trytond.transaction import Transaction, without_check_access
 
 
 def process_purchase(func):
     @wraps(func)
     def wrapper(cls, invoices):
         pool = Pool()
         Purchase = pool.get('purchase.purchase')
         transaction = Transaction()
         context = transaction.context
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             purchases = set(
                 p for i in cls.browse(invoices) for p in i.purchases)
         func(cls, invoices)
         if purchases:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
                 Purchase.__queue__.process(purchases)
@@ -57,32 +58,23 @@
         for line in self.lines:
             if isinstance(line.origin, PurchaseLine):
                 purchases.add(line.origin.purchase.id)
         return list(purchases)
 
     @classmethod
     def search_purchases(cls, name, clause):
-        return [('lines.origin.purchase' + clause[0].lstrip(name),)
-            + tuple(clause[1:3]) + ('purchase.line',) + tuple(clause[3:])]
+        return [('lines.origin.purchase' + clause[0][len(name):],
+                *clause[1:3], 'purchase.line', *clause[3:])]
 
     @classmethod
     @process_purchase
     def delete(cls, invoices):
         super(Invoice, cls).delete(invoices)
 
     @classmethod
-    def copy(cls, invoices, default=None):
-        if default is None:
-            default = {}
-        else:
-            default = default.copy()
-        default.setdefault('purchases', None)
-        return super(Invoice, cls).copy(invoices, default=default)
-
-    @classmethod
     @ModelView.button
     @Workflow.transition('draft')
     def draft(cls, invoices):
         for invoice in invoices:
             if invoice.purchases and invoice.state == 'cancelled':
                 raise AccessError(
                     gettext('purchase.msg_purchase_invoice_reset_draft',
@@ -105,25 +97,34 @@
     def cancel(cls, invoices):
         super(Invoice, cls).cancel(invoices)
 
 
 class InvoiceLine(metaclass=PoolMeta):
     __name__ = 'account.invoice.line'
 
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        if not cls.origin.domain:
+            cls.origin.domain = {}
+        cls.origin.domain['purchase.line'] = [
+            ('type', '=', Eval('type')),
+            ]
+
     @fields.depends('origin')
     def on_change_with_product_uom_category(self, name=None):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
         category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to invoice and the quantity to receive.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, PurchaseLine)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     def get_warehouse(self, name):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
         warehouse = super().get_warehouse(name)
         if (not warehouse
@@ -149,15 +150,15 @@
 
     @classmethod
     def delete(cls, lines):
         pool = Pool()
         Purchase = pool.get('purchase.purchase')
         transaction = Transaction()
         context = transaction.context
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             invoices = (l.invoice for l in cls.browse(lines)
                 if l.type == 'line' and l.invoice)
             purchases = set(p for i in invoices for p in i.purchases)
         super(InvoiceLine, cls).delete(lines)
         if purchases:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
```

### Comparing `trytond_purchase-6.6.3/locale/bg.po` & `trytond_purchase-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -189,30 +189,32 @@
 msgid "From Location"
 msgstr "От местонахождение"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Редове от фактура"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Направени движения"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Грешка при движение"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Движения"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Грешка при движение"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Игнорирани движения"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Направени движения"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Наново създаване на движения"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Бележка"
@@ -230,26 +232,36 @@
 msgstr "Категория мер. ед. на продукт"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Покупка"
 
 #, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Дата на покупка"
+
+#, fuzzy
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Дата на покупка"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Количество"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Доставчик"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Данъци"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Към местонахождение"
@@ -262,14 +274,19 @@
 msgid "Unit"
 msgstr "Единица"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Единична цена"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Склад"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Ред от покупка"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Данък"
@@ -599,14 +616,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -627,14 +650,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Минимално количество"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -675,35 +704,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Purchases"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Покупки"
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Ред от покупка"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Движения"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Покупки"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Покупки"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Покупки"
 
 #, fuzzy
@@ -795,14 +826,43 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Запитване"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Приключен"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Приключен"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -817,14 +877,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1238,38 +1304,50 @@
 msgstr "Въз основа на изпращане"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Ръчно"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Грешка"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Няма"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Платен"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Изчакващ"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Грешка"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Няма"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Получен"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Изчакващ"
```

### Comparing `trytond_purchase-6.6.3/locale/ca.po` & `trytond_purchase-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Moviments finalitzats"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Moviments en excepció"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Moviments en excepció"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Moviments ignorats"
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progres dels moviments"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Moviments recreats"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -211,26 +211,34 @@
 msgid "Product Uom Category"
 msgstr "Categoria UdM del producte"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Data compra"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Estat de compra"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Quantitat"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Resum"
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Proveïdor"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Impostos"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "A la ubicació"
@@ -243,14 +251,18 @@
 msgid "Unit"
 msgstr "Unitat"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Preu unitari"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Magatzem"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Línia de compra"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Impost"
@@ -565,14 +577,22 @@
 "El temps que es tarda a rebre els béns després de la confirmació de l'oferta quan el tercer s'utilitza com a proveïdor:\n"
 "Utilitzat quan no hi ha temps d'espera al producte de proveïdor."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr "La moneda per defecte per les compres d'aquest tercer."
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"El temps des de la confirmació de l'oferta fins a la recepció dels bens quan el tercer s'utilitza com a proveïdor.\n"
+"Utilitzat quan no hi ha temps d'espera al producte de proveïdor."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "El període durant el qual una compra confirmada es pot tornar a passar a esborrany.\n"
 "Aplica només si la cua de treballs està activada."
@@ -594,14 +614,22 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "El temps desde la confirmació de la comanda fins a la recepció dels productes:\n"
 "Si es deixa en blanc s'utilitza el temps d'espera del proveïdor."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+"Afegiu un preu per diferents criteris.\n"
+"S'utilitza l'ultima línia que coincideix."
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Quantitat mínima."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "La unitat en que s'especifica la quantitat."
@@ -634,31 +662,31 @@
 msgid "Configuration"
 msgstr "Configuració"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Compres"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Compres"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Compres"
 
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Línies de compra"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Moviments"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Compres"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Compres"
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Compres"
 
@@ -735,14 +763,39 @@
 msgstr "En procés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pressupost"
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Finalitzada"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr "Pendent"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Finalitzada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr "Pendent"
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "Esteu intentar modificar la UdM de compra en la que es basen els preus de "
 "compra."
@@ -763,14 +816,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "No podeu restaurar a esborrany la factura \"%(invoice)s\" perquè ha estat "
 "generada per una compra."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+"No podeu afegir línies a la compra \"%(purchase)s\" perquè ja no està en "
+"estat esborrany."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "Per eliminar la línia de compra \"%(line)s\" heu de cancel·lar o restablir a"
 " esborrany la compra \"%(purchase)s\"."
@@ -1175,38 +1236,50 @@
 msgstr "Basat en l'enviament"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "En espera de pagament"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Excepció"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Cap"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Pagada"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "En espera"
+msgid "Partially Paid"
+msgstr "Pagada parcialment"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr "Pendent"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Excepció"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Cap"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Enviada parcialment"
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Rebuda"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "En espera"
```

### Comparing `trytond_purchase-6.6.3/locale/cs.po` & `trytond_purchase-6.8.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,30 +175,31 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -216,26 +217,36 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Purchases"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Purchases"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Product Suppliers"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -248,14 +259,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr ""
@@ -585,14 +600,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -610,14 +631,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -652,31 +679,34 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
 msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Purchases"
@@ -760,14 +790,41 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -782,14 +839,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1201,38 +1264,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/de.po` & `trytond_purchase-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Erledigte Warenbewegungen"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Warenbewegungen mit Vorbehalt"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Warenbewegungen mit Vorbehalt"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignorierte Warenbewegungen"
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Lieferfortschritt"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Neu erstellte Warenbewegungen"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Notiz"
@@ -211,26 +211,34 @@
 msgid "Product Uom Category"
 msgstr "Maßeinheitenkategorie"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Einkauf"
 
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Bestelldatum"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Einkaufsstatus"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Menge"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Kurzbeschreibung"
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Lieferant"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Steuern"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Zu Lagerort"
@@ -243,14 +251,18 @@
 msgid "Unit"
 msgstr "Einheit"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Einzelpreis"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Logistikstandort"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Einkaufsposition"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Steuer"
@@ -566,14 +578,22 @@
 "Die Zeit zwischen der Bestellbestätigung und dem Erhalt der Ware bei Nutzung der Partei als Lieferant.\n"
 "Wird genutzt sofern auf dem Lieferantendatensatz keine Beschaffungszeit erfasst wurde."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr "Standardwährung für Einkäufe bei dieser Partei."
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"Die Zeit zwischen der Bestellbestätigung und dem Erhalt der Ware bei Nutzung der Partei als Lieferant.\n"
+"Wird genutzt sofern auf dem Lieferantendatensatz keine Beschaffungszeit erfasst wurde."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "Frist innerhalb der eine Bestellung noch auf Entwurf zurückgesetzt werden kann.\n"
 "Wird nur angewandt, wenn die Warteschlange aktiviert ist."
@@ -599,14 +619,22 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "Die Zeit zwischen der Bestellbestätigung und dem Erhalt der Ware.\n"
 "Wenn leer wird die Standardbeschaffungszeit des Lieferanten genutzt."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+"Erlaubt die Erfassung von Preisen für unterschiedliche Kriterien.\n"
+"Die letzte Zeile mit übereinstimmenden Kriterien wird verwendet."
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Minimale Menge."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "Die Maßheit in der die Menge angegeben ist."
@@ -639,31 +667,31 @@
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Einkäufe"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Einkäufe"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Einkäufe"
 
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Einkaufspositionen"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Einkäufe"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Einkäufe"
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Einkäufe"
 
@@ -740,14 +768,39 @@
 msgstr "In Ausführung"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Anfrage"
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Erledigt"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr "Ausstehend"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Erledigt"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr "Ausstehend"
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "Sie versuchen die Maßeinheit Einkauf zu ändern, auf der die Einkaufspreise "
 "basieren."
@@ -768,14 +821,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht auf den Entwurfsstatus\" zurückgesetzt "
 "werden, weil sie durch einen Einkauf erzeugt wurde."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+"Zu Einkauf \"%(purchase)s\" kann keine Position mehr hinzugefügt werden, da "
+"er nicht mehr im Entwurfsstatus ist."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "Um Einkaufsposition \"%(line)s\" zu löschen, muss zuerst der Einkauf "
 "\"%(purchase)s\" annulliert oder zurück auf den Entwurfsstatus gesetzt "
@@ -1181,38 +1242,50 @@
 msgstr "Bei Lieferung"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manuell"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "Zahlung Ausstehend"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Vorbehalt"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Kein"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Bezahlt"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Wartend"
+msgid "Partially Paid"
+msgstr "Teilweise Bezahlt"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr "Ausstehend"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Vorbehalt"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Kein"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Teilweise Versendet"
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Erhalten"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Wartend"
```

### Comparing `trytond_purchase-6.6.3/locale/es.po` & `trytond_purchase-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Movimientos finalizados"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Movimientos en excepción"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Movimientos en excepción"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimientos ignorados"
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progreso de los movimientos"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Movimientos recreados"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -211,26 +211,34 @@
 msgid "Product Uom Category"
 msgstr "Categoría UdM del producto"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Fecha de compra"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Estado de la compra"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Cantidad"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Resumen"
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Proveedor"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Impuestos"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "A ubicación"
@@ -243,14 +251,18 @@
 msgid "Unit"
 msgstr "Unidad"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Precio unitario"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Almacén"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Línea de compra"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Impuesto"
@@ -566,14 +578,22 @@
 "El tiempo desde que se ha confirmado el pedido de compra hasta recibir los bienes del tercero se utiliza como proveedor.\n"
 "Usado si no hay tiempo de espera establecido en el proveedor del producto."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr "La moneda por defecto para las compras de este tercero."
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"El tiempo desde que se ha confirmado el pedido de compra hasta recibir los bienes del tercero cuando se utiliza como proveedor.\n"
+"Usado si no hay tiempo de espera establecido en el proveedor del producto."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "El periodo durante el cual una compra confirmada se puede volver a estado borrador.\n"
 "Solo aplica si la cola de trabajos está activada."
@@ -597,14 +617,22 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "El tiempo desde que se ha confirmado el pedido de compra hasta recibir los productos.\n"
 "Si está vacío se usa el tiempo de espera del proveedor."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+"Añade un precio con distintos criterios.\n"
+"Se utiliza la última línea que coincide."
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Cantidad mínima."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "La unidad en que se especifica la cantidad."
@@ -637,31 +665,31 @@
 msgid "Configuration"
 msgstr "Configuración"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Compras"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Compras"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Compras"
 
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Líneas de compra"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Movimientos"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Compras"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Compras"
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Compras"
 
@@ -738,14 +766,39 @@
 msgstr "En proceso"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Presupuesto"
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Finalizada"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr "Pendiente"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Finalizada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr "Pendiente"
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "Está intentando modificar la UdM de compra en la que se basan los precios de"
 " compra."
@@ -766,14 +819,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "No puede restaurar a borrador la factura \"%(invoice)s\" porque se generó "
 "por una compra."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+"No se puede añadir líneas a la compra \"%(purchase)s\", porqué noe està en "
+"estado borrador."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "Para eliminar la línea \"%(line)s\" debe cancelar o restablecer a borrador "
 "la compra \"%(purchase)s\"."
@@ -1178,38 +1239,50 @@
 msgstr "Basado en el envío"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "A la espera de pago"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Excepción"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Ninguno"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Pagada"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "En espera"
+msgid "Partially Paid"
+msgstr "Pagada parcialmente"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr "Pendiente"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Excepción"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Ninguno"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Enviada parcialmente"
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Recibida"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "En espera"
```

### Comparing `trytond_purchase-6.6.3/locale/es_419.po` & `trytond_purchase-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -176,30 +176,31 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Estado de excepción"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -216,26 +217,36 @@
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Orden de compra Nº:"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Devolución a proveedor"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -248,14 +259,19 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Precio unitario"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Bodega"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr ""
@@ -577,14 +593,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -602,14 +624,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -644,31 +672,32 @@
 msgid "Configuration"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Proveedores de producto"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr ""
 
@@ -749,14 +778,39 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -771,14 +825,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1175,38 +1235,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/et.po` & `trytond_purchase-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -182,30 +182,32 @@
 msgid "From Location"
 msgstr "Asukohast"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Arveread"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Lõpetatud liikumised"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Liikumiste erand"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Liikumised"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Liikumiste erand"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignoreeritud liikumised"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Lõpetatud liikumised"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Taasloodud liikumised"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Märkus"
@@ -222,26 +224,36 @@
 msgid "Product Uom Category"
 msgstr "Toote mõõtühiku kategooria"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Ost"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Ostu kuupäev"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Ostu olek"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Kogus"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Hankija"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Maksud"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Asukohta"
@@ -254,14 +266,19 @@
 msgid "Unit"
 msgstr "Ühik"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Ühiku hind"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Ladu"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Ostu rida"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Maks"
@@ -586,14 +603,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -611,14 +634,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Miinimumkogus"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -654,32 +683,35 @@
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Ostud"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Ostud"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Ostud"
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Ostu rida"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Liikumised"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Ostud"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Ostud"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Ostud"
@@ -764,14 +796,43 @@
 msgstr "Käitluses"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pakkumine"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Kõik"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Tehtud"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Kõik"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Tehtud"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -786,14 +847,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1206,38 +1273,50 @@
 msgstr "Põhineb tarnel"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Käsitsi"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Erand"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Mitte"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Tasutud"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Ootel"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Erand"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Mitte"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Saabunud"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Ootel"
```

### Comparing `trytond_purchase-6.6.3/locale/fa.po` & `trytond_purchase-6.8.0/locale/fa.po`

 * *Files 5% similar despite different names*

```diff
@@ -185,30 +185,32 @@
 msgid "From Location"
 msgstr "از مکان"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "خطوط صورتحساب"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "جابجایی ها انجام شد"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "جابجایی های اعتراضی"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "جابجایی ها"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "جابجایی های اعتراضی"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "جابجایی های نادیده گرفته شده"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "جابجایی ها انجام شد"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "جابجایی های دوباره انجام شده"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "توجه"
@@ -225,26 +227,36 @@
 msgid "Product Uom Category"
 msgstr "دسته بندی واحد اندازه گیری محصول"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "خرید"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "تاریخ خرید"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "وضعیت خرید"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "مقدار/تعداد"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "تامین کننده"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "مالیات ها"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "به مکان"
@@ -257,14 +269,19 @@
 msgid "Unit"
 msgstr "واحد"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "قیمت واحد"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "انبار"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "خط خرید"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "مالیات"
@@ -591,14 +608,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "دوره فصلی که در آن تأیید خرید هنوز می تواند به پیش نویس مجدد تنظیم مجدد "
 "شود.فقط اگر یک کارگر فعال باشد اعمال می شود."
@@ -620,14 +643,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "حداقل مقدار"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -664,34 +693,37 @@
 msgid "Configuration"
 msgstr "پیکربندی"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "خریدها"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "خریدها"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "خریدها"
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "خط خرید"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "جابجایی ها"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "خریدها"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "خریدها"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "خریدها"
 
 #, fuzzy
@@ -774,14 +806,43 @@
 msgstr "در حال پردازش"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "نقل قول"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "همه"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "انجام شد"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "همه"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "انجام شد"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "شما در حال تلاش برای تغییرواحد قیمت خرید هستید، که قیمت خرید بر مبنای آن "
 "متکی است."
@@ -802,14 +863,21 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "شما نمیتوانید حالت صورتحساب: \"%(invoice)s\"را به پیش نویس تغیر دهید چراکه "
 "بوسیله یک خرید تولید شده است."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr "برای تغییر عنوان خرید:\"%(purchase)s\" باید در حالت پیش نویس باشد."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "برای حذف سطر: \"%(line)s\" شما باید خرید : \"%(purchase)s\" را لغو یا به "
 "حالت پیش نویس تغیر دهید."
@@ -1227,38 +1295,50 @@
 msgstr "براساس محموله"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "دستی"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "اعتراض"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "هیجکدام"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "پرداخت شده"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "در انتظار"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "اعتراض"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "هیجکدام"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "دریافت شده"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "در انتظار"
```

### Comparing `trytond_purchase-6.6.3/locale/fi.po` & `trytond_purchase-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,30 +175,31 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -216,26 +217,36 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Purchases"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Purchases"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Product Suppliers"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -248,14 +259,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr ""
@@ -584,14 +599,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -609,14 +630,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -651,31 +678,34 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
 msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Purchases"
@@ -759,14 +789,41 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -781,14 +838,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1200,38 +1263,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/fr.po` & `trytond_purchase-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr "Emplacement d'origine"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Lignes de facture"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Mouvements effectués"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Mouvements en exception"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mouvements en exception"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mouvements ignorés"
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progression des mouvements"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mouvements recréés"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Note"
@@ -211,26 +211,34 @@
 msgid "Product Uom Category"
 msgstr "Catégorie d'unité de mesure"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Achat"
 
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Date d'achat"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "État de l'achat"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Quantité"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Résumé"
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Fournisseur"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Taxes"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Emplacement de destination"
@@ -243,14 +251,18 @@
 msgid "Unit"
 msgstr "Unité"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Prix unitaire"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Entrepôt"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Ligne d'achat"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Taxe"
@@ -566,14 +578,22 @@
 "Le temps entre la confirmation de l'achat et la réception des biens dutiers lorsqu'il est utilisée en tant que fournisseur.\n"
 "Utilisé si aucun délai de livraison n'est défini sur le fournisseur du produit."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr "Devise par défaut pour les achats à ce tiers."
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"Le temps entre la confirmation de l'achat et la réception des biens du tiers lorsqu'il est utilisée en tant que fournisseur.\n"
+"Utilisé si aucun délai de livraison n'est défini sur le produit fournisseur."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "La période de grâce pendant laquelle un achat confirmé peut toujours être réinitialiser à l'état brouillon.\n"
 "S'applique si une file d'attente de travailleurs est activée."
@@ -597,14 +617,22 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "Le temps entre la confirmation du l'achat et la réception des produits.\n"
 "S'il est vide, le délai de livraison du fournisseur est utilisé."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+"Ajouter un prix pour différents critères.\n"
+"La dernière ligne correspondante est utilisée."
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Quantité minimale."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "L'unité dans laquelle la quantité est spécifiée."
@@ -637,31 +665,31 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Achats"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Achats"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Achats"
 
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Lignes d'achat"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Mouvements"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Achats"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Achats"
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Achats"
 
@@ -738,14 +766,39 @@
 msgstr "En traitement"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Devis"
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Toutes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Terminées"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr "En attentes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Tous"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Terminés"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr "En attentes"
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "Vous essayez de changer l'UDM d'achat sur laquelle le prix d'achat est basé."
 
@@ -765,14 +818,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Vous ne pouvez réinitialiser la facture « %(invoice)s » à l'état brouillon "
 "car elle a été générée par un achat."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+"Vous ne pouvez pas ajouter de lignes à l'achat « %(purchase)s » car il n'est"
+" plus dans l'état brouillon."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "Pour supprimer la ligne « %(line)s », vous devez annuler ou réinitialiser à "
 "l'état brouillon l'achat « %(purchase)s »."
@@ -1177,38 +1238,50 @@
 msgstr "Basé sur l'expédition"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manuel"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "En attente de paiement"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Exception"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Aucun"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Payée"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr "Partiellement payé"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr "En attente"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Exception"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Aucun"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Partiellement expédié"
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Reçu"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "En attente"
```

### Comparing `trytond_purchase-6.6.3/locale/hu.po` & `trytond_purchase-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -176,30 +176,31 @@
 msgid "From Location"
 msgstr "Induló tárhely"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Számlasorok"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Mozgások"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "visszautasítva"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Jegyzetek"
@@ -216,26 +217,36 @@
 msgid "Product Uom Category"
 msgstr "Mértékegység kategória"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Beszerzési rendelés"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Rendelés dátuma"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Mennyiség"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Leírás"
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Szállító"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Adók"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Cél tárhely"
@@ -248,14 +259,19 @@
 msgid "Unit"
 msgstr "Mértékegység"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Egységár"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Raktár"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Beszerzési rendelés sora"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Adó"
@@ -579,14 +595,23 @@
 "Az átfutási idő a beszerzési rendelés jóváhagyásától az áru átvételéig, ha ettől a szállítótól rendelünk.\n"
 "Akkor használja a rendszer, ha nincs más megadva a termékspecifikus szállítói információnál."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+#, fuzzy
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"Az átfutási idő a beszerzési rendelés jóváhagyásától az áru átvételéig, ha ettől a szállítótól rendelünk.\n"
+"Akkor használja a rendszer, ha nincs más megadva a termékspecifikus szállítói információnál."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -610,14 +635,20 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "Az átfutási idő a beszerzési rendelés jóváhagyásától az áru átvételéig.\n"
 "Ha üres, a szállítónál megadott átfutási időt használja a rendszer."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "A megadott egységárhoz szükséges legkisebb rendelési mennyiség."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "Ebben a mértékegységben van a mennyiség megadva."
@@ -650,31 +681,34 @@
 msgid "Configuration"
 msgstr "Beállítások"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Beszerzési rendelések"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Beszerzési rendelések"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Beszerzési rendelések"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Beszerzési rendelés sora"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Készletmozgások"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Beszerzési rendelések"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Beszerzési rendelések"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Beszerzési rendelések"
@@ -757,14 +791,43 @@
 msgstr "folyamatban"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "ajánlatkérés"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "összes"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Kész"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "összes"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Kész"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -779,14 +842,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1197,38 +1266,50 @@
 msgstr "szállítmányról"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "kézzel"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "visszautasítva"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "nincs"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Fizetve"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "várakozik"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "visszautasítva"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "nincs"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "átvett"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "várakozik"
```

### Comparing `trytond_purchase-6.6.3/locale/id.po` & `trytond_purchase-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -179,30 +179,32 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Baris Faktur"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Perpindahan Selesai"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Perpindahan"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Perpindahan Selesai"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Perpindahan Selesai"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Catatan"
@@ -219,26 +221,36 @@
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Pembelian"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Tanggal Pembelian"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Ringkasan"
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Pemasok"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Pajak-Pajak"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -251,14 +263,19 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Harga Satuan"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Gudang"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Baris Pembelian"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Pajak"
@@ -582,14 +599,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -607,14 +630,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -648,34 +677,37 @@
 msgid "Configuration"
 msgstr "Konfigurasi"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Pembelian"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr ""
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Baris Pembelian"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Perpindahan"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr ""
+msgstr "Pembelian"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr ""
+msgstr "Pembelian"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Pembelian"
 
 #, fuzzy
@@ -755,14 +787,39 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -777,14 +834,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1196,38 +1259,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Tidak ada"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Tidak ada"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/it.po` & `trytond_purchase-6.8.0/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -180,30 +180,32 @@
 msgid "From Location"
 msgstr "Da locazione"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Righe fattura"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Movimenti eseguiti"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "eccezione movimenti"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "eccezione movimenti"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimenti non considerati"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Movimenti eseguiti"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Movimenti ricreati"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -220,26 +222,36 @@
 msgid "Product Uom Category"
 msgstr "Categotia UdM prodotto"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Acquisto"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Data acquisto"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Stato ordine di acquisto"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Quantità"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Fornitore"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Imposte"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "A Locazione"
@@ -252,14 +264,19 @@
 msgid "Unit"
 msgstr "Unità"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Prezzo Unitario"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Magazzino"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Riga ordine di acquisto"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Imposta"
@@ -585,14 +602,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "Il periodo di tolleranza durante il quale l'acquisto confermato può ancora essere resettato in bozza.\n"
 "Applicato solo se è attivata una coda di lavoro."
@@ -615,14 +638,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Quantità minima."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -658,31 +687,34 @@
 msgid "Configuration"
 msgstr "Configurazione"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Acquisti"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Acquisti"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Acquisti"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Riga ordine di acquisto"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Movimenti"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Acquisti"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Acquisti"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Acquisti"
@@ -770,14 +802,43 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Preventivo"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Tutti"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Fatto"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Tutti"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Fatto"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -795,14 +856,20 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Non è possibile riportare a bozza il movimento \"%s\" perché è stato "
 "generato da un ordine di acquisto."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1218,38 +1285,50 @@
 msgstr "Basato su spedizione"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manuale"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Eccezione"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Nessuno"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Pagato"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "In attesa"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Eccezione"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Nessuno"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Ricevuto"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "In attesa"
```

### Comparing `trytond_purchase-6.6.3/locale/lo.po` & `trytond_purchase-6.8.0/locale/lo.po`

 * *Files 4% similar despite different names*

```diff
@@ -188,31 +188,32 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "ລາຍການເກັບເງິນ"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 #, fuzzy
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "ສະຖານະຍົກເວັ້ນ"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,note:"
 msgid "Note"
@@ -232,26 +233,36 @@
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "ສັ່ງຊື້"
 
 #, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "ວັນທີຈັດຊື້"
+
+#, fuzzy
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "ວັນທີຈັດຊື້"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "ຈຳນວນ"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "ຜູ້ສະໜອງ"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "ອາກອນ"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -267,14 +278,18 @@
 msgstr "ໜ່ວຍ"
 
 #, fuzzy
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "ລາຄາຫົວໜ່ວຍ"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "ວັນທີຈັດຊື້"
 
 #, fuzzy
 msgctxt "field:purchase.line-account.tax,tax:"
@@ -632,14 +647,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -657,14 +678,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -702,35 +729,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "ການຈັດຊື້"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "ການຈັດຊື້"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
-msgstr "ການຈັດຊື້"
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "ວັນທີຈັດຊື້"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "ການຈັດຊື້"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "ການຈັດຊື້"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "ການຈັດຊື້"
 
 #, fuzzy
@@ -818,14 +847,43 @@
 msgstr "ກຳລັງດຳເນີນການ"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "ທັງໝົດ"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "ແລ້ວໆ"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "ທັງໝົດ"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "ແລ້ວໆ"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -840,14 +898,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1275,41 +1339,53 @@
 
 #, fuzzy
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "ໃສ່ເອົາເອງ"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "ບໍ່ມີ"
 
 #, fuzzy
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "ຈ່າຍແລ້ວ"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "ບໍ່ມີ"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/lt.po` & `trytond_purchase-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -185,30 +185,32 @@
 msgid "From Location"
 msgstr "Išsiuntimo vieta"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Atliktos operacijos"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Operacijų išimtys"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Operacijos"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Operacijų išimtys"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignoruotos operacijos"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Atliktos operacijos"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Atkurtos operacijos"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Pastaba"
@@ -225,26 +227,36 @@
 msgid "Product Uom Category"
 msgstr "Prekės mato vieneto kategorija"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Pirkimas"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Pirkimo data"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Pirkimo būsena"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Kiekis"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Tiekėjas"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Mokesčiai"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Gavimo vieta"
@@ -257,14 +269,19 @@
 msgid "Unit"
 msgstr "Mato vienetas"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Kaina"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Sandėlys"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Pirkimo eilutė"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "PVM"
@@ -590,14 +607,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -615,14 +638,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Minimalus kiekis"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -659,32 +688,35 @@
 msgid "Configuration"
 msgstr "Nuostatos"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Pirkimai"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Pirkimai"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Pirkimai"
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Pirkimo eilutė"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Operacijos"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Pirkimai"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Pirkimai"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Pirkimai"
@@ -769,14 +801,43 @@
 msgstr "Vykdomi"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pasiūlymas"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Visi"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Pabaigta"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Visi"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Pabaigta"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -791,14 +852,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1212,38 +1279,50 @@
 msgstr "Pagal siuntimą"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Rankiniu būdu"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Išimtis"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Jokia"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Apmokėta"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Laukianti apmokėjimo"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Išimtis"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Jokia"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Gauta"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Laukianti apmokėjimo"
```

### Comparing `trytond_purchase-6.6.3/locale/nl.po` & `trytond_purchase-6.8.0/locale/nl.po`

 * *Files 10% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuurregels"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Voorraadbewegingen gereed"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Voorraad bewegingen uitzondering"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Voorraad bewegingen"
 
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Voorraad Mutaties Uitzondering"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Genegeerde voorraadbewegingen"
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Voorraad Mutaties Voortgang"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Opnieuw aangemaakte voorraadbewegingen"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Notitie"
@@ -211,26 +211,34 @@
 msgid "Product Uom Category"
 msgstr "Product maateenheid categorie"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Inkoop"
 
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Inkoopdatum"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Inkoop status"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Hoeveelheid"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr "Samenvatting"
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Leverancier"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Belastingen"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Naar locatie"
@@ -243,14 +251,18 @@
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Eenheidsprijs"
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Magazijn"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Inkoopregel"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Belasting"
@@ -566,14 +578,22 @@
 "De tijd vanaf de bevestiging van de inkooporder tot het ontvangen van de goederen van de relatie wanneer gebruikt als leverancier.\n"
 "Wordt gebruikt als er geen doorlooptijd is ingesteld op de leverancier in het product."
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr "Standaard valuta voor inkopen van deze relatie."
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+"De tijd vanaf de bevestiging van de inkooporder tot het ontvangen van de goederen van de relatie wanneer gebruikt als leverancier.\n"
+"Wordt gebruikt als er geen doorlooptijd is ingesteld op de leverancier in het product."
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "De periode waarin bevestigde aankoop nog steeds kan worden gereset naar concept.\n"
 "Alleen toegepast als de wachtrij is geactiveerd."
@@ -599,14 +619,22 @@
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 "De tijd tussen het bevestigen van de bestelling en het ontvangen van de producten.\n"
 "Indien leeg wordt de doorlooptijd van de leverancier gehanteerd."
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+"Voeg een prijs toe aan de hand van verschillende criteria.\n"
+"De laatst overeenkomende regel wordt gebruikt."
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Minimale hoeveelheid."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "De eenheid waarin de hoeveelheid is opgegeven."
@@ -639,31 +667,31 @@
 msgid "Configuration"
 msgstr "Instellingen"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Inkopen"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Inkopen"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Inkopen"
 
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Inkoopregels"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Voorraad bewegingen"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Inkopen"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Inkopen"
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Inkopen"
 
@@ -740,14 +768,39 @@
 msgstr "Verwerking"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Offerte"
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Afgerond"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr "In behandeling"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Afgerond"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr "In behandeling"
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 "U probeert de inkoop-maateenheid te wijzigen waarop de inkoopprijzen zijn "
 "gebaseerd."
@@ -768,14 +821,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "U kunt de factuur \"%(invoice)s\" niet terugzetten naar concept zetten omdat"
 " deze gegenereerd is door een inkooporder."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+"U kunt geen regels toevoegen aan inkoop \"%(purchase)s\" omdat deze niet "
+"meer in status concept staat."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "Om regel \"%(line)s\" te verwijderen, moet u de inkooporder \"%(purchase)s\""
 " annuleren, resetten of terugzetten naar concept."
@@ -1181,38 +1242,50 @@
 msgstr "Op basis van verzending"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Handmatig"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "In afwachting van betaling"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Uitzondering"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Geen"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Betaald"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "In afwachting"
+msgid "Partially Paid"
+msgstr "Gedeeltelijk betaald"
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr "In behandeling"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Uitzondering"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Geen"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Gedeeltelijk Verzonden"
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Ontvangen"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "In afwachting"
```

### Comparing `trytond_purchase-6.6.3/locale/pl.po` & `trytond_purchase-6.8.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -182,30 +182,31 @@
 msgid "From Location"
 msgstr "Z lokalizacji"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Wiersze faktury"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Ruchy"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Wyjątek"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Notatka"
@@ -222,26 +223,36 @@
 msgid "Product Uom Category"
 msgstr "Kategoria jm produktu"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Zakup"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Data zakupu"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Stan zakupu"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Ilość"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Dostawca"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Podatki"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Do lokalizacji"
@@ -254,14 +265,19 @@
 msgid "Unit"
 msgstr "Jednostka"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Cena jednostkowa"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Magazyn"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Wiersz zakupu"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Podatek"
@@ -588,14 +604,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -613,14 +635,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Minimalna ilość"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -660,35 +688,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
-msgstr "Purchases"
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Wiersz zakupu"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Ruchy"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Zakupy"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Zakupy"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Zakupy"
 
 #, fuzzy
@@ -781,14 +811,43 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Wykonano"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Wykonano"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -803,14 +862,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1224,38 +1289,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Wyjątek"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Brak"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Wyjątek"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Brak"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Odebrano"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/pt.po` & `trytond_purchase-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -185,30 +185,32 @@
 msgid "From Location"
 msgstr "Origem"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Linhas da fatura"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Movimentações feitas"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Exceção nas movimentações"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimentações"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Exceção nas movimentações"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimentações ignoradas"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Movimentações feitas"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Recriar movimentações"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Observação"
@@ -225,26 +227,36 @@
 msgid "Product Uom Category"
 msgstr "Categoria de UDM do produto"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Data da compra"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Estado da Compra"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Quantidade"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Fornecedor"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Impostos"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Destino"
@@ -257,14 +269,19 @@
 msgid "Unit"
 msgstr "Unidade"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Preço unitário"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Almoxarifado"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Linha da compra"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Impostos"
@@ -591,14 +608,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -618,14 +641,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Quantidade mínima"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -667,35 +696,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
-msgstr "Purchases"
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Linha da compra"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Movimentações"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Compras"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Compras"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Compras"
 
 #, fuzzy
@@ -788,14 +819,43 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Feito"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Feito"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -813,14 +873,20 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Não é possível restaurar para rascunho o movimento \"%s\" porque ele foi "
 "gerado por uma compra."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1235,38 +1301,50 @@
 msgstr "Baseado Na Remessa"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Exceção"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Nenhum"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Pago"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Espera"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Exceção"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Nenhum"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Recebido"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Espera"
```

### Comparing `trytond_purchase-6.6.3/locale/ro.po` & `trytond_purchase-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -177,30 +177,31 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Gestionare Excepție Factura"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -217,26 +218,36 @@
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Achiziții"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Furnizor"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Spre Locație"
@@ -249,14 +260,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Impozit"
@@ -439,15 +454,15 @@
 
 msgctxt "field:purchase.purchase,shipment_state:"
 msgid "Shipment State"
 msgstr ""
 
 msgctxt "field:purchase.purchase,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:purchase.purchase,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:purchase.purchase,tax_amount:"
 msgid "Tax"
@@ -575,14 +590,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -600,14 +621,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -642,33 +669,36 @@
 msgid "Configuration"
 msgstr "Configurație"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Achiziții"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr ""
+msgstr "Achiziții"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr ""
+msgstr "Achiziții"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Achiziții"
 
 #, fuzzy
@@ -694,15 +724,15 @@
 
 msgctxt "model:ir.action,name:act_return_form"
 msgid "Returns"
 msgstr "Retururi"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
-msgstr "Transporturi"
+msgstr "Expedieri"
 
 msgctxt "model:ir.action,name:report_purchase"
 msgid "Purchase"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_invoice_handle_exception"
 msgid "Handle Invoice Exception"
@@ -746,14 +776,39 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -768,14 +823,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1174,38 +1235,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/ru.po` & `trytond_purchase-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -189,30 +189,32 @@
 msgid "From Location"
 msgstr "Из местоположения"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Строки инвойса"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Перемещения выполнены"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Особые ситуации перемещения"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Перемещения"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Особые ситуации перемещения"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Игнорированные проводки"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Перемещения выполнены"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Созданные заново проводки"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Комментарий"
@@ -230,26 +232,36 @@
 msgstr "Категория ед. измерения продукции"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Покупки"
 
 #, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Дата покупки"
+
+#, fuzzy
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Дата покупки"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Кол-во"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Поставщик"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Налоги"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "В местоположение"
@@ -262,14 +274,19 @@
 msgid "Unit"
 msgstr "Единица измерения"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Цена за единицу"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Товарный склад"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Строка покупки"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Налог"
@@ -598,14 +615,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -625,14 +648,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Минимальное кол-во"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -673,35 +702,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "Purchases"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Покупки"
 
 #, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Строка покупки"
+
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Перемещения"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Покупки"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Покупки"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Покупки"
 
 #, fuzzy
@@ -794,14 +825,43 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Выполнено"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Выполнено"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -819,14 +879,20 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Вы не можете сбросить в черновик перемещение \"%s\" так как оно создано из "
 "покупки."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1243,38 +1309,50 @@
 msgstr "Основанные на доставке"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Ручной"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Особая ситуация"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Отсутствует"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Оплачен"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Ожидание"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Особая ситуация"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Отсутствует"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Поступило"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Ожидание"
```

### Comparing `trytond_purchase-6.6.3/locale/sl.po` & `trytond_purchase-6.8.0/locale/sl.po`

 * *Files 3% similar despite different names*

```diff
@@ -185,30 +185,32 @@
 msgid "From Location"
 msgstr "Iz lokacije"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Postavke računa"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "Zaključen promet"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Pridržani promet"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Promet"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Pridržani promet"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Prezrt promet"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Zaključen promet"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Ponovno izdelan promet"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "Opomba"
@@ -225,26 +227,36 @@
 msgid "Product Uom Category"
 msgstr "Katerogija EM izdelka"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Nabavni nalog"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Nabavljeno"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "Stanje nabave"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "Količina"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Dobavitelj"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "Davki"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "Na lokacijo"
@@ -257,14 +269,19 @@
 msgid "Unit"
 msgstr "enota"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "Cena"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "Skladišče"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "Nabavna postavka"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "Davek"
@@ -591,14 +608,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -616,14 +639,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "Minimalna količina"
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
@@ -665,35 +694,37 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
-msgstr "Purchases"
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Nabavna postavka"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "Promet"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Nabavni nalogi"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Nabavni nalogi"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Nabavni nalogi"
 
 #, fuzzy
@@ -786,14 +817,43 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "Zaključeno"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "Zaključeno"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -811,14 +871,20 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 "Prometa \"%s\", izdelanega iz nabavnega naloga, ni možno prestaviti v stanje"
 " priprave."
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1233,38 +1299,50 @@
 msgstr "Na podlagi pošiljke"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "Ročno"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "Pridržano"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "Brez"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "Plačano"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "Čakajoče"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "Pridržano"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "Brez"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "Prejeto"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "Čakajoče"
```

### Comparing `trytond_purchase-6.6.3/locale/tr.po` & `trytond_purchase-6.8.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -175,30 +175,31 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -216,26 +217,36 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "Purchases"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Purchases"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "Product Suppliers"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -248,14 +259,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr ""
@@ -584,14 +599,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -609,14 +630,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -651,31 +678,34 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
+msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_invoice_relate"
-msgid "Purchases"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
 msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "Purchases"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "Purchases"
@@ -759,14 +789,41 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -781,14 +838,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1199,38 +1262,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/uk.po` & `trytond_purchase-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line,move_exception:"
+msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
@@ -211,26 +211,35 @@
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "Звітність"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr ""
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr ""
@@ -243,14 +252,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr ""
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr ""
@@ -562,14 +575,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:purchase.handle.invoice.exception.ask,recreate_invoices:"
@@ -587,14 +606,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr ""
@@ -627,31 +652,32 @@
 msgid "Configuration"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "Звітність"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr ""
 
@@ -728,14 +754,39 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -750,14 +801,20 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1150,38 +1207,50 @@
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_purchase-6.6.3/locale/zh_CN.po` & `trytond_purchase-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -180,30 +180,32 @@
 msgid "From Location"
 msgstr "从位置"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "发票明细"
 
-msgctxt "field:purchase.line,move_done:"
-msgid "Moves Done"
-msgstr "完成移动"
-
-msgctxt "field:purchase.line,move_exception:"
-msgid "Moves Exception"
-msgstr "移动异常"
-
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "移动"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "移动异常"
+
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "已忽略的移动"
 
+#, fuzzy
+msgctxt "field:purchase.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "完成移动"
+
 msgctxt "field:purchase.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "已经重新创建的移动"
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr "注释"
@@ -220,26 +222,36 @@
 msgid "Product Uom Category"
 msgstr "产品计量单位类别"
 
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
 msgstr "采购"
 
+#, fuzzy
+msgctxt "field:purchase.line,purchase_date:"
+msgid "Purchase Date"
+msgstr "采购日期"
+
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr "购买状态"
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr "数量"
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,supplier:"
+msgid "Supplier"
+msgstr "供货商"
+
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr "税"
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
 msgstr "到位置"
@@ -252,14 +264,19 @@
 msgid "Unit"
 msgstr "计量单位"
 
 msgctxt "field:purchase.line,unit_price:"
 msgid "Unit Price"
 msgstr "单位价格"
 
+#, fuzzy
+msgctxt "field:purchase.line,warehouse:"
+msgid "Warehouse"
+msgstr "仓库"
+
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr "采购明细"
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
 msgstr "税款"
@@ -581,14 +598,20 @@
 "Used if no lead time is set on the product supplier."
 msgstr ""
 
 msgctxt "help:party.party.supplier_currency,supplier_currency:"
 msgid "Default currency for purchases from this party."
 msgstr ""
 
+msgctxt "help:party.party.supplier_lead_time,supplier_lead_time:"
+msgid ""
+"The time from confirming the purchase order to receiving the goods from the party when used as a supplier.\n"
+"Used if no lead time is set on the product supplier."
+msgstr ""
+
 msgctxt "help:purchase.configuration,purchase_process_after:"
 msgid ""
 "The grace period during which confirmed purchase can still be reset to draft.\n"
 "Applied only if a worker queue is activated."
 msgstr ""
 "采购项目已确认状态可以重置为草稿状态的宽限期\n"
 "仅在激活工作队列时应用."
@@ -608,14 +631,20 @@
 
 msgctxt "help:purchase.product_supplier,lead_time:"
 msgid ""
 "The time from confirming the purchase order to receiving the products.\n"
 "If empty the lead time of the supplier is used."
 msgstr ""
 
+msgctxt "help:purchase.product_supplier,prices:"
+msgid ""
+"Add price for different criteria.\n"
+"The last matching line is used."
+msgstr ""
+
 msgctxt "help:purchase.product_supplier.price,quantity:"
 msgid "Minimal quantity."
 msgstr "最小数量."
 
 msgctxt "help:purchase.product_supplier.price,uom:"
 msgid "The unit in which the quantity is specified."
 msgstr "指定数量的单位."
@@ -650,31 +679,34 @@
 msgid "Configuration"
 msgstr "设置"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
 msgstr "采购"
 
-msgctxt "model:ir.action,name:act_purchase_form2"
-msgid "Purchases"
-msgstr "采购"
-
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
 msgstr "采购"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_line_relate"
+msgid "Purchase Lines"
+msgstr "采购明细"
+
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr "移动"
 
-msgctxt "model:ir.action,name:act_purchase_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
 msgstr "采购"
 
-msgctxt "model:ir.action,name:act_purchase_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
 msgstr "采购"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
 msgstr "采购"
@@ -757,14 +789,43 @@
 msgstr "处理中"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
 msgstr "报价"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
+msgid "All"
+msgstr "全部"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
+msgid "Done"
+msgstr "完成"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
+msgid "All"
+msgstr "全部"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
+msgid "Done"
+msgstr "完成"
+
+msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase UoM on which the purchase prices are "
 "based."
 msgstr "您正在试图更改采购价格依赖的采购计量单位."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
@@ -779,14 +840,21 @@
 
 msgctxt "model:ir.message,text:msg_purchase_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a purchase."
 msgstr "无法将发票 \"%(invoice)s\" 重置为草稿状态，因为因为它与某个采购关联。"
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_purchase_line_create_draft"
+msgid ""
+"You cannot add lines to purchase \"%(purchase)s\" because it is no longer in"
+" a draft state."
+msgstr "状态在草案时，才能修改采购 \"%(purchase)s\" 标题."
+
 msgctxt "model:ir.message,text:msg_purchase_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft purchase "
 "\"%(purchase)s\"."
 msgstr "要删除明细 \"%(line)s\" ，你必须将采购 \"%(purchase)s\"取消或者重置为草稿状态."
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
@@ -1199,38 +1267,50 @@
 msgstr "基于发货"
 
 msgctxt "selection:purchase.purchase,invoice_method:"
 msgid "Manual"
 msgstr "手工"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Exception"
 msgstr "异常"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "None"
 msgstr "没有"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
 msgid "Paid"
 msgstr "已付费"
 
 msgctxt "selection:purchase.purchase,invoice_state:"
-msgid "Waiting"
-msgstr "正在等待"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Exception"
 msgstr "异常"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "None"
 msgstr "无"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Received"
 msgstr "已收货"
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr "正在等待"
```

### Comparing `trytond_purchase-6.6.3/message.xml` & `trytond_purchase-6.8.0/message.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/message.xml` & `trytond_purchase-6.8.0/message.xml`

```diff
@@ -32,14 +32,17 @@
     </record>
     <record model="ir.message" id="msg_purchase_invoice_reset_draft">
       <field name="text">You cannot reset invoice &quot;%(invoice)s&quot; to draft because it was generated by a purchase.</field>
     </record>
     <record model="ir.message" id="msg_purchase_move_reset_draft">
       <field name="text">You cannot reset move &quot;%(move)s&quot; to draft because it was generated by a purchase.</field>
     </record>
+    <record model="ir.message" id="msg_purchase_line_create_draft">
+      <field name="text">You cannot add lines to purchase &quot;%(purchase)s&quot; because it is no longer in a draft state.</field>
+    </record>
     <record model="ir.message" id="msg_purchase_line_tax_unique">
       <field name="text">A tax can be added only once to a purchase line.</field>
     </record>
     <record model="ir.message" id="msg_purchase_reporting_company">
       <field name="text">Company</field>
     </record>
     <record model="ir.message" id="msg_purchase_reporting_number">
```

### Comparing `trytond_purchase-6.6.3/party.py` & `trytond_purchase-6.8.0/party.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,38 @@
 # this repository contains the full copyright notices and license terms.
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.modules.party.exceptions import EraseError
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval
+from trytond.pyson import Eval, TimeDelta
 
 supplier_currency = fields.Many2One(
     'currency.currency', "Supplier Currency",
     help="Default currency for purchases from this party.")
+supplier_lead_time = fields.TimeDelta(
+    "Lead Time",
+    domain=['OR',
+        ('supplier_lead_time', '=', None),
+        ('supplier_lead_time', '>=', TimeDelta()),
+        ],
+    help="The time from confirming the purchase order to receiving "
+    "the goods from the party when used as a supplier.\n"
+    "Used if no lead time is set on the product supplier.")
 
 
 class Party(CompanyMultiValueMixin, metaclass=PoolMeta):
     __name__ = 'party.party'
     customer_code = fields.MultiValue(fields.Char('Customer Code',
             help="The code the party as supplier has assigned to the company"
             " as customer."))
     customer_codes = fields.One2Many(
         'party.party.customer_code', 'party', "Customer Codes")
-    supplier_lead_time = fields.MultiValue(fields.TimeDelta("Lead Time",
-            help="The time from confirming the purchase order to receiving "
-            "the goods from the party when used as a supplier.\n"
-            "Used if no lead time is set on the product supplier."))
+    supplier_lead_time = fields.MultiValue(supplier_lead_time)
     supplier_lead_times = fields.One2Many(
         'party.party.supplier_lead_time', 'party', "Lead Times")
     supplier_currency = fields.MultiValue(supplier_currency)
     supplier_currencies = fields.One2Many(
         'party.party.supplier_currency', 'party', "Supplier Currencies")
 
 
@@ -48,15 +54,15 @@
     __name__ = 'party.party.supplier_lead_time'
     party = fields.Many2One(
         'party.party', "Party", ondelete='CASCADE',
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
-    supplier_lead_time = fields.TimeDelta("Lead Time")
+    supplier_lead_time = supplier_lead_time
 
 
 class PartySupplierCurrency(ModelSQL, ValueMixin):
     "Party Supplier Currency"
     __name__ = 'party.party.supplier_currency'
     party = fields.Many2One(
         'party.party', "Party", ondelete='CASCADE')
```

### Comparing `trytond_purchase-6.6.3/party.xml` & `trytond_purchase-6.8.0/party.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/party.xml` & `trytond_purchase-6.8.0/party.xml`

```diff
@@ -4,29 +4,14 @@
 <tryton>
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
-    <record model="ir.action.act_window" id="act_purchase_form2">
-      <field name="name">Purchases</field>
-      <field name="res_model">purchase.purchase</field>
-      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('party', '=', Eval('active_id')), ('party', 'in', Eval('active_ids')))]" pyson="1"/>
-      <field name="search_value" eval="[('state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
-    </record>
-    <record model="ir.action.keyword" id="act_open_purchase_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">party.party,-1</field>
-      <field name="action" ref="act_purchase_form2"/>
-    </record>
-    <record model="ir.action-res.group" id="act_purchase_form2-group_purchase">
-      <field name="action" ref="act_purchase_form2"/>
-      <field name="group" ref="group_purchase"/>
-    </record>
     <record model="ir.model.field.access" id="access_party_supplier_currency">
       <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_currency')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_currency_group_sale">
       <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_currency')]"/>
```

### Comparing `trytond_purchase-6.6.3/product.py` & `trytond_purchase-6.8.0/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, MatchMixin, ModelSQL, ModelView, fields,
     sequence_ordered)
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Bool, Eval, If
+from trytond.pyson import Bool, Eval, If, TimeDelta
 from trytond.tools import is_full_text, lstrip_wildcard
 from trytond.transaction import Transaction
 
 from .exceptions import PurchaseUOMWarning
 
 
 class Template(metaclass=PoolMeta):
@@ -154,15 +154,15 @@
         The context that can have as keys:
             uom: the unit of measure
             supplier: the supplier party id
             currency: the currency id for the returned price
         '''
         pool = Pool()
         Uom = pool.get('product.uom')
-        User = pool.get('res.user')
+        Company = pool.get('company.company')
         Currency = pool.get('currency.currency')
         Date = pool.get('ir.date')
         ProductSupplier = pool.get('purchase.product_supplier')
         ProductSupplierPrice = pool.get('purchase.product_supplier.price')
 
         today = Date.today()
         context = Transaction().context
@@ -173,22 +173,21 @@
         uom = None
         if context.get('uom'):
             uom = Uom(context['uom'])
 
         currency = None
         if context.get('currency'):
             currency = Currency(context['currency'])
-
-        user = User(Transaction().user)
+        elif context.get('company'):
+            currency = Company(context['company']).currency
 
         for product in products:
             unit_price = product._get_purchase_unit_price(quantity=quantity)
             default_uom = product.default_uom
-            default_currency = (user.company.currency if user.company
-                else None)
+            default_currency = currency
             if not uom or default_uom.category != uom.category:
                 product_uom = default_uom
             else:
                 product_uom = uom
             pattern = ProductSupplier.get_pattern()
             product_suppliers = product.product_suppliers_used(**pattern)
             try:
@@ -276,20 +275,27 @@
         'party.party', 'Supplier', required=True, ondelete='CASCADE',
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     name = fields.Char("Name", translate=True)
     code = fields.Char("Code")
-    prices = fields.One2Many('purchase.product_supplier.price',
-            'product_supplier', 'Prices')
+    prices = fields.One2Many(
+        'purchase.product_supplier.price', 'product_supplier', "Prices",
+        help="Add price for different criteria.\n"
+        "The last matching line is used.")
     company = fields.Many2One(
         'company.company', "Company",
         required=True, ondelete='CASCADE')
-    lead_time = fields.TimeDelta('Lead Time',
+    lead_time = fields.TimeDelta(
+        "Lead Time",
+        domain=['OR',
+            ('lead_time', '=', None),
+            ('lead_time', '>=', TimeDelta()),
+            ],
         help="The time from confirming the purchase order to receiving the "
         "products.\n"
         "If empty the lead time of the supplier is used.")
     currency = fields.Many2One('currency.currency', 'Currency', required=True,
         ondelete='RESTRICT')
     uom = fields.Function(
         fields.Many2One('product.uom', "UOM"), 'on_change_with_uom')
@@ -399,19 +405,17 @@
         return domain
 
     @fields.depends(
         'product', '_parent_product.purchase_uom',
         'template', '_parent_template.purchase_uom')
     def on_change_with_uom(self, name=None):
         if self.product:
-            if self.product.purchase_uom:
-                return self.product.purchase_uom.id
+            return self.product.purchase_uom
         elif self.template:
-            if self.template.purchase_uom:
-                return self.template.purchase_uom.id
+            return self.template.purchase_uom
 
     @property
     def lead_time_used(self):
         # Use getattr because it can be called with an unsaved instance
         lead_time = getattr(self, 'lead_time', None)
         party = getattr(self, 'party', None)
         if lead_time is None and party:
@@ -496,21 +500,20 @@
 
     @staticmethod
     def default_quantity():
         return 0.0
 
     @fields.depends('product_supplier', '_parent_product_supplier.product')
     def on_change_with_uom(self, name=None):
-        if self.product_supplier and self.product_supplier.uom:
-            return self.product_supplier.uom.id
+        return self.product_supplier.uom if self.product_supplier else None
 
     @fields.depends('product_supplier', '_parent_product_supplier.currency')
     def on_change_with_currency(self, name=None):
-        if self.product_supplier and self.product_supplier.currency:
-            return self.product_supplier.currency.id
+        if self.product_supplier:
+            return self.product_supplier.currency
 
     @staticmethod
     def get_pattern():
         return {}
 
     def match(self, quantity, uom, pattern):
         pool = Pool()
```

### Comparing `trytond_purchase-6.6.3/product.xml` & `trytond_purchase-6.8.0/product.xml`

 * *Files 20% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/product.xml` & `trytond_purchase-6.8.0/product.xml`

```diff
@@ -1,12 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
+    <record model="ir.ui.view" id="template_view_form">
+      <field name="model">product.template</field>
+      <field name="inherit" ref="product.template_view_form"/>
+      <field name="name">template_form</field>
+    </record>
+    <record model="ir.ui.view" id="template_view_tree">
+      <field name="model">product.template</field>
+      <field name="inherit" ref="product.template_view_tree"/>
+      <field name="name">template_tree</field>
+    </record>
     <record model="ir.ui.view" id="product_view_list_purchase_line">
       <field name="model">product.product</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">product_list_purchase_line</field>
     </record>
   </data>
```

### Comparing `trytond_purchase-6.6.3/purchase.fodt` & `trytond_purchase-6.8.0/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/purchase.py` & `trytond_purchase-6.8.0/purchase.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,17 @@
     description = fields.Char('Description', size=None, states=_states)
     purchase_date = fields.Date('Purchase Date',
         states={
             'readonly': ~Eval('state').in_(['draft', 'quotation']),
             'required': ~Eval('state').in_(
                 ['draft', 'quotation', 'cancelled']),
             })
-    payment_term = fields.Many2One('account.invoice.payment_term',
-        'Payment Term', states={
+    payment_term = fields.Many2One(
+        'account.invoice.payment_term', "Payment Term", ondelete='RESTRICT',
+        states={
             'readonly': ~Eval('state').in_(['draft', 'quotation']),
             })
     party = fields.Many2One('party.party', 'Party', required=True,
         states={
             'readonly': ((Eval('state') != 'draft')
                 | (Eval('lines', [0]) & Eval('party'))),
             },
@@ -166,15 +167,17 @@
     invoice_method = fields.Selection([
             ('manual', 'Manual'),
             ('order', 'Based On Order'),
             ('shipment', 'Based On Shipment'),
             ], 'Invoice Method', required=True, states=_states)
     invoice_state = fields.Selection([
             ('none', 'None'),
-            ('waiting', 'Waiting'),
+            ('pending', "Pending"),
+            ('awaiting payment', "Awaiting Payment"),
+            ('partially paid', "Partially Paid"),
             ('paid', 'Paid'),
             ('exception', 'Exception'),
             ], 'Invoice State', readonly=True, required=True, sort=False)
     invoices = fields.Function(fields.Many2Many(
             'account.invoice', None, None, "Invoices"),
         'get_invoices', searcher='search_invoices')
     invoices_ignored = fields.Many2Many(
@@ -194,14 +197,15 @@
             'readonly': Eval('state').in_([
                     'processing', 'done', 'cancelled']),
             },
         help="The default delivery date for each line.")
     shipment_state = fields.Selection([
             ('none', 'None'),
             ('waiting', 'Waiting'),
+            ('partially shipped', 'Partially Shipped'),
             ('received', 'Received'),
             ('exception', 'Exception'),
             ], 'Shipment State', readonly=True, required=True, sort=False)
     shipments = fields.Function(fields.Many2Many(
             'stock.shipment.in', None, None, "Shipments"),
         'get_shipments', searcher='search_shipments')
     shipment_returns = fields.Function(fields.Many2Many(
@@ -372,14 +376,19 @@
                     where=sql_table.id.in_(sub_query.select(sub_query.id))))
 
         # Migration from 5.6: rename state cancel to cancelled
         cursor.execute(*sql_table.update(
                 [sql_table.state], ['cancelled'],
                 where=sql_table.state == 'cancel'))
 
+        # Migration from 6.6: rename invoice state waiting to pending
+        cursor.execute(*sql_table.update(
+                [sql_table.invoice_state], ['pending'],
+                where=sql_table.invoice_state == 'waiting'))
+
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
         return [CharLength(table.number), table.number]
 
     @classmethod
     def default_warehouse(cls):
@@ -581,49 +590,60 @@
             for invoice_line in line.invoice_lines:
                 if invoice_line.invoice:
                     invoices.add(invoice_line.invoice.id)
         return list(invoices)
 
     @classmethod
     def search_invoices(cls, name, clause):
-        return [('lines.invoice_lines.invoice' + clause[0].lstrip(name),)
-            + tuple(clause[1:])]
+        return [('lines.invoice_lines.invoice' + clause[0][len(name):],
+                *clause[1:])]
+
+    @property
+    def _invoices_for_state(self):
+        return self.invoices
 
     def get_invoice_state(self):
         '''
         Return the invoice state for the purchase.
         '''
-        skip_ids = set(x.id for x in self.invoices_ignored)
-        skip_ids.update(x.id for x in self.invoices_recreated)
-        invoices = [i for i in self.invoices if i.id not in skip_ids]
+        skips = set(self.invoices_ignored)
+        skips.update(self.invoices_recreated)
+        invoices = [i for i in self._invoices_for_state if i.id not in skips]
         if invoices:
             if any(i.state == 'cancelled' for i in invoices):
                 return 'exception'
             elif all(i.state == 'paid' for i in invoices):
                 return 'paid'
+            elif any(i.state == 'paid' for i in invoices):
+                return 'partially paid'
+            elif any(i.state == 'posted' for i in invoices):
+                return 'awaiting payment'
             else:
-                return 'waiting'
+                return 'pending'
         return 'none'
 
     get_shipments = get_shipments_returns('stock.shipment.in')
     get_shipment_returns = get_shipments_returns('stock.shipment.in.return')
 
     search_shipments = search_shipments_returns('stock.shipment.in')
     search_shipment_returns = search_shipments_returns(
         'stock.shipment.in.return')
 
     def get_shipment_state(self):
         '''
         Return the shipment state for the purchase.
         '''
         if self.moves:
-            if any(l.move_exception for l in self.lines):
+            if any(l.moves_exception for l in self.lines):
                 return 'exception'
-            elif all(l.move_done for l in self.lines):
+            elif all(l.moves_progress >= 1 for l in self.lines
+                    if l.moves_progress is not None):
                 return 'received'
+            elif any(l.moves_progress for l in self.lines):
+                return 'partially shipped'
             else:
                 return 'waiting'
         return 'none'
 
     def get_moves(self, name):
         return [m.id for l in self.lines for m in l.moves]
 
@@ -766,36 +786,27 @@
             purchase.tax_amount_cache = purchase.tax_amount
             purchase.total_amount_cache = purchase.total_amount
         cls.save(purchases)
 
     def _get_invoice_purchase(self):
         'Return invoice'
         pool = Pool()
-        Journal = pool.get('account.journal')
         Invoice = pool.get('account.invoice')
-
-        journals = Journal.search([
-                ('type', '=', 'expense'),
-                ], limit=1)
-        if journals:
-            journal, = journals
-        else:
-            journal = None
         party = self.invoice_party or self.party
-
-        return Invoice(
+        invoice = Invoice(
             company=self.company,
             type='in',
-            journal=journal,
             party=party,
             invoice_address=self.invoice_address,
             currency=self.currency,
             account=party.account_payable_used,
             payment_term=self.payment_term,
             )
+        invoice.journal = invoice.on_change_with_journal()
+        return invoice
 
     def create_invoice(self):
         'Create an invoice for the purchase and return it'
 
         if self.invoice_method == 'manual':
             return
 
@@ -997,16 +1008,19 @@
 
             for line in purchase.lines:
                 line.set_actual_quantity()
                 lines.append(line)
 
         for invoice_state, purchases in invoice_states.items():
             cls.write(purchases, {'invoice_state': invoice_state})
+            cls.log(purchases, 'transition', f'invoice_state:{invoice_state}')
         for shipment_state, purchases in shipment_states.items():
             cls.write(purchases, {'shipment_state': shipment_state})
+            cls.log(
+                purchases, 'transition', f'shipment_state:{shipment_state}')
         Line.save(lines)
 
     @classmethod
     def _process_state(cls, purchases):
         process, done = [], []
         for purchase in purchases:
             if purchase.is_done():
@@ -1063,91 +1077,113 @@
         ('comment', 'Comment'),
         ], "Type", required=True,
         states={
             'readonly': Eval('purchase_state') != 'draft',
             })
     quantity = fields.Float(
         "Quantity", digits='unit',
+        domain=[
+            If(Eval('type') != 'line',
+                ('quantity', '=', None),
+                ()),
+            ],
         states={
             'invisible': Eval('type') != 'line',
             'required': Eval('type') == 'line',
             'readonly': Eval('purchase_state') != 'draft',
             })
     actual_quantity = fields.Float(
         "Actual Quantity", digits='unit', readonly=True,
+        domain=[
+            If(Eval('type') != 'line',
+                ('actual_quantity', '=', None),
+                ()),
+            ],
         states={
-            'invisible': Eval('type') != 'line',
+            'invisible': ((Eval('type') != 'line') | ~Eval('actual_quantity')),
             })
     unit = fields.Many2One('product.uom', 'Unit',
         ondelete='RESTRICT',
         states={
             'required': Bool(Eval('product')),
             'invisible': Eval('type') != 'line',
             'readonly': Eval('purchase_state') != 'draft',
             },
         domain=[
             If(Bool(Eval('product_uom_category')),
                 ('category', '=', Eval('product_uom_category')),
                 ('category', '!=', -1)),
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             ])
     product = fields.Many2One('product.product', 'Product',
         ondelete='RESTRICT',
         domain=[
-            If(Eval('purchase_state').in_(['draft', 'quotation']),
-                [('purchasable', '=', True)],
-                []),
+            If(Eval('purchase_state').in_(['draft', 'quotation'])
+                & ~(Eval('quantity', 0) < 0),
+                ('purchasable', '=', True),
+                ()),
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('purchase_state') != 'draft',
             'required': Bool(Eval('product_supplier')),
             },
         context={
             'company': Eval('company', None),
             },
         search_context={
-            'locations': If(Bool(Eval('_parent_purchase', {}).get(
-                        'warehouse')),
-                [Eval('_parent_purchase', {}).get('warehouse', None)],
-                []),
-            'stock_date_end': Eval('_parent_purchase', {}).get(
-                'purchase_date'),
+            'locations': If(Bool(Eval('warehouse')),
+                [Eval('warehouse', -1)], []),
+            'stock_date_end': Eval('purchase_date', None),
             'stock_skip_warehouse': True,
-            'currency': Eval('_parent_purchase', {}).get('currency'),
-            'supplier': Eval('_parent_purchase', {}).get('party'),
-            'purchase_date': Eval('_parent_purchase', {}).get('purchase_date'),
+            'currency': Eval('currency', -1),
+            'supplier': Eval('supplier', -1),
+            'purchase_date': Eval('purchase_date', None),
             'uom': Eval('unit'),
             'taxes': Eval('taxes', []),
             'quantity': Eval('quantity'),
             },
         depends={'company'})
     product_supplier = fields.Many2One(
         'purchase.product_supplier', "Supplier's Product",
         ondelete='RESTRICT',
         domain=[
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             If(Bool(Eval('product')),
                 ['OR',
                     [
                         ('template.products', '=', Eval('product')),
                         ('product', '=', None),
                         ],
                     ('product', '=', Eval('product')),
                     ],
                 []),
-            ('party', '=', Eval('_parent_purchase', {}).get('party')),
+            ('party', '=', Eval('supplier', -1)),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('purchase_state') != 'draft',
             })
     product_uom_category = fields.Function(
         fields.Many2One('product.uom.category', 'Product Uom Category'),
         'on_change_with_product_uom_category')
     unit_price = Monetary(
         "Unit Price", currency='currency', digits=price_digits,
+        domain=[
+            If(Eval('type') != 'line',
+                ('unit_price', '=', None),
+                ()),
+            ],
         states={
             'invisible': Eval('type') != 'line',
             'required': Eval('type') == 'line',
             'readonly': Eval('purchase_state') != 'draft',
             })
     amount = fields.Function(Monetary(
             "Amount", currency='currency', digits='currency',
@@ -1160,130 +1196,176 @@
             'readonly': Eval('purchase_state') != 'draft',
             })
     summary = fields.Function(fields.Char('Summary'), 'on_change_with_summary')
     note = fields.Text('Note')
     taxes = fields.Many2Many('purchase.line-account.tax',
         'line', 'tax', 'Taxes',
         order=[('tax.sequence', 'ASC'), ('tax.id', 'ASC')],
-        domain=[('parent', '=', None), ['OR',
+        domain=[
+            ('parent', '=', None),
+            ['OR',
                 ('group', '=', None),
-                ('group.kind', 'in', ['purchase', 'both'])],
-                ('company', '=',
-                    Eval('_parent_purchase', {}).get('company', -1)),
+                ('group.kind', 'in', ['purchase', 'both']),
+                ],
+            ('company', '=', Eval('company', -1)),
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('purchase_state') != 'draft',
             })
-    invoice_lines = fields.One2Many('account.invoice.line', 'origin',
-        'Invoice Lines', readonly=True)
-    moves = fields.One2Many('stock.move', 'origin', 'Moves', readonly=True)
+    invoice_lines = fields.One2Many(
+        'account.invoice.line', 'origin', "Invoice Lines", readonly=True,
+        states={
+            'invisible': ~Eval('invoice_lines'),
+            })
+    moves = fields.One2Many(
+        'stock.move', 'origin', "Moves", readonly=True,
+        states={
+            'invisible': ~Eval('moves'),
+            })
     moves_ignored = fields.Many2Many('purchase.line-ignored-stock.move',
             'purchase_line', 'move', 'Ignored Moves', readonly=True)
     moves_recreated = fields.Many2Many('purchase.line-recreated-stock.move',
             'purchase_line', 'move', 'Recreated Moves', readonly=True)
-    move_done = fields.Function(fields.Boolean('Moves Done'), 'get_move_done')
-    move_exception = fields.Function(fields.Boolean('Moves Exception'),
-            'get_move_exception')
+    moves_exception = fields.Function(
+        fields.Boolean("Moves Exception"), 'get_moves_exception')
+    moves_progress = fields.Function(
+        fields.Float("Moves Progress", digits=(1, 4)),
+        'get_moves_progress')
+    warehouse = fields.Function(fields.Many2One(
+            'stock.location', "Warehouse"),
+        'on_change_with_warehouse')
     from_location = fields.Function(fields.Many2One('stock.location',
             'From Location'), 'get_from_location')
     to_location = fields.Function(fields.Many2One('stock.location',
             'To Location'), 'get_to_location')
     delivery_date = fields.Function(fields.Date('Delivery Date',
             states={
                 'invisible': Eval('type') != 'line',
                 'readonly': (Eval('purchase_state').in_(
                         ['processing', 'done', 'cancelled'])
                     | ~Eval('delivery_date_edit', False)),
                 }),
         'on_change_with_delivery_date', setter='set_delivery_date')
     delivery_date_edit = fields.Boolean(
         "Edit Delivery Date",
+        domain=[
+            If(Eval('type') != 'line',
+                ('delivery_date_edit', '=', None),
+                ()),
+            ],
         states={
             'invisible': (
                 (Eval('type') != 'line')
                 | Eval('purchase_state').in_(
                     ['processing', 'done', 'cancelled'])),
             'readonly': Eval('purchase_state').in_(
                 ['processing', 'done', 'cancelled']),
             },
         help="Check to edit the delivery date.")
     delivery_date_store = fields.Date(
         "Delivery Date", readonly=True,
+        domain=[
+            If(Eval('type') != 'line',
+                ('delivery_date_store', '=', None),
+                ()),
+            ],
         states={
             'invisible': Eval('type') != 'line',
             })
     purchase_state = fields.Function(
         fields.Selection('get_purchase_states', 'Purchase State'),
-        'on_change_with_purchase_state')
+        'on_change_with_purchase_state', searcher='search_purchase_state')
     company = fields.Function(
         fields.Many2One('company.company', "Company"),
         'on_change_with_company')
+    supplier = fields.Function(
+        fields.Many2One(
+            'party.party', "Supplier",
+            context={
+                'company': Eval('company', -1),
+                }),
+        'on_change_with_supplier', searcher='search_supplier')
+    purchase_date = fields.Function(
+        fields.Date("Purchase Date"),
+        'on_change_with_purchase_date', searcher='search_purchase_date')
     currency = fields.Function(
         fields.Many2One('currency.currency', 'Currency'),
         'on_change_with_currency')
 
     @classmethod
     def get_move_product_types(cls):
         pool = Pool()
         Move = pool.get('stock.move')
         return Move.get_product_types()
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('purchase')
+        cls._order.insert(0, ('purchase.purchase_date', 'DESC NULLS FIRST'))
+        cls._order.insert(1, ('purchase.id', 'DESC'))
 
     @classmethod
     def __register__(cls, module_name):
         super().__register__(module_name)
         table = cls.__table_handler__(module_name)
 
         # Migration from 4.6: drop required on description
         table.not_null_action('description', action='remove')
 
     @staticmethod
     def default_type():
         return 'line'
 
+    @fields.depends('type')
+    def on_change_type(self):
+        if self.type != 'line':
+            self.product = None
+            self.product_supplier = None
+            self.unit = None
+            self.taxes = None
+
     @classmethod
     def default_delivery_date_edit(cls):
         return False
 
     @property
     def _move_remaining_quantity(self):
         "Compute the remaining quantity to receive"
         pool = Pool()
         Uom = pool.get('product.uom')
         if self.type != 'line' or not self.product:
             return
         if self.product.type == 'service':
             return
-        skip_ids = set(x.id for x in self.moves_ignored)
+        skips = set(self.moves_ignored)
         quantity = abs(self.quantity)
         for move in self.moves:
-            if move.state == 'done' or move.id in skip_ids:
+            if move.state == 'done' or move in skips:
                 quantity -= Uom.compute_qty(move.uom, move.quantity, self.unit)
         return quantity
 
-    def get_move_done(self, name):
-        quantity = self._move_remaining_quantity
-        if quantity is None:
-            return True
-        else:
-            return self.unit.round(quantity) <= 0
+    def get_moves_exception(self, name):
+        skips = set(self.moves_ignored)
+        skips.update(self.moves_recreated)
+        return any(
+            m.state == 'cancelled' for m in self.moves if m not in skips)
 
-    def get_move_exception(self, name):
-        skip_ids = set(x.id for x in self.moves_ignored
-            + self.moves_recreated)
-        for move in self.moves:
-            if move.state == 'cancelled' \
-                    and move.id not in skip_ids:
-                return True
-        return False
+    def get_moves_progress(self, name):
+        progress = None
+        quantity = self._move_remaining_quantity
+        if quantity is not None and self.quantity:
+            progress = round(
+                (abs(self.quantity) - quantity) / abs(self.quantity), 4)
+            progress = max(0, min(1, progress))
+        return progress
 
     def _get_tax_rule_pattern(self):
         '''
         Get tax rule pattern
         '''
         return {}
 
@@ -1295,16 +1377,16 @@
         context = {}
         if self.purchase:
             if self.purchase.currency:
                 context['currency'] = self.purchase.currency.id
             if self.purchase.party:
                 context['supplier'] = self.purchase.party.id
             context['purchase_date'] = self.purchase.purchase_date
-            if self.company:
-                context['company'] = self.company.id
+        if self.company:
+            context['company'] = self.company.id
         if self.unit:
             context['uom'] = self.unit.id
         elif self.product:
             context['uom'] = self.product.purchase_uom.id
         if self.product_supplier:
             context['product_supplier'] = self.product_supplier.id
         context['taxes'] = [t.id for t in self.taxes or []]
@@ -1320,47 +1402,56 @@
             }
 
     @fields.depends('product', 'unit', 'purchase',
         '_parent_purchase.party', '_parent_purchase.invoice_party',
         'product_supplier', methods=['compute_taxes', 'compute_unit_price',
             '_get_product_supplier_pattern'])
     def on_change_product(self):
-        if not self.product:
-            return
-
         party = None
         if self.purchase:
             party = self.purchase.invoice_party or self.purchase.party
 
         # Set taxes before unit_price to have taxes in context of purchase
         # price
         self.taxes = self.compute_taxes(party)
 
-        category = self.product.purchase_uom.category
-        if not self.unit or self.unit.category != category:
-            self.unit = self.product.purchase_uom
-
-        product_suppliers = list(self.product.product_suppliers_used(
-                **self._get_product_supplier_pattern()))
-        if len(product_suppliers) == 1:
-            self.product_supplier, = product_suppliers
-        elif (self.product_supplier
-                and self.product_supplier not in product_suppliers):
-            self.product_supplier = None
+        if self.product:
+            category = self.product.purchase_uom.category
+            if not self.unit or self.unit.category != category:
+                self.unit = self.product.purchase_uom
+
+            product_suppliers = list(self.product.product_suppliers_used(
+                    **self._get_product_supplier_pattern()))
+            if len(product_suppliers) == 1:
+                self.product_supplier, = product_suppliers
+            elif (self.product_supplier
+                    and self.product_supplier not in product_suppliers):
+                self.product_supplier = None
 
         self.unit_price = self.compute_unit_price()
 
         self.type = 'line'
         self.amount = self.on_change_with_amount()
 
-    @fields.depends('product', methods=['_get_tax_rule_pattern'])
+    @fields.depends('product', 'company', methods=['_get_tax_rule_pattern'])
     def compute_taxes(self, party):
+        pool = Pool()
+        AccountConfiguration = pool.get('account.configuration')
         taxes = set()
         pattern = self._get_tax_rule_pattern()
-        for tax in self.product.supplier_taxes_used:
+        taxes_used = []
+        if self.product:
+            taxes_used = self.product.supplier_taxes_used
+        elif self.company:
+            account_config = AccountConfiguration(1)
+            account = account_config.get_multivalue(
+                'default_category_account_expense', company=self.company.id)
+            if account:
+                taxes_used = account.taxes
+        for tax in taxes_used:
             if party and party.supplier_tax_rule:
                 tax_ids = party.supplier_tax_rule.apply(tax, pattern)
                 if tax_ids:
                     taxes.update(tax_ids)
                 continue
             taxes.add(tax.id)
         if party and party.supplier_tax_rule:
@@ -1394,16 +1485,15 @@
             elif not self.product:
                 if len(self.product_supplier.template.products) == 1:
                     self.product, = self.product_supplier.template.products
         self.on_change_product()
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends(methods=['compute_unit_price'])
     def on_change_quantity(self):
         self.unit_price = self.compute_unit_price()
 
     @fields.depends(methods=['on_change_quantity'])
     def on_change_unit(self):
@@ -1438,14 +1528,18 @@
                 elif line2.type == 'subtotal':
                     if self == line2:
                         break
                     amount = Decimal('0.0')
             return amount
         return Decimal('0.0')
 
+    @fields.depends('purchase', '_parent_purchase.warehouse')
+    def on_change_with_warehouse(self, name=None):
+        return self.purchase.warehouse if self.purchase else None
+
     def get_from_location(self, name):
         if (self.quantity or 0) >= 0:
             if self.purchase.party.supplier_location:
                 return self.purchase.party.supplier_location.id
         elif self.purchase.return_from_location:
             return self.purchase.return_from_location.id
 
@@ -1522,23 +1616,47 @@
         return Purchase.fields_get(['state'])['state']['selection']
 
     @fields.depends('purchase', '_parent_purchase.state')
     def on_change_with_purchase_state(self, name=None):
         if self.purchase:
             return self.purchase.state
 
+    @classmethod
+    def search_purchase_state(cls, name, clause):
+        return [('purchase.state', *clause[1:])]
+
     @fields.depends('purchase', '_parent_purchase.company')
     def on_change_with_company(self, name=None):
-        if self.purchase and self.purchase.company:
-            return self.purchase.company.id
+        return self.purchase.company if self.purchase else None
+
+    @fields.depends('purchase', '_parent_purchase.party')
+    def on_change_with_supplier(self, name=None):
+        return self.purchase.party if self.purchase else None
+
+    @classmethod
+    def search_supplier(cls, name, clause):
+        return [('purchase.party' + clause[0][len(name):], *clause[1:])]
+
+    @fields.depends('purchase', '_parent_purchase.purchase_date')
+    def on_change_with_purchase_date(self, name=None):
+        if self.purchase:
+            return self.purchase.purchase_date
+
+    @classmethod
+    def search_purchase_date(cls, name, clause):
+        return [('purchase.purchase_date', *clause[1:])]
+
+    @classmethod
+    def order_purchase_date(cls, tables):
+        return cls.purchase.convert_order(
+            'purchase.purchase_date', tables, cls)
 
     @fields.depends('purchase', '_parent_purchase.currency')
     def on_change_with_currency(self, name=None):
-        if self.purchase and self.purchase.currency:
-            return self.purchase.currency.id
+        return self.purchase.currency if self.purchase else None
 
     def get_invoice_line(self):
         'Return a list of invoice line for purchase line'
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
         AccountConfiguration = pool.get('account.configuration')
         account_config = AccountConfiguration(1)
@@ -1779,14 +1897,26 @@
                 'spell', Eval('_parent_purchase', {}).get('party_lang')),
             ('//label[@id="delivery_date"]', 'states', {
                     'invisible': Eval('type') != 'line',
                     }),
             ]
 
     @classmethod
+    def create(cls, vlist):
+        pool = Pool()
+        Purchase = pool.get('purchase.purchase')
+        purchase_ids = filter(None, {v.get('purchase') for v in vlist})
+        for purchase in Purchase.browse(list(purchase_ids)):
+            if purchase.state != 'draft':
+                raise AccessError(
+                    gettext('purchase.msg_purchase_line_create_draft',
+                        purchase=purchase.rec_name))
+        return super().create(vlist)
+
+    @classmethod
     def delete(cls, lines):
         for line in lines:
             if line.purchase_state not in {'cancelled', 'draft'}:
                 raise AccessError(
                     gettext('purchase.msg_purchase_line_delete_cancel_draft',
                         line=line.rec_name,
                         purchase=line.purchase.rec_name))
@@ -2051,15 +2181,17 @@
         return values
 
     def transition_modify(self):
         pool = Pool()
         Line = pool.get('purchase.line')
 
         purchase = self.get_purchase()
-        purchase.__class__.write([purchase], self.start._save_values)
+        values = self.start._save_values
+        self.model.write([purchase], values)
+        self.model.log([purchase], 'write', ','.join(sorted(values.keys())))
 
         # Call on_change after the save to ensure parent sale
         # has the modified values
         for line in purchase.lines:
             line.on_change_product()
         Line.save(purchase.lines)
 
@@ -2079,20 +2211,19 @@
             Button("Cancel", 'end', 'tryton-cancel'),
             Button("Return", 'return_', 'tryton-ok', default=True),
             ])
     return_ = StateAction('purchase.act_purchase_form')
 
     def do_return_(self, action):
         purchases = self.records
-        return_purchases = self.model.copy(purchases)
-        for return_purchase, purchase in zip(return_purchases, purchases):
-            return_purchase.origin = purchase
-            for line in return_purchase.lines:
-                if line.type == 'line':
-                    line.quantity *= -1
-            return_purchase.lines = return_purchase.lines  # Force saving
-        self.model.save(return_purchases)
+        return_purchases = self.model.copy(purchases, default={
+                'origin': lambda data: (
+                    '%s,%s' % (self.model.__name__, data['id'])),
+                'lines.quantity': lambda data: (
+                    data['quantity'] * -1 if data['type'] == 'line'
+                    else data['quantity']),
+                })
 
         data = {'res_id': [s.id for s in return_purchases]}
         if len(return_purchases) == 1:
             action['views'].reverse()
         return action, data
```

### Comparing `trytond_purchase-6.6.3/purchase.xml` & `trytond_purchase-6.8.0/purchase.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/purchase.xml` & `trytond_purchase-6.8.0/purchase.xml`

```diff
@@ -23,14 +23,15 @@
       <field name="path">icons/tryton-purchase.svg</field>
     </record>
     <menuitem name="Purchases" sequence="70" id="menu_purchase" icon="tryton-purchase"/>
     <record model="ir.ui.menu-res.group" id="menu_purchase_group_purchase">
       <field name="menu" ref="menu_purchase"/>
       <field name="group" ref="group_purchase"/>
     </record>
+    <menuitem name="Reporting" parent="menu_purchase" sequence="100" id="menu_reporting" active="True"/>
     <record model="ir.action.wizard" id="wizard_shipment_handle_exception">
       <field name="name">Handle Shipment Exception</field>
       <field name="wiz_name">purchase.handle.shipment.exception</field>
       <field name="model">purchase.purchase</field>
     </record>
     <record model="ir.action.wizard" id="wizard_invoice_handle_exception">
       <field name="name">Handle Invoice Exception</field>
@@ -43,45 +44,14 @@
       <field name="name">purchase_form</field>
     </record>
     <record model="ir.ui.view" id="purchase_view_tree">
       <field name="model">purchase.purchase</field>
       <field name="type">tree</field>
       <field name="name">purchase_tree</field>
     </record>
-    <record model="ir.action.act_window" id="act_shipment_form">
-      <field name="name">Shipments</field>
-      <field name="res_model">stock.shipment.in</field>
-      <field name="domain" eval="[('moves.purchase', 'in', Eval('active_ids'))]" pyson="1"/>
-    </record>
-    <record model="ir.action.keyword" id="act_open_shipment_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">purchase.purchase,-1</field>
-      <field name="action" ref="act_shipment_form"/>
-    </record>
-    <record model="ir.action.act_window" id="act_return_form">
-      <field name="name">Returns</field>
-      <field name="res_model">stock.shipment.in.return</field>
-      <field name="domain" eval="[('moves.purchase', 'in', Eval('active_ids'))]" pyson="1"/>
-    </record>
-    <record model="ir.action.keyword" id="act_open_shipment_return_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">purchase.purchase,-1</field>
-      <field name="action" ref="act_return_form"/>
-    </record>
-    <record model="ir.action.act_window" id="act_invoice_form">
-      <field name="name">Invoices</field>
-      <field name="res_model">account.invoice</field>
-      <field name="context"/>
-      <field name="domain" eval="[('lines.origin.purchase.id', 'in', Eval('active_ids'), 'purchase.line')]" pyson="1"/>
-    </record>
-    <record model="ir.action.keyword" id="act_open_invoice_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">purchase.purchase,-1</field>
-      <field name="action" ref="act_invoice_form"/>
-    </record>
     <record model="ir.ui.view" id="handle_shipment_exception_ask_view_form">
       <field name="model">purchase.handle.shipment.exception.ask</field>
       <field name="type">form</field>
       <field name="name">handle_shipment_exception_ask_form</field>
     </record>
     <record model="ir.ui.view" id="handle_invoice_exception_ask_view_form">
       <field name="model">purchase.handle.invoice.exception.ask</field>
@@ -165,15 +135,79 @@
       <field name="act_window" ref="act_purchase_invoice_relate"/>
     </record>
     <record model="ir.action.keyword" id="act_purchase_invoice_relate_keyword">
       <field name="keyword">form_relate</field>
       <field name="model">account.invoice,-1</field>
       <field name="action" ref="act_purchase_invoice_relate"/>
     </record>
-    <menuitem name="Reporting" parent="menu_purchase" sequence="100" id="menu_reporting" active="True"/>
+    <record model="ir.action.act_window" id="act_purchase_relate">
+      <field name="name">Purchases</field>
+      <field name="res_model">purchase.purchase</field>
+      <field name="domain" eval="[                 If(Eval('active_model') == 'party.party',                 ('party', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_relate_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="purchase_view_tree"/>
+      <field name="act_window" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_relate_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="purchase_view_form"/>
+      <field name="act_window" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_relate_pending">
+      <field name="name">Pending</field>
+      <field name="sequence" eval="10"/>
+      <field name="domain" eval="[('state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_relate_done">
+      <field name="name">Done</field>
+      <field name="sequence" eval="20"/>
+      <field name="domain" eval="[('state', '=', 'done')]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_relate_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_relate_keyword_party">
+      <field name="keyword">form_relate</field>
+      <field name="model">party.party,-1</field>
+      <field name="action" ref="act_purchase_relate"/>
+    </record>
+    <record model="ir.action.act_window" id="act_purchase_relate_simple">
+      <field name="name">Purchases</field>
+      <field name="res_model">purchase.purchase</field>
+      <field name="domain" eval="[                 If(Eval('active_model') == 'stock.shipment.in',                 ('shipments', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'stock.shipment.in.return',                 ('shipment_returns', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_relate_simple_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="purchase_view_tree"/>
+      <field name="act_window" ref="act_purchase_relate_simple"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_relate_simple_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="purchase_view_form"/>
+      <field name="act_window" ref="act_purchase_relate_simple"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_relate_simple_keyword_shipment_in">
+      <field name="keyword">form_relate</field>
+      <field name="model">stock.shipment.in,-1</field>
+      <field name="action" ref="act_purchase_relate_simple"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_relate_simple_keyword_shipment_in_return">
+      <field name="keyword">form_relate</field>
+      <field name="model">stock.shipment.in.return,-1</field>
+      <field name="action" ref="act_purchase_relate_simple"/>
+    </record>
     <record model="ir.model.access" id="access_purchase">
       <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
@@ -189,14 +223,22 @@
       <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
+    <record model="ir.model.access" id="access_purchase_group_stock">
+      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="group" ref="stock.group_stock"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
     <record model="ir.model.button" id="purchase_cancel_button">
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
       <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button-res.group" id="purchase_cancel_button_group_purchase">
       <field name="button" ref="purchase_cancel_button"/>
@@ -304,14 +346,77 @@
     </record>
     <record model="ir.ui.view" id="purchase_line_view_tree_sequence">
       <field name="model">purchase.line</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">purchase_line_tree_sequence</field>
     </record>
+    <record model="ir.action.act_window" id="act_purchase_line_relate">
+      <field name="name">Purchase Lines</field>
+      <field name="res_model">purchase.line</field>
+      <field name="domain" eval="[('type', '=', 'line'),                 If(Eval('active_model') == 'purchase.purchase',                 ('purchase', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.product',                 ('product', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.template',                 ('product.template.id', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'party.party',                 ('supplier', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_line_relate_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="purchase_line_view_tree"/>
+      <field name="act_window" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_purchase_line_relate_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="purchase_line_view_form"/>
+      <field name="act_window" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_line_relate_pending">
+      <field name="name">Pending</field>
+      <field name="sequence" eval="10"/>
+      <field name="domain" eval="[('purchase_state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_line_relate_done">
+      <field name="name">Done</field>
+      <field name="sequence" eval="20"/>
+      <field name="domain" eval="[('purchase_state', '=', 'done')]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_purchase_line_relate_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_line_relate_keyword_purchase">
+      <field name="keyword">form_relate</field>
+      <field name="model">purchase.purchase,-1</field>
+      <field name="action" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_line_relate_keyword_product">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.product,-1</field>
+      <field name="action" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_line_relate_keyword_product_template">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.template,-1</field>
+      <field name="action" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_purchase_line_relate_keyword_party">
+      <field name="keyword">form_relate</field>
+      <field name="model">party.party,-1</field>
+      <field name="action" ref="act_purchase_line_relate"/>
+    </record>
+    <record model="ir.model.access" id="access_purchase_line_group_stock">
+      <field name="model" search="[('model', '=', 'purchase.line')]"/>
+      <field name="group" ref="stock.group_stock"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
     <record model="ir.ui.view" id="product_supplier_view_form">
       <field name="model">purchase.product_supplier</field>
       <field name="type">form</field>
       <field name="name">product_supplier_form</field>
     </record>
     <record model="ir.ui.view" id="product_supplier_view_tree">
       <field name="model">purchase.product_supplier</field>
@@ -385,24 +490,14 @@
       <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('product_supplier', '=', Eval('active_id')), ('product_supplier', 'in', Eval('active_ids')))]" pyson="1"/>
     </record>
     <record model="ir.action.keyword" id="act_product_supplier_price_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">purchase.product_supplier,-1</field>
       <field name="action" ref="act_product_supplier_price_form"/>
     </record>
-    <record model="ir.ui.view" id="template_view_form">
-      <field name="model">product.template</field>
-      <field name="inherit" ref="product.template_view_form"/>
-      <field name="name">template_form</field>
-    </record>
-    <record model="ir.ui.view" id="template_view_tree">
-      <field name="model">product.template</field>
-      <field name="inherit" ref="product.template_view_tree"/>
-      <field name="name">template_tree</field>
-    </record>
     <record model="ir.ui.view" id="return_purchase_start_view_form">
       <field name="model">purchase.return_purchase.start</field>
       <field name="type">form</field>
       <field name="name">return_purchase_start_form</field>
     </record>
     <record model="ir.action.wizard" id="wizard_return_purchase">
       <field name="name">Return Purchase</field>
@@ -435,49 +530,9 @@
       <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_purchase_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_purchase_companies"/>
     </record>
-    <record model="ir.model.access" id="access_invoice_purchase">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
-      <field name="group" ref="group_purchase"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_invoice_line_purchase">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
-      <field name="group" ref="group_purchase"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_move_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
-      <field name="group" ref="group_purchase"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_shipment_in_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.shipment.in')]"/>
-      <field name="group" ref="group_purchase"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_shipment_in_return_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
-      <field name="group" ref="group_purchase"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
   </data>
 </tryton>
```

### Comparing `trytond_purchase-6.6.3/purchase_reporting.py` & `trytond_purchase-6.8.0/purchase_reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,18 @@
     def _group_by(cls, tables):
         purchase = tables['line.purchase']
         return super()._group_by(tables) + [purchase.party]
 
     def get_rec_name(self, name):
         return self.supplier.rec_name
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('supplier.rec_name', *clause[1:])]
+
 
 class Supplier(SupplierMixin, Abstract, ModelView):
     "Purchase Reporting per Supplier"
     __name__ = 'purchase.reporting.supplier'
 
     time_series = fields.One2Many(
         'purchase.reporting.supplier.time_series', 'supplier',
@@ -348,14 +352,18 @@
 
         name = self.product.rec_name if self.product else None
         if context.get('supplier'):
             supplier = Party(context['supplier'])
             name += '@%s' % supplier.rec_name
         return name
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('product.rec_name', *clause[1:])]
+
 
 class Product(ProductMixin, Abstract, ModelView):
     "Purchase Reporting per Product"
     __name__ = 'purchase.reporting.product'
 
     time_series = fields.One2Many(
         'purchase.reporting.product.time_series', 'product',
```

### Comparing `trytond_purchase-6.6.3/purchase_reporting.xml` & `trytond_purchase-6.8.0/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/setup.py` & `trytond_purchase-6.8.0/setup.py`

 * *Files 6% similar despite different names*

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
@@ -37,38 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for purchase',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-purchase/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/purchase',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase',
     package_dir={'trytond.modules.purchase': '.'},
     packages=(
         ['trytond.modules.purchase']
         + ['trytond.modules.purchase.%s' % p for p in find_packages()]
         ),
@@ -105,24 +105,24 @@
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
         'sparklines': ['pygal'],
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
```

### Comparing `trytond_purchase-6.6.3/stock.py` & `trytond_purchase-6.8.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from sql.operators import Concat
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 def process_purchase(moves_field):
     def _process_purchase(func):
         @wraps(func)
         def wrapper(cls, shipments):
             pool = Pool()
             Purchase = pool.get('purchase.purchase')
             transaction = Transaction()
             context = transaction.context
-            with transaction.set_context(_check_access=False):
+            with without_check_access():
                 purchases = set(m.purchase for s in cls.browse(shipments)
                     for m in getattr(s, moves_field) if m.purchase)
             func(cls, shipments)
             if purchases:
                 with transaction.set_context(
                         queue_batch=context.get('queue_batch', True)):
                     Purchase.__queue__.process(purchases)
@@ -141,15 +141,15 @@
     def _process_purchase_move(func):
         @wraps(func)
         def wrapper(cls, moves):
             pool = Pool()
             Purchase = pool.get('purchase.purchase')
             transaction = Transaction()
             context = transaction.context
-            with transaction.set_context(_check_access=False):
+            with without_check_access():
                 p_moves = cls.browse(moves)
                 if without_shipment:
                     p_moves = [m for m in p_moves if not m.shipment]
                 purchases = set(m.purchase for m in p_moves if m.purchase)
             func(cls, moves)
             if purchases:
                 with transaction.set_context(
@@ -220,30 +220,30 @@
         category = super(Move, self).on_change_with_product_uom_category(
             name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to receive and the quantity to invoice.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, PurchaseLine)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     @property
     def origin_name(self):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
         name = super(Move, self).origin_name
         if isinstance(self.origin, PurchaseLine):
             name = self.origin.purchase.rec_name
         return name
 
     @classmethod
     def search_supplier(cls, name, clause):
-        return [('origin.purchase.party' + clause[0].lstrip(name),)
-            + tuple(clause[1:3]) + ('purchase.line',) + tuple(clause[3:])]
+        return [('origin.purchase.party' + clause[0][len(name):],
+                *clause[1:3], 'purchase.line', *clause[3:])]
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @process_purchase_move(without_shipment=True)
     def do(cls, moves):
         super().do(moves)
```

### Comparing `trytond_purchase-6.6.3/stock.xml` & `trytond_purchase-6.8.0/stock.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/stock.xml` & `trytond_purchase-6.8.0/stock.xml`

```diff
@@ -5,80 +5,32 @@
   <data>
     <record model="ir.ui.view" id="move_view_list_shipment">
       <field name="model">stock.move</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">move_list_shipment</field>
     </record>
+    <record model="ir.model.access" id="access_move_group_purchase">
+      <field name="model" search="[('model', '=', 'stock.move')]"/>
+      <field name="group" ref="group_purchase"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
     <record model="ir.ui.view" id="location_view_form">
       <field name="model">stock.location</field>
       <field name="inherit" ref="stock.location_view_form"/>
       <field name="name">location_form</field>
     </record>
     <record model="ir.ui.view" id="move_view_list_shipment_in">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_list_shipment_in"/>
       <field name="name">move_list_shipment_in</field>
     </record>
-    <record model="ir.model.access" id="access_purchase_group_stock">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
-      <field name="group" ref="stock.group_stock"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_purchase_line_group_stock">
-      <field name="model" search="[('model', '=', 'purchase.line')]"/>
-      <field name="group" ref="stock.group_stock"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.action.act_window" id="act_purchase_shipments_relate">
-      <field name="name">Purchases</field>
-      <field name="res_model">purchase.purchase</field>
-      <field name="domain" eval="[('shipments', 'in', Eval('active_ids'))]" pyson="1"/>
-    </record>
-    <record model="ir.action.act_window.view" id="act_purchase_shipments_relate_view1">
-      <field name="sequence" eval="10"/>
-      <field name="view" ref="purchase_view_tree"/>
-      <field name="act_window" ref="act_purchase_shipments_relate"/>
-    </record>
-    <record model="ir.action.act_window.view" id="act_purchase_shipments_relate_view2">
-      <field name="sequence" eval="20"/>
-      <field name="view" ref="purchase_view_form"/>
-      <field name="act_window" ref="act_purchase_shipments_relate"/>
-    </record>
-    <record model="ir.action.keyword" id="act_purchase_shipments_relate_keyword">
-      <field name="keyword">form_relate</field>
-      <field name="model">stock.shipment.in,-1</field>
-      <field name="action" ref="act_purchase_shipments_relate"/>
-    </record>
-    <record model="ir.action.act_window" id="act_purchase_shipment_returns_relate">
-      <field name="name">Purchases</field>
-      <field name="res_model">purchase.purchase</field>
-      <field name="domain" eval="[('shipment_returns', 'in', Eval('active_ids'))]" pyson="1"/>
-    </record>
-    <record model="ir.action.act_window.view" id="act_purchase_shipment_returns_relate_view1">
-      <field name="sequence" eval="10"/>
-      <field name="view" ref="purchase_view_tree"/>
-      <field name="act_window" ref="act_purchase_shipment_returns_relate"/>
-    </record>
-    <record model="ir.action.act_window.view" id="act_purchase_shipment_returns_relate_view2">
-      <field name="sequence" eval="20"/>
-      <field name="view" ref="purchase_view_form"/>
-      <field name="act_window" ref="act_purchase_shipment_returns_relate"/>
-    </record>
-    <record model="ir.action.keyword" id="act_purchase_shipment_returns_relate_keyword">
-      <field name="keyword">form_relate</field>
-      <field name="model">stock.shipment.in.return,-1</field>
-      <field name="action" ref="act_purchase_shipment_returns_relate"/>
-    </record>
     <record model="ir.action.act_window" id="act_purchase_move_relate">
       <field name="name">Moves</field>
       <field name="res_model">stock.move</field>
       <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('purchase', '=', Eval('active_id')), ('purchase', 'in', Eval('active_ids')))]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_form_view1">
       <field name="sequence" eval="10"/>
@@ -91,9 +43,45 @@
       <field name="act_window" ref="act_purchase_move_relate"/>
     </record>
     <record model="ir.action.keyword" id="act_move_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">purchase.purchase,-1</field>
       <field name="action" ref="act_purchase_move_relate"/>
     </record>
+    <record model="ir.action.act_window" id="act_shipment_form">
+      <field name="name">Shipments</field>
+      <field name="res_model">stock.shipment.in</field>
+      <field name="domain" eval="[('moves.purchase', 'in', Eval('active_ids'))]" pyson="1"/>
+    </record>
+    <record model="ir.action.keyword" id="act_open_shipment_keyword1">
+      <field name="keyword">form_relate</field>
+      <field name="model">purchase.purchase,-1</field>
+      <field name="action" ref="act_shipment_form"/>
+    </record>
+    <record model="ir.model.access" id="access_shipment_in_group_purchase">
+      <field name="model" search="[('model', '=', 'stock.shipment.in')]"/>
+      <field name="group" ref="group_purchase"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
+    <record model="ir.action.act_window" id="act_return_form">
+      <field name="name">Returns</field>
+      <field name="res_model">stock.shipment.in.return</field>
+      <field name="domain" eval="[('moves.purchase', 'in', Eval('active_ids'))]" pyson="1"/>
+    </record>
+    <record model="ir.action.keyword" id="act_open_shipment_return_keyword1">
+      <field name="keyword">form_relate</field>
+      <field name="model">purchase.purchase,-1</field>
+      <field name="action" ref="act_return_form"/>
+    </record>
+    <record model="ir.model.access" id="access_shipment_in_return_group_purchase">
+      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
+      <field name="group" ref="group_purchase"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 =================
 Purchase Scenario
 =================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
 
@@ -41,15 +41,15 @@
     >>> user.employee = employee
     >>> user.save()
     >>> set_user(user.id)
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> revenue = accounts['revenue']
@@ -178,15 +178,15 @@
     >>> purchase.confirmed_by == employee
     True
     >>> purchase.state
     'processing'
     >>> purchase.shipment_state
     'waiting'
     >>> purchase.invoice_state
-    'waiting'
+    'pending'
     >>> len(purchase.moves), len(purchase.shipment_returns), len(purchase.invoices)
     (2, 0, 1)
     >>> invoice, = purchase.invoices
     >>> invoice.origins == purchase.rec_name
     True
     >>> invoice.untaxed_amount, invoice.tax_amount, invoice.total_amount
     (Decimal('25.00'), Decimal('2.50'), Decimal('27.50'))
@@ -215,15 +215,15 @@
 
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> purchase.reload()
     >>> purchase.shipment_state
     'waiting'
     >>> purchase.invoice_state
-    'waiting'
+    'awaiting payment'
     >>> len(purchase.moves), len(purchase.shipment_returns), len(purchase.invoices)
     (2, 0, 1)
 
 Purchase 5 products with an invoice method 'on shipment'::
 
     >>> purchase = Purchase()
     >>> purchase.party = supplier
@@ -280,15 +280,15 @@
     'received'
     >>> len(purchase.shipments), len(purchase.shipment_returns)
     (1, 0)
 
 Open supplier invoice::
 
     >>> purchase.invoice_state
-    'waiting'
+    'pending'
     >>> invoice, = purchase.invoices
     >>> invoice.type
     'in'
     >>> invoice_line1, invoice_line2 = sorted(invoice.lines,
     ...     key=lambda l: l.quantity or 0)
     >>> for line in invoice.lines:
     ...     line.quantity = 1
@@ -354,25 +354,24 @@
     'waiting'
     >>> move_return, = ship_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     4.0
     >>> ship_return.click('assign_try')
-    True
     >>> ship_return.click('done')
     >>> ship_return.state
     'done'
     >>> return_.reload()
     >>> return_.state
     'processing'
     >>> return_.shipment_state
     'received'
     >>> return_.invoice_state
-    'waiting'
+    'pending'
 
 Open supplier credit note::
 
     >>> credit_note, = return_.invoices
     >>> credit_note.type
     'in'
     >>> len(credit_note.lines)
@@ -403,15 +402,15 @@
     >>> mix.click('quote')
     >>> mix.click('confirm')
     >>> mix.state
     'processing'
     >>> mix.shipment_state
     'waiting'
     >>> mix.invoice_state
-    'waiting'
+    'pending'
     >>> len(mix.moves), len(mix.shipment_returns), len(mix.invoices)
     (2, 1, 1)
 
 Checking Shipments::
 
     >>> mix_return, = mix.shipment_returns
     >>> mix_shipment = ShipmentIn()
@@ -425,15 +424,14 @@
     >>> mix_shipment.click('done')
     >>> mix.reload()
     >>> len(mix.shipments)
     1
 
     >>> mix_return.click('wait')
     >>> mix_return.click('assign_try')
-    True
     >>> mix_return.click('done')
     >>> move_return, = mix_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     2.0
 
@@ -493,15 +491,14 @@
     >>> mix_shipment.click('done')
     >>> mix.reload()
     >>> len(mix.shipments)
     1
 
     >>> mix_return.click('wait')
     >>> mix_return.click('assign_try')
-    True
     >>> mix_return.click('done')
     >>> move_return, = mix_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     3.0
 
@@ -517,22 +514,22 @@
     >>> service_purchase.click('quote')
     >>> service_purchase.click('confirm')
     >>> service_purchase.state
     'processing'
     >>> service_purchase.shipment_state
     'none'
     >>> service_purchase.invoice_state
-    'waiting'
+    'pending'
     >>> service_invoice, = service_purchase.invoices
 
 Pay the service invoice::
 
     >>> service_invoice.invoice_date = today
     >>> service_invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [service_invoice])
+    >>> pay = service_invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.form.amount = service_invoice.total_amount
     >>> pay.execute('choice')
     >>> service_invoice.reload()
     >>> service_invoice.state
     'paid'
```

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase_empty.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase_modify_header.rst`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     >>> purchase_line.quantity = 3
     >>> purchase.save()
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('15.00'), Decimal('1.50'), Decimal('16.50'))
 
 Change the party::
 
-    >>> modify_header = Wizard('purchase.modify_header', [purchase])
+    >>> modify_header = purchase.click('modify_header')
     >>> modify_header.form.party == supplier
     True
     >>> modify_header.form.party = another
     >>> modify_header.execute('modify')
 
     >>> purchase.party.name
     'Another Supplier'
```

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase_reporting.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-6.8.0/tests/scenario_purchase_return_wizard.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 ===============================
 Purchase Return Wizard Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
-
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
```

### Comparing `trytond_purchase-6.6.3/tests/test_module.py` & `trytond_purchase-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/tox.ini` & `trytond_purchase-6.8.0/tox.ini`

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
-    coverage run --include=./**/purchase/* -m unittest discover -s tests
-    coverage report --include=./**/purchase/* --omit=*/tests/*
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

### Comparing `trytond_purchase-6.6.3/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-6.8.0/trytond_purchase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-purchase
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 ###############
 Purchase Module
 ###############
```

### Comparing `trytond_purchase-6.6.3/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-6.8.0/trytond_purchase.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.rst
 __init__.py
 configuration.py
 configuration.xml
 exceptions.py
 invoice.py
+invoice.xml
 message.xml
 party.py
 party.xml
 product.py
 product.xml
 purchase.fodt
 purchase.py
@@ -24,14 +25,15 @@
 tox.ini
 tryton.cfg
 ./__init__.py
 ./configuration.py
 ./configuration.xml
 ./exceptions.py
 ./invoice.py
+./invoice.xml
 ./message.xml
 ./party.py
 ./party.xml
 ./product.py
 ./product.xml
 ./purchase.fodt
 ./purchase.py
```

### Comparing `trytond_purchase-6.6.3/view/party_form.xml` & `trytond_purchase-6.8.0/view/party_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/view/party_form.xml` & `trytond_purchase-6.8.0/view/party_form.xml`

```diff
@@ -1,13 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <data>
   <xpath expr="//group[@id='links']" position="inside">
-    <link icon="tryton-purchase" name="purchase.act_purchase_form2" empty="hide"/>
+    <link icon="tryton-purchase" name="purchase.act_purchase_relate" empty="hide"/>
+    <link icon="tryton-purchase" name="purchase.act_purchase_line_relate" empty="hide"/>
   </xpath>
   <xpath expr="/form/notebook/page[@id='general']" position="after">
     <page string="Supplier" id="supplier">
       <label name="customer_code"/>
       <field name="customer_code"/>
       <newline/>
       <label name="supplier_lead_time"/>
```

### Comparing `trytond_purchase-6.6.3/view/product_supplier_form.xml` & `trytond_purchase-6.8.0/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/view/purchase_form.xml` & `trytond_purchase-6.8.0/view/purchase_form.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/view/purchase_form.xml` & `trytond_purchase-6.8.0/view/purchase_form.xml`

```diff
@@ -7,16 +7,15 @@
   <label name="contact"/>
   <field name="contact"/>
   <label name="number"/>
   <field name="number"/>
   <label name="invoice_party"/>
   <field name="invoice_party"/>
   <label name="invoice_address"/>
-  <field name="invoice_address"/>
-  <newline/>
+  <field name="invoice_address" colspan="3"/>
   <label name="description"/>
   <field name="description" colspan="3"/>
   <label name="reference"/>
   <field name="reference"/>
   <notebook colspan="6">
     <page string="Purchase" id="purchase">
       <label name="purchase_date"/>
```

### Comparing `trytond_purchase-6.6.3/view/purchase_line_form.xml` & `trytond_purchase-6.8.0/view/purchase_line_form.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/view/purchase_line_form.xml` & `trytond_purchase-6.8.0/view/purchase_line_form.xml`

```diff
@@ -29,13 +29,19 @@
       </group>
       <separator name="description" colspan="4"/>
       <field name="description" colspan="4"/>
     </page>
     <page string="Taxes" id="taxes">
       <field name="taxes" colspan="4"/>
     </page>
+    <page name="moves" col="1">
+      <field name="moves"/>
+    </page>
+    <page name="invoice_lines" col="1">
+      <field name="invoice_lines"/>
+    </page>
     <page string="Notes" id="notes">
       <separator name="note" colspan="4"/>
       <field name="note" colspan="4"/>
     </page>
   </notebook>
 </form>
```

### Comparing `trytond_purchase-6.6.3/view/purchase_line_tree.xml` & `trytond_purchase-6.8.0/view/purchase_line_tree.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/view/purchase_line_tree.xml` & `trytond_purchase-6.8.0/view/purchase_line_tree.xml`

```diff
@@ -1,14 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tree>
   <field name="purchase" expand="1"/>
+  <field name="supplier" expand="1" optional="0"/>
+  <field name="purchase_date" optional="1"/>
   <field name="type" optional="1"/>
   <field name="product" expand="1" optional="0"/>
   <field name="product_supplier" expand="1" optional="1"/>
   <field name="summary" expand="1" optional="1"/>
-  <field name="quantity" symbol="unit"/>
+  <field name="actual_quantity" symbol="unit" optional="0"/>
+  <field name="quantity" symbol="unit" optional="0"/>
   <field name="unit_price"/>
-  <field name="taxes" optional="0"/>
   <field name="amount"/>
+  <field name="purchase_state"/>
 </tree>
```

### Comparing `trytond_purchase-6.6.3/view/purchase_line_tree_sequence.xml` & `trytond_purchase-6.8.0/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/view/purchase_reporting_context_form.xml` & `trytond_purchase-6.8.0/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/view/purchase_tree.xml` & `trytond_purchase-6.8.0/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.6.3/view/template_form.xml` & `trytond_purchase-6.8.0/view/template_form.xml`

 * *Files 13% similar despite different names*

#### Comparing `trytond_purchase-6.6.3/view/template_form.xml` & `trytond_purchase-6.8.0/view/template_form.xml`

```diff
@@ -9,10 +9,13 @@
   <xpath expr="/form/notebook/page[@id='general']" position="after">
     <page string="Suppliers" id="suppliers">
       <label name="purchasable"/>
       <field name="purchasable"/>
       <label name="purchase_uom"/>
       <field name="purchase_uom"/>
       <field name="product_suppliers" colspan="4" view_ids="purchase.product_supplier_view_tree_sequence"/>
+      <group id="suppliers_links" col="-1" colspan="4">
+        <link icon="tryton-purchase" name="purchase.act_purchase_line_relate" empty="hide"/>
+      </group>
     </page>
   </xpath>
 </data>
```

