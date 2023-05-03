# Comparing `tmp/trytond_sale-6.6.2.tar.gz` & `tmp/trytond_sale-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-6.6.2.tar", last modified: Wed May  3 16:46:55 2023, max compression
+gzip compressed data, was "trytond_sale-6.8.0.tar", last modified: Mon May  1 12:01:27 2023, max compression
```

## Comparing `trytond_sale-6.6.2.tar` & `trytond_sale-6.8.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.714213 trytond_sale-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     5867 2023-05-03 16:46:51.000000 trytond_sale-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-03 16:46:51.000000 trytond_sale-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-05-03 16:46:55.714213 trytond_sale-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5014 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.697546 trytond_sale-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_sale-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9118 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.704213 trytond_sale-6.6.2/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/doc/usage/presales.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2022-12-19 12:02:51.000000 trytond_sale-6.6.2/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-12-19 12:02:51.000000 trytond_sale-6.6.2/doc/usage/reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2022-12-19 12:02:52.000000 trytond_sale-6.6.2/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2022-12-19 12:02:54.000000 trytond_sale-6.6.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.704213 trytond_sale-6.6.2/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5302 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.667546 trytond_sale-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    40496 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40889 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35486 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41531 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41042 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33963 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38958 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43482 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35447 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41369 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39759 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36697 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38078 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39455 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39999 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40886 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37012 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38299 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41206 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40538 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37984 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35438 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33441 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35665 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4616 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3316 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2156 2023-04-08 09:35:50.000000 trytond_sale-6.6.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    68698 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    77365 2023-04-22 21:24:47.000000 trytond_sale-6.6.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24475 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    38738 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:46:55.714213 trytond_sale-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4540 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7450 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1704 2023-04-08 09:35:50.000000 trytond_sale-6.6.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.674213 trytond_sale-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20247 2023-04-08 09:35:50.000000 trytond_sale-6.6.2/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2978 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12776 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2526 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.710880 trytond_sale-6.6.2/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-05-03 16:46:54.000000 trytond_sale-6.6.2/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4895 2023-05-03 16:46:55.000000 trytond_sale-6.6.2/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:46:54.000000 trytond_sale-6.6.2/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-05-03 16:46:54.000000 trytond_sale-6.6.2/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:40:41.000000 trytond_sale-6.6.2/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-05-03 16:46:54.000000 trytond_sale-6.6.2/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:46:54.000000 trytond_sale-6.6.2/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:46:55.690880 trytond_sale-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2022-12-19 12:02:53.000000 trytond_sale-6.6.2/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:52.000000 trytond_sale-6.6.2/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2022-12-19 12:02:53.000000 trytond_sale-6.6.2/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      762 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2022-12-19 12:02:50.000000 trytond_sale-6.6.2/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1366 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      762 2023-04-08 09:35:50.000000 trytond_sale-6.6.2/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-13 16:52:41.000000 trytond_sale-6.6.2/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6223 2023-05-01 11:14:41.000000 trytond_sale-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:14:41.000000 trytond_sale-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5173 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.900536 trytond_sale-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9118 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.903869 trytond_sale-6.8.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/presales.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.903869 trytond_sale-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.890535 trytond_sale-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    42111 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42743 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37074 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43431 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42922 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35457 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40621 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    45323 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37035 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43294 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41625 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38328 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39740 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41170 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41661 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42791 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38642 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39960 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43083 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42203 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39643 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34909 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37290 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4405 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4574 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9820 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2671 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76266 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81894 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24722 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    39881 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4515 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7402 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.893869 trytond_sale-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20162 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12999 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2526 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-05-01 11:14:35.000000 trytond_sale-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4921 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale-6.8.0/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.900536 trytond_sale-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3721 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/template_tree.xml
```

### Comparing `trytond_sale-6.6.2/CHANGELOG` & `trytond_sale-6.8.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 
-Version 6.6.2 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Fill taxes from default account for line without product
+* Add partially shipped to shipment state
+* Add pending, awaiting payment and partially paid to invoice state
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Add related stock moves and invoice lines on sale line
+* Add relate to sale lines from party and product
+* Simplify relate to sales
+* Prevent creation of lines for non draft sales
+* Allow searching reporting records by name
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add sale reporting per region
 * Support warehouse pickup
 * Use MultiValue for product lead time
```

### Comparing `trytond_sale-6.6.2/COPYRIGHT` & `trytond_sale-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/LICENSE` & `trytond_sale-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/PKG-INFO` & `trytond_sale-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale
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
 
 ###########
 Sale Module
 ###########
```

### Comparing `trytond_sale-6.6.2/__init__.py` & `trytond_sale-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/configuration.py` & `trytond_sale-6.8.0/configuration.py`

 * *Files 6% similar despite different names*

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
 
 sale_invoice_method = fields.Selection(
     'get_sale_invoice_methods', "Sale Invoice Method")
 sale_shipment_method = fields.Selection(
     'get_sale_shipment_methods', "Sale Shipment Method")
 
@@ -44,15 +44,20 @@
                     [Eval('context', {}).get('company', -1), None]),
                 ('sequence_type', '=', Id('sale', 'sequence_type_sale')),
                 ]))
     sale_invoice_method = fields.MultiValue(sale_invoice_method)
     get_sale_invoice_methods = get_sale_methods('invoice_method')
     sale_shipment_method = fields.MultiValue(sale_shipment_method)
     get_sale_shipment_methods = get_sale_methods('shipment_method')
-    sale_process_after = fields.TimeDelta("Process Sale after",
+    sale_process_after = fields.TimeDelta(
+        "Process Sale after",
+        domain=['OR',
+            ('sale_process_after', '=', None),
+            ('sale_process_after', '>=', TimeDelta()),
+            ],
         help="The grace period during which confirmed sale "
         "can still be reset to draft.\n"
         "Applied if a worker queue is activated.")
 
     @classmethod
     def multivalue_model(cls, field):
         pool = Pool()
```

### Comparing `trytond_sale-6.6.2/configuration.xml` & `trytond_sale-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/doc/conf.py` & `trytond_sale-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale-6.6.2/doc/design.rst` & `trytond_sale-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/doc/usage/presales.rst` & `trytond_sale-6.8.0/doc/usage/presales.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/doc/usage/process.rst` & `trytond_sale-6.8.0/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/doc/usage/reporting.rst` & `trytond_sale-6.8.0/doc/usage/reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/doc/usage/returns.rst` & `trytond_sale-6.8.0/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/icons/LICENSE` & `trytond_sale-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/invoice.py` & `trytond_sale-6.8.0/invoice.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # this repository contains the full copyright notices and license terms.
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
-from trytond.transaction import Transaction
+from trytond.pyson import Eval
+from trytond.transaction import Transaction, without_check_access
 
 
 def process_sale(func):
     @wraps(func)
     def wrapper(cls, invoices):
         pool = Pool()
         Sale = pool.get('sale.sale')
         transaction = Transaction()
         context = transaction.context
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             sales = set(s for i in cls.browse(invoices) for s in i.sales)
         func(cls, invoices)
         if sales:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
                 Sale.__queue__.process(sales)
     return wrapper
@@ -56,25 +57,16 @@
         for line in self.lines:
             if isinstance(line.origin, SaleLine):
                 sales.add(line.origin.sale.id)
         return list(sales)
 
     @classmethod
     def search_sales(cls, name, clause):
-        return [('lines.origin.sale' + clause[0].lstrip(name),)
-            + tuple(clause[1:3]) + ('sale.line',) + tuple(clause[3:])]
-
-    @classmethod
-    def copy(cls, invoices, default=None):
-        if default is None:
-            default = {}
-        else:
-            default = default.copy()
-        default.setdefault('sales', None)
-        return super(Invoice, cls).copy(invoices, default=default)
+        return [('lines.origin.sale' + clause[0][len(name):],
+                *clause[1:3], 'sale.line', *clause[3:])]
 
     @classmethod
     @process_sale
     def delete(cls, invoices):
         super(Invoice, cls).delete(invoices)
 
     @classmethod
@@ -103,25 +95,34 @@
 
         return super(Invoice, cls).draft(invoices)
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'account.invoice.line'
 
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        if not cls.origin.domain:
+            cls.origin.domain = {}
+        cls.origin.domain['sale.line'] = [
+            ('type', '=', Eval('type')),
+            ]
+
     @fields.depends('origin')
     def on_change_with_product_uom_category(self, name=None):
         pool = Pool()
         SaleLine = pool.get('sale.line')
         category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to invoice and the quantity to ship.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, SaleLine)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     def get_warehouse(self, name):
         pool = Pool()
         SaleLine = pool.get('sale.line')
         warehouse = super().get_warehouse(name)
         if (not warehouse
@@ -147,15 +148,15 @@
 
     @classmethod
     def delete(cls, lines):
         pool = Pool()
         Sale = pool.get('sale.sale')
         transaction = Transaction()
         context = transaction.context
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             invoices = (l.invoice for l in cls.browse(lines)
                 if l.type == 'line' and l.invoice)
             sales = set(s for i in invoices for s in i.sales)
         super().delete(lines)
         if sales:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
```

### Comparing `trytond_sale-6.6.2/locale/bg.po` & `trytond_sale-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice,sale_exception_state:"
 msgid "Exception State"
-msgstr "Състояние на грешка"
+msgstr "Состояние ситуации"
 
 msgctxt "field:account.invoice,sales:"
 msgid "Sales"
-msgstr "Продажби"
+msgstr "Продажи"
 
 #, fuzzy
 msgctxt "field:party.party,customer_currencies:"
 msgid "Customer Currencies"
-msgstr "Клиенти"
+msgstr "Заказчики"
 
 #, fuzzy
 msgctxt "field:party.party,customer_currency:"
 msgid "Customer Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:party.party,sale_invoice_method:"
 msgid "Invoice Method"
-msgstr "Начин на фактуриране"
+msgstr "Метод инвойса"
 
 #, fuzzy
 msgctxt "field:party.party,sale_methods:"
 msgid "Sale Methods"
-msgstr "Начин на фактурине на продажба"
+msgstr "Метод инвойса продажи"
 
 #, fuzzy
 msgctxt "field:party.party,sale_shipment_method:"
 msgid "Shipment Method"
-msgstr "Начин на изпращане"
+msgstr "Метод доставки"
 
 #, fuzzy
 msgctxt "field:party.party.customer_currency,customer_currency:"
 msgid "Customer Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:party.party.customer_currency,party:"
 msgid "Party"
-msgstr "Партньор"
+msgstr "Контрагент"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,party:"
 msgid "Party"
-msgstr "Партньор"
+msgstr "Контрагент"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Начин на фактурине на продажба"
+msgstr "Метод инвойса продажи"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Начин на фактуриране на продажба"
+msgstr "Способ доставки продажи"
 
 msgctxt "field:product.configuration,default_lead_time:"
 msgid "Default Lead Time"
 msgstr ""
 
 msgctxt "field:product.configuration.default_lead_time,default_lead_time:"
 msgid "Default Lead Time"
@@ -81,261 +81,281 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product,salable:"
 msgid "Salable"
-msgstr "Продажен"
+msgstr "Для продажи"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,sale_uom:"
 msgid "Sale UOM"
-msgstr "Мер. ед. на продажба"
+msgstr "Ед.измерения продажи"
 
 #, fuzzy
 msgctxt "field:product.sale.context,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:product.sale.context,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:product.sale.context,customer:"
 msgid "Customer"
-msgstr "Клиенти"
+msgstr "Заказчики"
 
 #, fuzzy
 msgctxt "field:product.sale.context,locations:"
 msgid "Warehouses"
-msgstr "Склад"
+msgstr "Товарный склад"
 
 #, fuzzy
 msgctxt "field:product.sale.context,quantity:"
 msgid "Quantity"
-msgstr "Количество"
+msgstr "Кол-во"
 
 #, fuzzy
 msgctxt "field:product.sale.context,sale_date:"
 msgid "Sale Date"
-msgstr "Дата на продажба"
+msgstr "Дата продажи"
 
 msgctxt "field:product.sale.context,stock_date_end:"
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
-msgstr "Продажен"
+msgstr "Для продажи"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
-msgstr "Мер. ед. на продажба"
+msgstr "Ед.измерения продажи"
 
 msgctxt "field:sale.configuration,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Начин на фактурине на продажба"
+msgstr "Метод инвойса продажи"
 
 msgctxt "field:sale.configuration,sale_process_after:"
 msgid "Process Sale after"
 msgstr ""
 
 msgctxt "field:sale.configuration,sale_sequence:"
 msgid "Sale Sequence"
 msgstr ""
 
 msgctxt "field:sale.configuration,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Начин на фактуриране на продажба"
+msgstr "Способ доставки продажи"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sale_method,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Начин на фактурине на продажба"
+msgstr "Метод инвойса продажи"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sale_method,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Начин на фактуриране на продажба"
+msgstr "Способ доставки продажи"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sequence,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 msgctxt "field:sale.configuration.sequence,sale_sequence:"
 msgid "Sale Sequence"
 msgstr ""
 
 msgctxt "field:sale.handle.invoice.exception.ask,domain_invoices:"
 msgid "Domain Invoices"
-msgstr "Фактури на домейн"
+msgstr "Домен инвойсов"
 
 msgctxt "field:sale.handle.invoice.exception.ask,recreate_invoices:"
 msgid "Recreate Invoices"
-msgstr "Наново създаване на фактури"
+msgstr "Создать заново инвойсы"
 
 msgctxt "field:sale.handle.shipment.exception.ask,domain_moves:"
 msgid "Domain Moves"
-msgstr "Движение на домейн"
+msgstr "Домен проводок"
 
 msgctxt "field:sale.handle.shipment.exception.ask,recreate_moves:"
 msgid "Recreate Moves"
-msgstr "Наново създаване на движения"
+msgstr "Создать заново проводки"
 
 #, fuzzy
 msgctxt "field:sale.line,actual_quantity:"
 msgid "Actual Quantity"
-msgstr "Количество"
+msgstr "Кол-во"
 
 msgctxt "field:sale.line,amount:"
 msgid "Amount"
-msgstr "Сума"
+msgstr "Сумма"
 
 #, fuzzy
 msgctxt "field:sale.line,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
+
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Заказчики"
 
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
-msgstr "От местонахождение"
+msgstr "Из местоположения"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Редове от фактура"
-
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Направени движения"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Грешка при движение"
+msgstr "Строки инвойса"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
-msgstr "Движения"
+msgstr "Перемещения"
+
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Особые ситуации перемещения"
 
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
-msgstr "Игнорирани движения"
+msgstr "Игнорированные проводки"
+
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Перемещения выполнены"
 
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
-msgstr "Наново създаване на движения"
+msgstr "Созданные заново проводки"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
-msgstr "Бележка"
+msgstr "Комментарий"
 
 msgctxt "field:sale.line,product:"
 msgid "Product"
 msgstr "Продукт"
 
 msgctxt "field:sale.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Категория мер. ед. на продукт"
+msgstr "Категория ед. измерения продукции"
 
 msgctxt "field:sale.line,quantity:"
 msgid "Quantity"
-msgstr "Количество"
+msgstr "Кол-во"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
+
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Дата продажи"
 
 #, fuzzy
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
-msgstr "Дата на продажба"
+msgstr "Дата продажи"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
 
 msgctxt "field:sale.line,summary:"
 msgid "Summary"
 msgstr ""
 
 msgctxt "field:sale.line,taxes:"
 msgid "Taxes"
-msgstr "Данъци"
+msgstr "Налоги"
 
 msgctxt "field:sale.line,to_location:"
 msgid "To Location"
-msgstr "Към местонахождение"
+msgstr "В местоположение"
 
 msgctxt "field:sale.line,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr "Тип"
 
 msgctxt "field:sale.line,unit:"
 msgid "Unit"
-msgstr "Единица"
+msgstr "Единица измерения"
 
 msgctxt "field:sale.line,unit_price:"
 msgid "Unit Price"
-msgstr "Единична цена"
+msgstr "Цена за единицу"
 
 msgctxt "field:sale.line,warehouse:"
 msgid "Warehouse"
-msgstr "Склад"
+msgstr "Товарный склад"
 
 msgctxt "field:sale.line-account.tax,line:"
 msgid "Sale Line"
-msgstr "Ред от продажба"
+msgstr "Строка продажи"
 
 msgctxt "field:sale.line-account.tax,tax:"
 msgid "Tax"
-msgstr "Данък"
+msgstr "Налог"
 
 msgctxt "field:sale.line-ignored-stock.move,move:"
 msgid "Move"
-msgstr "Движение"
+msgstr "Перемещение"
 
 msgctxt "field:sale.line-ignored-stock.move,sale_line:"
 msgid "Sale Line"
-msgstr "Ред от продажба"
+msgstr "Строка продажи"
 
 msgctxt "field:sale.line-recreated-stock.move,move:"
 msgid "Move"
-msgstr "Движение"
+msgstr "Перемещение"
 
 msgctxt "field:sale.line-recreated-stock.move,sale_line:"
 msgid "Sale Line"
-msgstr "Ред от продажба"
+msgstr "Строка продажи"
 
 #, fuzzy
 msgctxt "field:sale.reporting.context,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 msgctxt "field:sale.reporting.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:sale.reporting.context,period:"
 msgid "Period"
@@ -344,15 +364,15 @@
 msgctxt "field:sale.reporting.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.context,warehouse:"
 msgid "Warehouse"
-msgstr "Склад"
+msgstr "Товарный склад"
 
 msgctxt "field:sale.reporting.country,country:"
 msgid "Country"
 msgstr ""
 
 msgctxt "field:sale.reporting.country.subdivision,country:"
 msgid "Country"
@@ -386,15 +406,15 @@
 msgctxt "field:sale.reporting.country.tree,region:"
 msgid "Region"
 msgstr "Open Region"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer,customer:"
 msgid "Customer"
-msgstr "Клиенти"
+msgstr "Заказчики"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category,category:"
 msgid "Category"
 msgstr "Sales per Category"
 
 #, fuzzy
@@ -405,33 +425,33 @@
 msgctxt "field:sale.reporting.customer.category.tree,children:"
 msgid "Children"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:sale.reporting.customer.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,revenue:"
 msgid "Revenue"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.time_series,customer:"
 msgid "Customer"
-msgstr "Клиенти"
+msgstr "Заказчики"
 
 #, fuzzy
 msgctxt "field:sale.reporting.product,product:"
 msgid "Product"
 msgstr "Продукт"
 
 #, fuzzy
@@ -447,20 +467,20 @@
 msgctxt "field:sale.reporting.product.category.tree,children:"
 msgid "Children"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:sale.reporting.product.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,revenue:"
 msgid "Revenue"
@@ -470,20 +490,20 @@
 msgctxt "field:sale.reporting.product.time_series,product:"
 msgid "Product"
 msgstr "Продукт"
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:sale.reporting.region.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.region.tree,revenue:"
 msgid "Revenue"
@@ -491,194 +511,194 @@
 
 msgctxt "field:sale.reporting.region.tree,subregions:"
 msgid "Subregions"
 msgstr ""
 
 msgctxt "field:sale.sale,comment:"
 msgid "Comment"
-msgstr "Коментар"
+msgstr "Комментарии"
 
 msgctxt "field:sale.sale,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:sale.sale,confirmed_by:"
 msgid "Confirmed By"
-msgstr "Потвърден"
+msgstr "Confirmed"
 
 msgctxt "field:sale.sale,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.sale,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 msgctxt "field:sale.sale,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:sale.sale,invoice_address:"
 msgid "Invoice Address"
-msgstr "Адрес за фактура"
+msgstr "Адрес для инвойса"
 
 msgctxt "field:sale.sale,invoice_method:"
 msgid "Invoice Method"
-msgstr "Начин на фактуриране"
+msgstr "Метод инвойса"
 
 #, fuzzy
 msgctxt "field:sale.sale,invoice_party:"
 msgid "Invoice Party"
-msgstr "Състояние на фактура"
+msgstr "Состояние инвойса"
 
 msgctxt "field:sale.sale,invoice_state:"
 msgid "Invoice State"
-msgstr "Състояние на фактура"
+msgstr "Состояние инвойса"
 
 msgctxt "field:sale.sale,invoices:"
 msgid "Invoices"
-msgstr "Фактури"
+msgstr "Инвойсы"
 
 msgctxt "field:sale.sale,invoices_ignored:"
 msgid "Ignored Invoices"
-msgstr "Игнорирани фактури"
+msgstr "Игнорированные инвойсы"
 
 msgctxt "field:sale.sale,invoices_recreated:"
 msgid "Recreated Invoices"
-msgstr "Наново създадени на фактури"
+msgstr "Созданные заново инвойсы"
 
 msgctxt "field:sale.sale,lines:"
 msgid "Lines"
-msgstr "Редове"
+msgstr "Строки"
 
 msgctxt "field:sale.sale,moves:"
 msgid "Moves"
-msgstr "Движения"
+msgstr "Перемещения"
 
 #, fuzzy
 msgctxt "field:sale.sale,number:"
 msgid "Number"
 msgstr "Номер"
 
 #, fuzzy
 msgctxt "field:sale.sale,origin:"
 msgid "Origin"
-msgstr "Източник"
+msgstr "Первоисточник"
 
 msgctxt "field:sale.sale,party:"
 msgid "Party"
-msgstr "Партньор"
+msgstr "Контрагент"
 
 msgctxt "field:sale.sale,party_lang:"
 msgid "Party Language"
-msgstr "Език на партньор"
+msgstr "Язык контрагента"
 
 msgctxt "field:sale.sale,payment_term:"
 msgid "Payment Term"
-msgstr "Условие за плащане"
+msgstr "Правило оплаты"
 
 #, fuzzy
 msgctxt "field:sale.sale,quoted_by:"
 msgid "Quoted By"
 msgstr "Quote"
 
 msgctxt "field:sale.sale,reference:"
 msgid "Reference"
-msgstr "Отпратка"
+msgstr "Ссылка"
 
 msgctxt "field:sale.sale,sale_date:"
 msgid "Sale Date"
-msgstr "Дата на продажба"
+msgstr "Дата продажи"
 
 msgctxt "field:sale.sale,shipment_address:"
 msgid "Shipment Address"
-msgstr "Адрес за доставка"
+msgstr "Адрес доставки"
 
 msgctxt "field:sale.sale,shipment_method:"
 msgid "Shipment Method"
-msgstr "Начин на изпращане"
+msgstr "Метод доставки"
 
 msgctxt "field:sale.sale,shipment_party:"
 msgid "Shipment Party"
 msgstr ""
 
 msgctxt "field:sale.sale,shipment_returns:"
 msgid "Shipment Returns"
-msgstr "Върнати доставки"
+msgstr "Возврат"
 
 msgctxt "field:sale.sale,shipment_state:"
 msgid "Shipment State"
-msgstr "Състояние на пратка"
+msgstr "Состояние доставки"
 
 msgctxt "field:sale.sale,shipments:"
 msgid "Shipments"
-msgstr "Изпращания"
+msgstr "Доставка"
 
 #, fuzzy
 msgctxt "field:sale.sale,shipping_date:"
 msgid "Shipping Date"
-msgstr "Състояние на пратка"
+msgstr "Состояние доставки"
 
 msgctxt "field:sale.sale,state:"
 msgid "State"
-msgstr "Състояние"
+msgstr "Состояние"
 
 msgctxt "field:sale.sale,tax_amount:"
 msgid "Tax"
-msgstr "Данък"
+msgstr "Налог"
 
 msgctxt "field:sale.sale,tax_amount_cache:"
 msgid "Tax Cache"
-msgstr "Данък в брой"
+msgstr "Облагаемые налогом"
 
 msgctxt "field:sale.sale,total_amount:"
 msgid "Total"
-msgstr "Общо"
+msgstr "Итого"
 
 #, fuzzy
 msgctxt "field:sale.sale,total_amount_cache:"
 msgid "Total Cache"
-msgstr "Данък в брой"
+msgstr "Облагаемые налогом"
 
 msgctxt "field:sale.sale,untaxed_amount:"
 msgid "Untaxed"
-msgstr "Необложен с данък"
+msgstr "Без налога"
 
 msgctxt "field:sale.sale,untaxed_amount_cache:"
 msgid "Untaxed Cache"
-msgstr "Наличност преди данъци"
+msgstr "Необлагаемые налогом"
 
 msgctxt "field:sale.sale,warehouse:"
 msgid "Warehouse"
-msgstr "Склад"
+msgstr "Товарный склад"
 
 msgctxt "field:sale.sale-ignored-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Фактура"
+msgstr "Инвойс"
 
 msgctxt "field:sale.sale-ignored-account.invoice,sale:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "field:sale.sale-recreated-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Фактура"
+msgstr "Инвойс"
 
 msgctxt "field:sale.sale-recreated-account.invoice,sale:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "field:stock.move,sale:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "field:stock.move,sale_exception_state:"
 msgid "Exception State"
-msgstr "Състояние на грешка"
+msgstr "Состояние ситуации"
 
 msgctxt "help:party.party,customer_currency:"
 msgid "Default currency for sales to this party."
 msgstr ""
 
 msgctxt "help:party.party,sale_invoice_method:"
 msgid ""
@@ -698,14 +718,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -720,15 +746,15 @@
 "Applied if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:sale.handle.invoice.exception.ask,recreate_invoices:"
 msgid ""
 "The selected invoices will be recreated. The other ones will be ignored."
 msgstr ""
-"Избраните фактури ще бъдат наново създадени. Останалите ще бъдат игнорирани."
+"Выбранные инвойсы будут созданы заново. Остальные будут проигнорированы."
 
 msgctxt "help:sale.sale,shipping_date:"
 msgid "When the shipping of goods should start."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
@@ -780,20 +806,20 @@
 msgctxt "model:ir.action,name:act_reporting_customer_time_series"
 msgid "Sales per Customer"
 msgstr "Sales per Customer"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Sales"
-msgstr "Продажби"
+msgstr "Продажи"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Sales"
-msgstr "Продажби"
+msgstr "Продажи"
 
 msgctxt "model:ir.action,name:act_reporting_product"
 msgid "Sales per Product"
 msgstr "Sales per Product"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_product_category"
@@ -831,36 +857,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Управление на продажби"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Строка продажи"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
-msgstr "Движения"
+msgstr "Перемещения"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Продажи"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Управление на продажби"
+msgstr "Продажи"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
 #, fuzzy
@@ -886,53 +908,82 @@
 msgctxt "model:ir.action,name:wizard_reporting_region_tree_open"
 msgid "Open Region"
 msgstr "Open Region"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_return_sale"
 msgid "Return Sale"
-msgstr "Създаване на меню Продажби"
+msgstr "Создать возврат продажи"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_shipment_handle_exception"
 msgid "Handle Shipment Exception"
 msgstr "Handle Shipment Exception"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_all"
 msgid "All"
 msgstr "All"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_confirmed"
 msgid "Confirmed"
-msgstr "Потвърден"
+msgstr "Confirmed"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_draft"
 msgid "Draft"
-msgstr "Проект"
+msgstr "Draft"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_exception"
 msgid "Exception"
-msgstr "Грешка"
+msgstr "Особая ситуация"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_processing"
 msgid "Processing"
-msgstr "Обработване"
+msgstr "Processing"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
-msgstr "Запитване"
+msgstr "Quotation"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Выполнено"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Выполнено"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
@@ -959,14 +1010,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -992,20 +1049,20 @@
 "To invoice sale \"%(sale)s\" you must define an account revenue for product "
 "\"%(product)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_company"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Организация"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_currency"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Валюта"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_date"
 msgid "Date"
 msgstr "Дата:"
 
 #, fuzzy
@@ -1186,15 +1243,15 @@
 msgctxt "model:party.party.customer_currency,name:"
 msgid "Party Customer Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:party.party.sale_method,name:"
 msgid "Party Sale Method"
-msgstr "Начин на фактурине на продажба"
+msgstr "Метод инвойса продажи"
 
 msgctxt "model:product.configuration.default_lead_time,name:"
 msgid "Product Default Lead Time"
 msgstr ""
 
 msgctxt "model:product.lead_time,name:"
 msgid "Product Lead Time"
@@ -1212,47 +1269,47 @@
 #, fuzzy
 msgctxt "model:res.group,name:group_sale_admin"
 msgid "Sales Administrator"
 msgstr "Sales Administrator"
 
 msgctxt "model:sale.configuration,name:"
 msgid "Sale Configuration"
-msgstr "Конфигурация на продажба"
+msgstr "Конфигурация продаж"
 
 msgctxt "model:sale.configuration.sale_method,name:"
 msgid "Sale Configuration Sale Method"
 msgstr ""
 
 msgctxt "model:sale.configuration.sequence,name:"
 msgid "Sale Configuration Sequence"
 msgstr ""
 
 msgctxt "model:sale.handle.invoice.exception.ask,name:"
 msgid "Handle Invoice Exception"
-msgstr "Обработване за грешка в фактура"
+msgstr "Обработка особых ситуаций инвойса"
 
 msgctxt "model:sale.handle.shipment.exception.ask,name:"
 msgid "Handle Shipment Exception"
-msgstr "Обработване на грешка при пратка"
+msgstr "Обработка особых ситуаций доставки"
 
 msgctxt "model:sale.line,name:"
 msgid "Sale Line"
-msgstr "Ред от продажба"
+msgstr "Строка продажи"
 
 msgctxt "model:sale.line-account.tax,name:"
 msgid "Sale Line - Tax"
-msgstr "Ред от продажба - Данък"
+msgstr "Строка продажи - Налоги"
 
 msgctxt "model:sale.line-ignored-stock.move,name:"
 msgid "Sale Line - Ignored Move"
-msgstr "Ред от продажба - Игнорирано движение"
+msgstr "Строка продажи - Игнорированные перемещения"
 
 msgctxt "model:sale.line-recreated-stock.move,name:"
 msgid "Sale Line - Recreated Move"
-msgstr "Ред от продажба - Нановосъздадено движение"
+msgstr "Строка продажи - Созданные заново перемещения"
 
 msgctxt "model:sale.reporting.context,name:"
 msgid "Sale Reporting Context"
 msgstr ""
 
 msgctxt "model:sale.reporting.country,name:"
 msgid "Sale Reporting per Country"
@@ -1335,113 +1392,118 @@
 msgctxt "model:sale.reporting.region.tree,name:"
 msgid "Sale Reporting per Region"
 msgstr "Sales per Category"
 
 #, fuzzy
 msgctxt "model:sale.return_sale.start,name:"
 msgid "Return Sale"
-msgstr "Създаване на меню Продажби"
+msgstr "Создать возврат продажи"
 
 msgctxt "model:sale.sale,name:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "model:sale.sale-ignored-account.invoice,name:"
 msgid "Sale - Ignored Invoice"
-msgstr "Продажба - Игнорирани фактури"
+msgstr "Продажи - Игнорируемые инвойсы"
 
 msgctxt "model:sale.sale-recreated-account.invoice,name:"
 msgid "Sale - Recreated Invoice"
-msgstr "Продажба - Наново създадена фактура"
+msgstr "Продажи - Созданные заново инвойсы"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:sale.sale:"
 msgid "Amount"
-msgstr "Сума"
+msgstr "Сумма"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Дата:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Адрес для инвойса"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Описание:"
 
 msgctxt "report:sale.sale:"
 msgid "Draft Sale Order"
-msgstr "Проект на поръчка за продажба"
+msgstr "Черновой заказ на продажу"
 
 msgctxt "report:sale.sale:"
 msgid "Quantity"
-msgstr "Количество"
+msgstr "Кол-во"
 
 msgctxt "report:sale.sale:"
 msgid "Quotation N°:"
-msgstr "Запитване N°:"
+msgstr "Котировка N°:"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Reference:"
-msgstr "Отпратка"
+msgstr "Ссылка"
 
 msgctxt "report:sale.sale:"
 msgid "Sale Order N°:"
-msgstr "Поръчка за продажба N°:"
+msgstr "Заказ на продажу №:"
 
 msgctxt "report:sale.sale:"
 msgid "Taxes"
-msgstr "Данъци"
+msgstr "Налоги"
 
 msgctxt "report:sale.sale:"
 msgid "Taxes:"
-msgstr "Данъци:"
+msgstr "Налоги:"
 
 msgctxt "report:sale.sale:"
 msgid "Total (excl. taxes):"
-msgstr "Общо (без данъци):"
+msgstr "Итого (без налогов):"
 
 msgctxt "report:sale.sale:"
 msgid "Total:"
-msgstr "Общо:"
+msgstr "Итого:"
 
 msgctxt "report:sale.sale:"
 msgid "Unit Price"
-msgstr "Единична цена"
+msgstr "Цена за единицу"
 
 msgctxt "selection:account.invoice,sale_exception_state:"
 msgid "Ignored"
-msgstr "Игнорирано"
+msgstr "Игнорируется"
 
 msgctxt "selection:account.invoice,sale_exception_state:"
 msgid "Recreated"
-msgstr "Създаден наново"
+msgstr "Создано заново"
 
 msgctxt "selection:sale.line,type:"
 msgid "Comment"
-msgstr "Коментар"
+msgstr "Комментарии"
 
 msgctxt "selection:sale.line,type:"
 msgid "Line"
-msgstr "Ред"
+msgstr "Строка"
 
 msgctxt "selection:sale.line,type:"
 msgid "Subtotal"
-msgstr "Междинна сума"
+msgstr "Подитог"
 
 msgctxt "selection:sale.line,type:"
 msgid "Title"
-msgstr "Заглавие"
+msgstr "Заголовок"
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Month"
@@ -1449,131 +1511,143 @@
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "Manual"
-msgstr "Ръчно"
+msgstr "Ручной"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Order Processed"
-msgstr "При обработена поръчка"
+msgstr "При обработке заказа"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
-msgstr "При изпращане на пратка"
+msgstr "При отправке груза"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
-msgstr "Грешка"
+msgstr "Особая ситуация"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
-msgstr "Няма"
+msgstr "Отсутствует"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
-msgstr "Платен"
+msgstr "Оплачен"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Изчакващ"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
-msgstr "Ръчно"
+msgstr "Ручной"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
-msgstr "При плащане на фактура"
+msgstr "При оплате инвойса"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Order Processed"
-msgstr "При обработена поръчка"
+msgstr "При обработке заказа"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Exception"
-msgstr "Грешка"
+msgstr "Особая ситуация"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
-msgstr "Няма"
+msgstr "Отсутствует"
+
+msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
-msgstr "Изпратен"
+msgstr "Отправлен"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
-msgstr "Изчакващ"
+msgstr "Ожидание"
 
 #, fuzzy
 msgctxt "selection:sale.sale,state:"
 msgid "Cancelled"
-msgstr "Отказан"
+msgstr "Отменено"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Confirmed"
-msgstr "Потвърден"
+msgstr "Подтвержденно"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Done"
-msgstr "Приключен"
+msgstr "Выполнено"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Draft"
-msgstr "Проект"
+msgstr "Черновик"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Processing"
-msgstr "Обработване"
+msgstr "Обработка"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Quotation"
-msgstr "Запитване"
+msgstr "Котировка"
 
 msgctxt "selection:stock.move,sale_exception_state:"
 msgid "Ignored"
-msgstr "Игнорирано"
+msgstr "Игнорируется"
 
 msgctxt "selection:stock.move,sale_exception_state:"
 msgid "Recreated"
-msgstr "Създаден наново"
+msgstr "Создано заново"
 
 #, fuzzy
 msgctxt "view:party.party:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "view:product.template:"
 msgid "Customers"
-msgstr "Клиенти"
+msgstr "Заказчики"
 
 #, fuzzy
 msgctxt "view:sale.handle.invoice.exception.ask:"
 msgid "Choose invoices to recreate:"
-msgstr "Избор на фактури за ново създаване"
+msgstr "Выберите инвойсы для пересоздания"
 
 #, fuzzy
 msgctxt "view:sale.handle.shipment.exception.ask:"
 msgid "Choose move to recreate:"
-msgstr "Избор на движение за ново създаване"
+msgstr "Выберите проводки для пересоздания"
 
 msgctxt "view:sale.line:"
 msgid "General"
-msgstr "Основен"
+msgstr "Основной"
 
 msgctxt "view:sale.line:"
 msgid "Notes"
-msgstr "Бележки"
+msgstr "Комментарии"
 
 msgctxt "view:sale.line:"
 msgid "Taxes"
-msgstr "Данъци"
+msgstr "Налоги"
 
 #, fuzzy
 msgctxt "view:sale.reporting.country.subdivision.time_series:"
 msgid "Number"
 msgstr "Номер"
 
 msgctxt "view:sale.reporting.country.subdivision.time_series:"
@@ -1645,47 +1719,47 @@
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Other Info"
-msgstr "Друга информация"
+msgstr "Другая информация"
 
 msgctxt "view:sale.sale:"
 msgid "Sale"
-msgstr "Продажба"
+msgstr "Продажа"
 
 msgctxt "wizard_button:sale.handle.invoice.exception,ask,end:"
 msgid "Cancel"
-msgstr "Отказ"
+msgstr "Отменить"
 
 msgctxt "wizard_button:sale.handle.invoice.exception,ask,handle:"
 msgid "OK"
-msgstr "Добре"
+msgstr "Ок"
 
 msgctxt "wizard_button:sale.handle.shipment.exception,ask,end:"
 msgid "Cancel"
-msgstr "Отказ"
+msgstr "Отменить"
 
 msgctxt "wizard_button:sale.handle.shipment.exception,ask,handle:"
 msgid "OK"
-msgstr "Добре"
+msgstr "Ок"
 
 #, fuzzy
 msgctxt "wizard_button:sale.modify_header,start,end:"
 msgid "Cancel"
-msgstr "Отказ"
+msgstr "Отменить"
 
 msgctxt "wizard_button:sale.modify_header,start,modify:"
 msgid "Modify"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:sale.return_sale,start,end:"
 msgid "Cancel"
-msgstr "Отказване"
+msgstr "Отменить"
 
 #, fuzzy
 msgctxt "wizard_button:sale.return_sale,start,return_:"
 msgid "Return"
-msgstr "Връщане"
+msgstr "Возвраты"
```

### Comparing `trytond_sale-6.6.2/locale/ca.po` & `trytond_sale-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr "Plantilla"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Temps d'espera"
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Temps d'espera"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Vendible"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Preu de venda"
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr "Data final existències"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Temps d'espera"
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Temps d'espera"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Vendible"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "UdM de venda"
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Client"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Moviments finalitzats"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Moviments en excepció"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Moviments en excepció"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Moviments ignorats"
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progres dels moviments"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Moviments recreats"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr "Quantitat"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Venda"
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Data venda"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Estat de la venda"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Data d'enviament"
@@ -654,14 +670,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "El temps desde la confirmació de la venda fins que s'envien els productes.\n"
 "Utilitzats als productes sense temps d'espera."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"El temps desde la confirmació de la venda fins que s'envien els productes.\n"
+"Utilitzats als productes sense temps d'espera."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "El temps desde que es confirma la comanda fins que s'envien els productes.\n"
 "Si es deixa en blanc s'utilitza el temps d'enviament per defecte de la configuració."
@@ -776,31 +800,27 @@
 msgid "Configuration"
 msgstr "Configuració"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Vendes"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Vendes"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Vendes"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Línies de venda"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Moviments"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Vendes"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Vendes"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Albarans"
 
@@ -856,14 +876,38 @@
 msgstr "En procés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pressupost"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Finalitzada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr "Pendent"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Finalitzada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr "Pendent"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "No podeu eliminar el tercer \"%(party)s\" mentre tingui vendes pendents amb "
 "l'empresa \"%(company)s\"."
@@ -900,14 +944,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "No podeu restablir la factura \"%(invoice)s\" a esborrany perquè es va "
 "generar des d'una venda."
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"No podeu afegir línies a la venda \"%(sale)s\" perquè no està en estat "
+"esborrany."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Per eliminar la línia \"%(line)s\" heu de cancel·lar o restablir a esborrany"
 " la venda \"%(sale)s\"."
@@ -1291,14 +1343,18 @@
 msgstr "Import"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Adreça d'enviament:"
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Descripció:"
 
@@ -1387,28 +1443,36 @@
 msgstr "Al processar la comanda"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Al enviar-ho"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "En espera de pagament"
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Excepció"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Cap"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Pagada"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "En espera"
+msgid "Partially Paid"
+msgstr "Pagada parcialment"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr "Pendent"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1423,14 +1487,18 @@
 msgstr "Excepció"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Cap"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Enviada parcialment"
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Enviada"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "En espera"
```

### Comparing `trytond_sale-6.6.2/locale/cs.po` & `trytond_sale-6.8.0/locale/cs.po`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -123,14 +127,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -195,42 +203,48 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Sales per Customer"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr ""
@@ -248,14 +262,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Sales"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Sales"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -677,14 +696,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -804,31 +829,30 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
@@ -888,14 +912,40 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -921,14 +971,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1321,14 +1377,18 @@
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr ""
 
@@ -1417,27 +1477,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1453,14 +1521,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/de.po` & `trytond_sale-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr "Artikelvorlage"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Beschaffungszeit"
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Beschaffungszeiten"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Verkäuflich"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Verkaufspreis"
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr "Lager Enddatum"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Beschaffungszeit"
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Beschaffungszeiten"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Verkäuflich"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Maßeinheit Verkauf"
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Währung"
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Kunde"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Erledigte Warenbewegungen"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Warenbewegungen mit Vorbehalt"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Warenbewegungen mit Vorbehalt"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignorierte Warenbewegungen"
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Lieferfortschritt"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Neu erstellte Warenbewegungen"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Notiz"
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr "Menge"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Verkauf"
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Verkaufsdatum"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Verkaufsstatus"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Lieferdatum"
@@ -654,14 +670,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "Die Zeit zwischen der Auftragsbestätigung und dem Versand der Ware.\n"
 "Wird für Artikel genutzt für die keine Beschaffungszeit erfasst wurde."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"Die Zeit zwischen der Auftragsbestätigung und dem Versand der Ware.\n"
+"Wird für Artikel genutzt für die keine Beschaffungszeit erfasst wurde."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Die Zeit zwischen der Auftragsbestätigung und dem Versand der Ware.\n"
 "Wenn leer wird die Standardbeschaffungszeit aus den Einstellungen benutzt."
@@ -777,31 +801,27 @@
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Verkauf"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Verkauf"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Verkauf"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Verkaufspositionen"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Verkäufe"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Verkäufe"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Lieferungen"
 
@@ -857,14 +877,38 @@
 msgstr "In Ausführung"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Angebot"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Erledigt"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr "Ausstehend"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Erledigt"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr "Ausstehend"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "Die Partei \"%(party)s\" kann nicht gelöscht werden, solange es für sie "
 "unerledigte Verkäufe bei Unternehmen \"%(company)s\" gibt."
@@ -903,14 +947,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "Die Rechnung \"%(invoice)s\" kann nicht auf den Entwurfsstatus zurückgesetzt"
 " werden, weil sie automatisch aus einem Verkauf erstellt wurde."
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"Zu Verkauf \"%(sale)s\" können keine Positionen hinzugefügt werden, da der "
+"er nicht mehr im Entwurfsstatus ist."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Damit die Verkaufsposition \"%(line)s\" gelöscht werden kann, muss zuerst "
 "der Verkauf \"%(sale)s\" annulliert oder auf den Entwurfsstatus "
@@ -1296,14 +1348,18 @@
 msgstr "Betrag"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Datum:"
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Lieferadresse:"
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Beschreibung:"
 
@@ -1392,28 +1448,36 @@
 msgstr "Bei Auftragsausführung"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Bei Lieferung"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "Zahlung Ausstehend"
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Vorbehalt"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Kein"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Bezahlt"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Wartend"
+msgid "Partially Paid"
+msgstr "Teilweise Bezahlt"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr "Ausstehend"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manuell"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1428,14 +1492,18 @@
 msgstr "Vorbehalt"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Kein"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Teilweise Versendet"
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Gesendet"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "Wartend"
```

### Comparing `trytond_sale-6.6.2/locale/es.po` & `trytond_sale-6.8.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr "Plantilla"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Tiempo de espera"
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Tiempos de espera"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Vendible"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Precio de venta"
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr "Fecha final existencias"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Tiempo de espera"
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Tiempos de espera"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Vendible"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "UdM de venta"
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Cliente"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Movimientos finalizados"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Movimientos en excepción"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Movimientos en excepción"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimientos ignorados"
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progreso de los movimientos"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Movimientos recreados"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr "Cantidad"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Venta"
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Fecha venta"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Estado de venta"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Fecha envío"
@@ -654,14 +670,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "El tiempo desde que se ha confirmado la de venta hasta que se envian los productos.\n"
 "Usado en los productos sin tiempo de espera."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"El tiempo desde que se ha confirmado la de venta hasta que se envían los productos.\n"
+"Usado en los productos sin tiempo de espera."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "El tiempo desde que se confirma el pedido hasta que se envian los productos.\n"
 "Si se deja en blaco s'utlitza el tiempo de envío por defecto de la configuración."
@@ -776,31 +800,27 @@
 msgid "Configuration"
 msgstr "Configuración"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Ventas"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Ventas"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Ventas"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Líneas de venta"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Movimientos"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Ventas"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Ventas"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Albaranes"
 
@@ -856,14 +876,38 @@
 msgstr "En proceso"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Presupuesto"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Finalizada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr "Pendiente"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Finalizada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr "Pendiente"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "No puede eliminar el tercero \"%(party)s\" mientras tenga ventas pendientes "
 "en la empresa \"%(company)s\"."
@@ -899,14 +943,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "No puede establecer la factura \"%(invoice)s\" como borrador porque fue "
 "generada desde una venta."
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"No podéis añadir lineas a la venta \"%(sale)s\" porqué no esta en estado "
+"borrador."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Para eliminar la línea \"%(line)s\" debe cancelar o establecer como borrador"
 " la venta \"%(sale)s\"."
@@ -1290,14 +1342,18 @@
 msgstr "Importe"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Fecha:"
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Dirección de envío:"
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Descripción:"
 
@@ -1386,28 +1442,36 @@
 msgstr "Al procesar el pedido"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Al enviar"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "A la espera de pago"
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Excepción"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Ninguno"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Pagada"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "En espera"
+msgid "Partially Paid"
+msgstr "Pagada parcialmente"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr "Pendiente"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1422,14 +1486,18 @@
 msgstr "Excepción"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Ninguno"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Enviada parcialmente"
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Enviada"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "En espera"
```

### Comparing `trytond_sale-6.6.2/locale/es_419.po` & `trytond_sale-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -117,14 +121,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -189,42 +197,47 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr ""
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Estado excepción"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr ""
@@ -241,14 +254,18 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr ""
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr ""
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -655,14 +672,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -770,31 +793,27 @@
 msgid "Configuration"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr ""
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Envíos"
@@ -854,14 +873,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Cotización"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -887,14 +930,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1265,14 +1314,18 @@
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr ""
 
@@ -1361,27 +1414,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1397,14 +1458,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/et.po` & `trytond_sale-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Täitmise aeg"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Täitmise aeg"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Müüdav"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Müügihind"
@@ -134,14 +139,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Täitmise aeg"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Täitmise aeg"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Müüdav"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Müügiühik"
@@ -209,42 +219,49 @@
 msgstr "Ettevõte"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Valuuta"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Klient"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Kirjeldus"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Asukohast"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Arve read"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Kanded tehtud"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Kannete erand"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Kanded"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Kannete erand"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignoreeritud kanded"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Kanded tehtud"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Taasloodud kanded"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Märkus"
@@ -261,14 +278,19 @@
 msgid "Quantity"
 msgstr "Kogus"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Müük"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Müügi kuupäev"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Müügi staatus"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Tarne kuupäev"
@@ -698,14 +720,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -825,34 +853,33 @@
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Müügid"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Müügid"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Müügid"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Müügi rida"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Kanded"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Müügid"
+msgstr "Müük"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Müügid"
+msgstr "Müük"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Lähetused"
 
 msgctxt "model:ir.action,name:report_sale"
 msgid "Sale"
@@ -909,14 +936,42 @@
 msgstr "Töötluses"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pakkumus"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Kõik"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Tehtud"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Kõik"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Tehtud"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "Osapoolt \"%(osapooli)\" ei saa kustutada, kuniks neil on ettevõttega "
 "\"%(ettevõtetega)\" avatud müügid."
@@ -944,14 +999,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1358,14 +1419,19 @@
 msgid "Amount"
 msgstr "Summa"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Kuupäev:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Arve aadress"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Kirjeldus"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Kirjeldus:"
@@ -1455,28 +1521,36 @@
 msgstr "Protsessitakse tellimusel"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Tarnel saadetud"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Erand"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Mitte"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Makstud"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Ootel"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Käsitsi"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1491,14 +1565,18 @@
 msgstr "Erand"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Mitte"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Saadetud"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "Ootel"
```

### Comparing `trytond_sale-6.6.2/locale/fa.po` & `trytond_sale-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "زمان پیشبرد"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "زمان پیشبرد"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "قابل فروش"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "قیمت فروش"
@@ -134,14 +139,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "زمان پیشبرد"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "زمان پیشبرد"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "قابل فروش"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "واحد اندازی گیری فروش"
@@ -209,42 +219,49 @@
 msgstr "شرکت"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "مشتری"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "شرح"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "از مکان"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "خطوط صورتحساب"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "جابجایی ها انجام شد"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "جابجایی های اعتراضی"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "جابجایی ها"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "جابجایی های اعتراضی"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "جابجایی های نادیده گرفته شده"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "جابجایی ها انجام شد"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "جابجایی های دوباره انجام شده"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "توجه"
@@ -261,14 +278,19 @@
 msgid "Quantity"
 msgstr "مقدار/تعداد"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "فروش"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "تاریخ فروش"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "وضعیت فروش"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "تاریخ ارسال"
@@ -698,14 +720,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -828,32 +856,31 @@
 msgid "Configuration"
 msgstr "پیکربندی"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "فروش ها"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "فروش ها"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "فروش ها"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "سطر فروش"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "جابجایی ها"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "فروش ها"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "فروش ها"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "محموله ها"
 
@@ -912,14 +939,42 @@
 msgstr "در حال پردازش"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "نقل قول"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "همه"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "انجام شد"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "همه"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "انجام شد"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "شما نمیتوانید نهاد/سازمان: \"%(party)s\"را هنگامی که فروش هایی معوق با شرکت:"
 " \"%(company)s\"دارد را حذف کنید."
@@ -955,14 +1010,21 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "شما نمیتوانید صورتحساب :\"%(invoice)s\"را به حالت پیش نویس بازنشانی کنید "
 "چراکه توسط یک فروش ایجاد شده است."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr "برای تغیر عنوان فروش :\"%(sale)s\" حالت آن باید به پیش نویس بازنشانی شود."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "برای حذف سطر:\"%(line)s\" شما باید فروش :\"%(sale)s\"را لغو یا به حالت پیش "
 "نویس بازنشانی کنید."
@@ -1369,14 +1431,19 @@
 msgid "Amount"
 msgstr "مقدار"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "تاریخ :"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "آدرس صورتحساب"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "شرح"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "توضیحات :"
@@ -1466,28 +1533,36 @@
 msgstr "در دستور پردازش شده"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "در ارسال حمل و نقل"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "اعتراض"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "هیجکدام"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "پرداخت شده"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "در انتظار"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "دستی"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1502,14 +1577,18 @@
 msgstr "اعتراض"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "هیجکدام"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "ارسال"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "در انتظار"
```

### Comparing `trytond_sale-6.6.2/locale/fi.po` & `trytond_sale-6.8.0/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -123,14 +127,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -195,42 +203,48 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Sales per Customer"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr ""
@@ -248,14 +262,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Sales"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Sales"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -674,14 +693,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -801,31 +826,30 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
@@ -885,14 +909,40 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -918,14 +968,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1318,14 +1374,18 @@
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr ""
 
@@ -1414,27 +1474,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1450,14 +1518,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/fr.po` & `trytond_sale-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr "Modèle"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Délai d'exécution"
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Délais d'exécution"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Vendable"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Prix de vente"
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr "Date de fin de stock"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Délai d'exécution"
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Délais d'exécution"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Vendable"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "UDM de vente"
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Devise"
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Client"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Description"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Emplacement d'origine"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Lignes de facture"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Mouvements effectués"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Mouvements en exception"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mouvements en exception"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mouvements ignorés"
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progression des mouvements"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mouvements recréés"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Note"
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr "Quantité"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Vente"
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Date de la vente"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "État de la vente"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Date de livraison"
@@ -654,14 +670,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "Le délai entre la confirmation de la vente et l'envoi des produits.\n"
 "Utilisé pour les produits sans délai d'éxécution."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"Le délai entre la confirmation de la vente et l'envoi des produits.\n"
+"Utilisé pour les produits sans délai d’exécution."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Le délai entre la confirmation de la vente et l'envoi des produits.\n"
 "Si vide, le délai d'éxécution par défaut de la configuration est utilisé."
@@ -776,31 +800,27 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Ventes"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Ventes"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Ventes"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Lignes de vente"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Mouvements"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Ventes"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Ventes"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Expéditions"
 
@@ -856,14 +876,38 @@
 msgstr "En traitement"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Devis"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Toutes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Terminées"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr "En attentes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Toutes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Terminées"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr "En attentes"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "Vous ne pouvez pas effacer le tiers « %(party)s » tant qu'il a des ventes en"
 " attentes pour la société « %(company)s »."
@@ -900,14 +944,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "Vous ne pouvez pas réinitialiser à l'état brouillon la facture "
 "« %(invoice)s » car elle a été générée par une vente."
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"Vous ne pouvez pas ajouter de lignes à la vente « %(sale)s » car elle n'est "
+"plus dans l'état brouillon."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Pour supprimer la ligne « %(line)s », vous devez annuler ou réinitialiser à "
 "l'état brouillon la vente « %(sale)s »."
@@ -1291,14 +1343,18 @@
 msgstr "Montant"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Date :"
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Adresse de livraison :"
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Description"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Description :"
 
@@ -1387,27 +1443,35 @@
 msgstr "Sur traitement de l'ordre"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "À l'envoi de l'expédition"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "En attente de paiement"
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Exception"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Aucun"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Payée"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr "Partiellement payée"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr "En attente"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manuel"
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1423,14 +1487,18 @@
 msgstr "Exception"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Aucun"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Partiellement expédié"
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Envoyé"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "En attente"
```

### Comparing `trytond_sale-6.6.2/locale/hu.po` & `trytond_sale-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Átfutási idő"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Átfutási idő"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Eladható"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Listaár"
@@ -126,14 +131,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Átfutási idő"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Átfutási idő"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Eladható"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Értékesítési ME"
@@ -199,42 +209,48 @@
 msgid "Company"
 msgstr "Cég"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Pénznem"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Vevő"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Leírás"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Induló tárhely"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Számlasorok"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mozgások"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "visszautasítva"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Jegyzetek"
@@ -251,14 +267,19 @@
 msgid "Quantity"
 msgstr "Mennyiség"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Vevői rendelés"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Rendelés dátuma"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Kiszállítás dátuma"
@@ -692,14 +713,23 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "Az átfutási idő a vevői rendelés jóváhagyásától az áru kiszállításáig.\n"
 "Azoknál a termékeknél használja a rendszer, amiknél nincs egyéni átfutási idő megadva."
 
+#, fuzzy
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"Az átfutási idő a vevői rendelés jóváhagyásától az áru kiszállításáig.\n"
+"Azoknál a termékeknél használja a rendszer, amiknél nincs egyéni átfutási idő megadva."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Az átfutási idő a vevői rendelés jóváhagyásától az áru kiszállításáig.\n"
 "Ha üres, a termékbeállításoknál megadott átfutási időt használja a rendszer."
@@ -823,31 +853,30 @@
 msgid "Configuration"
 msgstr "Beállítások"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Vevői rendelések"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Vevői rendelések"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Vevői rendelések"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Vevői rendelés sora"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Készletmozgások"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Vevői rendelések"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Vevői rendelések"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Szállítmányok"
 
@@ -905,14 +934,42 @@
 msgstr "folyamatban"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "ajánlat"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "összes"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Kész"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "összes"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Kész"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -938,14 +995,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1328,14 +1391,19 @@
 msgid "Amount"
 msgstr "Összeg"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Dátum:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Számlázási cím"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Leírás"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Description:"
@@ -1426,28 +1494,36 @@
 msgstr "a rendelés alapján"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "a vevői szállítmány alapján"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "visszautasítva"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "nincs"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Fizetve"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "várakozik"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "kézzel"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1462,14 +1538,18 @@
 msgstr "visszautasítva"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "nincs"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "várakozik"
```

### Comparing `trytond_sale-6.6.2/locale/id.po` & `trytond_sale-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -126,14 +130,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -200,42 +208,49 @@
 msgstr "Perusahaan"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Mata uang"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Pelanggan"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Deskripsi"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Baris Faktur"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Perpindahan Selesai"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Perpindahan"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Perpindahan Selesai"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Perpindahan Selesai"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Catatan"
@@ -252,14 +267,19 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Penjualan"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Tanggal Penjualan"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -678,14 +698,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -804,34 +830,33 @@
 msgid "Configuration"
 msgstr "Konfigurasi"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr ""
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr ""
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Baris Penjualan"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Perpindahan"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr ""
+msgstr "Penjualan"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr ""
+msgstr "Penjualan"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_sale"
 msgid "Sale"
@@ -887,14 +912,38 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -920,14 +969,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1324,14 +1379,19 @@
 msgid "Amount"
 msgstr "Jumlah"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Tanggal:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Alamat Faktur"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Deskripsi"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Deskripsi:"
@@ -1421,27 +1481,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Tidak ada"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1457,14 +1525,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Tidak ada"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/it.po` & `trytond_sale-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Tempi di consegna"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Tempi di consegna"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "vendibile"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -131,14 +136,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Tempi di consegna"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Tempi di consegna"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "vendibile"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "UdM di vendita"
@@ -208,42 +218,49 @@
 msgstr "Azienda"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Clienti"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Descrizione"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "da locazione"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Righe fattura"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "movimenti eseguiti"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "eccezione movimenti"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "eccezione movimenti"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "movimenti ignorati"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "movimenti eseguiti"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "movimenti ricreati"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -260,14 +277,19 @@
 msgid "Quantity"
 msgstr "Quantità"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Vendite"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "data ordine"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "stato ordine"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "data di spedizione"
@@ -694,14 +716,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -825,36 +853,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "riga ordine"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Movimenti"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vendite"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vendite"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Spedizioni"
 
 #, fuzzy
 msgctxt "model:ir.action,name:report_sale"
@@ -920,14 +944,42 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Eseguito"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Eseguito"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -953,14 +1005,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1354,14 +1412,19 @@
 msgid "Amount"
 msgstr "Importo"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Indirizzo di fatturazione"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descrizione"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Descrizione:"
@@ -1452,28 +1515,36 @@
 msgstr "Su ordine processato"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Su spedizione"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Eccezione"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Nessuno"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Pagato"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "In attesa"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manuale"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1488,14 +1559,18 @@
 msgstr "Eccezione"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Nessuno"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Inviato"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "In attesa"
```

### Comparing `trytond_sale-6.6.2/locale/lo.po` & `trytond_sale-6.8.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -130,14 +134,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -208,44 +216,50 @@
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Sales per Customer"
+
+#, fuzzy
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "ເນື້ອໃນລາຍການ"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "ລາຍການເກັບເງິນ"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 #, fuzzy
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "ສະຖານະຍົກເວັ້ນ"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,note:"
 msgid "Note"
@@ -266,14 +280,19 @@
 msgstr "ຈຳນວນ"
 
 #, fuzzy
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "ຂາຍ"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "ວັນທີບັນທຶກ"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -726,14 +745,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -856,34 +881,30 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "ຂາຍ"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "ຂາຍ"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "ຂາຍ"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "ຮ່ວງ"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "ຂາຍ"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "ຂາຍ"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
@@ -947,14 +968,42 @@
 msgstr "ກຳລັງດຳເນີນການ"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "ທັງໝົດ"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "ແລ້ວໆ"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "ທັງໝົດ"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "ແລ້ວໆ"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -980,14 +1029,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1389,14 +1444,19 @@
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "ວັນທີ:"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "ທີ່ຢູ່"
+
+#, fuzzy
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "ເນື້ອໃນລາຍການ"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "ເນື້ອໃນລາຍການ"
@@ -1498,29 +1558,37 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "ບໍ່ມີ"
 
 #, fuzzy
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "ຈ່າຍແລ້ວ"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "ໃສ່ເອົາເອງ"
 
@@ -1538,14 +1606,18 @@
 
 #, fuzzy
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "ບໍ່ມີ"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/lt.po` & `trytond_sale-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Tiekimo laikas"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Tiekimo laikas"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Parduodama"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Pardavimo kaina"
@@ -134,14 +139,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Tiekimo laikas"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Tiekimo laikas"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Parduodama"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Mato vienetas parduodant"
@@ -209,42 +219,49 @@
 msgstr "Organizacija"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Pirkėjas"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Aprašymas"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Išsiuntimo vieta"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Atliktos operacijos"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Operacijų išimtys"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Operacijos"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Operacijų išimtys"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignoruotos operacijos"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Atliktos operacijos"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Atkurtos operacijos"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Pastaba"
@@ -261,14 +278,19 @@
 msgid "Quantity"
 msgstr "Kiekis"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Pardavimas"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Pardavimo data"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Pardavimo būsena"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Išsiuntimo data"
@@ -698,14 +720,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -826,32 +854,31 @@
 msgid "Configuration"
 msgstr "Nuostatos"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Pardavimai"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Pardavimai"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Pardavimai"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Pardavimo eilutė"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Operacijos"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Pardavimai"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Pardavimai"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Siuntimai"
 
@@ -910,14 +937,42 @@
 msgstr "Vykdomi"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Pasiūlymai"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Visi"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Pabaigta"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Visi"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Pabaigta"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -943,14 +998,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1357,14 +1418,19 @@
 msgid "Amount"
 msgstr "Suma"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Juridinis adresas"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Aprašymas"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Aprašymas:"
@@ -1454,28 +1520,36 @@
 msgstr "Vykdant užsakymą"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Išsiunčiant krovinį"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Išimtis"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Jokia"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Apmokėta"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Laukianti apmokėjimo"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Rankiniu būdu"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1490,14 +1564,18 @@
 msgstr "Išimtis"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Jokia"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Išsiųsta"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "Laukiantis"
```

### Comparing `trytond_sale-6.6.2/locale/nl.po` & `trytond_sale-6.8.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr "Template"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Doorlooptijd"
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Doorlooptijden"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Verkoopbaar"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Verkoopprijs"
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr "Eind datum voorraad"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Doorlooptijd"
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Doorlooptijden"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Verkoopbaar"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Verkoop maateeheid"
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Klant"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Omschrijving"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuur regels"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Mutaties gereed"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Mutaties uitzondering"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mutaties"
 
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mutaties Uitzondering"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Genegeerde mutaties"
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Mutaties Voortgang"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Opnieuw aangemaakte mutaties"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Notitie"
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr "Hoeveelheid"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Verkoop"
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Verkoop datum"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Verkoop status"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Verzend datum"
@@ -654,14 +670,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "De tijd tussen de bevestiging van de verkooporder en het verzenden van de producten.\n"
 "Gebruikt voor producten zonder doorlooptijd."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"De tijd vanaf de bevestiging van de verkooporder tot het verzenden van de producten.\n"
+"Wordt gebruikt voor producten zonder doorlooptijd."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "De tijd tussen de bevestiging van de verkooporder en het verzenden van de producten.\n"
 "Indien leeg wordt de standaard doorlooptijd uit de configuratie gebruikt."
@@ -777,33 +801,29 @@
 msgid "Configuration"
 msgstr "Instellingen"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Verkoop"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Verkoop"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Verkoop"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Verkoop regels"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Mutaties"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Verkoop"
+msgstr "Verkopen"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Verkoop"
+msgstr "Verkopen"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Leveringen"
 
 msgctxt "model:ir.action,name:report_sale"
 msgid "Sale"
@@ -857,14 +877,38 @@
 msgstr "Verwerking"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Offerte"
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Afgerond"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr "In behandeling"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Afgerond"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr "In behandeling"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "U kunt de relatie \"% (party) s\" niet verwijderen terwijl ze facturen in "
 "behandeling hebben bij bedrijf \"%(company)s\"."
@@ -900,14 +944,22 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "U kunt de factuur \"%(invoice)s\" niet terug zetten naar concept omdat ze is"
 " gegenereerd door een verkoop."
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"U kunt geen regels toevoegen aan verkoop \"%(sale)s\" omdat deze niet langer"
+" status \"concept\" staat."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Om regel \"%(line)s\" te verwijderen, moet u de verkoop \"%(sale)s\" "
 "annuleren of terug zetten naar concept."
@@ -988,15 +1040,15 @@
 msgid "To get a quote for sale \"%(sale)s\" you must enter a warehouse."
 msgstr ""
 "Om een offerte voor verkoop \"%(sale)s\" te krijgen, moet u een magazijn "
 "invoeren."
 
 msgctxt "model:ir.model.button,string:sale_cancel_button"
 msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Annuleer"
 
 msgctxt "model:ir.model.button,string:sale_confirm_button"
 msgid "Confirm"
 msgstr "Bevestigen"
 
 msgctxt "model:ir.model.button,string:sale_draft_button"
 msgid "Draft"
@@ -1292,14 +1344,18 @@
 msgstr "Bedrag"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Datum:"
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Aflever Adres:"
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Omschrijving"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Omschrijving:"
 
@@ -1388,28 +1444,36 @@
 msgstr "Na verwerking order"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Na verzending"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr "In afwachting van betaling"
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Uitzondering"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Geen"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Betaald"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "In afwachting"
+msgid "Partially Paid"
+msgstr "Gedeeltelijk betaald"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr "In behandeling"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Handmatig"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1424,14 +1488,18 @@
 msgstr "Uitzondering"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Geen"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr "Gedeeltelijk Verzonden"
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Verzonden"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "In afwachting"
```

### Comparing `trytond_sale-6.6.2/locale/pl.po` & `trytond_sale-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Cena sprzedaży"
@@ -131,14 +135,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Jm sprzedaży"
@@ -206,42 +214,49 @@
 msgstr "Firma"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Waluta"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Odbiorcy"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Z lokalizacji"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Wiersze faktury"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Wykonane ruchy"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Ruchy"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Wyjątek"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Zignorowane ruchy"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Wykonane ruchy"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Notatka"
@@ -258,14 +273,19 @@
 msgid "Quantity"
 msgstr "Ilość"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Sprzedaż"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Data sprzedaży"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Stan sprzedaży"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Data wysyłki"
@@ -687,14 +707,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -818,36 +844,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Wiersz sprzedaży"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Ruchy"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Sprzedaż"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Sprzedaż"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
 #, fuzzy
@@ -912,14 +934,42 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Wykonano"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Wykonano"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -945,14 +995,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1346,14 +1402,19 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Adres faktury"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Opis:"
@@ -1443,27 +1504,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Wyjątek"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Brak"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1479,14 +1548,18 @@
 msgstr "Wyjątek"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Brak"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Wysłano"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/pt.po` & `trytond_sale-6.8.0/locale/pt.po`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Tempo de Espera"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Tempo de Espera"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Vendável"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Preço de Venda"
@@ -134,14 +139,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Tempo de Espera"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Tempo de Espera"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Vendável"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "UM para venda"
@@ -209,42 +219,49 @@
 msgstr "Empresa"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Moeda"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Clientes"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Descrição"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Origem"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Linhas da fatura"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Movimentações feitas"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Exceção nas movimentações"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimentações"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Exceção nas movimentações"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimentações ignoradas"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Movimentações feitas"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Recriar movimentações"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Observação"
@@ -261,14 +278,19 @@
 msgid "Quantity"
 msgstr "Quantidade"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Venda"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Data da venda"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Estado da Venda"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Data da Remessa"
@@ -693,14 +715,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -826,36 +854,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Linha da fatura"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Movimentações"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vendas"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vendas"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
 #, fuzzy
@@ -922,14 +946,42 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Feito"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Feito"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -955,14 +1007,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1357,14 +1415,19 @@
 msgid "Amount"
 msgstr "Quantidade"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Endereço para faturamento"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descrição"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Descrição:"
@@ -1454,28 +1517,36 @@
 msgstr "Ao Processar a Ordem"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "No Envio da Remessa"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Exceção"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Nenhum"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Pago"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Espera"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1490,14 +1561,18 @@
 msgstr "Exceção"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Nenhum"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Emitido"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "Espera"
```

### Comparing `trytond_sale-6.6.2/locale/ro.po` & `trytond_sale-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 msgid "Exception State"
 msgstr "Stare de excepție"
 
 msgctxt "field:account.invoice,sales:"
 msgid "Sales"
 msgstr "Vânzări"
 
-#, fuzzy
 msgctxt "field:party.party,customer_currencies:"
 msgid "Customer Currencies"
-msgstr "Clienți"
+msgstr "Valute Clienți"
 
 #, fuzzy
 msgctxt "field:party.party,customer_currency:"
 msgid "Customer Currency"
 msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:party.party,sale_invoice_method:"
 msgid "Invoice Method"
 msgstr "Metoda de facturare"
 
 msgctxt "field:party.party,sale_methods:"
 msgid "Sale Methods"
 msgstr "Metode de Vânzare"
@@ -70,20 +68,25 @@
 #, fuzzy
 msgctxt "field:product.lead_time,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
 msgctxt "field:product.lead_time,template:"
 msgid "Template"
-msgstr ""
+msgstr "Șablon"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Timp de livrare"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Marfă"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Preț de vânzare"
@@ -120,14 +123,19 @@
 msgid "Stock End Date"
 msgstr "Data încheiere Stoc"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Timp de livrare"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Marfă"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Vânzare UM"
@@ -190,44 +198,50 @@
 
 msgctxt "field:sale.line,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
+
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Client"
 
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Din locație"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rând factură"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Mișcari Finalizate"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Excepție de Miscare"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mișcări"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Excepție de Miscare"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mișcări ignorate"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Mișcari Finalizate"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mișcări recreate"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Nota"
@@ -244,14 +258,19 @@
 msgid "Quantity"
 msgstr "Cantitate"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Vânzare"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Data vânzării"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Starea vanzarii"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Data de expediere"
@@ -576,15 +595,15 @@
 
 msgctxt "field:sale.sale,shipment_state:"
 msgid "Shipment State"
 msgstr "Data de expediere"
 
 msgctxt "field:sale.sale,shipments:"
 msgid "Shipments"
-msgstr "Transporturi"
+msgstr "Expedieri"
 
 msgctxt "field:sale.sale,shipping_date:"
 msgid "Shipping Date"
 msgstr "Data de expediere"
 
 msgctxt "field:sale.sale,state:"
 msgid "State"
@@ -673,14 +692,22 @@
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "Timpul între confirmarea vânzării pana la trimiterea al produselor.\n"
 "Utilizat pentru produse fără un timp de execuţie."
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+"Timpul dintre confirmarea vânzării și trimiterea produselor.\n"
+"Utilizat pentru produse fără un timp de execuţie."
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Timpul de la confirmarea vânzării pana la trimiterea al produselor.\n"
 "Daca este gol se va folosi timpul implicit de execuţie."
@@ -796,37 +823,36 @@
 msgid "Configuration"
 msgstr "Configurare"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Vânzări"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Vânzări"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Vânzări"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Rând de vânzare"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Mișcări"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Vânzări"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Vânzări"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
-msgstr "Transporturi"
+msgstr "Expedieri"
 
 msgctxt "model:ir.action,name:report_sale"
 msgid "Sale"
 msgstr "Vânzare"
 
 msgctxt "model:ir.action,name:wizard_invoice_handle_exception"
 msgid "Handle Invoice Exception"
@@ -878,14 +904,42 @@
 msgstr "Se prelucreaza"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Ofertă"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "Tot"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Terminat"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "Tot"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Terminat"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "Nu se poate șterge parte \"%(party)s\" când au vănzări nefinalizate cu "
 "compania \"%(company)s\"."
@@ -921,14 +975,23 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "Nu puteți devalida factura \"%(invoice)s\", deoarece a fost generată de o "
 "vânzare."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+"Pentru a modifica antetul vânzării \"%(sale)s\", acesta trebuie să fie în "
+"stare devalidata."
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Pentru a șterge rândul \"%(line)s\" trebuie anulat sau resetat \"%(sale)s\" "
 "la proiectul de vânzare."
@@ -969,15 +1032,14 @@
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "model:ir.message,text:msg_sale_reporting_currency"
 msgid "Currency"
 msgstr "Valută"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_date"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "model:ir.message,text:msg_sale_reporting_number"
 msgid "#"
 msgstr "#"
@@ -1317,14 +1379,19 @@
 msgid "Amount"
 msgstr "Suma"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Adresa de facturare"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Descriere:"
@@ -1414,28 +1481,36 @@
 msgstr "La procesarea comenzii"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "La expediere trimis"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Excepție"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Nici unul"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Plătit"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "În Aşteptare"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1450,14 +1525,18 @@
 msgstr "Excepție"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Nici unul"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Trimis"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "În Aşteptare"
```

### Comparing `trytond_sale-6.6.2/locale/ru.po` & `trytond_sale-6.8.0/locale/bg.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice,sale_exception_state:"
 msgid "Exception State"
-msgstr "Состояние ситуации"
+msgstr "Състояние на грешка"
 
 msgctxt "field:account.invoice,sales:"
 msgid "Sales"
-msgstr "Продажи"
+msgstr "Продажби"
 
 #, fuzzy
 msgctxt "field:party.party,customer_currencies:"
 msgid "Customer Currencies"
-msgstr "Заказчики"
+msgstr "Клиенти"
 
 #, fuzzy
 msgctxt "field:party.party,customer_currency:"
 msgid "Customer Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:party.party,sale_invoice_method:"
 msgid "Invoice Method"
-msgstr "Метод инвойса"
+msgstr "Начин на фактуриране"
 
 #, fuzzy
 msgctxt "field:party.party,sale_methods:"
 msgid "Sale Methods"
-msgstr "Метод инвойса продажи"
+msgstr "Начин на фактурине на продажба"
 
 #, fuzzy
 msgctxt "field:party.party,sale_shipment_method:"
 msgid "Shipment Method"
-msgstr "Метод доставки"
+msgstr "Начин на изпращане"
 
 #, fuzzy
 msgctxt "field:party.party.customer_currency,customer_currency:"
 msgid "Customer Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:party.party.customer_currency,party:"
 msgid "Party"
-msgstr "Контрагент"
+msgstr "Партньор"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,party:"
 msgid "Party"
-msgstr "Контрагент"
+msgstr "Партньор"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Метод инвойса продажи"
+msgstr "Начин на фактурине на продажба"
 
 #, fuzzy
 msgctxt "field:party.party.sale_method,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Способ доставки продажи"
+msgstr "Начин на фактуриране на продажба"
 
 msgctxt "field:product.configuration,default_lead_time:"
 msgid "Default Lead Time"
 msgstr ""
 
 msgctxt "field:product.configuration.default_lead_time,default_lead_time:"
 msgid "Default Lead Time"
@@ -81,261 +81,281 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product,salable:"
 msgid "Salable"
-msgstr "Для продажи"
+msgstr "Продажен"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,sale_uom:"
 msgid "Sale UOM"
-msgstr "Ед.измерения продажи"
+msgstr "Мер. ед. на продажба"
 
 #, fuzzy
 msgctxt "field:product.sale.context,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:product.sale.context,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:product.sale.context,customer:"
 msgid "Customer"
-msgstr "Заказчики"
+msgstr "Клиенти"
 
 #, fuzzy
 msgctxt "field:product.sale.context,locations:"
 msgid "Warehouses"
-msgstr "Товарный склад"
+msgstr "Склад"
 
 #, fuzzy
 msgctxt "field:product.sale.context,quantity:"
 msgid "Quantity"
-msgstr "Кол-во"
+msgstr "Количество"
 
 #, fuzzy
 msgctxt "field:product.sale.context,sale_date:"
 msgid "Sale Date"
-msgstr "Дата продажи"
+msgstr "Дата на продажба"
 
 msgctxt "field:product.sale.context,stock_date_end:"
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
-msgstr "Для продажи"
+msgstr "Продажен"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
-msgstr "Ед.измерения продажи"
+msgstr "Мер. ед. на продажба"
 
 msgctxt "field:sale.configuration,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Метод инвойса продажи"
+msgstr "Начин на фактурине на продажба"
 
 msgctxt "field:sale.configuration,sale_process_after:"
 msgid "Process Sale after"
 msgstr ""
 
 msgctxt "field:sale.configuration,sale_sequence:"
 msgid "Sale Sequence"
 msgstr ""
 
 msgctxt "field:sale.configuration,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Способ доставки продажи"
+msgstr "Начин на фактуриране на продажба"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sale_method,sale_invoice_method:"
 msgid "Sale Invoice Method"
-msgstr "Метод инвойса продажи"
+msgstr "Начин на фактурине на продажба"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sale_method,sale_shipment_method:"
 msgid "Sale Shipment Method"
-msgstr "Способ доставки продажи"
+msgstr "Начин на фактуриране на продажба"
 
 #, fuzzy
 msgctxt "field:sale.configuration.sequence,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 msgctxt "field:sale.configuration.sequence,sale_sequence:"
 msgid "Sale Sequence"
 msgstr ""
 
 msgctxt "field:sale.handle.invoice.exception.ask,domain_invoices:"
 msgid "Domain Invoices"
-msgstr "Домен инвойсов"
+msgstr "Фактури на домейн"
 
 msgctxt "field:sale.handle.invoice.exception.ask,recreate_invoices:"
 msgid "Recreate Invoices"
-msgstr "Создать заново инвойсы"
+msgstr "Наново създаване на фактури"
 
 msgctxt "field:sale.handle.shipment.exception.ask,domain_moves:"
 msgid "Domain Moves"
-msgstr "Домен проводок"
+msgstr "Движение на домейн"
 
 msgctxt "field:sale.handle.shipment.exception.ask,recreate_moves:"
 msgid "Recreate Moves"
-msgstr "Создать заново проводки"
+msgstr "Наново създаване на движения"
 
 #, fuzzy
 msgctxt "field:sale.line,actual_quantity:"
 msgid "Actual Quantity"
-msgstr "Кол-во"
+msgstr "Количество"
 
 msgctxt "field:sale.line,amount:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Сума"
 
 #, fuzzy
 msgctxt "field:sale.line,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
+
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Клиенти"
 
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
-msgstr "Из местоположения"
+msgstr "От местонахождение"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Строки инвойса"
-
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Перемещения выполнены"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Особые ситуации перемещения"
+msgstr "Редове от фактура"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
-msgstr "Перемещения"
+msgstr "Движения"
+
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Грешка при движение"
 
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
-msgstr "Игнорированные проводки"
+msgstr "Игнорирани движения"
+
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Направени движения"
 
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
-msgstr "Созданные заново проводки"
+msgstr "Наново създаване на движения"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
-msgstr "Комментарий"
+msgstr "Бележка"
 
 msgctxt "field:sale.line,product:"
 msgid "Product"
 msgstr "Продукт"
 
 msgctxt "field:sale.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Категория ед. измерения продукции"
+msgstr "Категория мер. ед. на продукт"
 
 msgctxt "field:sale.line,quantity:"
 msgid "Quantity"
-msgstr "Кол-во"
+msgstr "Количество"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
+
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Дата на продажба"
 
 #, fuzzy
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
-msgstr "Дата продажи"
+msgstr "Дата на продажба"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
 
 msgctxt "field:sale.line,summary:"
 msgid "Summary"
 msgstr ""
 
 msgctxt "field:sale.line,taxes:"
 msgid "Taxes"
-msgstr "Налоги"
+msgstr "Данъци"
 
 msgctxt "field:sale.line,to_location:"
 msgid "To Location"
-msgstr "В местоположение"
+msgstr "Към местонахождение"
 
 msgctxt "field:sale.line,type:"
 msgid "Type"
-msgstr "Тип"
+msgstr "Вид"
 
 msgctxt "field:sale.line,unit:"
 msgid "Unit"
-msgstr "Единица измерения"
+msgstr "Единица"
 
 msgctxt "field:sale.line,unit_price:"
 msgid "Unit Price"
-msgstr "Цена за единицу"
+msgstr "Единична цена"
 
 msgctxt "field:sale.line,warehouse:"
 msgid "Warehouse"
-msgstr "Товарный склад"
+msgstr "Склад"
 
 msgctxt "field:sale.line-account.tax,line:"
 msgid "Sale Line"
-msgstr "Строка продажи"
+msgstr "Ред от продажба"
 
 msgctxt "field:sale.line-account.tax,tax:"
 msgid "Tax"
-msgstr "Налог"
+msgstr "Данък"
 
 msgctxt "field:sale.line-ignored-stock.move,move:"
 msgid "Move"
-msgstr "Перемещение"
+msgstr "Движение"
 
 msgctxt "field:sale.line-ignored-stock.move,sale_line:"
 msgid "Sale Line"
-msgstr "Строка продажи"
+msgstr "Ред от продажба"
 
 msgctxt "field:sale.line-recreated-stock.move,move:"
 msgid "Move"
-msgstr "Перемещение"
+msgstr "Движение"
 
 msgctxt "field:sale.line-recreated-stock.move,sale_line:"
 msgid "Sale Line"
-msgstr "Строка продажи"
+msgstr "Ред от продажба"
 
 #, fuzzy
 msgctxt "field:sale.reporting.context,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 msgctxt "field:sale.reporting.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:sale.reporting.context,period:"
 msgid "Period"
@@ -344,15 +364,15 @@
 msgctxt "field:sale.reporting.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.context,warehouse:"
 msgid "Warehouse"
-msgstr "Товарный склад"
+msgstr "Склад"
 
 msgctxt "field:sale.reporting.country,country:"
 msgid "Country"
 msgstr ""
 
 msgctxt "field:sale.reporting.country.subdivision,country:"
 msgid "Country"
@@ -386,15 +406,15 @@
 msgctxt "field:sale.reporting.country.tree,region:"
 msgid "Region"
 msgstr "Open Region"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer,customer:"
 msgid "Customer"
-msgstr "Заказчики"
+msgstr "Клиенти"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category,category:"
 msgid "Category"
 msgstr "Sales per Category"
 
 #, fuzzy
@@ -405,33 +425,33 @@
 msgctxt "field:sale.reporting.customer.category.tree,children:"
 msgid "Children"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:sale.reporting.customer.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,revenue:"
 msgid "Revenue"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.customer.time_series,customer:"
 msgid "Customer"
-msgstr "Заказчики"
+msgstr "Клиенти"
 
 #, fuzzy
 msgctxt "field:sale.reporting.product,product:"
 msgid "Product"
 msgstr "Продукт"
 
 #, fuzzy
@@ -447,20 +467,20 @@
 msgctxt "field:sale.reporting.product.category.tree,children:"
 msgid "Children"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:sale.reporting.product.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,revenue:"
 msgid "Revenue"
@@ -470,20 +490,20 @@
 msgctxt "field:sale.reporting.product.time_series,product:"
 msgid "Product"
 msgstr "Продукт"
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:sale.reporting.region.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.region.tree,revenue:"
 msgid "Revenue"
@@ -491,194 +511,194 @@
 
 msgctxt "field:sale.reporting.region.tree,subregions:"
 msgid "Subregions"
 msgstr ""
 
 msgctxt "field:sale.sale,comment:"
 msgid "Comment"
-msgstr "Комментарии"
+msgstr "Коментар"
 
 msgctxt "field:sale.sale,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:sale.sale,confirmed_by:"
 msgid "Confirmed By"
-msgstr "Confirmed"
+msgstr "Потвърден"
 
 msgctxt "field:sale.sale,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.sale,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 msgctxt "field:sale.sale,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:sale.sale,invoice_address:"
 msgid "Invoice Address"
-msgstr "Адрес для инвойса"
+msgstr "Адрес за фактура"
 
 msgctxt "field:sale.sale,invoice_method:"
 msgid "Invoice Method"
-msgstr "Метод инвойса"
+msgstr "Начин на фактуриране"
 
 #, fuzzy
 msgctxt "field:sale.sale,invoice_party:"
 msgid "Invoice Party"
-msgstr "Состояние инвойса"
+msgstr "Състояние на фактура"
 
 msgctxt "field:sale.sale,invoice_state:"
 msgid "Invoice State"
-msgstr "Состояние инвойса"
+msgstr "Състояние на фактура"
 
 msgctxt "field:sale.sale,invoices:"
 msgid "Invoices"
-msgstr "Инвойсы"
+msgstr "Фактури"
 
 msgctxt "field:sale.sale,invoices_ignored:"
 msgid "Ignored Invoices"
-msgstr "Игнорированные инвойсы"
+msgstr "Игнорирани фактури"
 
 msgctxt "field:sale.sale,invoices_recreated:"
 msgid "Recreated Invoices"
-msgstr "Созданные заново инвойсы"
+msgstr "Наново създадени на фактури"
 
 msgctxt "field:sale.sale,lines:"
 msgid "Lines"
-msgstr "Строки"
+msgstr "Редове"
 
 msgctxt "field:sale.sale,moves:"
 msgid "Moves"
-msgstr "Перемещения"
+msgstr "Движения"
 
 #, fuzzy
 msgctxt "field:sale.sale,number:"
 msgid "Number"
 msgstr "Номер"
 
 #, fuzzy
 msgctxt "field:sale.sale,origin:"
 msgid "Origin"
-msgstr "Первоисточник"
+msgstr "Източник"
 
 msgctxt "field:sale.sale,party:"
 msgid "Party"
-msgstr "Контрагент"
+msgstr "Партньор"
 
 msgctxt "field:sale.sale,party_lang:"
 msgid "Party Language"
-msgstr "Язык контрагента"
+msgstr "Език на партньор"
 
 msgctxt "field:sale.sale,payment_term:"
 msgid "Payment Term"
-msgstr "Правило оплаты"
+msgstr "Условие за плащане"
 
 #, fuzzy
 msgctxt "field:sale.sale,quoted_by:"
 msgid "Quoted By"
 msgstr "Quote"
 
 msgctxt "field:sale.sale,reference:"
 msgid "Reference"
-msgstr "Ссылка"
+msgstr "Отпратка"
 
 msgctxt "field:sale.sale,sale_date:"
 msgid "Sale Date"
-msgstr "Дата продажи"
+msgstr "Дата на продажба"
 
 msgctxt "field:sale.sale,shipment_address:"
 msgid "Shipment Address"
-msgstr "Адрес доставки"
+msgstr "Адрес за доставка"
 
 msgctxt "field:sale.sale,shipment_method:"
 msgid "Shipment Method"
-msgstr "Метод доставки"
+msgstr "Начин на изпращане"
 
 msgctxt "field:sale.sale,shipment_party:"
 msgid "Shipment Party"
 msgstr ""
 
 msgctxt "field:sale.sale,shipment_returns:"
 msgid "Shipment Returns"
-msgstr "Возврат"
+msgstr "Върнати доставки"
 
 msgctxt "field:sale.sale,shipment_state:"
 msgid "Shipment State"
-msgstr "Состояние доставки"
+msgstr "Състояние на пратка"
 
 msgctxt "field:sale.sale,shipments:"
 msgid "Shipments"
-msgstr "Доставка"
+msgstr "Изпращания"
 
 #, fuzzy
 msgctxt "field:sale.sale,shipping_date:"
 msgid "Shipping Date"
-msgstr "Состояние доставки"
+msgstr "Състояние на пратка"
 
 msgctxt "field:sale.sale,state:"
 msgid "State"
-msgstr "Состояние"
+msgstr "Състояние"
 
 msgctxt "field:sale.sale,tax_amount:"
 msgid "Tax"
-msgstr "Налог"
+msgstr "Данък"
 
 msgctxt "field:sale.sale,tax_amount_cache:"
 msgid "Tax Cache"
-msgstr "Облагаемые налогом"
+msgstr "Данък в брой"
 
 msgctxt "field:sale.sale,total_amount:"
 msgid "Total"
-msgstr "Итого"
+msgstr "Общо"
 
 #, fuzzy
 msgctxt "field:sale.sale,total_amount_cache:"
 msgid "Total Cache"
-msgstr "Облагаемые налогом"
+msgstr "Данък в брой"
 
 msgctxt "field:sale.sale,untaxed_amount:"
 msgid "Untaxed"
-msgstr "Без налога"
+msgstr "Необложен с данък"
 
 msgctxt "field:sale.sale,untaxed_amount_cache:"
 msgid "Untaxed Cache"
-msgstr "Необлагаемые налогом"
+msgstr "Наличност преди данъци"
 
 msgctxt "field:sale.sale,warehouse:"
 msgid "Warehouse"
-msgstr "Товарный склад"
+msgstr "Склад"
 
 msgctxt "field:sale.sale-ignored-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Инвойс"
+msgstr "Фактура"
 
 msgctxt "field:sale.sale-ignored-account.invoice,sale:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "field:sale.sale-recreated-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Инвойс"
+msgstr "Фактура"
 
 msgctxt "field:sale.sale-recreated-account.invoice,sale:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "field:stock.move,sale:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "field:stock.move,sale_exception_state:"
 msgid "Exception State"
-msgstr "Состояние ситуации"
+msgstr "Състояние на грешка"
 
 msgctxt "help:party.party,customer_currency:"
 msgid "Default currency for sales to this party."
 msgstr ""
 
 msgctxt "help:party.party,sale_invoice_method:"
 msgid ""
@@ -698,14 +718,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -720,15 +746,15 @@
 "Applied if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:sale.handle.invoice.exception.ask,recreate_invoices:"
 msgid ""
 "The selected invoices will be recreated. The other ones will be ignored."
 msgstr ""
-"Выбранные инвойсы будут созданы заново. Остальные будут проигнорированы."
+"Избраните фактури ще бъдат наново създадени. Останалите ще бъдат игнорирани."
 
 msgctxt "help:sale.sale,shipping_date:"
 msgid "When the shipping of goods should start."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
@@ -780,20 +806,20 @@
 msgctxt "model:ir.action,name:act_reporting_customer_time_series"
 msgid "Sales per Customer"
 msgstr "Sales per Customer"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Sales"
-msgstr "Продажи"
+msgstr "Продажби"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Sales"
-msgstr "Продажи"
+msgstr "Продажби"
 
 msgctxt "model:ir.action,name:act_reporting_product"
 msgid "Sales per Product"
 msgstr "Sales per Product"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_product_category"
@@ -831,36 +857,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Продажи"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Ред от продажба"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
-msgstr "Перемещения"
+msgstr "Движения"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Продажби"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Продажи"
+msgstr "Продажби"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
 #, fuzzy
@@ -886,54 +908,81 @@
 msgctxt "model:ir.action,name:wizard_reporting_region_tree_open"
 msgid "Open Region"
 msgstr "Open Region"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_return_sale"
 msgid "Return Sale"
-msgstr "Создать возврат продажи"
+msgstr "Създаване на меню Продажби"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_shipment_handle_exception"
 msgid "Handle Shipment Exception"
 msgstr "Handle Shipment Exception"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_all"
 msgid "All"
 msgstr "All"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_confirmed"
 msgid "Confirmed"
-msgstr "Confirmed"
+msgstr "Потвърден"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Проект"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_exception"
 msgid "Exception"
-msgstr "Особая ситуация"
+msgstr "Грешка"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_processing"
 msgid "Processing"
-msgstr "Processing"
+msgstr "Обработване"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
-msgstr "Quotation"
+msgstr "Запитване"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Приключен"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Приключен"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
@@ -960,14 +1009,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -993,20 +1048,20 @@
 "To invoice sale \"%(sale)s\" you must define an account revenue for product "
 "\"%(product)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_company"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_currency"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Валута"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_date"
 msgid "Date"
 msgstr "Дата:"
 
 #, fuzzy
@@ -1187,15 +1242,15 @@
 msgctxt "model:party.party.customer_currency,name:"
 msgid "Party Customer Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:party.party.sale_method,name:"
 msgid "Party Sale Method"
-msgstr "Метод инвойса продажи"
+msgstr "Начин на фактурине на продажба"
 
 msgctxt "model:product.configuration.default_lead_time,name:"
 msgid "Product Default Lead Time"
 msgstr ""
 
 msgctxt "model:product.lead_time,name:"
 msgid "Product Lead Time"
@@ -1213,47 +1268,47 @@
 #, fuzzy
 msgctxt "model:res.group,name:group_sale_admin"
 msgid "Sales Administrator"
 msgstr "Sales Administrator"
 
 msgctxt "model:sale.configuration,name:"
 msgid "Sale Configuration"
-msgstr "Конфигурация продаж"
+msgstr "Конфигурация на продажба"
 
 msgctxt "model:sale.configuration.sale_method,name:"
 msgid "Sale Configuration Sale Method"
 msgstr ""
 
 msgctxt "model:sale.configuration.sequence,name:"
 msgid "Sale Configuration Sequence"
 msgstr ""
 
 msgctxt "model:sale.handle.invoice.exception.ask,name:"
 msgid "Handle Invoice Exception"
-msgstr "Обработка особых ситуаций инвойса"
+msgstr "Обработване за грешка в фактура"
 
 msgctxt "model:sale.handle.shipment.exception.ask,name:"
 msgid "Handle Shipment Exception"
-msgstr "Обработка особых ситуаций доставки"
+msgstr "Обработване на грешка при пратка"
 
 msgctxt "model:sale.line,name:"
 msgid "Sale Line"
-msgstr "Строка продажи"
+msgstr "Ред от продажба"
 
 msgctxt "model:sale.line-account.tax,name:"
 msgid "Sale Line - Tax"
-msgstr "Строка продажи - Налоги"
+msgstr "Ред от продажба - Данък"
 
 msgctxt "model:sale.line-ignored-stock.move,name:"
 msgid "Sale Line - Ignored Move"
-msgstr "Строка продажи - Игнорированные перемещения"
+msgstr "Ред от продажба - Игнорирано движение"
 
 msgctxt "model:sale.line-recreated-stock.move,name:"
 msgid "Sale Line - Recreated Move"
-msgstr "Строка продажи - Созданные заново перемещения"
+msgstr "Ред от продажба - Нановосъздадено движение"
 
 msgctxt "model:sale.reporting.context,name:"
 msgid "Sale Reporting Context"
 msgstr ""
 
 msgctxt "model:sale.reporting.country,name:"
 msgid "Sale Reporting per Country"
@@ -1336,113 +1391,118 @@
 msgctxt "model:sale.reporting.region.tree,name:"
 msgid "Sale Reporting per Region"
 msgstr "Sales per Category"
 
 #, fuzzy
 msgctxt "model:sale.return_sale.start,name:"
 msgid "Return Sale"
-msgstr "Создать возврат продажи"
+msgstr "Създаване на меню Продажби"
 
 msgctxt "model:sale.sale,name:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "model:sale.sale-ignored-account.invoice,name:"
 msgid "Sale - Ignored Invoice"
-msgstr "Продажи - Игнорируемые инвойсы"
+msgstr "Продажба - Игнорирани фактури"
 
 msgctxt "model:sale.sale-recreated-account.invoice,name:"
 msgid "Sale - Recreated Invoice"
-msgstr "Продажи - Созданные заново инвойсы"
+msgstr "Продажба - Наново създадена фактура"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:sale.sale:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Сума"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Дата:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Адрес за фактура"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Описание:"
 
 msgctxt "report:sale.sale:"
 msgid "Draft Sale Order"
-msgstr "Черновой заказ на продажу"
+msgstr "Проект на поръчка за продажба"
 
 msgctxt "report:sale.sale:"
 msgid "Quantity"
-msgstr "Кол-во"
+msgstr "Количество"
 
 msgctxt "report:sale.sale:"
 msgid "Quotation N°:"
-msgstr "Котировка N°:"
+msgstr "Запитване N°:"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Reference:"
-msgstr "Ссылка"
+msgstr "Отпратка"
 
 msgctxt "report:sale.sale:"
 msgid "Sale Order N°:"
-msgstr "Заказ на продажу №:"
+msgstr "Поръчка за продажба N°:"
 
 msgctxt "report:sale.sale:"
 msgid "Taxes"
-msgstr "Налоги"
+msgstr "Данъци"
 
 msgctxt "report:sale.sale:"
 msgid "Taxes:"
-msgstr "Налоги:"
+msgstr "Данъци:"
 
 msgctxt "report:sale.sale:"
 msgid "Total (excl. taxes):"
-msgstr "Итого (без налогов):"
+msgstr "Общо (без данъци):"
 
 msgctxt "report:sale.sale:"
 msgid "Total:"
-msgstr "Итого:"
+msgstr "Общо:"
 
 msgctxt "report:sale.sale:"
 msgid "Unit Price"
-msgstr "Цена за единицу"
+msgstr "Единична цена"
 
 msgctxt "selection:account.invoice,sale_exception_state:"
 msgid "Ignored"
-msgstr "Игнорируется"
+msgstr "Игнорирано"
 
 msgctxt "selection:account.invoice,sale_exception_state:"
 msgid "Recreated"
-msgstr "Создано заново"
+msgstr "Създаден наново"
 
 msgctxt "selection:sale.line,type:"
 msgid "Comment"
-msgstr "Комментарии"
+msgstr "Коментар"
 
 msgctxt "selection:sale.line,type:"
 msgid "Line"
-msgstr "Строка"
+msgstr "Ред"
 
 msgctxt "selection:sale.line,type:"
 msgid "Subtotal"
-msgstr "Подитог"
+msgstr "Междинна сума"
 
 msgctxt "selection:sale.line,type:"
 msgid "Title"
-msgstr "Заголовок"
+msgstr "Заглавие"
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Month"
@@ -1450,131 +1510,143 @@
 
 msgctxt "selection:sale.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "Manual"
-msgstr "Ручной"
+msgstr "Ръчно"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Order Processed"
-msgstr "При обработке заказа"
+msgstr "При обработена поръчка"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
-msgstr "При отправке груза"
+msgstr "При изпращане на пратка"
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
-msgstr "Особая ситуация"
+msgstr "Грешка"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
-msgstr "Отсутствует"
+msgstr "Няма"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
-msgstr "Оплачен"
+msgstr "Платен"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Ожидание"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
-msgstr "Ручной"
+msgstr "Ръчно"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
-msgstr "При оплате инвойса"
+msgstr "При плащане на фактура"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Order Processed"
-msgstr "При обработке заказа"
+msgstr "При обработена поръчка"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Exception"
-msgstr "Особая ситуация"
+msgstr "Грешка"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
-msgstr "Отсутствует"
+msgstr "Няма"
+
+msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
-msgstr "Отправлен"
+msgstr "Изпратен"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
-msgstr "Ожидание"
+msgstr "Изчакващ"
 
 #, fuzzy
 msgctxt "selection:sale.sale,state:"
 msgid "Cancelled"
-msgstr "Отменено"
+msgstr "Отказан"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Confirmed"
-msgstr "Подтвержденно"
+msgstr "Потвърден"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Done"
-msgstr "Выполнено"
+msgstr "Приключен"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Draft"
-msgstr "Черновик"
+msgstr "Проект"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Processing"
-msgstr "Обработка"
+msgstr "Обработване"
 
 msgctxt "selection:sale.sale,state:"
 msgid "Quotation"
-msgstr "Котировка"
+msgstr "Запитване"
 
 msgctxt "selection:stock.move,sale_exception_state:"
 msgid "Ignored"
-msgstr "Игнорируется"
+msgstr "Игнорирано"
 
 msgctxt "selection:stock.move,sale_exception_state:"
 msgid "Recreated"
-msgstr "Создано заново"
+msgstr "Създаден наново"
 
 #, fuzzy
 msgctxt "view:party.party:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "view:product.template:"
 msgid "Customers"
-msgstr "Заказчики"
+msgstr "Клиенти"
 
 #, fuzzy
 msgctxt "view:sale.handle.invoice.exception.ask:"
 msgid "Choose invoices to recreate:"
-msgstr "Выберите инвойсы для пересоздания"
+msgstr "Избор на фактури за ново създаване"
 
 #, fuzzy
 msgctxt "view:sale.handle.shipment.exception.ask:"
 msgid "Choose move to recreate:"
-msgstr "Выберите проводки для пересоздания"
+msgstr "Избор на движение за ново създаване"
 
 msgctxt "view:sale.line:"
 msgid "General"
-msgstr "Основной"
+msgstr "Основен"
 
 msgctxt "view:sale.line:"
 msgid "Notes"
-msgstr "Комментарии"
+msgstr "Бележки"
 
 msgctxt "view:sale.line:"
 msgid "Taxes"
-msgstr "Налоги"
+msgstr "Данъци"
 
 #, fuzzy
 msgctxt "view:sale.reporting.country.subdivision.time_series:"
 msgid "Number"
 msgstr "Номер"
 
 msgctxt "view:sale.reporting.country.subdivision.time_series:"
@@ -1646,47 +1718,47 @@
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Other Info"
-msgstr "Другая информация"
+msgstr "Друга информация"
 
 msgctxt "view:sale.sale:"
 msgid "Sale"
-msgstr "Продажа"
+msgstr "Продажба"
 
 msgctxt "wizard_button:sale.handle.invoice.exception,ask,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Отказ"
 
 msgctxt "wizard_button:sale.handle.invoice.exception,ask,handle:"
 msgid "OK"
-msgstr "Ок"
+msgstr "Добре"
 
 msgctxt "wizard_button:sale.handle.shipment.exception,ask,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Отказ"
 
 msgctxt "wizard_button:sale.handle.shipment.exception,ask,handle:"
 msgid "OK"
-msgstr "Ок"
+msgstr "Добре"
 
 #, fuzzy
 msgctxt "wizard_button:sale.modify_header,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Отказ"
 
 msgctxt "wizard_button:sale.modify_header,start,modify:"
 msgid "Modify"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:sale.return_sale,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Отказване"
 
 #, fuzzy
 msgctxt "wizard_button:sale.return_sale,start,return_:"
 msgid "Return"
-msgstr "Возвраты"
+msgstr "Връщане"
```

### Comparing `trytond_sale-6.6.2/locale/sl.po` & `trytond_sale-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Dobavni rok"
 
+#, fuzzy
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr "Dobavni rok"
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Za prodajo"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Prodajna cena"
@@ -134,14 +139,19 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Dobavni rok"
 
+#, fuzzy
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr "Dobavni rok"
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Za prodajo"
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr "Prodajna ME"
@@ -209,42 +219,49 @@
 msgstr "Družba"
 
 #, fuzzy
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Kupci"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr "Iz lokacije"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Postavke računa"
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr "Zaključen promet"
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr "Pridržani promet"
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Promet"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Pridržani promet"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Prezrt promet"
 
+#, fuzzy
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr "Zaključen promet"
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Ponovno izdelan promet"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Opomba"
@@ -261,14 +278,19 @@
 msgid "Quantity"
 msgstr "Količina"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Prodajni nalog"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Datum prodaje"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Stanje prodajnega naloga"
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr "Datum odpreme"
@@ -693,14 +715,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -825,36 +853,32 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
-msgstr "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
+msgstr "Postavka"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Promet"
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Prodajni nalogi"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Prodajni nalogi"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
 #, fuzzy
@@ -921,14 +945,42 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "Zaključeno"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "Zaključeno"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -954,14 +1006,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1356,14 +1414,19 @@
 msgid "Amount"
 msgstr "Znesek"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Datum:"
 
+#, fuzzy
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr "Naslov plačnika"
+
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr "Opis:"
@@ -1453,28 +1516,36 @@
 msgstr "Po obdelavi naloga"
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "Po izvršeni odpremi"
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Pridržano"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "Brez"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Plačano"
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
-msgstr "Čakajoče"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
+msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Ročno"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1489,14 +1560,18 @@
 msgstr "Pridržano"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Brez"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Odpremljeno"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr "Čakajoče"
```

### Comparing `trytond_sale-6.6.2/locale/tr.po` & `trytond_sale-6.8.0/locale/tr.po`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -123,14 +127,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -195,42 +203,48 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Sales per Customer"
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "Handle Invoice Exception"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr ""
@@ -248,14 +262,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Sales"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "Sales"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -674,14 +693,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -801,31 +826,30 @@
 msgid "Configuration"
 msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Shipments"
 
@@ -885,14 +909,40 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -918,14 +968,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1317,14 +1373,18 @@
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr ""
 
@@ -1413,27 +1473,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1449,14 +1517,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/uk.po` & `trytond_sale-6.8.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -114,14 +118,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -186,42 +194,46 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr ""
+
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line,move_exception:"
+msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr ""
@@ -238,14 +250,18 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr ""
 
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr ""
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -648,14 +664,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -763,31 +785,27 @@
 msgid "Configuration"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr ""
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr ""
 
@@ -843,14 +861,38 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -876,14 +918,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1253,14 +1301,18 @@
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
+msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
 msgstr ""
 
@@ -1349,27 +1401,35 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1385,14 +1445,18 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/locale/zh_CN.po` & `trytond_sale-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 msgid "Template"
 msgstr ""
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.product,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr ""
@@ -123,14 +127,18 @@
 msgid "Stock End Date"
 msgstr ""
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+msgctxt "field:product.template,lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr ""
 
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UOM"
 msgstr ""
@@ -196,42 +204,48 @@
 msgstr ""
 
 msgctxt "field:sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:sale.line,customer:"
+msgid "Customer"
+msgstr "Sales per Customer"
+
+#, fuzzy
 msgctxt "field:sale.line,description:"
 msgid "Description"
 msgstr "描述"
 
 msgctxt "field:sale.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
-msgctxt "field:sale.line,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,moves_exception:"
+msgid "Moves Exception"
+msgstr "处理发票异常"
+
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,note:"
 msgid "Note"
@@ -250,14 +264,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Sales"
 
+#, fuzzy
+msgctxt "field:sale.line,sale_date:"
+msgid "Sale Date"
+msgstr "写入日期"
+
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.line,shipping_date:"
 msgid "Shipping Date"
 msgstr ""
@@ -682,14 +701,20 @@
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 
+msgctxt "help:product.configuration.default_lead_time,default_lead_time:"
+msgid ""
+"The time from confirming the sales order to sending the products.\n"
+"Used for products without a lead time."
+msgstr ""
+
 msgctxt "help:product.product,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 
 msgctxt "help:product.template,lead_time:"
@@ -809,31 +834,30 @@
 msgid "Configuration"
 msgstr "设置"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_form2"
-msgid "Sales"
-msgstr "Sales"
-
-msgctxt "model:ir.action,name:act_sale_invoice_relate"
-msgid "Sales"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_line_relate"
+msgid "Sale Lines"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_sale_shipment_returns_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Sales"
 
-msgctxt "model:ir.action,name:act_sale_shipments_relate"
+#, fuzzy
+msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "发货"
 
@@ -894,14 +918,42 @@
 msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Quotation"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
+msgid "All"
+msgstr "全部"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
+msgid "Done"
+msgstr "完成"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
+msgid "All"
+msgstr "全部"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
+msgid "Done"
+msgstr "完成"
+
+msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
@@ -927,14 +979,20 @@
 
 msgctxt "model:ir.message,text:msg_sale_invoice_reset_draft"
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_line_create_draft"
+msgid ""
+"You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
+" state."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
@@ -1326,14 +1384,18 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr ""
 
+msgctxt "report:sale.sale:"
+msgid "Delivery Address:"
+msgstr ""
+
 #, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "描述"
 
 #, fuzzy
 msgctxt "report:sale.sale:"
@@ -1425,28 +1487,36 @@
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
+msgid "Awaiting Payment"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
 msgstr "注释"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:sale.sale,invoice_state:"
-msgid "Waiting"
+msgid "Partially Paid"
+msgstr ""
+
+msgctxt "selection:sale.sale,invoice_state:"
+msgid "Pending"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_method:"
@@ -1463,14 +1533,18 @@
 
 #, fuzzy
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "注释"
 
 msgctxt "selection:sale.sale,shipment_state:"
+msgid "Partially Shipped"
+msgstr ""
+
+msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
 msgstr ""
```

### Comparing `trytond_sale-6.6.2/message.xml` & `trytond_sale-6.8.0/message.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale-6.6.2/message.xml` & `trytond_sale-6.8.0/message.xml`

```diff
@@ -38,14 +38,17 @@
     </record>
     <record model="ir.message" id="msg_sale_line_delete_cancel_draft">
       <field name="text">To delete line &quot;%(line)s&quot; you must cancel or reset to draft sale &quot;%(sale)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_sale_modify_header_draft">
       <field name="text">To modify the header of sale &quot;%(sale)s&quot;, it must be in &quot;draft&quot; state.</field>
     </record>
+    <record model="ir.message" id="msg_sale_line_create_draft">
+      <field name="text">You cannot add lines to sale &quot;%(sale)s&quot; because it is no longer in a draft state.</field>
+    </record>
     <record model="ir.message" id="msg_sale_reporting_company">
       <field name="text">Company</field>
     </record>
     <record model="ir.message" id="msg_sale_reporting_number">
       <field name="text">#</field>
     </record>
     <record model="ir.message" id="msg_sale_reporting_number_help">
```

### Comparing `trytond_sale-6.6.2/party.py` & `trytond_sale-6.8.0/party.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,16 @@
         return super().multivalue_model(field)
 
     get_sale_invoice_method = get_sale_methods('invoice_method')
     get_sale_shipment_method = get_sale_methods('shipment_method')
 
     @classmethod
     def copy(cls, parties, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             fields = [
                 'sale_methods', 'sale_invoice_method', 'sale_shipment_method']
             default_values = cls.default_get(fields, with_rec_name=False)
             for fname in fields:
                 default.setdefault(fname, default_values.get(fname))
         return super().copy(parties, default=default)
```

### Comparing `trytond_sale-6.6.2/party.xml` & `trytond_sale-6.8.0/party.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_sale-6.6.2/party.xml` & `trytond_sale-6.8.0/party.xml`

```diff
@@ -1,27 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
-    <record model="ir.action.act_window" id="act_sale_form2">
-      <field name="name">Sales</field>
-      <field name="res_model">sale.sale</field>
-      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('party', '=', Eval('active_id')), ('party', 'in', Eval('active_ids')))]" pyson="1"/>
-      <field name="search_value" eval="[('state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
+    <record model="ir.ui.view" id="party_view_form">
+      <field name="model">party.party</field>
+      <field name="inherit" ref="party.party_view_form"/>
+      <field name="name">party_form</field>
     </record>
-    <record model="ir.action.keyword" id="act_open_sale_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">party.party,-1</field>
-      <field name="action" ref="act_sale_form2"/>
-    </record>
-    <record model="ir.action-res.group" id="act_sale_form2-group_sale">
-      <field name="action" ref="act_sale_form2"/>
-      <field name="group" ref="group_sale"/>
+    <record model="ir.action.wizard" id="act_open_customer">
+      <field name="name">Parties associated to Sales</field>
+      <field name="wiz_name">sale.open_customer</field>
     </record>
+    <menuitem name="Associated to Sales" parent="party.menu_party_form" action="act_open_customer" sequence="50" id="menu_customer" icon="tryton-list"/>
     <record model="ir.model.field.access" id="access_party_sale_invoice_method">
       <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_method')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_invoice_method_group_sale">
       <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_method')]"/>
```

### Comparing `trytond_sale-6.6.2/product.py` & `trytond_sale-6.8.0/product.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
 from sql import Null
 
 from trytond.model import ModelSQL, ModelView, ValueMixin, fields
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval
+from trytond.pyson import Eval, TimeDelta
 from trytond.transaction import Transaction
 
+default_lead_time = fields.TimeDelta(
+    "Default Lead Time",
+    domain=['OR',
+        ('default_lead_time', '=', None),
+        ('default_lead_time', '>=', TimeDelta()),
+        ],
+    help="The time from confirming the sales order to sending the "
+    "products.\n"
+    "Used for products without a lead time.")
+
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'product.configuration'
 
-    default_lead_time = fields.MultiValue(
-        fields.TimeDelta(
-            "Default Lead Time",
-            help="The time from confirming the sales order to sending the "
-            "products.\n"
-            "Used for products without a lead time."))
-
-    @classmethod
-    def default_default_lead_time(cls, **pattern):
-        return datetime.timedelta(0)
+    default_lead_time = fields.MultiValue(default_lead_time)
 
 
 class DefaultLeadTime(ModelSQL, ValueMixin):
     "Product Default Lead Time"
     __name__ = 'product.configuration.default_lead_time'
-    default_lead_time = fields.TimeDelta("Default Lead Time")
+    default_lead_time = default_lead_time
 
 
 class Template(metaclass=PoolMeta):
     __name__ = 'product.template'
     salable = fields.Boolean("Salable")
     sale_uom = fields.Many2One(
         'product.uom', "Sale UOM",
@@ -43,20 +44,26 @@
             'required': Eval('salable', False),
             },
         domain=[
             ('category', '=', Eval('default_uom_category')),
             ])
     lead_time = fields.MultiValue(fields.TimeDelta(
             "Lead Time",
+            domain=['OR',
+                ('lead_time', '=', None),
+                ('lead_time', '>=', TimeDelta()),
+                ],
             states={
                 'invisible': ~Eval('salable', False),
                 },
             help="The time from confirming the sales order to sending the "
             "products.\n"
             "If empty the default lead time from the configuration is used."))
+    lead_times = fields.One2Many(
+        'product.lead_time', 'template', "Lead Times")
 
     @classmethod
     def __register__(cls, module_name):
         transaction = Transaction()
         cursor = transaction.connection.cursor()
         update = transaction.connection.cursor()
         table = cls.__table_handler__(module_name)
@@ -108,15 +115,20 @@
 
 class ProductLeadTime(ModelSQL, ValueMixin):
     "Product Lead Time"
     __name__ = 'product.lead_time'
 
     template = fields.Many2One(
         'product.template', "Template", ondelete='CASCADE')
-    lead_time = fields.TimeDelta("Lead Time")
+    lead_time = fields.TimeDelta(
+        "Lead Time",
+        domain=['OR',
+            ('lead_time', '=', None),
+            ('lead_time', '>=', TimeDelta()),
+            ])
 
     @classmethod
     def __register__(cls, module_name):
         pool = Pool()
         Template = pool.get('product.template')
         template = Template.__table__()
         table = cls.__table__()
@@ -154,48 +166,50 @@
         Return the sale price for products and quantity.
         It uses if exists from the context:
             uom: the unit of measure or the sale uom of the product
             currency: the currency id for the returned price
         '''
         pool = Pool()
         Uom = pool.get('product.uom')
-        User = pool.get('res.user')
+        Company = pool.get('company.company')
         Currency = pool.get('currency.currency')
         Date = pool.get('ir.date')
 
         today = Date.today()
+        context = Transaction().context
         prices = {}
 
         assert len(products) == len(set(products)), "Duplicate products"
 
         uom = None
-        if Transaction().context.get('uom'):
-            uom = Uom(Transaction().context.get('uom'))
+        if context.get('uom'):
+            uom = Uom(context['uom'])
 
         currency = None
         if Transaction().context.get('currency'):
             currency = Currency(Transaction().context.get('currency'))
-
-        user = User(Transaction().user)
+        company = None
+        if context.get('company'):
+            company = Company(context['company'])
 
         for product in products:
             unit_price = product._get_sale_unit_price(quantity=quantity)
             if unit_price is not None:
                 if uom and product.default_uom.category == uom.category:
                     unit_price = Uom.compute_price(
                         product.default_uom, unit_price, uom)
                 else:
                     unit_price = Uom.compute_price(
                         product.default_uom, unit_price, product.sale_uom)
-            if currency and user.company and unit_price is not None:
-                if user.company.currency != currency:
+            if currency and company and unit_price is not None:
+                if company.currency != currency:
                     date = Transaction().context.get('sale_date') or today
                     with Transaction().set_context(date=date):
                         unit_price = Currency.compute(
-                            user.company.currency, unit_price,
+                            company.currency, unit_price,
                             currency, round=False)
             prices[product.id] = unit_price
         return prices
 
     @property
     def lead_time_used(self):
         pool = Pool()
```

### Comparing `trytond_sale-6.6.2/product.xml` & `trytond_sale-6.8.0/product.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_sale-6.6.2/product.xml` & `trytond_sale-6.8.0/product.xml`

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
     <record model="ir.ui.view" id="product_view_list_sale_line">
       <field name="model">product.product</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">product_list_sale_line</field>
     </record>
     <record model="ir.action.act_window" id="act_product">
```

### Comparing `trytond_sale-6.6.2/sale.fodt` & `trytond_sale-6.8.0/sale.fodt`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale-6.6.2/sale.fodt` & `trytond_sale-6.8.0/sale.fodt`

```diff
@@ -1,193 +1,209 @@
 <?xml version="1.0" encoding="utf-8"?>
-<office:document xmlns:officeooo="http://openoffice.org/2009/office" xmlns:grddl="http://www.w3.org/2003/g/data-view#" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xforms="http://www.w3.org/2002/xforms" xmlns:dom="http://www.w3.org/2001/xml-events" xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0" xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0" xmlns:math="http://www.w3.org/1998/Math/MathML" xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0" xmlns:dr3d="urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0" xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0" xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0" xmlns:formx="urn:openoffice:names:experimental:ooxml-odf-interop:xmlns:form:1.0" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:ooo="http://openoffice.org/2004/office" xmlns:loext="urn:org:documentfoundation:names:experimental:office:xmlns:loext:1.0" xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0" xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0" xmlns:field="urn:openoffice:names:experimental:ooo-ms-interop:xmlns:field:1.0" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0" xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0" xmlns:calcext="urn:org:documentfoundation:names:experimental:calc:xmlns:calcext:1.0" xmlns:svg="urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0" xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2" xmlns:chart="urn:oasis:names:tc:opendocument:xmlns:chart:1.0" xmlns:rpt="http://openoffice.org/2005/report" xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0" xmlns:css3t="http://www.w3.org/TR/css3-text/" xmlns:number="urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0" xmlns:ooow="http://openoffice.org/2004/writer" xmlns:oooc="http://openoffice.org/2004/calc" xmlns:tableooo="http://openoffice.org/2009/table" xmlns:drawooo="http://openoffice.org/2010/draw" office:version="1.2" office:mimetype="application/vnd.oasis.opendocument.text">
+<office:document xmlns:css3t="http://www.w3.org/TR/css3-text/" xmlns:grddl="http://www.w3.org/2003/g/data-view#" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xforms="http://www.w3.org/2002/xforms" xmlns:dom="http://www.w3.org/2001/xml-events" xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0" xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0" xmlns:math="http://www.w3.org/1998/Math/MathML" xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0" xmlns:ooo="http://openoffice.org/2004/office" xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0" xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0" xmlns:ooow="http://openoffice.org/2004/writer" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:drawooo="http://openoffice.org/2010/draw" xmlns:oooc="http://openoffice.org/2004/calc" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:calcext="urn:org:documentfoundation:names:experimental:calc:xmlns:calcext:1.0" xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0" xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0" xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2" xmlns:tableooo="http://openoffice.org/2009/table" xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0" xmlns:dr3d="urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0" xmlns:rpt="http://openoffice.org/2005/report" xmlns:formx="urn:openoffice:names:experimental:ooxml-odf-interop:xmlns:form:1.0" xmlns:svg="urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0" xmlns:chart="urn:oasis:names:tc:opendocument:xmlns:chart:1.0" xmlns:officeooo="http://openoffice.org/2009/office" xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0" xmlns:field="urn:openoffice:names:experimental:ooo-ms-interop:xmlns:field:1.0" xmlns:number="urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0" xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0" xmlns:loext="urn:org:documentfoundation:names:experimental:office:xmlns:loext:1.0" office:version="1.3" office:mimetype="application/vnd.oasis.opendocument.text">
   <office:meta>
-    <meta:generator>LibreOffice/6.4.6.2$Linux_X86_64 LibreOffice_project/40$Build-2</meta:generator>
+    <meta:generator>LibreOffice/7.4.4.2$Linux_X86_64 LibreOffice_project/40$Build-2</meta:generator>
     <meta:creation-date>2008-06-07T15:28:22</meta:creation-date>
     <dc:date>2009-01-10T16:03:33</dc:date>
     <meta:editing-cycles>1</meta:editing-cycles>
     <meta:editing-duration>PT0S</meta:editing-duration>
-    <meta:document-statistic meta:table-count="3" meta:image-count="0" meta:object-count="0" meta:page-count="5" meta:paragraph-count="85" meta:word-count="199" meta:character-count="2195" meta:non-whitespace-character-count="2081"/>
+    <meta:document-statistic meta:table-count="3" meta:image-count="0" meta:object-count="0" meta:page-count="5" meta:paragraph-count="89" meta:word-count="210" meta:character-count="2408" meta:non-whitespace-character-count="2287"/>
     <meta:user-defined meta:name="Info 1"/>
     <meta:user-defined meta:name="Info 2"/>
     <meta:user-defined meta:name="Info 3"/>
     <meta:user-defined meta:name="Info 4"/>
   </office:meta>
   <office:settings>
     <config:config-item-set config:name="ooo:view-settings">
-      <config:config-item config:name="ViewAreaTop" config:type="long">24977</config:config-item>
+      <config:config-item config:name="ViewAreaTop" config:type="long">22013</config:config-item>
       <config:config-item config:name="ViewAreaLeft" config:type="long">0</config:config-item>
-      <config:config-item config:name="ViewAreaWidth" config:type="long">26301</config:config-item>
+      <config:config-item config:name="ViewAreaWidth" config:type="long">48129</config:config-item>
       <config:config-item config:name="ViewAreaHeight" config:type="long">24026</config:config-item>
       <config:config-item config:name="ShowRedlineChanges" config:type="boolean">true</config:config-item>
       <config:config-item config:name="InBrowseMode" config:type="boolean">false</config:config-item>
       <config:config-item-map-indexed config:name="Views">
         <config:config-item-map-entry>
           <config:config-item config:name="ViewId" config:type="string">view2</config:config-item>
-          <config:config-item config:name="ViewLeft" config:type="long">4355</config:config-item>
-          <config:config-item config:name="ViewTop" config:type="long">33754</config:config-item>
+          <config:config-item config:name="ViewLeft" config:type="long">5225</config:config-item>
+          <config:config-item config:name="ViewTop" config:type="long">34452</config:config-item>
           <config:config-item config:name="VisibleLeft" config:type="long">0</config:config-item>
-          <config:config-item config:name="VisibleTop" config:type="long">24977</config:config-item>
-          <config:config-item config:name="VisibleRight" config:type="long">26300</config:config-item>
-          <config:config-item config:name="VisibleBottom" config:type="long">49001</config:config-item>
+          <config:config-item config:name="VisibleTop" config:type="long">22013</config:config-item>
+          <config:config-item config:name="VisibleRight" config:type="long">48128</config:config-item>
+          <config:config-item config:name="VisibleBottom" config:type="long">46038</config:config-item>
           <config:config-item config:name="ZoomType" config:type="short">0</config:config-item>
           <config:config-item config:name="ViewLayoutColumns" config:type="short">0</config:config-item>
           <config:config-item config:name="ViewLayoutBookMode" config:type="boolean">false</config:config-item>
           <config:config-item config:name="ZoomFactor" config:type="short">100</config:config-item>
           <config:config-item config:name="IsSelectedFrame" config:type="boolean">false</config:config-item>
+          <config:config-item config:name="KeepRatio" config:type="boolean">false</config:config-item>
+          <config:config-item config:name="HideWhitespace" config:type="boolean">false</config:config-item>
           <config:config-item config:name="AnchoredTextOverflowLegacy" config:type="boolean">false</config:config-item>
         </config:config-item-map-entry>
       </config:config-item-map-indexed>
     </config:config-item-set>
     <config:config-item-set config:name="ooo:configuration-settings">
       <config:config-item config:name="PrintProspect" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintReversed" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintSingleJobs" config:type="boolean">false</config:config-item>
       <config:config-item config:name="PrintLeftPages" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintPageBackground" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PrintTables" config:type="boolean">true</config:config-item>
       <config:config-item config:name="PrintControls" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PrintPageBackground" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PrintDrawings" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PrintBlackFonts" config:type="boolean">false</config:config-item>
       <config:config-item config:name="PrintAnnotationMode" config:type="short">0</config:config-item>
-      <config:config-item config:name="PrintGraphics" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintRightPages" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintFaxName" config:type="string"/>
-      <config:config-item config:name="PrintPaperFromSetup" config:type="boolean">false</config:config-item>
       <config:config-item config:name="PrintTextPlaceholder" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="HeaderSpacingBelowLastPara" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="ContinuousEndnotes" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ProtectFields" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ProtectBookmarks" config:type="boolean">false</config:config-item>
       <config:config-item config:name="EmptyDbFieldHidesPara" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="DisableOffPagePositioning" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="SubtractFlysAnchoredAtFlys" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PropLineSpacingShrinksFirstLine" config:type="boolean">false</config:config-item>
       <config:config-item config:name="ApplyParagraphMarkFormatToNumbering" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrintReversed" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="TabOverMargin" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="GutterAtTop" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="TreatSingleColumnBreakAsPageBreak" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="EmbedSystemFonts" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="EmbedComplexScriptFonts" config:type="boolean">true</config:config-item>
       <config:config-item config:name="EmbedAsianScriptFonts" config:type="boolean">true</config:config-item>
       <config:config-item config:name="EmbedLatinScriptFonts" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="DisableOffPagePositioning" config:type="boolean">true</config:config-item>
       <config:config-item config:name="EmbedOnlyUsedFonts" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="WordLikeWrapForAsCharFlys" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ContinuousEndnotes" config:type="boolean">false</config:config-item>
       <config:config-item config:name="EmbedFonts" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="SurroundTextWrapSmall" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="BackgroundParaOverDrawings" config:type="boolean">false</config:config-item>
       <config:config-item config:name="ClippedPictures" config:type="boolean">false</config:config-item>
       <config:config-item config:name="FloattableNomargins" config:type="boolean">false</config:config-item>
       <config:config-item config:name="UnbreakableNumberings" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="EmbedSystemFonts" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="TabOverflow" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrintTables" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintSingleJobs" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="SmallCapsPercentage66" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="CollapseEmptyCellPara" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="RsidRoot" config:type="int">204959</config:config-item>
-      <config:config-item config:name="IsLabelDocument" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrinterName" config:type="string"/>
-      <config:config-item config:name="OutlineLevelYieldsNumbering" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="UpdateFromTemplate" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintBlackFonts" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="TableRowKeep" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="IgnoreTabsAndBlanksForLineCalculation" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="EmbedComplexScriptFonts" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="HeaderSpacingBelowLastPara" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="AllowPrintJobCancel" config:type="boolean">true</config:config-item>
       <config:config-item config:name="UseOldPrinterMetrics" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="InvertBorderSpacing" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="SaveGlobalDocumentLinks" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="TabOverMargin" config:type="boolean">false</config:config-item>
       <config:config-item config:name="TabsRelativeToIndent" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="Rsid" config:type="int">1744494</config:config-item>
-      <config:config-item config:name="EmbeddedDatabaseName" config:type="string"/>
-      <config:config-item config:name="SaveThumbnail" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="PrintProspectRTL" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrintEmptyPages" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="ApplyUserData" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrintHiddenText" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="AddParaTableSpacingAtStart" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="FieldAutoUpdate" config:type="boolean">true</config:config-item>
       <config:config-item config:name="UseOldNumbering" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="AddParaTableSpacing" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="MsWordCompTrailingBlanks" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="IgnoreFirstLineIndentInNumbering" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrinterPaperFromSetup" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="CharacterCompressionType" config:type="short">0</config:config-item>
-      <config:config-item config:name="SaveVersionOnClose" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="ChartAutoUpdate" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="InvertBorderSpacing" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintPaperFromSetup" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="UpdateFromTemplate" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="CurrentDatabaseCommandType" config:type="int">0</config:config-item>
+      <config:config-item config:name="LinkUpdateMode" config:type="short">1</config:config-item>
+      <config:config-item config:name="AddParaSpacingToTableCells" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="FrameAutowidthWithMorePara" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="CurrentDatabaseCommand" config:type="string"/>
       <config:config-item config:name="PrinterIndependentLayout" config:type="string">high-resolution</config:config-item>
+      <config:config-item config:name="ApplyUserData" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintFaxName" config:type="string"/>
+      <config:config-item config:name="CurrentDatabaseDataSource" config:type="string"/>
+      <config:config-item config:name="ClipAsCharacterAnchoredWriterFlyFrames" config:type="boolean">false</config:config-item>
       <config:config-item config:name="IsKernAsianPunctuation" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="UseFormerObjectPositioning" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="TreatSingleColumnBreakAsPageBreak" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="MathBaselineAlignment" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="AddFrameOffsets" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="AddVerticalFrameOffsets" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="SubtractFlysAnchoredAtFlys" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="AddParaSpacingToTableCells" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="SaveThumbnail" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="UseFormerTextWrapping" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="AutoFirstLineIndentDisregardLineSpace" config:type="boolean">false</config:config-item>
       <config:config-item config:name="AddExternalLeading" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="CurrentDatabaseDataSource" config:type="string"/>
-      <config:config-item config:name="AllowPrintJobCancel" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="ProtectForm" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="AddParaTableSpacing" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="StylesNoDefault" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ChartAutoUpdate" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="PrinterSetup" config:type="base64Binary"/>
+      <config:config-item config:name="AddParaTableSpacingAtStart" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="Rsid" config:type="int">1753347</config:config-item>
+      <config:config-item config:name="EmbeddedDatabaseName" config:type="string"/>
+      <config:config-item config:name="FieldAutoUpdate" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="OutlineLevelYieldsNumbering" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="FootnoteInColumnToPageEnd" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="AlignTabStopPosition" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="CharacterCompressionType" config:type="short">0</config:config-item>
+      <config:config-item config:name="PrinterName" config:type="string"/>
+      <config:config-item config:name="SaveGlobalDocumentLinks" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrinterPaperFromSetup" config:type="boolean">false</config:config-item>
       <config:config-item config:name="UseFormerLineSpacing" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="PrintDrawings" config:type="boolean">true</config:config-item>
-      <config:config-item config:name="UseFormerTextWrapping" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="UnxForceZeroExtLeading" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="AddParaLineSpacingToTableCells" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="UseFormerObjectPositioning" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintGraphics" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="ImagePreferredDPI" config:type="int">0</config:config-item>
+      <config:config-item config:name="SurroundTextWrapSmall" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ConsiderTextWrapOnObjPos" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="MsWordCompTrailingBlanks" config:type="boolean">false</config:config-item>
       <config:config-item config:name="TabAtLeftIndentForParagraphsInList" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintRightPages" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="TabOverSpacing" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="IgnoreFirstLineIndentInNumbering" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="NoNumberingShowFollowBy" config:type="boolean">false</config:config-item>
       <config:config-item config:name="RedlineProtectionKey" config:type="base64Binary"/>
-      <config:config-item config:name="PropLineSpacingShrinksFirstLine" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="ConsiderTextWrapOnObjPos" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="StylesNoDefault" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="LinkUpdateMode" config:type="short">1</config:config-item>
-      <config:config-item config:name="AlignTabStopPosition" config:type="boolean">true</config:config-item>
       <config:config-item config:name="DoNotJustifyLinesWithManualBreak" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintProspectRTL" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="PrintEmptyPages" config:type="boolean">true</config:config-item>
       <config:config-item config:name="DoNotResetParaAttrsForNumFont" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="CurrentDatabaseCommandType" config:type="int">0</config:config-item>
+      <config:config-item config:name="AddFrameOffsets" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="IgnoreTabsAndBlanksForLineCalculation" config:type="boolean">false</config:config-item>
       <config:config-item config:name="LoadReadonly" config:type="boolean">false</config:config-item>
       <config:config-item config:name="DoNotCaptureDrawObjsOnPage" config:type="boolean">false</config:config-item>
-      <config:config-item config:name="CurrentDatabaseCommand" config:type="string"/>
-      <config:config-item config:name="PrinterSetup" config:type="base64Binary"/>
-      <config:config-item config:name="ClipAsCharacterAnchoredWriterFlyFrames" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="AddVerticalFrameOffsets" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="UnxForceZeroExtLeading" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="IsLabelDocument" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="TableRowKeep" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="RsidRoot" config:type="int">204959</config:config-item>
+      <config:config-item config:name="PrintHiddenText" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="ProtectForm" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="MsWordCompMinLineHeightByFly" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="BackgroundParaOverDrawings" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="SaveVersionOnClose" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="MathBaselineAlignment" config:type="boolean">false</config:config-item>
+      <config:config-item config:name="SmallCapsPercentage66" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="CollapseEmptyCellPara" config:type="boolean">true</config:config-item>
+      <config:config-item config:name="TabOverflow" config:type="boolean">false</config:config-item>
     </config:config-item-set>
   </office:settings>
   <office:scripts>
     <office:script script:language="ooo:Basic">
       <ooo:libraries xmlns:ooo="http://openoffice.org/2004/office" xmlns:xlink="http://www.w3.org/1999/xlink"/>
     </office:script>
   </office:scripts>
   <office:font-face-decls>
-    <style:font-face style:name="StarSymbol" svg:font-family="StarSymbol"/>
-    <style:font-face style:name="Liberation Serif2" svg:font-family="'Liberation Serif'" style:font-family-generic="roman" style:font-pitch="variable"/>
-    <style:font-face style:name="Liberation Serif1" svg:font-family="'Liberation Serif'" style:font-adornments="Bold" style:font-family-generic="roman" style:font-pitch="variable"/>
-    <style:font-face style:name="Liberation Serif" svg:font-family="'Liberation Serif'" style:font-adornments="Regular" style:font-family-generic="roman" style:font-pitch="variable"/>
-    <style:font-face style:name="Thorndale AMT" svg:font-family="'Thorndale AMT'" style:font-family-generic="roman" style:font-pitch="variable"/>
-    <style:font-face style:name="Liberation Sans" svg:font-family="'Liberation Sans'" style:font-adornments="Regular" style:font-family-generic="swiss" style:font-pitch="variable"/>
     <style:font-face style:name="Andale Sans UI" svg:font-family="'Andale Sans UI'" style:font-family-generic="system" style:font-pitch="variable"/>
     <style:font-face style:name="DejaVu Sans" svg:font-family="'DejaVu Sans'" style:font-family-generic="system" style:font-pitch="variable"/>
+    <style:font-face style:name="Liberation Sans" svg:font-family="'Liberation Sans'" style:font-adornments="Regular" style:font-family-generic="swiss" style:font-pitch="variable"/>
+    <style:font-face style:name="Liberation Serif" svg:font-family="'Liberation Serif'" style:font-family-generic="roman" style:font-pitch="variable"/>
+    <style:font-face style:name="Liberation Serif1" svg:font-family="'Liberation Serif'" style:font-adornments="Bold" style:font-family-generic="roman" style:font-pitch="variable"/>
+    <style:font-face style:name="Liberation Serif2" svg:font-family="'Liberation Serif'" style:font-adornments="Regular" style:font-family-generic="roman" style:font-pitch="variable"/>
+    <style:font-face style:name="StarSymbol" svg:font-family="StarSymbol"/>
+    <style:font-face style:name="Thorndale AMT" svg:font-family="'Thorndale AMT'" style:font-family-generic="roman" style:font-pitch="variable"/>
   </office:font-face-decls>
   <office:styles>
+    <draw:gradient draw:name="gradient" draw:style="linear" draw:start-color="#000000" draw:end-color="#ffffff" draw:start-intensity="100%" draw:end-intensity="100%" draw:angle="0deg" draw:border="0%"/>
+    <draw:hatch draw:name="hatch" draw:style="single" draw:color="#3465a4" draw:distance="0.02cm" draw:rotation="0"/>
     <style:default-style style:family="graphic">
       <style:graphic-properties svg:stroke-color="#000000" draw:fill-color="#99ccff" fo:wrap-option="no-wrap" draw:shadow-offset-x="0.3cm" draw:shadow-offset-y="0.3cm" draw:start-line-spacing-horizontal="0.283cm" draw:start-line-spacing-vertical="0.283cm" draw:end-line-spacing-horizontal="0.283cm" draw:end-line-spacing-vertical="0.283cm" style:flow-with-text="false"/>
-      <style:paragraph-properties style:text-autospace="ideograph-alpha" style:line-break="strict" style:writing-mode="lr-tb" style:font-independent-line-spacing="false">
+      <style:paragraph-properties style:text-autospace="ideograph-alpha" style:line-break="strict" style:font-independent-line-spacing="false">
         <style:tab-stops/>
       </style:paragraph-properties>
-      <style:text-properties style:use-window-font-color="true" style:font-name="Thorndale AMT" fo:font-size="12pt" fo:language="en" fo:country="US" style:letter-kerning="true" style:font-name-asian="Andale Sans UI" style:font-size-asian="10.5pt" style:language-asian="zxx" style:country-asian="none" style:font-name-complex="Andale Sans UI" style:font-size-complex="12pt" style:language-complex="zxx" style:country-complex="none"/>
+      <style:text-properties style:use-window-font-color="true" loext:opacity="0%" loext:color-lum-mod="100%" loext:color-lum-off="0%" style:font-name="Thorndale AMT" fo:font-size="12pt" fo:language="en" fo:country="US" style:letter-kerning="true" style:font-name-asian="Andale Sans UI" style:font-size-asian="10.5pt" style:language-asian="zxx" style:country-asian="none" style:font-name-complex="Andale Sans UI" style:font-size-complex="12pt" style:language-complex="zxx" style:country-complex="none"/>
     </style:default-style>
     <style:default-style style:family="paragraph">
       <style:paragraph-properties fo:hyphenation-ladder-count="no-limit" style:text-autospace="ideograph-alpha" style:punctuation-wrap="hanging" style:line-break="strict" style:tab-stop-distance="1.251cm" style:writing-mode="lr-tb"/>
-      <style:text-properties style:use-window-font-color="true" style:font-name="Thorndale AMT" fo:font-size="12pt" fo:language="en" fo:country="US" style:letter-kerning="true" style:font-name-asian="Andale Sans UI" style:font-size-asian="10.5pt" style:language-asian="zxx" style:country-asian="none" style:font-name-complex="Andale Sans UI" style:font-size-complex="12pt" style:language-complex="zxx" style:country-complex="none" fo:hyphenate="false" fo:hyphenation-remain-char-count="2" fo:hyphenation-push-char-count="2" loext:hyphenation-no-caps="false"/>
+      <style:text-properties style:use-window-font-color="true" loext:opacity="0%" style:font-name="Thorndale AMT" fo:font-size="12pt" fo:language="en" fo:country="US" style:letter-kerning="true" style:font-name-asian="Andale Sans UI" style:font-size-asian="10.5pt" style:language-asian="zxx" style:country-asian="none" style:font-name-complex="Andale Sans UI" style:font-size-complex="12pt" style:language-complex="zxx" style:country-complex="none" fo:hyphenate="false" fo:hyphenation-remain-char-count="2" fo:hyphenation-push-char-count="2" loext:hyphenation-no-caps="false" loext:hyphenation-no-last-word="false" loext:hyphenation-word-char-count="5" loext:hyphenation-zone="no-limit"/>
     </style:default-style>
     <style:default-style style:family="table">
       <style:table-properties table:border-model="collapsing"/>
     </style:default-style>
     <style:default-style style:family="table-row">
       <style:table-row-properties fo:keep-together="auto"/>
     </style:default-style>
     <style:style style:name="Standard" style:family="paragraph" style:class="text">
       <style:text-properties style:font-name="Liberation Sans" fo:font-family="'Liberation Sans'" style:font-style-name="Regular" style:font-family-generic="swiss" style:font-pitch="variable" style:font-size-asian="10.5pt"/>
     </style:style>
     <style:style style:name="Heading" style:family="paragraph" style:parent-style-name="Standard" style:next-style-name="Text_20_body" style:class="text">
-      <style:paragraph-properties fo:margin-top="0.423cm" fo:margin-bottom="0.212cm" loext:contextual-spacing="false" fo:keep-with-next="always"/>
-      <style:text-properties style:font-name="Liberation Serif" fo:font-family="'Liberation Serif'" style:font-style-name="Regular" style:font-family-generic="roman" style:font-pitch="variable" fo:font-size="16pt" style:font-name-asian="DejaVu Sans" style:font-family-asian="'DejaVu Sans'" style:font-family-generic-asian="system" style:font-pitch-asian="variable" style:font-size-asian="14pt" style:font-name-complex="DejaVu Sans" style:font-family-complex="'DejaVu Sans'" style:font-family-generic-complex="system" style:font-pitch-complex="variable" style:font-size-complex="14pt"/>
+      <style:paragraph-properties fo:margin-top="0.423cm" fo:margin-bottom="0.212cm" style:contextual-spacing="false" fo:keep-with-next="always"/>
+      <style:text-properties style:font-name="Liberation Serif2" fo:font-family="'Liberation Serif'" style:font-style-name="Regular" style:font-family-generic="roman" style:font-pitch="variable" fo:font-size="16pt" style:font-name-asian="DejaVu Sans" style:font-family-asian="'DejaVu Sans'" style:font-family-generic-asian="system" style:font-pitch-asian="variable" style:font-size-asian="14pt" style:font-name-complex="DejaVu Sans" style:font-family-complex="'DejaVu Sans'" style:font-family-generic-complex="system" style:font-pitch-complex="variable" style:font-size-complex="14pt"/>
     </style:style>
     <style:style style:name="Text_20_body" style:display-name="Text body" style:family="paragraph" style:parent-style-name="Standard" style:class="text">
-      <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0.212cm" loext:contextual-spacing="false"/>
+      <style:paragraph-properties fo:margin-top="0cm" fo:margin-bottom="0.212cm" style:contextual-spacing="false"/>
       <style:text-properties style:font-name="Liberation Sans" fo:font-family="'Liberation Sans'" style:font-style-name="Regular" style:font-family-generic="swiss" style:font-pitch="variable" style:font-size-asian="10.5pt"/>
     </style:style>
     <style:style style:name="List" style:family="paragraph" style:parent-style-name="Text_20_body" style:class="list">
       <style:text-properties style:font-size-asian="12pt"/>
     </style:style>
     <style:style style:name="Caption" style:family="paragraph" style:parent-style-name="Standard" style:class="extra">
-      <style:paragraph-properties fo:margin-top="0.212cm" fo:margin-bottom="0.212cm" loext:contextual-spacing="false" text:number-lines="false" text:line-number="0"/>
+      <style:paragraph-properties fo:margin-top="0.212cm" fo:margin-bottom="0.212cm" style:contextual-spacing="false" text:number-lines="false" text:line-number="0"/>
       <style:text-properties fo:font-size="12pt" fo:font-style="italic" style:font-size-asian="12pt" style:font-style-asian="italic" style:font-size-complex="12pt" style:font-style-complex="italic"/>
     </style:style>
     <style:style style:name="Index" style:family="paragraph" style:parent-style-name="Standard" style:class="index">
       <style:paragraph-properties text:number-lines="false" text:line-number="0"/>
       <style:text-properties style:font-size-asian="12pt"/>
     </style:style>
     <style:style style:name="Heading_20_1" style:display-name="Heading 1" style:family="paragraph" style:parent-style-name="Heading" style:next-style-name="Text_20_body" style:class="text">
@@ -234,59 +250,59 @@
       <style:text-properties fo:font-size="14pt" fo:font-weight="bold" style:font-size-asian="14pt" style:font-weight-asian="bold" style:font-size-complex="14pt" style:font-weight-complex="bold"/>
     </style:style>
     <style:style style:name="Text_20_body_20_indent" style:display-name="Text body indent" style:family="paragraph" style:parent-style-name="Text_20_body" style:class="text">
       <style:paragraph-properties fo:margin-left="0.499cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
     </style:style>
     <style:style style:name="Text" style:family="paragraph" style:parent-style-name="Caption" style:class="extra"/>
     <style:style style:name="Quotations" style:family="paragraph" style:parent-style-name="Standard" style:class="html">
-      <style:paragraph-properties fo:margin-left="1cm" fo:margin-right="1cm" fo:margin-top="0cm" fo:margin-bottom="0.499cm" loext:contextual-spacing="false" fo:text-indent="0cm" style:auto-text-indent="false"/>
+      <style:paragraph-properties fo:margin-left="1cm" fo:margin-right="1cm" fo:margin-top="0cm" fo:margin-bottom="0.499cm" style:contextual-spacing="false" fo:text-indent="0cm" style:auto-text-indent="false"/>
     </style:style>
     <style:style style:name="Title" style:family="paragraph" style:parent-style-name="Heading" style:next-style-name="Text_20_body" style:class="chapter">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties fo:font-size="28pt" fo:font-weight="bold" style:font-size-asian="28pt" style:font-weight-asian="bold" style:font-size-complex="28pt" style:font-weight-complex="bold"/>
     </style:style>
     <style:style style:name="Subtitle" style:family="paragraph" style:parent-style-name="Heading" style:next-style-name="Text_20_body" style:class="chapter">
-      <style:paragraph-properties fo:margin-top="0.106cm" fo:margin-bottom="0.212cm" loext:contextual-spacing="false" fo:text-align="center" style:justify-single-word="false"/>
+      <style:paragraph-properties fo:margin-top="0.106cm" fo:margin-bottom="0.212cm" style:contextual-spacing="false" fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties fo:font-size="18pt" style:font-size-asian="18pt" style:font-size-complex="18pt"/>
     </style:style>
     <style:style style:name="Placeholder" style:family="text">
-      <style:text-properties fo:font-variant="small-caps" fo:color="#008080" style:text-underline-style="dotted" style:text-underline-width="auto" style:text-underline-color="font-color"/>
+      <style:text-properties fo:font-variant="small-caps" fo:color="#008080" loext:opacity="100%" style:text-underline-style="dotted" style:text-underline-width="auto" style:text-underline-color="font-color"/>
     </style:style>
     <style:style style:name="Bullet_20_Symbols" style:display-name="Bullet Symbols" style:family="text">
       <style:text-properties style:font-name="StarSymbol" fo:font-family="StarSymbol" fo:font-size="9pt" style:font-name-asian="StarSymbol" style:font-family-asian="StarSymbol" style:font-size-asian="9pt" style:font-name-complex="StarSymbol" style:font-family-complex="StarSymbol" style:font-size-complex="9pt"/>
     </style:style>
     <text:outline-style style:name="Outline">
-      <text:outline-level-style text:level="1" style:num-format="">
+      <text:outline-level-style text:level="1" loext:num-list-format="%1%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="2" style:num-format="">
+      <text:outline-level-style text:level="2" loext:num-list-format="%2%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="3" style:num-format="">
+      <text:outline-level-style text:level="3" loext:num-list-format="%3%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="4" style:num-format="">
+      <text:outline-level-style text:level="4" loext:num-list-format="%4%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="5" style:num-format="">
+      <text:outline-level-style text:level="5" loext:num-list-format="%5%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="6" style:num-format="">
+      <text:outline-level-style text:level="6" loext:num-list-format="%6%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="7" style:num-format="">
+      <text:outline-level-style text:level="7" loext:num-list-format="%7%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="8" style:num-format="">
+      <text:outline-level-style text:level="8" loext:num-list-format="%8%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="9" style:num-format="">
+      <text:outline-level-style text:level="9" loext:num-list-format="%9%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
-      <text:outline-level-style text:level="10" style:num-format="">
+      <text:outline-level-style text:level="10" loext:num-list-format="%10%" style:num-format="">
         <style:list-level-properties text:min-label-distance="0.381cm"/>
       </text:outline-level-style>
     </text:outline-style>
     <text:notes-configuration text:note-class="footnote" style:num-format="1" text:start-value="0" text:footnotes-position="page" text:start-numbering-at="document"/>
     <text:notes-configuration text:note-class="endnote" style:num-format="i" text:start-value="0"/>
     <text:linenumbering-configuration text:number-lines="false" text:offset="0.499cm" style:num-format="1" text:number-position="left" text:increment="5"/>
   </office:styles>
@@ -408,14 +424,42 @@
     </style:style>
     <style:style style:name="Table4.B2" style:family="table-cell">
       <style:table-cell-properties fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="0.05pt solid #000000" fo:border-top="none" fo:border-bottom="0.05pt solid #000000"/>
     </style:style>
     <style:style style:name="Table4.B3" style:family="table-cell">
       <style:table-cell-properties fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="0.05pt solid #000000" fo:border-top="none" fo:border-bottom="0.05pt solid #000000"/>
     </style:style>
+    <style:style style:name="Table4" style:family="table">
+      <style:table-properties style:width="7.969cm" table:align="right" style:may-break-between-rows="true"/>
+    </style:style>
+    <style:style style:name="Table4.A" style:family="table-column">
+      <style:table-column-properties style:column-width="5.308cm"/>
+    </style:style>
+    <style:style style:name="Table4.B" style:family="table-column">
+      <style:table-column-properties style:column-width="2.662cm"/>
+    </style:style>
+    <style:style style:name="Table4.A1" style:family="table-cell">
+      <style:table-cell-properties fo:background-color="#cccccc" fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="none" fo:border-top="0.05pt solid #000000" fo:border-bottom="0.05pt solid #000000">
+        <style:background-image/>
+      </style:table-cell-properties>
+    </style:style>
+    <style:style style:name="Table4.B1" style:family="table-cell">
+      <style:table-cell-properties fo:padding="0.097cm" fo:border="0.05pt solid #000000"/>
+    </style:style>
+    <style:style style:name="Table4.A2" style:family="table-cell">
+      <style:table-cell-properties fo:background-color="#cccccc" fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="none" fo:border-top="none" fo:border-bottom="0.05pt solid #000000">
+        <style:background-image/>
+      </style:table-cell-properties>
+    </style:style>
+    <style:style style:name="Table4.B2" style:family="table-cell">
+      <style:table-cell-properties fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="0.05pt solid #000000" fo:border-top="none" fo:border-bottom="0.05pt solid #000000"/>
+    </style:style>
+    <style:style style:name="Table4.B3" style:family="table-cell">
+      <style:table-cell-properties fo:padding="0.097cm" fo:border-left="0.05pt solid #000000" fo:border-right="0.05pt solid #000000" fo:border-top="none" fo:border-bottom="0.05pt solid #000000"/>
+    </style:style>
     <style:style style:name="P1" style:family="paragraph" style:parent-style-name="Header">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties officeooo:paragraph-rsid="00066dfa"/>
     </style:style>
     <style:style style:name="P2" style:family="paragraph" style:parent-style-name="Footer">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties officeooo:paragraph-rsid="00066dfa"/>
@@ -424,104 +468,142 @@
       <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
       <style:text-properties fo:font-size="12pt" officeooo:paragraph-rsid="00066dfa" style:font-size-asian="12pt" style:font-size-complex="12pt"/>
     </style:style>
     <style:style style:name="P4" style:family="paragraph" style:parent-style-name="Header">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties officeooo:paragraph-rsid="00066dfa"/>
     </style:style>
-    <style:style style:name="P5" style:family="paragraph" style:parent-style-name="Header">
-      <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
-      <style:text-properties fo:font-size="12pt" officeooo:paragraph-rsid="00066dfa" style:font-size-asian="12pt" style:font-size-complex="12pt"/>
-    </style:style>
-    <style:style style:name="P6" style:family="paragraph" style:parent-style-name="Footer">
+    <style:style style:name="P5" style:family="paragraph" style:parent-style-name="Footer">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties officeooo:paragraph-rsid="00066dfa"/>
     </style:style>
-    <style:style style:name="P7" style:family="paragraph" style:parent-style-name="Standard">
-      <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
+    <style:style style:name="P6" style:family="paragraph" style:parent-style-name="Table_20_Contents">
+      <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
+    </style:style>
+    <style:style style:name="P7" style:family="paragraph" style:parent-style-name="Header">
+      <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
+      <style:text-properties fo:font-size="12pt" officeooo:paragraph-rsid="00066dfa" style:font-size-asian="12pt" style:font-size-complex="12pt"/>
     </style:style>
     <style:style style:name="P8" style:family="paragraph" style:parent-style-name="Standard">
       <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
-      <style:text-properties officeooo:paragraph-rsid="0011a01d"/>
     </style:style>
-    <style:style style:name="P9" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
-      <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" style:page-number="auto" fo:break-before="page"/>
-      <style:text-properties officeooo:paragraph-rsid="000ce218"/>
+    <style:style style:name="P9" style:family="paragraph" style:parent-style-name="Standard">
+      <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
+      <style:text-properties officeooo:paragraph-rsid="0011a01d"/>
     </style:style>
     <style:style style:name="P10" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
       <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" style:page-number="auto" fo:break-before="page"/>
       <style:text-properties officeooo:paragraph-rsid="0011a01d"/>
     </style:style>
-    <style:style style:name="P11" style:family="paragraph" style:parent-style-name="Table_20_Heading">
-      <style:paragraph-properties fo:text-align="end" style:justify-single-word="false"/>
+    <style:style style:name="P11" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
+      <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" style:page-number="auto" fo:break-before="page"/>
+      <style:text-properties officeooo:paragraph-rsid="000ce218"/>
     </style:style>
-    <style:style style:name="P12" style:family="paragraph" style:parent-style-name="Table_20_Contents">
+    <style:style style:name="P12" style:family="paragraph" style:parent-style-name="Table_20_Heading">
       <style:paragraph-properties fo:text-align="end" style:justify-single-word="false"/>
     </style:style>
     <style:style style:name="P13" style:family="paragraph" style:parent-style-name="Table_20_Contents">
       <style:paragraph-properties fo:text-align="end" style:justify-single-word="false"/>
-      <style:text-properties officeooo:paragraph-rsid="0008048e"/>
     </style:style>
     <style:style style:name="P14" style:family="paragraph" style:parent-style-name="Table_20_Contents">
-      <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
+      <style:paragraph-properties fo:text-align="end" style:justify-single-word="false"/>
+      <style:text-properties officeooo:paragraph-rsid="0008048e"/>
     </style:style>
     <style:style style:name="P15" style:family="paragraph" style:parent-style-name="Text_20_body">
       <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
     </style:style>
-    <style:style style:name="P16" style:family="paragraph" style:parent-style-name="Text_20_body">
+    <style:style style:name="P16" style:family="paragraph" style:parent-style-name="Heading_20_2">
       <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
-      <style:text-properties style:text-underline-style="none"/>
     </style:style>
     <style:style style:name="P17" style:family="paragraph" style:parent-style-name="Text_20_body">
+      <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
+      <style:text-properties style:text-underline-style="none"/>
+    </style:style>
+    <style:style style:name="P18" style:family="paragraph" style:parent-style-name="Text_20_body">
       <style:text-properties officeooo:rsid="0007edf0" officeooo:paragraph-rsid="0007edf0"/>
     </style:style>
-    <style:style style:name="P18" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
+    <style:style style:name="P19" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
       <style:paragraph-properties style:page-number="auto" fo:break-before="auto" fo:break-after="auto"/>
     </style:style>
-    <style:style style:name="P19" style:family="paragraph" style:parent-style-name="Standard">
+    <style:style style:name="P20" style:family="paragraph" style:parent-style-name="Standard">
       <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
-      <style:text-properties style:font-name="Liberation Serif2"/>
+      <style:text-properties style:font-name="Liberation Serif"/>
     </style:style>
-    <style:style style:name="P20" style:family="paragraph" style:parent-style-name="Standard">
+    <style:style style:name="P21" style:family="paragraph" style:parent-style-name="Standard">
       <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:text-align="start" style:justify-single-word="false" fo:text-indent="0cm" style:auto-text-indent="false"/>
-      <style:text-properties style:font-name="Liberation Serif2"/>
+      <style:text-properties style:font-name="Liberation Serif"/>
     </style:style>
-    <style:style style:name="P21" style:family="paragraph" style:parent-style-name="Standard">
+    <style:style style:name="P22" style:family="paragraph" style:parent-style-name="Standard">
       <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
-      <style:text-properties style:font-name="Liberation Serif2" officeooo:paragraph-rsid="0014b27d"/>
+      <style:text-properties style:font-name="Liberation Serif" officeooo:paragraph-rsid="0014b27d"/>
     </style:style>
-    <style:style style:name="P22" style:family="paragraph" style:parent-style-name="Heading_20_1">
+    <style:style style:name="P23" style:family="paragraph" style:parent-style-name="Heading_20_1">
       <style:paragraph-properties fo:text-align="center" style:justify-single-word="false"/>
       <style:text-properties style:text-underline-style="solid" style:text-underline-width="auto" style:text-underline-color="font-color"/>
     </style:style>
-    <style:style style:name="P23" style:family="paragraph" style:parent-style-name="Heading_20_2">
+    <style:style style:name="P24" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
+      <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" style:page-number="auto" fo:break-before="page"/>
+      <style:text-properties fo:font-size="6pt" officeooo:paragraph-rsid="0011a01d" style:font-size-asian="5.25pt" style:font-size-complex="6pt"/>
+    </style:style>
+    <style:style style:name="P25" style:family="paragraph" style:parent-style-name="Text_20_body" style:master-page-name="">
+      <loext:graphic-properties draw:fill-gradient-name="gradient" draw:fill-hatch-name="hatch"/>
+      <style:paragraph-properties style:page-number="auto" fo:keep-with-next="auto"/>
+      <style:text-properties officeooo:paragraph-rsid="001ac103"/>
+    </style:style>
+    <style:style style:name="P26" style:family="paragraph" style:parent-style-name="Text_20_body" style:master-page-name="">
+      <loext:graphic-properties draw:fill-gradient-name="gradient" draw:fill-hatch-name="hatch"/>
+      <style:paragraph-properties style:page-number="auto" fo:break-before="column" fo:keep-with-next="auto"/>
+      <style:text-properties officeooo:paragraph-rsid="001ac103"/>
+    </style:style>
+    <style:style style:name="P27" style:family="paragraph" style:parent-style-name="Text_20_body">
+      <loext:graphic-properties draw:fill-gradient-name="gradient" draw:fill-hatch-name="hatch"/>
+      <style:paragraph-properties fo:margin-left="1cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" fo:keep-with-next="auto"/>
+      <style:text-properties officeooo:rsid="001ac103" officeooo:paragraph-rsid="001ac103"/>
+    </style:style>
+    <style:style style:name="P28" style:family="paragraph" style:parent-style-name="Text_20_body">
       <style:paragraph-properties fo:text-align="start" style:justify-single-word="false"/>
+      <style:text-properties style:text-underline-style="none" officeooo:paragraph-rsid="001ac103"/>
     </style:style>
-    <style:style style:name="P24" style:family="paragraph" style:parent-style-name="Standard">
-      <style:paragraph-properties fo:margin-left="11.28cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false"/>
-      <style:text-properties officeooo:paragraph-rsid="0011a01d"/>
+    <style:style style:name="P29" style:family="paragraph" style:parent-style-name="Text_20_body" style:master-page-name="">
+      <loext:graphic-properties draw:fill-gradient-name="gradient" draw:fill-hatch-name="hatch"/>
+      <style:paragraph-properties style:page-number="auto" fo:keep-with-next="always"/>
+    </style:style>
+    <style:style style:name="P30" style:family="paragraph" style:parent-style-name="Text_20_body" style:master-page-name="">
+      <loext:graphic-properties draw:fill-gradient-name="gradient" draw:fill-hatch-name="hatch"/>
+      <style:paragraph-properties style:page-number="auto" fo:keep-with-next="auto"/>
+      <style:text-properties officeooo:rsid="0007edf0" officeooo:paragraph-rsid="0007edf0"/>
     </style:style>
-    <style:style style:name="P25" style:family="paragraph" style:parent-style-name="Standard" style:master-page-name="">
-      <style:paragraph-properties fo:margin-left="0cm" fo:margin-right="0cm" fo:text-indent="0cm" style:auto-text-indent="false" style:page-number="auto" fo:break-before="page"/>
-      <style:text-properties fo:font-size="6pt" officeooo:paragraph-rsid="0011a01d" style:font-size-asian="5.25pt" style:font-size-complex="6pt"/>
+    <style:style style:name="T1" style:family="text">
+      <style:text-properties officeooo:rsid="001ac103"/>
+    </style:style>
+    <style:style style:name="Sect1" style:family="section">
+      <style:section-properties text:dont-balance-text-columns="true" style:editable="false">
+        <style:columns fo:column-count="2" fo:column-gap="0cm">
+          <style:column style:rel-width="32767*" fo:start-indent="0cm" fo:end-indent="0cm"/>
+          <style:column style:rel-width="32768*" fo:start-indent="0cm" fo:end-indent="0cm"/>
+        </style:columns>
+      </style:section-properties>
     </style:style>
     <style:page-layout style:name="pm1">
-      <style:page-layout-properties fo:page-width="21.59cm" fo:page-height="27.94cm" style:num-format="1" style:print-orientation="portrait" fo:margin-top="2cm" fo:margin-bottom="2cm" fo:margin-left="2cm" fo:margin-right="2cm" style:writing-mode="lr-tb" style:layout-grid-color="#c0c0c0" style:layout-grid-lines="44" style:layout-grid-base-height="0.55cm" style:layout-grid-ruby-height="0cm" style:layout-grid-mode="none" style:layout-grid-ruby-below="false" style:layout-grid-print="true" style:layout-grid-display="true" style:footnote-max-height="0cm">
+      <style:page-layout-properties fo:page-width="21.59cm" fo:page-height="27.94cm" style:num-format="1" style:print-orientation="portrait" fo:margin-top="2cm" fo:margin-bottom="2cm" fo:margin-left="2cm" fo:margin-right="2cm" style:writing-mode="lr-tb" style:layout-grid-color="#c0c0c0" style:layout-grid-lines="44" style:layout-grid-base-height="0.55cm" style:layout-grid-ruby-height="0cm" style:layout-grid-mode="none" style:layout-grid-ruby-below="false" style:layout-grid-print="true" style:layout-grid-display="true" style:footnote-max-height="0cm" loext:margin-gutter="0cm">
         <style:footnote-sep style:width="0.018cm" style:distance-before-sep="0.101cm" style:distance-after-sep="0.101cm" style:line-style="none" style:adjustment="left" style:rel-width="25%" style:color="#000000"/>
       </style:page-layout-properties>
       <style:header-style>
         <style:header-footer-properties fo:min-height="0cm" fo:margin-left="0cm" fo:margin-right="0cm" fo:margin-bottom="0.499cm"/>
       </style:header-style>
       <style:footer-style>
         <style:header-footer-properties fo:min-height="0cm" fo:margin-left="0cm" fo:margin-right="0cm" fo:margin-top="0.499cm"/>
       </style:footer-style>
     </style:page-layout>
+    <style:style style:name="dp1" style:family="drawing-page">
+      <style:drawing-page-properties draw:background-size="full"/>
+    </style:style>
   </office:automatic-styles>
   <office:master-styles>
-    <style:master-page style:name="Standard" style:page-layout-name="pm1">
+    <style:master-page style:name="Standard" style:page-layout-name="pm1" draw:style-name="dp1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
@@ -563,89 +645,104 @@
       <text:sequence-decls>
         <text:sequence-decl text:display-outline-level="0" text:name="Illustration"/>
         <text:sequence-decl text:display-outline-level="0" text:name="Table"/>
         <text:sequence-decl text:display-outline-level="0" text:name="Text"/>
         <text:sequence-decl text:display-outline-level="0" text:name="Drawing"/>
         <text:sequence-decl text:display-outline-level="0" text:name="Figure"/>
       </text:sequence-decls>
-      <text:p text:style-name="P18">
+      <text:p text:style-name="P19">
         <text:placeholder text:placeholder-type="text">&lt;for each=&quot;sale in records&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P25"/>
-      <text:p text:style-name="P8">
+      <text:p text:style-name="P24"/>
+      <text:p text:style-name="P9">
         <text:placeholder text:placeholder-type="text">&lt;replace text:p=&quot;set_lang(sale.party.lang)&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P8">
+      <text:p text:style-name="P9">
         <text:placeholder text:placeholder-type="text">&lt;replace text:p=&quot;sale.set_lang(sale.party.lang)&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in sale.report_address.splitlines()&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;if test=&quot;sale.party.tax_identifier&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;sale.party.tax_identifier.type_string&gt;</text:placeholder>
         :
         <text:placeholder text:placeholder-type="text">&lt;sale.party.tax_identifier.code&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P7">
+      <text:p text:style-name="P8">
         <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
       </text:p>
       <text:p text:style-name="P15">
         <text:placeholder text:placeholder-type="text">&lt;choose test=&quot;&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;when test=&quot;sale.state == 'draft'&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P22">Draft Sale Order</text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P23">Draft Sale Order</text:p>
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;when test=&quot;sale.state == 'quotation'&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P22">
+      <text:p text:style-name="P23">
         Quotation N°:
         <text:placeholder text:placeholder-type="text">&lt;sale.full_number&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;otherwise test=&quot;&quot;&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P22">
+      <text:p text:style-name="P23">
         Sale Order N°:
         <text:placeholder text:placeholder-type="text">&lt;sale.full_number&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P17">
         <text:placeholder text:placeholder-type="text">&lt;/otherwise&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="P16">
+      <text:p text:style-name="P28">
         <text:placeholder text:placeholder-type="text">&lt;/choose&gt;</text:placeholder>
       </text:p>
-      <text:p text:style-name="Text_20_body">
-        Description:
-        <text:placeholder text:placeholder-type="text">&lt;sale.description or ''&gt;</text:placeholder>
-      </text:p>
-      <text:p text:style-name="P17">
-        Reference:
-        <text:placeholder text:placeholder-type="text">&lt;sale.reference or ''&gt;</text:placeholder>
-      </text:p>
-      <text:p text:style-name="Text_20_body">
-        Date:
-        <text:placeholder text:placeholder-type="text">&lt;format_date(sale.sale_date or today, sale.party.lang)&gt;</text:placeholder>
-      </text:p>
+      <text:section text:style-name="Sect1" text:name="Section1">
+        <text:p text:style-name="P29">
+          Description:
+          <text:placeholder text:placeholder-type="text">&lt;sale.description or ''&gt;</text:placeholder>
+        </text:p>
+        <text:p text:style-name="P30">
+          Reference:
+          <text:placeholder text:placeholder-type="text">&lt;sale.reference or ''&gt;</text:placeholder>
+        </text:p>
+        <text:p text:style-name="P25">
+          Date:
+          <text:placeholder text:placeholder-type="text">&lt;format_date(sale.sale_date or today, sale.party.lang)&gt;</text:placeholder>
+        </text:p>
+        <text:p text:style-name="P26">
+          <text:soft-page-break/>
+          <text:span text:style-name="T1">Delivery Address:</text:span>
+        </text:p>
+        <text:p text:style-name="P27">
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in sale.delivery_full_address.splitlines()&quot;&gt;</text:placeholder>
+        </text:p>
+        <text:p text:style-name="P27">
+          <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
+        </text:p>
+        <text:p text:style-name="P27">
+          <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
+        </text:p>
+      </text:section>
       <table:table table:name="Table1" table:style-name="Table1">
         <table:table-column table:style-name="Table1.A"/>
         <table:table-column table:style-name="Table1.B" table:number-columns-repeated="4"/>
         <table:table-header-rows>
           <table:table-row>
             <table:table-cell table:style-name="Table1.A1" office:value-type="string">
               <text:p text:style-name="Table_20_Heading">Description</text:p>
@@ -661,113 +758,113 @@
             </table:table-cell>
             <table:table-cell table:style-name="Table1.E1" office:value-type="string">
               <text:p text:style-name="Table_20_Heading">Amount</text:p>
             </table:table-cell>
           </table:table-row>
         </table:table-header-rows>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in sale.lines&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;choose test=&quot;&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;when test=&quot;line.type == 'line'&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A5" office:value-type="string">
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product&quot;&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;line.product.rec_name&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.description&quot;&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;description in line.description.split('\n')&quot;&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P21">
+            <text:p text:style-name="P22">
               <text:placeholder text:placeholder-type="text">&lt;description&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P21">
+            <text:p text:style-name="P22">
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P21">
+            <text:p text:style-name="P22">
               <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
-          <table:table-cell table:style-name="Table1.D5" office:value-type="string">
-            <text:p text:style-name="P12">
+          <table:table-cell table:style-name="Table1.B5" office:value-type="string">
+            <text:p text:style-name="P13">
               <text:placeholder text:placeholder-type="text">&lt;format_number_symbol(line.quantity, sale.party.lang, line.unit, digits=line.unit.digits) if line.unit else format_number(line.quantity, sale.party.lang)&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
-          <table:table-cell table:style-name="Table1.D5" office:value-type="string">
-            <text:p text:style-name="P13">
+          <table:table-cell table:style-name="Table1.B5" office:value-type="string">
+            <text:p text:style-name="P14">
               <text:placeholder text:placeholder-type="text">&lt;format_currency(line.unit_price, sale.party.lang, sale.currency, digits=line.__class__.unit_price.digits[1])&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
-          <table:table-cell table:style-name="Table1.D5" office:value-type="string">
-            <text:p text:style-name="P14">
+          <table:table-cell table:style-name="Table1.B5" office:value-type="string">
+            <text:p text:style-name="P6">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;tax in line.taxes&quot;&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P14">
+            <text:p text:style-name="P6">
               <text:placeholder text:placeholder-type="text">&lt;tax.description&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P14">
+            <text:p text:style-name="P6">
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
-          <table:table-cell table:style-name="Table1.E8" office:value-type="string">
-            <text:p text:style-name="P12">
+          <table:table-cell table:style-name="Table1.E5" office:value-type="string">
+            <text:p text:style-name="P13">
               <text:placeholder text:placeholder-type="text">&lt;format_currency(line.amount, sale.party.lang, sale.currency)&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;when test=&quot;line.type == 'subtotal'&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
@@ -777,40 +874,41 @@
           <table:table-cell table:style-name="Table1.A8" table:number-columns-spanned="4" office:value-type="string">
             <text:p text:style-name="Heading_20_2">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;description in (line.description or '').split('\n')&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Heading_20_2">
               <text:placeholder text:placeholder-type="text">&lt;description&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P23">
+            <text:p text:style-name="P16">
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
-          <table:table-cell table:style-name="Table1.E8" office:value-type="string">
-            <text:p text:style-name="P12">
+          <table:table-cell table:style-name="Table1.E5" office:value-type="string">
+            <text:p text:style-name="P13">
               <text:placeholder text:placeholder-type="text">&lt;format_currency(line.amount, sale.party.lang, sale.currency)&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
+        <text:soft-page-break/>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;when test=&quot;line.type == 'title'&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
@@ -821,145 +919,144 @@
             <text:p text:style-name="Heading_20_2">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;description in (line.description or '').split('\n')&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Heading_20_2">
               <text:placeholder text:placeholder-type="text">&lt;description&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Heading_20_2">
-              <text:soft-page-break/>
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;otherwise test=&quot;&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
-            <text:p text:style-name="P19">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;description in (line.description or '').split('\n')&quot;&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P19">
+            <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;description&gt;</text:placeholder>
             </text:p>
-            <text:p text:style-name="P20">
+            <text:p text:style-name="P21">
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/otherwise&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/choose&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
-          <table:table-cell table:style-name="Table1.A17" table:number-columns-spanned="5" office:value-type="string">
+          <table:table-cell table:style-name="Table1.A2" table:number-columns-spanned="5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
       </table:table>
       <text:p text:style-name="Text_20_body"/>
       <table:table table:name="Table2" table:style-name="Table2">
         <table:table-column table:style-name="Table2.A"/>
         <table:table-column table:style-name="Table2.B"/>
+        <text:soft-page-break/>
         <table:table-row>
           <table:table-cell office:value-type="string">
             <text:p text:style-name="Table_20_Contents"/>
           </table:table-cell>
           <table:table-cell office:value-type="string">
             <table:table table:name="Table4" table:style-name="Table4">
               <table:table-column table:style-name="Table4.A"/>
               <table:table-column table:style-name="Table4.B"/>
               <table:table-row>
                 <table:table-cell table:style-name="Table4.A1" office:value-type="string">
-                  <text:p text:style-name="P11">Total (excl. taxes):</text:p>
+                  <text:p text:style-name="P12">Total (excl. taxes):</text:p>
                 </table:table-cell>
                 <table:table-cell table:style-name="Table4.B1" office:value-type="string">
-                  <text:p text:style-name="P12">
+                  <text:p text:style-name="P13">
                     <text:placeholder text:placeholder-type="text">&lt;format_currency(sale.untaxed_amount, sale.party.lang, sale.currency)&gt;</text:placeholder>
                   </text:p>
                 </table:table-cell>
               </table:table-row>
               <table:table-row>
                 <table:table-cell table:style-name="Table4.A2" office:value-type="string">
-                  <text:p text:style-name="P11">Taxes:</text:p>
+                  <text:p text:style-name="P12">Taxes:</text:p>
                 </table:table-cell>
-                <table:table-cell table:style-name="Table4.B3" office:value-type="string">
-                  <text:p text:style-name="P12">
+                <table:table-cell table:style-name="Table4.B2" office:value-type="string">
+                  <text:p text:style-name="P13">
                     <text:placeholder text:placeholder-type="text">&lt;format_currency(sale.tax_amount, sale.party.lang, sale.currency)&gt;</text:placeholder>
                   </text:p>
                 </table:table-cell>
               </table:table-row>
               <table:table-row>
                 <table:table-cell table:style-name="Table4.A2" office:value-type="string">
-                  <text:p text:style-name="P11">Total:</text:p>
+                  <text:p text:style-name="P12">Total:</text:p>
                 </table:table-cell>
-                <table:table-cell table:style-name="Table4.B3" office:value-type="string">
-                  <text:p text:style-name="P12">
+                <table:table-cell table:style-name="Table4.B2" office:value-type="string">
+                  <text:p text:style-name="P13">
                     <text:placeholder text:placeholder-type="text">&lt;format_currency(sale.total_amount, sale.party.lang, sale.currency)&gt;</text:placeholder>
                   </text:p>
                 </table:table-cell>
               </table:table-row>
             </table:table>
             <text:p text:style-name="Table_20_Contents"/>
           </table:table-cell>
         </table:table-row>
       </table:table>
       <text:p text:style-name="Text_20_body">
-        <text:soft-page-break/>
         <text:placeholder text:placeholder-type="text">&lt;for each=&quot;comment in (sale.comment or '').split('\n')&quot;&gt;</text:placeholder>
       </text:p>
       <text:p text:style-name="Text_20_body">
         <text:placeholder text:placeholder-type="text">&lt;comment&gt;</text:placeholder>
       </text:p>
       <text:p text:style-name="Text_20_body">
         <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
```

### Comparing `trytond_sale-6.6.2/sale.py` & `trytond_sale-6.8.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
             })
     sale_date = fields.Date('Sale Date',
         states={
             'readonly': ~Eval('state').in_(['draft', 'quotation']),
             'required': ~Eval('state').in_(
                 ['draft', 'quotation', 'cancelled']),
             })
-    payment_term = fields.Many2One('account.invoice.payment_term',
-        'Payment Term',
+    payment_term = fields.Many2One(
+        'account.invoice.payment_term', "Payment Term", ondelete='RESTRICT',
         states={
             'readonly': Eval('state') != 'draft',
             })
     party = fields.Many2One(
         'party.party', "Party", required=True,
         states={
             'readonly': ((Eval('state') != 'draft')
@@ -195,15 +195,17 @@
             ],
         'Invoice Method', required=True, states={
             'readonly': Eval('state') != 'draft',
             })
     invoice_method_string = invoice_method.translated('invoice_method')
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
     invoices_ignored = fields.Many2Many('sale.sale-ignored-account.invoice',
@@ -219,14 +221,15 @@
         states={
             'readonly': Eval('state') != 'draft',
             })
     shipment_method_string = shipment_method.translated('shipment_method')
     shipment_state = fields.Selection([
             ('none', 'None'),
             ('waiting', 'Waiting'),
+            ('partially shipped', 'Partially Shipped'),
             ('sent', 'Sent'),
             ('exception', 'Exception'),
             ], "Shipment State", readonly=True, required=True, sort=False)
     shipments = fields.Function(fields.Many2Many(
             'stock.shipment.out', None, None, "Shipments"),
         'get_shipments', searcher='search_shipments')
     shipment_returns = fields.Function(fields.Many2Many(
@@ -373,14 +376,19 @@
         table.not_null_action('payment_term', 'remove')
 
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
     def default_payment_term(cls, **pattern):
@@ -592,49 +600,60 @@
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
         Return the invoice state for the sale.
         '''
-        skip_ids = set(x.id for x in self.invoices_ignored)
-        skip_ids.update(x.id for x in self.invoices_recreated)
-        invoices = [i for i in self.invoices if i.id not in skip_ids]
+        skips = set(self.invoices_ignored)
+        skips.update(self.invoices_recreated)
+        invoices = [i for i in self._invoices_for_state if i not in skips]
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
 
     get_shipments = get_shipments_returns('stock.shipment.out')
     get_shipment_returns = get_shipments_returns('stock.shipment.out.return')
 
     search_shipments = search_shipments_returns('stock.shipment.out')
     search_shipment_returns = search_shipments_returns(
         'stock.shipment.out.return')
 
     def get_shipment_state(self):
         '''
         Return the shipment state for the sale.
         '''
         if self.moves:
-            if any(l.move_exception for l in self.lines):
+            if any(l.moves_exception for l in self.lines):
                 return 'exception'
-            elif all(l.move_done for l in self.lines):
+            elif all(l.moves_progress >= 1.0 for l in self.lines
+                    if l.moves_progress is not None):
                 return 'sent'
+            elif any(l.moves_progress for l in self.lines):
+                return 'partially shipped'
             else:
                 return 'waiting'
         return 'none'
 
     def get_moves(self, name):
         return [m.id for l in self.lines for m in l.moves]
 
@@ -657,14 +676,20 @@
     @property
     def report_address(self):
         if self.invoice_address:
             return self.invoice_address.full_address
         else:
             return ''
 
+    @property
+    def delivery_full_address(self):
+        if self.shipment_address:
+            return self.shipment_address.full_address
+        return ''
+
     @classmethod
     def validate_fields(cls, sales, field_names):
         super().validate_fields(sales, field_names)
         cls.check_method(sales, field_names)
 
     @classmethod
     def check_method(cls, sales, field_names=None):
@@ -827,15 +852,15 @@
             company=self.company,
             type='out',
             party=party,
             invoice_address=self.invoice_address,
             currency=self.currency,
             account=party.account_receivable_used,
             )
-        invoice.on_change_type()
+        invoice.journal = invoice.on_change_with_journal()
         invoice.payment_term = self.payment_term
         return invoice
 
     def create_invoice(self):
         'Create and return an invoice'
         if self.invoice_method == 'manual':
             return
@@ -875,14 +900,15 @@
     def _get_shipment_sale(self, Shipment, key):
         values = {
             'customer': self.shipment_party or self.party,
             'company': self.company,
             }
         values.update(dict(key))
         shipment = Shipment(**values)
+        shipment.on_change_warehouse()
         if Shipment.__name__ == 'stock.shipment.out':
             if self.shipment_address == self.warehouse.address:
                 shipment.delivery_address = shipment.warehouse.address
             else:
                 shipment.delivery_address = self.shipment_address
         elif Shipment.__name__ == 'stock.shipment.out.return':
             shipment.contact_address = values['customer'].address_get()
@@ -1074,16 +1100,18 @@
 
             for line in sale.lines:
                 line.set_actual_quantity()
                 lines.append(line)
 
         for invoice_state, sales in invoice_states.items():
             cls.write(sales, {'invoice_state': invoice_state})
+            cls.log(sales, 'transition', f'invoice_state:{invoice_state}')
         for shipment_state, sales in shipment_states.items():
             cls.write(sales, {'shipment_state': shipment_state})
+            cls.log(sales, 'transition', f'shipment_state:{shipment_state}')
         Line.save(lines)
 
     @classmethod
     def _process_state(cls, sales):
         done, process = [], []
         for sale in sales:
             if sale.is_done():
@@ -1140,67 +1168,89 @@
         ('comment', 'Comment'),
         ], "Type", required=True,
         states={
             'readonly': Eval('sale_state') != 'draft',
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
             'readonly': Eval('sale_state') != 'draft',
             })
     actual_quantity = fields.Float(
         "Actual Quantity", digits='unit', readonly=True,
+        domain=[
+            If(Eval('type') != 'line',
+                ('quantity', '=', None),
+                ()),
+            ],
         states={
-            'invisible': Eval('type') != 'line',
+            'invisible': ((Eval('type') != 'line') | ~Eval('actual_quantity')),
             })
     unit = fields.Many2One('product.uom', 'Unit', ondelete='RESTRICT',
             states={
                 'required': Bool(Eval('product')),
                 'invisible': Eval('type') != 'line',
                 'readonly': Eval('sale_state') != 'draft',
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
-            If(Eval('sale_state').in_(['draft', 'quotation']),
+            If(Eval('sale_state').in_(['draft', 'quotation'])
+                & ~(Eval('quantity', 0) < 0),
                 ('salable', '=', True),
                 ()),
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('sale_state') != 'draft',
             },
         context={
             'company': Eval('company', None),
             },
         search_context={
-            'locations': If(Bool(Eval('_parent_sale', {}).get('warehouse')),
-                [Eval('_parent_sale', {}).get('warehouse', 0)], []),
-            'stock_date_end': Eval('_parent_sale', {}).get('sale_date'),
+            'locations': If(Bool(Eval('warehouse')),
+                [Eval('warehouse', -1)], []),
+            'stock_date_end': Eval('sale_date', None),
             'stock_skip_warehouse': True,
-            'currency': Eval('_parent_sale', {}).get('currency'),
-            'customer': Eval('_parent_sale', {}).get('party'),
-            'sale_date': Eval('_parent_sale', {}).get('sale_date'),
+            'currency': Eval('currency', -1),
+            'customer': Eval('customer', -1),
+            'sale_date': Eval('sale_date', None),
             'uom': Eval('unit'),
             'taxes': Eval('taxes', []),
             'quantity': Eval('quantity'),
             },
         depends={'company'})
     product_uom_category = fields.Function(
         fields.Many2One('product.uom.category', 'Product Uom Category'),
         'on_change_with_product_uom_category')
     unit_price = Monetary(
         "Unit Price", digits=price_digits, currency='currency',
+        domain=[
+            If(Eval('type') != 'line',
+                ('unit_price', '=', None),
+                ()),
+            ],
         states={
             'invisible': Eval('type') != 'line',
             'required': Eval('type') == 'line',
             'readonly': Eval('sale_state') != 'draft'
             })
     amount = fields.Function(Monetary(
             "Amount", digits='currency', currency='currency',
@@ -1216,107 +1266,140 @@
             'readonly': Eval('sale_state') != 'draft',
             },
         depends=['sale_state'])
     summary = fields.Function(fields.Char('Summary'), 'on_change_with_summary')
     note = fields.Text('Note')
     taxes = fields.Many2Many('sale.line-account.tax', 'line', 'tax', 'Taxes',
         order=[('tax.sequence', 'ASC'), ('tax.id', 'ASC')],
-        domain=[('parent', '=', None), ['OR',
+        domain=[
+            ('parent', '=', None),
+            ['OR',
                 ('group', '=', None),
-                ('group.kind', 'in', ['sale', 'both'])],
-                ('company', '=',
-                    Eval('_parent_sale', {}).get('company', -1)),
+                ('group.kind', 'in', ['sale', 'both']),
+                ],
+            ('company', '=', Eval('company', -1)),
+            If(Eval('type') != 'line',
+                ('id', '=', None),
+                ()),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('sale_state') != 'draft',
             },
         depends={'sale'})
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
     moves_ignored = fields.Many2Many('sale.line-ignored-stock.move',
             'sale_line', 'move', 'Ignored Moves', readonly=True)
     moves_recreated = fields.Many2Many('sale.line-recreated-stock.move',
             'sale_line', 'move', 'Recreated Moves', readonly=True)
-    move_done = fields.Function(fields.Boolean('Moves Done'), 'get_move_done')
-    move_exception = fields.Function(fields.Boolean('Moves Exception'),
-            'get_move_exception')
-    warehouse = fields.Function(fields.Many2One('stock.location',
-            'Warehouse'), 'get_warehouse')
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
     shipping_date = fields.Function(fields.Date('Shipping Date',
             states={
                 'invisible': Eval('type') != 'line',
                 }),
         'on_change_with_shipping_date')
     sale_state = fields.Function(
         fields.Selection('get_sale_states', "Sale State"),
-        'on_change_with_sale_state')
+        'on_change_with_sale_state', searcher='search_sale_state')
     company = fields.Function(
         fields.Many2One('company.company', "Company"),
         'on_change_with_company')
+    customer = fields.Function(
+        fields.Many2One(
+            'party.party', "Customer",
+            context={
+                'company': Eval('company', -1),
+                }),
+        'on_change_with_customer', searcher='search_customer')
+    sale_date = fields.Function(
+        fields.Date("Sale Date"),
+        'on_change_with_sale_date', searcher='search_sale_date')
 
     @classmethod
     def get_move_product_types(cls):
         pool = Pool()
         Move = pool.get('stock.move')
         return Move.get_product_types()
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('sale')
+        cls._order.insert(0, ('sale.sale_date', 'DESC NULLS FIRST'))
+        cls._order.insert(1, ('sale.id', 'DESC'))
 
     @classmethod
     def __register__(cls, module_name):
         super(SaleLine, cls).__register__(module_name)
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
+            self.unit = None
+            self.taxes = None
+
     @property
     def _move_remaining_quantity(self):
         "Compute the remaining quantity to ship"
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
-        skip_ids = set(x.id for x in self.moves_ignored)
-        skip_ids.update(x.id for x in self.moves_recreated)
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
 
     @property
     def taxable_lines(self):
         # In case we're called from an on_change
         # we have to use some sensible defaults
         if getattr(self, 'type', None) == 'line':
             return [(
@@ -1359,38 +1442,48 @@
         return context
 
     @fields.depends('product', 'unit', 'sale',
         '_parent_sale.party', '_parent_sale.invoice_party',
         methods=['compute_taxes', 'compute_unit_price',
             'on_change_with_amount'])
     def on_change_product(self):
-        if not self.product:
-            return
-
         party = None
         if self.sale:
             party = self.sale.invoice_party or self.sale.party
 
         # Set taxes before unit_price to have taxes in context of sale price
         self.taxes = self.compute_taxes(party)
 
-        category = self.product.sale_uom.category
-        if not self.unit or self.unit.category != category:
-            self.unit = self.product.sale_uom
+        if self.product:
+            category = self.product.sale_uom.category
+            if not self.unit or self.unit.category != category:
+                self.unit = self.product.sale_uom
 
         self.unit_price = self.compute_unit_price()
 
         self.type = 'line'
         self.amount = self.on_change_with_amount()
 
-    @fields.depends('product', methods=['_get_tax_rule_pattern'])
+    @fields.depends('product', 'company', methods=['_get_tax_rule_pattern'])
     def compute_taxes(self, party):
+        pool = Pool()
+        AccountConfiguration = pool.get('account.configuration')
+
         taxes = set()
         pattern = self._get_tax_rule_pattern()
-        for tax in self.product.customer_taxes_used:
+        taxes_used = []
+        if self.product:
+            taxes_used = self.product.customer_taxes_used
+        elif self.company:
+            account_config = AccountConfiguration(1)
+            account = account_config.get_multivalue(
+                'default_category_account_revenue', company=self.company.id)
+            if account:
+                taxes_used = account.taxes
+        for tax in taxes_used:
             if party and party.customer_tax_rule:
                 tax_ids = party.customer_tax_rule.apply(tax, pattern)
                 if tax_ids:
                     taxes.update(tax_ids)
                 continue
             taxes.add(tax.id)
         if party and party.customer_tax_rule:
@@ -1415,16 +1508,15 @@
                 self.quantity or 0)[self.product.id]
             if unit_price is not None:
                 unit_price = round_price(unit_price)
             return unit_price
 
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
@@ -1463,16 +1555,17 @@
                 elif line2.type == 'subtotal':
                     if self == line2:
                         break
                     amount = Decimal('0.0')
             return amount
         return Decimal('0.0')
 
-    def get_warehouse(self, name):
-        return self.sale.warehouse.id if self.sale.warehouse else None
+    @fields.depends('sale', '_parent_sale.warehouse')
+    def on_change_with_warehouse(self, name=None):
+        return self.sale.warehouse if self.sale else None
 
     def get_from_location(self, name):
         if (self.quantity or 0) >= 0:
             if self.warehouse:
                 return self.warehouse.output_location.id
         else:
             party = self.sale.shipment_party or self.sale.party
@@ -1517,32 +1610,55 @@
                     company_id = transaction.context.get('company')
                 with transaction.set_context(company=company_id):
                     shipping_date = max(shipping_date, Date.today())
             return shipping_date
 
     @fields.depends('sale', '_parent_sale.currency')
     def on_change_with_currency(self, name=None):
-        if self.sale and self.sale.currency:
-            return self.sale.currency.id
+        return self.sale.currency if self.sale else None
 
     @classmethod
     def get_sale_states(cls):
         pool = Pool()
         Sale = pool.get('sale.sale')
         return Sale.fields_get(['state'])['state']['selection']
 
     @fields.depends('sale', '_parent_sale.state')
     def on_change_with_sale_state(self, name=None):
         if self.sale:
             return self.sale.state
 
+    @classmethod
+    def search_sale_state(cls, name, clause):
+        return [('sale.state', *clause[1:])]
+
     @fields.depends('sale', '_parent_sale.company')
     def on_change_with_company(self, name=None):
-        if self.sale and self.sale.company:
-            return self.sale.company.id
+        return self.sale.company if self.sale else None
+
+    @fields.depends('sale', '_parent_sale.party')
+    def on_change_with_customer(self, name=None):
+        return self.sale.party if self.sale else None
+
+    @classmethod
+    def search_customer(cls, name, clause):
+        return [('sale.party' + clause[0][len(name):], *clause[1:])]
+
+    @fields.depends('sale', '_parent_sale.sale_date')
+    def on_change_with_sale_date(self, name=None):
+        if self.sale:
+            return self.sale.sale_date
+
+    @classmethod
+    def search_sale_date(cls, name, clause):
+        return [('sale.sale_date', *clause[1:])]
+
+    @classmethod
+    def order_sale_date(cls, tables):
+        return cls.sale.convert_order('sale.sale_date', tables, cls)
 
     def get_invoice_line(self):
         'Return a list of invoice lines for sale line'
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
         AccountConfiguration = pool.get('account.configuration')
         account_config = AccountConfiguration(1)
@@ -1791,14 +1907,26 @@
     @classmethod
     def view_attributes(cls):
         return super().view_attributes() + [
             ('/form//field[@name="note"]|/form//field[@name="description"]',
                 'spell', Eval('_parent_sale', {}).get('party_lang'))]
 
     @classmethod
+    def create(cls, vlist):
+        pool = Pool()
+        Sale = pool.get('sale.sale')
+        sale_ids = filter(None, {v.get('sale') for v in vlist})
+        for sale in Sale.browse(list(sale_ids)):
+            if sale.state != 'draft':
+                raise AccessError(
+                    gettext('sale.msg_sale_line_create_draft',
+                        sale=sale.rec_name))
+        return super().create(vlist)
+
+    @classmethod
     def delete(cls, lines):
         for line in lines:
             if line.sale_state not in {'cancelled', 'draft'}:
                 raise AccessError(
                     gettext('sale.msg_sale_line_delete_cancel_draft',
                         line=line.rec_name,
                         sale=line.sale.rec_name))
@@ -2025,22 +2153,21 @@
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Return', 'return_', 'tryton-ok', default=True),
             ])
     return_ = StateAction('sale.act_sale_form')
 
     def do_return_(self, action):
         sales = self.records
-        return_sales = self.model.copy(sales)
-        for return_sale, sale in zip(return_sales, sales):
-            return_sale.origin = sale
-            for line in return_sale.lines:
-                if line.type == 'line':
-                    line.quantity *= -1
-            return_sale.lines = return_sale.lines  # Force saving
-        self.model.save(return_sales)
+        return_sales = self.model.copy(sales, default={
+                'origin': lambda data: (
+                    '%s,%s' % (self.model.__name__, data['id'])),
+                'lines.quantity': lambda data: (
+                    data['quantity'] * -1 if data['type'] == 'line'
+                    else data['quantity']),
+                })
 
         data = {'res_id': [s.id for s in return_sales]}
         if len(return_sales) == 1:
             action['views'].reverse()
         return action, data
 
 
@@ -2090,15 +2217,17 @@
         return values
 
     def transition_modify(self):
         pool = Pool()
         Line = pool.get('sale.line')
 
         sale = self.get_sale()
-        self.model.write([sale], self.start._save_values)
+        values = self.start._save_values
+        self.model.write([sale], values)
+        self.model.log([sale], 'write', ','.join(sorted(values.keys())))
 
         # Call on_change after the save to ensure parent sale
         # has the modified values
         for line in sale.lines:
             line.on_change_product()
         Line.save(sale.lines)
```

### Comparing `trytond_sale-6.6.2/sale.xml` & `trytond_sale-6.8.0/sale.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_sale-6.6.2/sale.xml` & `trytond_sale-6.8.0/sale.xml`

```diff
@@ -73,24 +73,14 @@
       <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('moves.sale', '=', Eval('active_id')), ('moves.sale', 'in', Eval('active_ids')))]" pyson="1"/>
     </record>
     <record model="ir.action.keyword" id="act_open_shipment_return_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">sale.sale,-1</field>
       <field name="action" ref="act_return_form"/>
     </record>
-    <record model="ir.action.act_window" id="act_invoice_form">
-      <field name="name">Invoices</field>
-      <field name="res_model">account.invoice</field>
-      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('lines.origin.sale.id', '=', Eval('active_id'), 'sale.line'), ('lines.origin.sale.id', 'in', Eval('active_ids'), 'sale.line'))]" pyson="1"/>
-    </record>
-    <record model="ir.action.keyword" id="act_open_invoice_keyword1">
-      <field name="keyword">form_relate</field>
-      <field name="model">sale.sale,-1</field>
-      <field name="action" ref="act_invoice_form"/>
-    </record>
     <record model="ir.action.act_window" id="act_sale_form">
       <field name="name">Sales</field>
       <field name="res_model">sale.sale</field>
       <field name="search_value"/>
     </record>
     <record model="ir.action.act_window.view" id="act_sale_form_view1">
       <field name="sequence" eval="10"/>
@@ -144,73 +134,83 @@
       <field name="act_window" ref="act_sale_form"/>
     </record>
     <menuitem parent="menu_sale" action="act_sale_form" sequence="10" id="menu_sale_form"/>
     <record model="ir.ui.menu-res.group" id="menu_sale_form_group_sale">
       <field name="menu" ref="menu_sale_form"/>
       <field name="group" ref="group_sale"/>
     </record>
-    <record model="ir.action.act_window" id="act_sale_invoice_relate">
+    <record model="ir.action.act_window" id="act_sale_relate">
       <field name="name">Sales</field>
       <field name="res_model">sale.sale</field>
-      <field name="domain" eval="[('invoices', 'in', Eval('active_ids'))]" pyson="1"/>
+      <field name="domain" eval="[                 If(Eval('active_model') == 'party.party',                 ('party', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_invoice_relate_view1">
+    <record model="ir.action.act_window.view" id="act_sale_relate_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="sale_view_tree"/>
-      <field name="act_window" ref="act_sale_invoice_relate"/>
+      <field name="act_window" ref="act_sale_relate"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_invoice_relate_view2">
+    <record model="ir.action.act_window.view" id="act_sale_relate_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="sale_view_form"/>
-      <field name="act_window" ref="act_sale_invoice_relate"/>
-    </record>
-    <record model="ir.action.keyword" id="act_sale_invoice_relate_keyword">
-      <field name="keyword">form_relate</field>
-      <field name="model">account.invoice,-1</field>
-      <field name="action" ref="act_sale_invoice_relate"/>
-    </record>
-    <record model="ir.action.act_window" id="act_sale_shipments_relate">
-      <field name="name">Sales</field>
-      <field name="res_model">sale.sale</field>
-      <field name="domain" eval="[('shipments', 'in', Eval('active_ids'))]" pyson="1"/>
+      <field name="act_window" ref="act_sale_relate"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_shipments_relate_view1">
+    <record model="ir.action.act_window.domain" id="act_sale_relate_pending">
+      <field name="name">Pending</field>
       <field name="sequence" eval="10"/>
-      <field name="view" ref="sale_view_tree"/>
-      <field name="act_window" ref="act_sale_shipments_relate"/>
+      <field name="domain" eval="[('state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_sale_relate"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_shipments_relate_view2">
+    <record model="ir.action.act_window.domain" id="act_sale_relate_done">
+      <field name="name">Done</field>
       <field name="sequence" eval="20"/>
-      <field name="view" ref="sale_view_form"/>
-      <field name="act_window" ref="act_sale_shipments_relate"/>
+      <field name="domain" eval="[('state', '=', 'done')]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_sale_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_sale_relate_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_sale_relate"/>
     </record>
-    <record model="ir.action.keyword" id="act_sale_shipments_relate_keyword">
+    <record model="ir.action.keyword" id="act_sale_relate_keyword_party">
       <field name="keyword">form_relate</field>
-      <field name="model">stock.shipment.out,-1</field>
-      <field name="action" ref="act_sale_shipments_relate"/>
+      <field name="model">party.party,-1</field>
+      <field name="action" ref="act_sale_relate"/>
     </record>
-    <record model="ir.action.act_window" id="act_sale_shipment_returns_relate">
+    <record model="ir.action.act_window" id="act_sale_relate_simple">
       <field name="name">Sales</field>
       <field name="res_model">sale.sale</field>
-      <field name="domain" eval="[('shipment_returns', 'in', Eval('active_ids'))]" pyson="1"/>
+      <field name="domain" eval="[                 If(Eval('active_model') == 'account.invoice',                 ('invoices', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'stock.shipment.out',                 ('shipments', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'stock.shipment.out.return',                 ('shipment_returns', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_shipment_returns_relate_view1">
+    <record model="ir.action.act_window.view" id="act_sale_relate_simple_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="sale_view_tree"/>
-      <field name="act_window" ref="act_sale_shipment_returns_relate"/>
+      <field name="act_window" ref="act_sale_relate_simple"/>
     </record>
-    <record model="ir.action.act_window.view" id="act_sale_shipment_returns_relate_view2">
+    <record model="ir.action.act_window.view" id="act_sale_relate_simple_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="sale_view_form"/>
-      <field name="act_window" ref="act_sale_shipment_returns_relate"/>
+      <field name="act_window" ref="act_sale_relate_simple"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_relate_simple_keyword_invoice">
+      <field name="keyword">form_relate</field>
+      <field name="model">account.invoice,-1</field>
+      <field name="action" ref="act_sale_relate_simple"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_relate_simple_keyword_shipment_out">
+      <field name="keyword">form_relate</field>
+      <field name="model">stock.shipment.out,-1</field>
+      <field name="action" ref="act_sale_relate_simple"/>
     </record>
-    <record model="ir.action.keyword" id="act_sale_shipment_returns_relate_keyword">
+    <record model="ir.action.keyword" id="act_sale_relate_simple_keyword_shipment_out_return">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.out.return,-1</field>
-      <field name="action" ref="act_sale_shipment_returns_relate"/>
+      <field name="action" ref="act_sale_relate_simple"/>
     </record>
     <record model="ir.model.access" id="access_sale">
       <field name="model" search="[('model', '=', 'sale.sale')]"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
@@ -219,14 +219,23 @@
       <field name="model" search="[('model', '=', 'sale.sale')]"/>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
+    <record model="ir.rule.group" id="rule_group_sale_companies">
+      <field name="name">User in companies</field>
+      <field name="model" search="[('model', '=', 'sale.sale')]"/>
+      <field name="global_p" eval="True"/>
+    </record>
+    <record model="ir.rule" id="rule_sale_companies">
+      <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
+      <field name="rule_group" ref="rule_group_sale_companies"/>
+    </record>
     <record model="ir.model.button" id="sale_cancel_button">
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
       <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_cancel_button_group_sale">
       <field name="button" ref="sale_cancel_button"/>
@@ -334,34 +343,69 @@
     </record>
     <record model="ir.ui.view" id="sale_line_view_tree_sequence">
       <field name="model">sale.line</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">sale_line_tree_sequence</field>
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
-    <record model="ir.ui.view" id="party_view_form">
-      <field name="model">party.party</field>
-      <field name="inherit" ref="party.party_view_form"/>
-      <field name="name">party_form</field>
-    </record>
-    <record model="ir.action.wizard" id="act_open_customer">
-      <field name="name">Parties associated to Sales</field>
-      <field name="wiz_name">sale.open_customer</field>
+    <record model="ir.action.act_window" id="act_sale_line_relate">
+      <field name="name">Sale Lines</field>
+      <field name="res_model">sale.line</field>
+      <field name="domain" eval="[('type', '=', 'line'),                 If(Eval('active_model') == 'sale.sale',                 ('sale', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.product',                 ('product', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.template',                 ('product.template.id', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'party.party',                 ('customer', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_sale_line_relate_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="sale_line_view_tree"/>
+      <field name="act_window" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_sale_line_relate_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="sale_line_view_form"/>
+      <field name="act_window" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_sale_line_relate_pending">
+      <field name="name">Pending</field>
+      <field name="sequence" eval="10"/>
+      <field name="domain" eval="[('sale_state', 'not in', ['done', 'cancelled'])]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_sale_line_relate_done">
+      <field name="name">Done</field>
+      <field name="sequence" eval="20"/>
+      <field name="domain" eval="[('sale_state', '=', 'done')]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_sale_line_relate_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_line_relate_keyword_sale">
+      <field name="keyword">form_relate</field>
+      <field name="model">sale.sale,-1</field>
+      <field name="action" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_line_relate_keyword_product">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.product,-1</field>
+      <field name="action" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_line_relate_keyword_product_template">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.template,-1</field>
+      <field name="action" ref="act_sale_line_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_sale_line_relate_keyword_party">
+      <field name="keyword">form_relate</field>
+      <field name="model">party.party,-1</field>
+      <field name="action" ref="act_sale_line_relate"/>
     </record>
-    <menuitem name="Associated to Sales" parent="party.menu_party_form" action="act_open_customer" sequence="50" id="menu_customer" icon="tryton-list"/>
     <record model="ir.ui.view" id="return_sale_start_view_form">
       <field name="model">sale.return_sale.start</field>
       <field name="type">form</field>
       <field name="name">return_sale_start_form</field>
     </record>
     <record model="ir.action.wizard" id="wizard_return_sale">
       <field name="name">Return Sale</field>
@@ -380,58 +424,9 @@
     </record>
     <record model="ir.ui.view" id="modify_header_form">
       <field name="model">sale.sale</field>
       <field name="inherit" ref="sale.sale_view_form"/>
       <field name="name">modify_header_form</field>
       <field name="domain" eval="Eval('context', {}).get('modify_header', False)" pyson="1"/>
     </record>
-    <record model="ir.rule.group" id="rule_group_sale_companies">
-      <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_sale_companies">
-      <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_sale_companies"/>
-    </record>
-    <record model="ir.model.access" id="access_invoice_sale">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
-      <field name="group" ref="group_sale"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_invoice_line_sale">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
-      <field name="group" ref="group_sale"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_move_group_sale">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
-      <field name="group" ref="group_sale"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_shipment_out_group_sale">
-      <field name="model" search="[('model', '=', 'stock.shipment.out')]"/>
-      <field name="group" ref="group_sale"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_shipment_out_return_group_sale">
-      <field name="model" search="[('model', '=', 'stock.shipment.out.return')]"/>
-      <field name="group" ref="group_sale"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale-6.6.2/sale_reporting.py` & `trytond_sale-6.8.0/sale_reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,14 +348,18 @@
         line = tables['line']
         return super(CustomerMixin, cls)._group_by(tables, withs) + [
             line.customer]
 
     def get_rec_name(self, name):
         return self.customer.rec_name
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('customer.rec_name', *clause[1:])]
+
 
 class Customer(CustomerMixin, Abstract, ModelView):
     "Sale Reporting per Customer"
     __name__ = 'sale.reporting.customer'
 
     time_series = fields.One2Many(
         'sale.reporting.customer.time_series', 'customer',
@@ -432,14 +436,18 @@
         where = super()._where(tables, withs)
         where &= party_category.category != Null
         return where
 
     def get_rec_name(self, name):
         return self.category.rec_name if self.category else None
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('category.rec_name', *clause[1:])]
+
 
 class CustomerCategory(CustomerCategoryMixin, Abstract, ModelView):
     "Sale Reporting per Customer Category"
     __name__ = 'sale.reporting.customer.category'
 
     time_series = fields.One2Many(
         'sale.reporting.customer.category.time_series', 'category',
@@ -462,15 +470,16 @@
     __name__ = 'sale.reporting.customer.category.time_series'
 
 
 class CustomerCategoryTree(ModelSQL, ModelView):
     "Sale Reporting per Customer Category"
     __name__ = 'sale.reporting.customer.category.tree'
 
-    name = fields.Function(fields.Char("Name"), 'get_name')
+    name = fields.Function(
+        fields.Char("Name"), 'get_name', searcher='search_name')
     parent = fields.Many2One('sale.reporting.customer.category.tree', "Parent")
     children = fields.One2Many(
         'sale.reporting.customer.category.tree', 'parent', "Children")
     revenue = fields.Function(Monetary(
             "Revenue", digits='currency', currency='currency'), 'get_total')
 
     currency = fields.Function(fields.Many2One(
@@ -491,14 +500,20 @@
     def get_name(cls, categories, name):
         pool = Pool()
         Category = pool.get('party.category')
         categories = Category.browse(categories)
         return {c.id: c.name for c in categories}
 
     @classmethod
+    def search_name(cls, name, clause):
+        pool = Pool()
+        Category = pool.get('party.category')
+        return [('id', 'in', Category.search([clause], query=True))]
+
+    @classmethod
     def order_name(cls, tables):
         pool = Pool()
         Category = pool.get('party.category')
         table, _ = tables[None]
         if 'category' not in tables:
             category = Category.__table__()
             tables['category'] = {
@@ -603,14 +618,18 @@
         where = super(ProductMixin, cls)._where(tables, withs)
         where &= line.product != Null
         return where
 
     def get_rec_name(self, name):
         return self.product.rec_name if self.product else None
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('product.rec_name', *clause[1:])]
+
 
 class Product(ProductMixin, Abstract, ModelView):
     "Sale Reporting per Product"
     __name__ = 'sale.reporting.product'
 
     time_series = fields.One2Many(
         'sale.reporting.product.time_series', 'product',
@@ -692,14 +711,18 @@
         where = super()._where(tables, withs)
         where &= template_category.category != Null
         return where
 
     def get_rec_name(self, name):
         return self.category.rec_name if self.category else None
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('category.rec_name', *clause[1:])]
+
 
 class ProductCategory(ProductCategoryMixin, Abstract, ModelView):
     "Sale Reporting per Product Category"
     __name__ = 'sale.reporting.product.category'
 
     time_series = fields.One2Many(
         'sale.reporting.product.category.time_series', 'category',
@@ -722,15 +745,16 @@
     __name__ = 'sale.reporting.product.category.time_series'
 
 
 class ProductCategoryTree(ModelSQL, ModelView):
     "Sale Reporting per Product Category"
     __name__ = 'sale.reporting.product.category.tree'
 
-    name = fields.Function(fields.Char("Name"), 'get_name')
+    name = fields.Function(
+        fields.Char("Name"), 'get_name', searcher='search_name')
     parent = fields.Many2One('sale.reporting.product.category.tree', "Parent")
     children = fields.One2Many(
         'sale.reporting.product.category.tree', 'parent', "Children")
     revenue = fields.Function(Monetary(
             "Revenue", digits='currency'), 'get_total')
 
     currency = fields.Function(fields.Many2One(
@@ -751,14 +775,20 @@
     def get_name(cls, categories, name):
         pool = Pool()
         Category = pool.get('product.category')
         categories = Category.browse(categories)
         return {c.id: c.name for c in categories}
 
     @classmethod
+    def search_name(cls, name, clause):
+        pool = Pool()
+        Category = pool.get('product.category')
+        return [('id', 'in', Category.search([clause], query=True))]
+
+    @classmethod
     def order_name(cls, tables):
         pool = Pool()
         Category = pool.get('product.category')
         table, _ = tables[None]
         if 'category' not in tables:
             category = Category.__table__()
             tables['category'] = {
@@ -867,14 +897,21 @@
     @classmethod
     def _where(cls, tables, withs):
         address = tables['line.shipment_address']
         where = super(CountryMixin, cls)._where(tables, withs)
         where &= address.country != Null
         return where
 
+    def get_rec_name(self, name):
+        return self.country.rec_name
+
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('country.rec_name', *clause[1:])]
+
 
 class RegionTree(ModelSQL, ModelView):
     "Sale Reporting per Region"
     __name__ = 'sale.reporting.region.tree'
 
     name = fields.Function(fields.Char("Name"), 'get_name')
     parent = fields.Many2One('sale.reporting.region.tree', "Parent")
@@ -1018,17 +1055,14 @@
         cls._order.insert(0, ('country', 'ASC'))
 
     @classmethod
     def _column_id(cls, tables, withs):
         address = tables['line.shipment_address']
         return address.country
 
-    def get_rec_name(self, name):
-        return self.country.rec_name
-
 
 class CountryTimeseries(CountryMixin, AbstractTimeseries, ModelView):
     "Sale Reporting per Country"
     __name__ = 'sale.reporting.country.time_series'
 
 
 class SubdivisionMixin(CountryMixin):
@@ -1050,14 +1084,21 @@
     @classmethod
     def _where(cls, tables, withs):
         address = tables['line.shipment_address']
         where = super(SubdivisionMixin, cls)._where(tables, withs)
         where &= address.subdivision != Null
         return where
 
+    def get_rec_name(self, name):
+        return self.subdivision.rec_name
+
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('subdivision.rec_name', *clause[1:])]
+
 
 class Subdivision(SubdivisionMixin, Abstract):
     "Sale Reporting per Subdivision"
     __name__ = 'sale.reporting.country.subdivision'
 
     time_series = fields.One2Many(
         'sale.reporting.country.subdivision.time_series', 'subdivision',
@@ -1069,17 +1110,14 @@
         cls._order.insert(0, ('subdivision', 'ASC'))
 
     @classmethod
     def _column_id(cls, tables, withs):
         address = tables['line.shipment_address']
         return address.subdivision
 
-    def get_rec_name(self, name):
-        return self.subdivision.rec_name
-
 
 class SubdivisionTimeseries(SubdivisionMixin, AbstractTimeseries, ModelView):
     "Sale Reporting per Subdivision"
     __name__ = 'sale.reporting.country.subdivision.time_series'
 
 
 class CountryTree(UnionMixin, Abstract, ModelView):
```

### Comparing `trytond_sale-6.6.2/sale_reporting.xml` & `trytond_sale-6.8.0/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/setup.py` & `trytond_sale-6.8.0/setup.py`

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
@@ -37,38 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4', 'python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for sale',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-sale/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/sale',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale',
     package_dir={'trytond.modules.sale': '.'},
     packages=(
         ['trytond.modules.sale']
         + ['trytond.modules.sale.%s' % p for p in find_packages()]
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

### Comparing `trytond_sale-6.6.2/stock.py` & `trytond_sale-6.8.0/stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.modules.product import round_price
 from trytond.pool import Pool, PoolMeta
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 def process_sale(moves_field):
     def _process_sale(func):
         @wraps(func)
         def wrapper(cls, shipments):
             pool = Pool()
             Sale = pool.get('sale.sale')
             transaction = Transaction()
             context = transaction.context
-            with transaction.set_context(_check_access=False):
+            with without_check_access():
                 sales = set(m.sale for s in cls.browse(shipments)
                     for m in getattr(s, moves_field) if m.sale)
             func(cls, shipments)
             if sales:
                 with transaction.set_context(
                         queue_batch=context.get('queue_batch', True)):
                     Sale.__queue__.process(sales)
@@ -93,15 +93,15 @@
 def process_sale_move(func):
     @wraps(func)
     def wrapper(cls, moves):
         pool = Pool()
         Sale = pool.get('sale.sale')
         transaction = Transaction()
         context = transaction.context
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             sales = set(m.sale for m in cls.browse(moves) if m.sale)
         func(cls, moves)
         if sales:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
                 Sale.__queue__.process(sales)
     return wrapper
@@ -150,22 +150,21 @@
             return 'ignored'
         return ''
 
     @fields.depends('origin')
     def on_change_with_product_uom_category(self, name=None):
         pool = Pool()
         SaleLine = pool.get('sale.line')
-        category = super(Move, self).on_change_with_product_uom_category(
-            name=name)
+        category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to ship and the quantity to invoice.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, SaleLine)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     def get_cost_price(self, product_cost_price=None):
         pool = Pool()
         SaleLine = pool.get('sale.line')
         Sale = pool.get('sale.sale')
         # For return sale's move use the cost price of the original sale
```

### Comparing `trytond_sale-6.6.2/tests/scenario_sale.rst` & `trytond_sale-6.8.0/tests/scenario_sale.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 =============
 Sale Scenario
 =============
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
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
 
 Activate modules::
 
     >>> config = activate_modules('sale')
 
 Create company::
 
@@ -171,15 +168,15 @@
     >>> sale.confirmed_by == employee
     True
     >>> sale.state
     'processing'
     >>> sale.shipment_state
     'waiting'
     >>> sale.invoice_state
-    'waiting'
+    'pending'
     >>> len(sale.shipments), len(sale.shipment_returns), len(sale.invoices)
     (1, 0, 1)
     >>> invoice, = sale.invoices
     >>> invoice.origins == sale.rec_name
     True
     >>> shipment, = sale.shipments
     >>> shipment.origins == sale.rec_name
@@ -209,14 +206,16 @@
 
 
     >>> for invoice in sale.invoices:
     ...     invoice.click('post')
     >>> sale.reload()
     >>> len(sale.shipments), len(sale.shipment_returns), len(sale.invoices)
     (1, 0, 1)
+    >>> sale.invoice_state
+    'awaiting payment'
 
 Testing the report::
 
     >>> sale_report = Report('sale.sale')
     >>> ext, _, _, name = sale_report.execute([sale], {})
     >>> ext
     'odt'
@@ -264,24 +263,23 @@
     0
     >>> len(stock_move2.invoice_lines)
     0
 
 Validate Shipments::
 
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.click('done')
 
 Open customer invoice::
 
     >>> sale.reload()
     >>> sale.invoice_state
-    'waiting'
+    'pending'
     >>> invoice, = sale.invoices
     >>> invoice.type
     'out'
     >>> invoice_line1, invoice_line2 = sorted(invoice.lines,
     ...     key=lambda l: l.quantity or 0)
     >>> for line in invoice.lines:
     ...     line.quantity = 1
@@ -315,15 +313,15 @@
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
     >>> sale.shipment_state
     'none'
     >>> sale.invoice_state
-    'waiting'
+    'pending'
     >>> len(sale.shipments), len(sale.shipment_returns), len(sale.invoices)
     (0, 0, 1)
 
 Not yet linked to stock moves::
 
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
@@ -333,15 +331,15 @@
 Post and Pay Invoice for 4 products::
 
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity
     5.0
     >>> invoice_line.quantity = 4.0
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> invoice.reload()
     >>> invoice.state
     'paid'
 
 Invoice lines linked to 1 move::
@@ -364,15 +362,14 @@
 Ship 3 products::
 
     >>> stock_inventory_move, = shipment.inventory_moves
     >>> stock_inventory_move.quantity
     4.0
     >>> stock_inventory_move.quantity = 3.0
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 New shipments created::
@@ -425,17 +422,17 @@
     >>> move_return.quantity = 3
     >>> ship_return.click('receive')
 
 Check Return::
 
     >>> return_.reload()
     >>> return_.shipment_state
-    'waiting'
+    'partially shipped'
     >>> return_.invoice_state
-    'waiting'
+    'pending'
     >>> (len(return_.shipments), len(return_.shipment_returns),
     ...     len(return_.invoices))
     (0, 2, 1)
 
 Open customer credit note::
 
     >>> credit_note, = return_.invoices
@@ -460,15 +457,15 @@
 
 Check Return::
 
     >>> return_.reload()
     >>> return_.shipment_state
     'sent'
     >>> return_.invoice_state
-    'waiting'
+    'awaiting payment'
     >>> (len(return_.shipments), len(return_.shipment_returns),
     ...     len(return_.invoices))
     (0, 2, 2)
 
 Mixing return and sale::
 
     >>> mix = Sale()
@@ -490,30 +487,29 @@
     >>> mix.click('quote')
     >>> mix.click('confirm')
     >>> mix.state
     'processing'
     >>> mix.shipment_state
     'waiting'
     >>> mix.invoice_state
-    'waiting'
+    'pending'
     >>> len(mix.shipments), len(mix.shipment_returns), len(mix.invoices)
     (1, 1, 1)
 
 Checking Shipments::
 
     >>> mix_return, = mix.shipment_returns
     >>> mix_shipment, = mix.shipments
     >>> mix_return.click('receive')
     >>> move_return, = mix_return.incoming_moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     2.0
     >>> mix_shipment.click('assign_try')
-    True
     >>> mix_shipment.click('pick')
     >>> mix_shipment.click('pack')
     >>> mix_shipment.click('done')
     >>> move_shipment, = mix_shipment.outgoing_moves
     >>> move_shipment.product.rec_name
     'product'
     >>> move_shipment.quantity
@@ -567,15 +563,14 @@
     >>> mix_return.click('receive')
     >>> move_return, = mix_return.incoming_moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     3.0
     >>> mix_shipment.click('assign_try')
-    True
     >>> mix_shipment.click('pick')
     >>> mix_shipment.click('pack')
     >>> move_shipment, = mix_shipment.outgoing_moves
     >>> move_shipment.product.rec_name
     'product'
     >>> move_shipment.quantity
     6.0
@@ -592,21 +587,21 @@
     >>> service_sale.click('quote')
     >>> service_sale.click('confirm')
     >>> service_sale.state
     'processing'
     >>> service_sale.shipment_state
     'none'
     >>> service_sale.invoice_state
-    'waiting'
+    'pending'
     >>> service_invoice, = service_sale.invoices
 
 Pay the service invoice::
 
     >>> service_invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [service_invoice])
+    >>> pay = service_invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> service_invoice.reload()
     >>> service_invoice.state
     'paid'
 
 Check service sale states::
@@ -656,15 +651,14 @@
     >>> line.quantity = 10.0
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> shipment, = sale.shipments
     >>> for move in shipment.inventory_moves:
     ...     move.quantity = 5.0
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.click('done')
     >>> sale.reload()
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity
@@ -689,20 +683,23 @@
     >>> sale.click('confirm')
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
     >>> invoice_line.stock_moves == []
     True
     >>> invoice_line.quantity = 5.0
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> invoice.reload()
     >>> invoice.state
     'paid'
+    >>> sale.reload()
+    >>> sale.invoice_state
+    'partially paid'
     >>> invoice_line.reload()
     >>> stock_move, = invoice_line.stock_moves
     >>> stock_move.quantity
     5.0
     >>> stock_move.state
     'draft'
```

### Comparing `trytond_sale-6.6.2/tests/scenario_sale_default_methods.rst` & `trytond_sale-6.8.0/tests/scenario_sale_default_methods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/tests/scenario_sale_empty.rst` & `trytond_sale-6.8.0/tests/scenario_sale_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/tests/scenario_sale_modify_header.rst` & `trytond_sale-6.8.0/tests/scenario_sale_modify_header.rst`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     >>> sale_line.quantity = 3
     >>> sale.save()
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('30.00'), Decimal('3.00'), Decimal('33.00'))
 
 Change the party::
 
-    >>> modify_header = Wizard('sale.modify_header', [sale])
+    >>> modify_header = sale.click('modify_header')
     >>> modify_header.form.party == customer
     True
     >>> modify_header.form.party = another
     >>> modify_header.execute('modify')
 
     >>> sale.party.name
     'Another Customer'
```

### Comparing `trytond_sale-6.6.2/tests/scenario_sale_reporting.rst` & `trytond_sale-6.8.0/tests/scenario_sale_reporting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,17 @@
     >>> with config.set_context(context=context):
     ...     sorted((r.name, r.revenue) for r in tree) == sorted([
     ...         ('Root1', Decimal('40')),
     ...         ('Child1', Decimal('30')),
     ...         ('Child2', Decimal('10')),
     ...         ('Root2', Decimal('30'))])
     True
+    >>> child1, = CustomerCategoryTree.find([('rec_name', '=', 'Child1')])
+    >>> child1.rec_name
+    'Child1'
 
 Check sale reporting per product::
 
     >>> Product = Model.get('sale.reporting.product')
     >>> ProductTimeseries = Model.get('sale.reporting.product.time_series')
     >>> with config.set_context(context=context):
     ...     reports = Product.find([])
@@ -276,14 +279,17 @@
     ...     sorted((r.name, r.revenue) for r in tree) == sorted([
     ...         ('Root1', Decimal('40')),
     ...         ('Child1', Decimal('30')),
     ...         ('Child2', Decimal('10')),
     ...         ('Root2', Decimal('30')),
     ...         ('Account Category', Decimal('40'))])
     True
+    >>> child1, = ProductCategoryTree.find([('rec_name', '=', 'Child1')])
+    >>> child1.rec_name
+    'Child1'
 
 Check sale reporting per countries::
 
     >>> RegionTree = Model.get('sale.reporting.region.tree')
     >>> CountryTree = Model.get('sale.reporting.country.tree')
     >>> CountryTimeseries = Model.get('sale.reporting.country.time_series')
     >>> SubdivisionTimeseries = Model.get(
```

### Comparing `trytond_sale-6.6.2/tests/test_module.py` & `trytond_sale-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-6.8.0/trytond_sale.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale
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
 
 ###########
 Sale Module
 ###########
```

### Comparing `trytond_sale-6.6.2/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-6.8.0/trytond_sale.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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
 sale.fodt
 sale.py
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
 ./sale.fodt
 ./sale.py
```

### Comparing `trytond_sale-6.6.2/view/configuration_form.xml` & `trytond_sale-6.8.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/party_form.xml` & `trytond_sale-6.8.0/view/party_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_sale-6.6.2/view/party_form.xml` & `trytond_sale-6.8.0/view/party_form.xml`

```diff
@@ -1,13 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <data>
   <xpath expr="//group[@id='links']" position="inside">
-    <link icon="tryton-sale" name="sale.act_sale_form2" empty="hide"/>
+    <link icon="tryton-sale" name="sale.act_sale_relate" empty="hide"/>
+    <link icon="tryton-sale" name="sale.act_sale_line_relate" empty="hide"/>
   </xpath>
   <xpath expr="/form/notebook" position="inside">
     <page id="sale" string="Sale">
       <label name="sale_invoice_method"/>
       <field name="sale_invoice_method"/>
       <label name="sale_shipment_method"/>
       <field name="sale_shipment_method"/>
```

### Comparing `trytond_sale-6.6.2/view/product_list_sale_line.xml` & `trytond_sale-6.8.0/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/product_sale_context_form.xml` & `trytond_sale-6.8.0/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/sale_form.xml` & `trytond_sale-6.8.0/view/sale_form.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_sale-6.6.2/view/sale_form.xml` & `trytond_sale-6.8.0/view/sale_form.xml`

```diff
@@ -7,21 +7,19 @@
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
   <label name="shipment_party"/>
   <field name="shipment_party"/>
   <label name="shipment_address"/>
-  <field name="shipment_address"/>
-  <newline/>
+  <field name="shipment_address" colspan="3"/>
   <label name="description"/>
   <field name="description" colspan="3"/>
   <label name="reference"/>
   <field name="reference"/>
   <notebook colspan="6">
     <page string="Sale" id="sale">
       <label name="sale_date"/>
```

### Comparing `trytond_sale-6.6.2/view/sale_line_form.xml` & `trytond_sale-6.8.0/view/sale_line_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_sale-6.6.2/view/sale_line_form.xml` & `trytond_sale-6.8.0/view/sale_line_form.xml`

```diff
@@ -25,13 +25,19 @@
       <field name="shipping_date"/>
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

### Comparing `trytond_sale-6.6.2/view/sale_line_tree_sequence.xml` & `trytond_sale-6.8.0/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/sale_reporting_context_form.xml` & `trytond_sale-6.8.0/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/sale_reporting_customer_category_list.xml` & `trytond_sale-6.8.0/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/sale_reporting_product_category_list.xml` & `trytond_sale-6.8.0/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.6.2/view/sale_tree.xml` & `trytond_sale-6.8.0/view/sale_tree.xml`

 * *Files identical despite different names*

