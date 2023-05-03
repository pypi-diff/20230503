# Comparing `tmp/trytond_account_invoice-6.6.5.tar.gz` & `tmp/trytond_account_invoice-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-6.6.5.tar", last modified: Wed May  3 16:59:17 2023, max compression
+gzip compressed data, was "trytond_account_invoice-6.8.0.tar", last modified: Mon May  1 11:45:58 2023, max compression
```

## Comparing `trytond_account_invoice-6.6.5.tar` & `trytond_account_invoice-6.8.0.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.294545 trytond_account_invoice-6.6.5/
--rw-r--r--   0 ced       (1000) ced       (1000)     7750 2023-05-03 16:59:13.000000 trytond_account_invoice-6.6.5/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-03 16:59:13.000000 trytond_account_invoice-6.6.5/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2604 2023-05-03 16:59:17.294545 trytond_account_invoice-6.6.5/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1871 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17489 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4994 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.284544 trytond_account_invoice-6.6.5/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.287877 trytond_account_invoice-6.6.5/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/doc/usage/amend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/doc/usage/prepare.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3685 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      813 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.287877 trytond_account_invoice-6.6.5/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    83227 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   130651 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21948 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.264542 trytond_account_invoice-6.6.5/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    35417 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36628 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30533 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37166 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36341 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31383 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34584 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38523 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30507 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37025 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33004 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32771 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33634 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35894 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34292 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36341 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31117 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33947 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34576 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36128 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33329 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30489 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    29287 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34828 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5944 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3977 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3403 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15131 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:59:17.294545 trytond_account_invoice-6.6.5/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4630 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.267876 trytond_account_invoice-6.6.5/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4069 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12510 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6480 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2832 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2766 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1855 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2599 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3561 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3063 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7413 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3472 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3575 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3473 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3778 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.291211 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2604 2023-05-03 16:59:16.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5713 2023-05-03 16:59:17.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:59:16.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-03 16:59:16.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:25:24.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-03 16:59:16.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:59:16.000000 trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:59:17.284544 trytond_account_invoice-6.6.5/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4492 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      973 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-05-03 16:22:12.000000 trytond_account_invoice-6.6.5/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-13 16:52:41.000000 trytond_account_invoice-6.6.5/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:49.000000 trytond_account_invoice-6.6.5/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-05-01 11:04:03.000000 trytond_account_invoice-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:04:02.000000 trytond_account_invoice-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1900 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18805 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/amend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/prepare.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3685 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    83227 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   130495 2023-04-29 11:01:18.000000 trytond_account_invoice-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24250 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.885674 trytond_account_invoice-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    36045 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37302 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31162 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37906 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37027 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32038 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35126 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39011 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31136 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37812 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33682 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33571 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34282 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36613 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34940 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31760 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34582 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35422 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36762 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33969 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31118 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    29853 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35375 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6174 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3977 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15131 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.895674 trytond_account_invoice-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3188 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4029 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12415 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2856 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3472 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3426 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2713 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1868 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2606 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3521 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3480 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3582 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3408 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-05-01 11:03:56.000000 trytond_account_invoice-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.905674 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5919 2023-05-01 11:45:58.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.899007 trytond_account_invoice-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4492 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-28 07:43:48.000000 trytond_account_invoice-6.8.0/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-28 07:46:16.000000 trytond_account_invoice-6.8.0/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-6.6.5/CHANGELOG` & `trytond_account_invoice-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,15 @@
 
-Version 6.6.5 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.4 - 2023-04-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.3 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2022-12-06
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Support payment with currency exchange
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Warn when cancelling a move related to an invoice
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Support alternative payees on invoice
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_account_invoice-6.6.5/COPYRIGHT` & `trytond_account_invoice-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/LICENSE` & `trytond_account_invoice-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/PKG-INFO` & `trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_invoice
-Version: 6.6.5
+Name: trytond-account-invoice
+Version: 6.8.0
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice
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
 
 ######################
 Account Invoice Module
 ######################
```

### Comparing `trytond_account_invoice-6.6.5/__init__.py` & `trytond_account_invoice-6.8.0/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,11 +47,12 @@
         invoice.RescheduleLinesToPay,
         invoice.DelegateLinesToPay,
         party.Replace,
         party.Erase,
         account.RenewFiscalYear,
         account.RescheduleLines,
         account.DelegateLines,
+        account.CancelMoves,
         module='account_invoice', type_='wizard')
     Pool.register(
         invoice.InvoiceReport,
         module='account_invoice', type_='report')
```

### Comparing `trytond_account_invoice-6.6.5/account.py` & `trytond_account_invoice-6.8.0/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import OrderedDict
+from itertools import islice
 
 from sql import Literal
 from sql.conditionals import Coalesce
 
 from trytond.i18n import gettext
 from trytond.model import (
     MatchMixin, ModelSQL, ModelView, Workflow, fields, sequence_ordered)
 from trytond.modules.account.exceptions import ClosePeriodError
 from trytond.modules.company.model import CompanyValueMixin
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Id, If
 from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
+from .exceptions import CancelInvoiceMoveWarning
+
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'account.configuration'
 
     default_customer_payment_term = fields.MultiValue(
         fields.Many2One(
             'account.invoice.payment_term', "Default Customer Payment Term"))
@@ -459,7 +462,38 @@
                 ('additional_moves', 'in', move_ids),
                 ])
         Invoice.write(invoices, {
                 'alternative_payees': [('add', [party.id])],
                 'additional_moves': [('add', [move.id])],
                 })
         return move
+
+
+class CancelMoves(metaclass=PoolMeta):
+    __name__ = 'account.move.cancel'
+
+    def transition_cancel(self):
+        pool = Pool()
+        Invoice = pool.get('account.invoice')
+        Warning = pool.get('res.user.warning')
+
+        moves_w_invoices = {
+            m: m.origin for m in self.records
+            if (isinstance(m.origin, Invoice)
+                and m.origin.state not in {'paid', 'cancelled'})}
+        if moves_w_invoices:
+            move_names = ', '.join(m.rec_name
+                for m in islice(moves_w_invoices, None, 5))
+            invoice_names = ', '.join(i.rec_name
+                for i in islice(moves_w_invoices.values(), None, 5))
+            if len(moves_w_invoices) > 5:
+                move_names += '...'
+                invoice_names += '...'
+            key = Warning.format('cancel_invoice_move', moves_w_invoices)
+            if Warning.check(key):
+                raise CancelInvoiceMoveWarning(key,
+                    gettext('account_invoice.msg_cancel_invoice_move',
+                        moves=move_names, invoices=invoice_names),
+                    gettext(
+                        'account_invoice.msg_cancel_invoice_move_description'))
+
+        return super().transition_cancel()
```

### Comparing `trytond_account_invoice-6.6.5/account.xml` & `trytond_account_invoice-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/company.py` & `trytond_account_invoice-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/doc/conf.py` & `trytond_account_invoice-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_invoice-6.6.5/doc/configuration.rst` & `trytond_account_invoice-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/doc/design.rst` & `trytond_account_invoice-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/doc/usage/amend.rst` & `trytond_account_invoice-6.8.0/doc/usage/amend.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/doc/usage/prepare.rst` & `trytond_account_invoice-6.8.0/doc/usage/prepare.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/doc/usage/process.rst` & `trytond_account_invoice-6.8.0/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/exceptions.py` & `trytond_account_invoice-6.8.0/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,7 +39,11 @@
 
 class InvoiceFutureWarning(UserWarning):
     pass
 
 
 class InvoiceSimilarWarning(UserWarning):
     pass
+
+
+class CancelInvoiceMoveWarning(UserWarning):
+    pass
```

### Comparing `trytond_account_invoice-6.6.5/icons/LICENSE` & `trytond_account_invoice-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/invoice.fodt` & `trytond_account_invoice-6.8.0/invoice.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/invoice.py` & `trytond_account_invoice-6.8.0/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 from trytond.rpc import RPC
 from trytond.tools import firstline, grouped_slice, reduce_ids
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import (
-    InvoiceFutureWarning, InvoiceLineValidationError, InvoiceNumberError,
-    InvoicePaymentTermDateWarning, InvoiceSimilarWarning,
-    InvoiceTaxValidationError, InvoiceValidationError, PayInvoiceError)
+    InvoiceFutureWarning, InvoiceNumberError, InvoicePaymentTermDateWarning,
+    InvoiceSimilarWarning, InvoiceTaxValidationError, InvoiceValidationError,
+    PayInvoiceError)
 
 if config.getboolean('account_invoice', 'filestore', default=False):
     file_id = 'invoice_report_cache_id'
     store_prefix = config.get('account_invoice', 'store_prefix', default=None)
 else:
     file_id = None
     store_prefix = None
@@ -123,15 +123,19 @@
             'readonly': (
                 _states['readonly']
                 | (Eval('lines', [0]) & Eval('currency'))),
             })
     currency_date = fields.Function(fields.Date('Currency Date'),
         'on_change_with_currency_date')
     journal = fields.Many2One(
-        'account.journal', 'Journal', required=True, states=_states,
+        'account.journal', 'Journal',
+        states={
+            'readonly': _states['readonly'],
+            'required': Eval('state') != 'draft',
+            },
         context={
             'company': Eval('company', -1),
             }, depends={'company'})
     move = fields.Many2One('account.move', 'Move', readonly=True,
         domain=[
             ('company', '=', Eval('company', -1)),
             ])
@@ -161,45 +165,59 @@
                 ('type.payable', '=', True)),
             ],
         context={
             'date': If(Eval('accounting_date'),
                 Eval('accounting_date'),
                 Eval('invoice_date')),
             })
-    payment_term = fields.Many2One('account.invoice.payment_term',
-        'Payment Term', states=_states)
+    payment_term = fields.Many2One(
+        'account.invoice.payment_term', "Payment Term",
+        ondelete='RESTRICT', states=_states)
     alternative_payees = fields.Many2Many(
         'account.invoice.alternative_payee', 'invoice', 'party',
         "Alternative Payee", states=_states,
         size=If(~Eval('move'), 1, None),
         context={
             'company': Eval('company', -1),
             },
         depends=['company'])
     lines = fields.One2Many('account.invoice.line', 'invoice', 'Lines',
         domain=[
             ('company', '=', Eval('company', -1)),
             ('currency', '=', Eval('currency', -1)),
             ['OR',
+                ('account', '=', None),
+                ('account', '!=', Eval('account', -1)),
+                ],
+            ['OR',
                 ('invoice_type', '=', Eval('type')),
                 ('invoice_type', '=', None),
                 ],
             ['OR',
                 ('party', '=', Eval('party', -1)),
                 ('party', '=', None),
                 ],
             ],
         states={
             'readonly': (
                 (Eval('state') != 'draft')
                 | ~Eval('company')
-                | ~Eval('currency')),
+                | ~Eval('currency')
+                | ~Eval('account')),
+            })
+    taxes = fields.One2Many(
+        'account.invoice.tax', 'invoice', 'Tax Lines',
+        domain=[
+            ('account', '!=', Eval('account', -1)),
+            ],
+        states={
+            'readonly': (
+                (Eval('state') != 'draft')
+                | ~Eval('account')),
             })
-    taxes = fields.One2Many('account.invoice.tax', 'invoice', 'Tax Lines',
-        states=_states)
     comment = fields.Text('Comment', states=_states)
     origins = fields.Function(fields.Char('Origins'), 'get_origins')
     untaxed_amount = fields.Function(Monetary(
             "Untaxed", currency='currency', digits='currency'),
         'get_amount', searcher='search_untaxed_amount')
     tax_amount = fields.Function(Monetary(
             "Tax", currency='currency', digits='currency'),
@@ -216,14 +234,18 @@
             'account.move.line', None, None, 'Lines to Pay'),
         'get_lines_to_pay')
     payment_lines = fields.Many2Many('account.invoice-account.move.line',
         'invoice', 'line', string='Payment Lines',
         domain=[
             ('account', '=', Eval('account', -1)),
             ['OR',
+                ('currency', '=', Eval('currency', -1)),
+                ('second_currency', '=', Eval('currency', -1)),
+                ],
+            ['OR',
                 ('party', 'in', [None, Eval('party', -1)]),
                 ('party', 'in', Eval('alternative_payees', [])),
                 ],
             ['OR',
                 ('invoice_payment', '=', None),
                 ('invoice_payment', '=', Eval('id', -1)),
                 ],
@@ -253,14 +275,16 @@
         'get_amount_to_pay')
     invoice_report_cache = fields.Binary('Invoice Report', readonly=True,
         file_id=file_id, store_prefix=store_prefix)
     invoice_report_cache_id = fields.Char('Invoice Report ID', readonly=True)
     invoice_report_format = fields.Char('Invoice Report Format', readonly=True)
     allow_cancel = fields.Function(
         fields.Boolean("Allow Cancel Invoice"), 'get_allow_cancel')
+    has_payment_method = fields.Function(
+        fields.Boolean("Has Payment Method"), 'get_has_payment_method')
 
     del _states
 
     @classmethod
     def __setup__(cls):
         cls.number.search_unaccented = False
         cls.reference.search_unaccented = False
@@ -334,16 +358,18 @@
                             ('type', '!=', 'in'),
                         ],
                     'invisible': (~Eval('state').in_(['draft', 'validated'])
                         | ((Eval('state') == 'posted') & Bool(Eval('move')))),
                     'depends': ['state', 'move'],
                     },
                 'pay': {
-                    'invisible': Eval('state') != 'posted',
-                    'depends': ['state'],
+                    'invisible': (
+                        (Eval('state') != 'posted')
+                        | ~Eval('has_payment_method', False)),
+                    'depends': ['state', 'has_payment_method'],
                     },
                 'reschedule_lines_to_pay': {
                     'invisible': (
                         ~Eval('lines_to_pay') | Eval('reconciled', False)),
                     'depends': ['lines_to_pay', 'reconciled'],
                     },
                 'delegate_lines_to_pay': {
@@ -425,14 +451,17 @@
         cursor.execute(*sql_table.update(
                 [sql_table.state], ['cancelled'],
                 where=sql_table.state == 'cancel'))
 
         # Migration from 5.8: drop foreign key for sequence
         table.drop_fk('sequence')
 
+        # Migration from 6.6: drop not null on journal
+        table.not_null_action('journal', 'remove')
+
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
         return [CharLength(table.number), table.number]
 
     @staticmethod
     def default_type():
@@ -451,52 +480,51 @@
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('company')
     def on_change_with_company_party(self, name=None):
-        if self.company:
-            return self.company.party.id
+        return self.company.party if self.company else None
 
     @fields.depends(
         'state', 'account', 'party', 'type', 'accounting_date', 'invoice_date')
     def on_change_with_account(self):
         if self.state != 'draft':
             return self.account
         account = None
         if self.party:
             with Transaction().set_context(
                     date=self.accounting_date or self.invoice_date):
                 if self.type == 'out':
                     account = self.party.account_receivable_used
                 elif self.type == 'in':
                     account = self.party.account_payable_used
-        return account.id if account else None
-
-    @fields.depends('type')
-    def on_change_type(self):
-        Journal = Pool().get('account.journal')
-        journal_type = {
-            'out': 'revenue',
-            'in': 'expense',
-            }.get(self.type or 'out', 'revenue')
-        journals = Journal.search([
-                ('type', '=', journal_type),
-                ], limit=1)
-        if journals:
-            self.journal, = journals
+        return account
 
     @classmethod
     def _journal_types(cls, invoice_type):
         if invoice_type == 'out':
             return ['revenue']
         else:
             return ['expense']
 
+    @fields.depends('state', 'journal', 'type')
+    def on_change_with_journal(self, pattern=None):
+        pool = Pool()
+        Journal = pool.get('account.journal')
+        if self.state != 'draft':
+            return self.journal
+        pattern = pattern.copy() if pattern is not None else {}
+        pattern.setdefault('type', {
+                'out': 'revenue',
+                'in': 'expense',
+                }.get(self.type))
+        return Journal.find(pattern)
+
     @classmethod
     def order_accounting_date(cls, tables):
         table, _ = tables[None]
         return [Coalesce(table.accounting_date, table.invoice_date)]
 
     @fields.depends('party', 'type')
     def on_change_party(self):
@@ -908,14 +936,30 @@
     def get_allow_cancel(self, name):
         if self.state in {'draft', 'validated'}:
             return True
         if self.state == 'posted':
             return self.type == 'in' or self.company.cancel_invoice_out
         return False
 
+    @classmethod
+    def get_has_payment_method(cls, invoices, name):
+        pool = Pool()
+        Method = pool.get('account.invoice.payment.method')
+        methods = {}
+        for (company, account), sub_invoices in groupby(
+                invoices, key=lambda i: (i.company, i.account)):
+            sub_invoice_ids = [i.id for i in sub_invoices]
+            value = bool(Method.search([
+                        ('company', '=', company.id),
+                        ('debit_account', '!=', account.id),
+                        ('credit_account', '!=', account.id),
+                        ], limit=1))
+            methods.update(dict.fromkeys(sub_invoice_ids, value))
+        return methods
+
     @property
     def taxable_lines(self):
         taxable_lines = []
         for line in self.lines:
             if getattr(line, 'type', None) == 'line':
                 taxable_lines.extend(line.taxable_lines)
         return taxable_lines
@@ -1071,19 +1115,19 @@
                         invoice=self.rec_name,
                         date=lang.strftime(min(past_payment_term_dates))))
         if not self.currency.is_zero(remainder_total_currency):
             move_lines[-1].amount_second_currency -= \
                 remainder_total_currency
 
         accounting_date = self.accounting_date or self.invoice_date or today
-        period_id = Period.find(self.company.id, date=accounting_date)
+        period = Period.find(self.company, date=accounting_date)
 
         move = Move()
         move.journal = self.journal
-        move.period = period_id
+        move.period = period
         move.date = accounting_date
         move.origin = self
         move.company = self.company
         move.lines = move_lines
         return move
 
     @classmethod
@@ -1152,19 +1196,18 @@
 
         if pattern is None:
             pattern = {}
         else:
             pattern = pattern.copy()
 
         accounting_date = self.accounting_date or self.invoice_date
-        period_id = Period.find(
-            self.company.id, date=accounting_date,
+        period = Period.find(
+            self.company, date=accounting_date,
             test_state=self.type != 'in')
 
-        period = Period(period_id)
         fiscalyear = period.fiscalyear
         pattern.setdefault('company', self.company.id)
         pattern.setdefault('fiscalyear', fiscalyear.id)
         pattern.setdefault('period', period.id)
 
         for invoice_sequence in fiscalyear.invoice_sequences:
             if invoice_sequence.match(pattern):
@@ -1236,15 +1279,14 @@
         if operator.startswith('!') or operator.startswith('not '):
             bool_op = 'AND'
         else:
             bool_op = 'OR'
         return [bool_op,
             ('number', *clause[1:]),
             ('reference', *clause[1:]),
-            ('party', *clause[1:]),
             ]
 
     def get_origins(self, name):
         return ', '.join(set(filter(None,
                     (l.origin_name for l in self.lines))))
 
     @classmethod
@@ -1304,128 +1346,136 @@
         default.setdefault('invoice_report_cache', None)
         default.setdefault('invoice_report_cache_id', None)
         default.setdefault('invoice_report_format', None)
         default.setdefault('payment_lines', None)
         default.setdefault('invoice_date', None)
         default.setdefault('accounting_date', None)
         default.setdefault('payment_term_date', None)
-        default.setdefault('lines_to_pay', None)
         return super(Invoice, cls).copy(invoices, default=default)
 
     @classmethod
     def validate(cls, invoices):
         super(Invoice, cls).validate(invoices)
         for invoice in invoices:
             invoice.check_payment_lines()
 
-    @classmethod
-    def validate_fields(cls, invoices, field_names):
-        super().validate_fields(invoices, field_names)
-        cls.check_same_account(invoices, field_names)
-
-    @classmethod
-    def check_same_account(cls, invoices, field_names=None):
-        if field_names and not (field_names & {'lines', 'account'}):
-            return
-        for invoice in invoices:
-            for line in invoice.lines:
-                if (line.type == 'line'
-                        and line.account == invoice.account):
-                    raise InvoiceValidationError(
-                        gettext(
-                            'account_invoice.msg_invoice_same_account_line',
-                            account=invoice.account.rec_name,
-                            invoice=invoice.rec_name,
-                            line=line.rec_name))
-
     def check_payment_lines(self):
-        amount = sum(l.debit - l.credit for l in self.lines_to_pay)
-        payment_amount = sum(l.debit - l.credit for l in self.payment_lines)
+        def balance(line):
+            if self.currency == line.second_currency:
+                return line.amount_second_currency
+            elif self.currency == self.company.currency:
+                return line.debit - line.credit
+            else:
+                return 0
+        amount = sum(map(balance, self.lines_to_pay))
+        payment_amount = sum(map(balance, self.payment_lines))
         if abs(amount) < abs(payment_amount):
             raise InvoiceValidationError(
                 gettext('account_invoice'
                     '.msg_invoice_payment_lines_greater_amount',
                     invoice=self.rec_name))
 
-    def get_reconcile_lines_for_amount(self, amount, party=None):
+    def get_reconcile_lines_for_amount(self, amount, currency, party=None):
         '''
         Return list of lines and the remainder to make reconciliation.
         '''
         Result = namedtuple('Result', ['lines', 'remainder'])
 
         if party is None:
             party = self.party
 
+        assert currency in [self.currency, self.company.currency]
+
+        def balance(line):
+            if currency == line.second_currency:
+                return line.amount_second_currency
+            elif currency == self.company.currency:
+                return line.debit - line.credit
+            else:
+                return 0
+
         lines = [
             l for l in self.payment_lines + self.lines_to_pay
             if not l.reconciliation
             and (not self.account.party_required or l.party == party)]
 
         best = Result([], self.total_amount)
         for n in range(len(lines), 0, -1):
             for comb_lines in combinations(lines, n):
-                remainder = sum((l.debit - l.credit) for l in comb_lines)
+                remainder = sum(map(balance, comb_lines))
                 remainder -= amount
                 result = Result(list(comb_lines), remainder)
-                if self.currency.is_zero(remainder):
+                if currency.is_zero(remainder):
                     return result
                 if abs(remainder) < abs(best.remainder):
                     best = result
         return best
 
-    def pay_invoice(self, amount, payment_method, date, description=None,
-            amount_second_currency=None, second_currency=None, overpayment=0,
-            overpayment_second_currency=0, party=None):
+    def pay_invoice(
+            self, amount, payment_method, date, description=None,
+            overpayment=0, party=None):
         '''
         Adds a payment of amount to an invoice using the journal, date and
         description.
         If overpayment is set, then only the amount minus the overpayment is
         used to pay off the invoice.
         Returns the payment lines.
         '''
         pool = Pool()
+        Currency = pool.get('currency.currency')
         Move = pool.get('account.move')
         Line = pool.get('account.move.line')
         Period = pool.get('account.period')
 
         if party is None:
             party = self.party
 
         pay_line = Line(account=self.account)
         counterpart_line = Line()
         lines = [pay_line, counterpart_line]
 
         pay_amount = amount - overpayment
-        if amount_second_currency is not None:
-            pay_amount_second_currency = (
-                amount_second_currency - overpayment_second_currency)
+        if self.currency != self.company.currency:
+            amount_second_currency = pay_amount
+            second_currency = self.currency
+            overpayment_second_currency = overpayment
+            with Transaction().set_context(date=date):
+                amount = Currency.compute(
+                    self.currency, amount, self.company.currency)
+                overpayment = Currency.compute(
+                    self.currency, overpayment, self.company.currency)
+                pay_amount = amount - overpayment
+        else:
+            amount_second_currency = None
+            second_currency = None
+            overpayment_second_currency = None
         if pay_amount >= 0:
             if self.type == 'out':
                 pay_line.debit, pay_line.credit = 0, pay_amount
             else:
                 pay_line.debit, pay_line.credit = pay_amount, 0
         else:
             if self.type == 'out':
                 pay_line.debit, pay_line.credit = -pay_amount, 0
             else:
                 pay_line.debit, pay_line.credit = 0, -pay_amount
         if amount_second_currency is not None:
             pay_line.amount_second_currency = (
-                pay_amount_second_currency.copy_sign(
+                amount_second_currency.copy_sign(
                     pay_line.debit - pay_line.credit))
             pay_line.second_currency = second_currency
 
         if overpayment:
             overpayment_line = Line(account=self.account)
             lines.insert(1, overpayment_line)
             overpayment_line.debit = (
                 abs(overpayment) if pay_line.debit else 0)
             overpayment_line.credit = (
                 abs(overpayment) if pay_line.credit else 0)
-            if amount_second_currency is not None:
+            if overpayment_second_currency is not None:
                 overpayment_line.amount_second_currency = (
                     overpayment_second_currency.copy_sign(
                         overpayment_line.debit - overpayment_line.credit))
                 overpayment_line.second_currency = second_currency
 
         counterpart_line.debit = abs(amount) if pay_line.credit else 0
         counterpart_line.credit = abs(amount) if pay_line.debit else 0
@@ -1441,18 +1491,18 @@
                     counterpart_line.debit - counterpart_line.credit))
             counterpart_line.second_currency = second_currency
 
         for line in lines:
             if line.account.party_required:
                 line.party = party
 
-        period_id = Period.find(self.company.id, date=date)
+        period = Period.find(self.company, date=date)
 
         move = Move(
-            journal=payment_method.journal, period=period_id, date=date,
+            journal=payment_method.journal, period=period, date=date,
             origin=self, description=description,
             company=self.company, lines=lines)
         move.save()
         Move.post([move])
 
         payment_lines = [l for l in move.lines if l.account == self.account]
         payment_line = [l for l in payment_lines
@@ -1926,14 +1976,26 @@
         'account.invoice', "Invoice", ondelete='CASCADE',
         states={
             'required': (~Eval('invoice_type') & Eval('party')
                 & Eval('currency') & Eval('company')),
             'invisible': Bool(Eval('context', {}).get('standalone')),
             'readonly': _states['readonly'] & Bool(Eval('invoice')),
             })
+    invoice_party = fields.Function(
+        fields.Many2One(
+            'party.party', "Party",
+            context={
+                'company': Eval('company', -1),
+                },
+            depends=['company']),
+        'on_change_with_invoice_party', searcher='search_invoice_party')
+    invoice_description = fields.Function(
+        fields.Char("Invoice Description"),
+        'on_change_with_invoice_description',
+        searcher='search_invoice_description')
     invoice_state = fields.Function(
         fields.Selection('get_invoice_states', "Invoice State"),
         'on_change_with_invoice_state')
     invoice_type = fields.Selection(
         'get_invoice_types', "Invoice Type",
         states={
             'readonly': Eval('context', {}).get('type') | Eval('type'),
@@ -2081,14 +2143,15 @@
         super(InvoiceLine, cls).__setup__()
         cls._check_modify_exclude = {'note', 'origin'}
 
         # Set account domain dynamically for kind
         cls.account.domain = [
             ('closed', '!=', True),
             ('company', '=', Eval('company', -1)),
+            ('id', '!=', Eval('_parent_invoice', {}).get('account', -1)),
             If(Bool(Eval('_parent_invoice')),
                 If(Eval('_parent_invoice', {}).get('type') == 'out',
                     cls._account_domain('out'),
                     If(Eval('_parent_invoice', {}).get('type') == 'in',
                         cls._account_domain('in'),
                         ['OR',
                             cls._account_domain('out'),
@@ -2180,14 +2243,43 @@
     def default_company():
         return Transaction().context.get('company')
 
     @staticmethod
     def default_type():
         return 'line'
 
+    @fields.depends('party', 'invoice', '_parent_invoice.party')
+    def on_change_with_invoice_party(self, name=None):
+        if self.invoice and self.invoice.party:
+            return self.invoice.party
+        elif self.party:
+            return self.party
+
+    @classmethod
+    def search_invoice_party(cls, name, clause):
+        operator = clause[1]
+        if operator.startswith('!') or operator.startswith('not '):
+            bool_op = 'AND'
+        else:
+            bool_op = 'OR'
+        nested = clause[0][len(name) + 1:]
+        return [bool_op,
+            ('invoice.party' + nested, *clause[1:]),
+            ('party' + nested, *clause[1:]),
+            ]
+
+    @fields.depends('invoice', '_parent_invoice.description')
+    def on_change_with_invoice_description(self, name=None):
+        if self.invoice:
+            return self.invoice.description
+
+    @classmethod
+    def search_invoice_description(cls, name, clause):
+        return [('invoice.description', *clause[1:])]
+
     @classmethod
     def default_invoice_state(cls):
         return 'draft'
 
     @classmethod
     def get_invoice_states(cls):
         pool = Pool()
@@ -2404,16 +2496,15 @@
 
         category = self.product.default_uom.category
         if not self.unit or self.unit.category != category:
             self.unit = self.product.default_uom.id
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends('account', 'product', 'invoice',
         '_parent_invoice.party', '_parent_invoice.type',
         'party', 'invoice', 'invoice_type',
         methods=['_get_tax_rule_pattern'])
     def on_change_account(self):
         if self.product:
@@ -2523,54 +2614,33 @@
         actions = iter(args)
         for lines, values in zip(actions, actions):
             cls.check_modify(lines, set(values))
         super(InvoiceLine, cls).write(*args)
 
     @classmethod
     def create(cls, vlist):
-        Invoice = Pool().get('account.invoice')
-        invoice_ids = []
-        for vals in vlist:
-            if vals.get('invoice'):
-                invoice_ids.append(vals.get('invoice'))
-        for invoice in Invoice.browse(invoice_ids):
-            if invoice.state in ('posted', 'paid', 'cancelled'):
+        pool = Pool()
+        Invoice = pool.get('account.invoice')
+        invoice_ids = filter(None, {v.get('invoice') for v in vlist})
+        for invoice in Invoice.browse(list(invoice_ids)):
+            if invoice.state != 'draft':
                 raise AccessError(
                     gettext('account_invoice.msg_invoice_line_create',
                         invoice=invoice.rec_name))
         return super(InvoiceLine, cls).create(vlist)
 
     @classmethod
     def copy(cls, lines, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('origin', None)
         return super(InvoiceLine, cls).copy(lines, default=default)
 
-    @classmethod
-    def validate_fields(cls, lines, field_names):
-        super().validate_fields(lines, field_names)
-        cls.check_same_account(lines, field_names)
-
-    @classmethod
-    def check_same_account(cls, lines, field_names=None):
-        if field_names and not (field_names & {'type', 'invoice', 'account'}):
-            return
-        for line in lines:
-            if (line.type == 'line'
-                    and line.invoice
-                    and line.account == line.invoice.account):
-                raise InvoiceLineValidationError(
-                    gettext('account_invoice.msg_invoice_same_account_line',
-                        account=line.account.rec_name,
-                        invoice=line.invoice.rec_name,
-                        line=line.rec_name))
-
     def _compute_taxes(self):
         pool = Pool()
         Currency = pool.get('currency.currency')
         TaxLine = pool.get('account.tax.line')
 
         tax_lines = []
         if self.type != 'line':
@@ -2693,14 +2763,15 @@
     sequence_number = fields.Function(fields.Integer('Sequence Number'),
             'get_sequence_number')
     account = fields.Many2One('account.account', 'Account', required=True,
         domain=[
             ('type', '!=', None),
             ('closed', '!=', True),
             ('company', '=', Eval('_parent_invoice', {}).get('company', 0)),
+            ('id', '!=', Eval('_parent_invoice', {}).get('account', -1)),
             ],
         states=_states, depends={'invoice'})
     base = Monetary(
         "Base", currency='currency', digits='currency', required=True,
         states=_states)
     amount = Monetary(
         "Amount", currency='currency', digits='currency', required=True,
@@ -2708,18 +2779,27 @@
         depends={'tax', 'base', 'manual'})
     currency = fields.Function(fields.Many2One('currency.currency',
         'Currency'), 'on_change_with_currency')
     manual = fields.Boolean('Manual', states=_states)
     tax = fields.Many2One('account.tax', 'Tax',
         ondelete='RESTRICT',
         domain=[
+            ['OR',
+                ('group', '=', None),
+                ('group.kind', 'in',
+                    If(Eval('_parent_invoice', {}).get('type') == 'out',
+                        ['sale', 'both'],
+                        ['purchase', 'both']),
+                    )],
             ('company', '=', Eval('_parent_invoice', {}).get('company', 0)),
             ],
         states={
-            'readonly': ~Eval('manual', False) | _states['readonly'],
+            'readonly': (
+                ~Eval('manual', False) | ~Bool(Eval('invoice'))
+                | _states['readonly']),
             },
         depends={'invoice'})
     legal_notice = fields.Text("Legal Notice", states=_states)
 
     del _states
 
     @classmethod
@@ -2764,16 +2844,15 @@
     @fields.depends('invoice', '_parent_invoice.state')
     def on_change_with_invoice_state(self, name=None):
         if self.invoice:
             return self.invoice.state
 
     @fields.depends('invoice', '_parent_invoice.currency')
     def on_change_with_currency(self, name=None):
-        if self.invoice:
-            return self.invoice.currency.id
+        return self.invoice.currency if self.invoice else None
 
     @fields.depends('tax', 'invoice', '_parent_invoice.party', 'base')
     def on_change_tax(self):
         Tax = Pool().get('account.tax')
         if not self.tax:
             return
         if self.invoice:
@@ -2857,43 +2936,24 @@
     def write(cls, *args):
         taxes = sum(args[0::2], [])
         cls.check_modify(taxes)
         super(InvoiceTax, cls).write(*args)
 
     @classmethod
     def create(cls, vlist):
-        Invoice = Pool().get('account.invoice')
-        invoice_ids = []
-        for vals in vlist:
-            if vals.get('invoice'):
-                invoice_ids.append(vals['invoice'])
-        for invoice in Invoice.browse(invoice_ids):
-            if invoice.state in ('posted', 'paid', 'cancelled'):
+        pool = Pool()
+        Invoice = pool.get('account.invoice')
+        invoice_ids = filter(None, {v.get('invoice') for v in vlist})
+        for invoice in Invoice.browse(list(invoice_ids)):
+            if invoice.state != 'draft':
                 raise AccessError(
-                    gettext('account_invoice.msg_invoice_tax_create',
+                    gettext('account_invoice.msg_invoice_tax_create_draft',
                         invoice=invoice.rec_name))
         return super(InvoiceTax, cls).create(vlist)
 
-    @classmethod
-    def validate_fields(cls, taxes, field_names):
-        super().validate_fields(taxes, field_names)
-        cls.check_same_account(taxes, field_names)
-
-    @classmethod
-    def check_same_account(cls, taxes, field_names=None):
-        if field_names and not (field_names & {'account', 'invoice'}):
-            return
-        for tax in taxes:
-            if tax.account == tax.invoice.account:
-                raise InvoiceTaxValidationError(
-                    gettext('account_invoice.msg_invoice_same_account_line',
-                        account=tax.account.rec_name,
-                        invoice=tax.invoice.rec_name,
-                        line=tax.rec_name))
-
     def get_move_lines(self):
         '''
         Return a list of move lines instances for invoice tax
         '''
         Currency = Pool().get('currency.currency')
         pool = Pool()
         Currency = pool.get('currency.currency')
@@ -3073,15 +3133,15 @@
         'party.party', None, None, "Payees", readonly=True,
         context={
             'company': Eval('company', -1),
             },
         depends=['company'])
     amount = Monetary(
         "Amount", currency='currency', digits='currency', required=True)
-    currency = fields.Many2One('currency.currency', 'Currency', required=True)
+    currency = fields.Many2One('currency.currency', 'Currency', readonly=True)
     description = fields.Char('Description', size=None)
     company = fields.Many2One('company.company', "Company", readonly=True)
     invoice_account = fields.Many2One(
         'account.account', "Invoice Account", readonly=True)
     payment_method = fields.Many2One(
         'account.invoice.payment.method', "Payment Method", required=True,
         domain=[
@@ -3114,27 +3174,22 @@
         states={
             'invisible': Eval('type') != 'writeoff',
             'required': Eval('type') == 'writeoff',
             })
     amount = Monetary(
         "Payment Amount",
         currency='currency', digits='currency', readonly=True)
-    currency = fields.Many2One('currency.currency', 'Payment Currency',
-            readonly=True)
+    currency = fields.Many2One('currency.currency', "Currency", readonly=True)
     amount_writeoff = Monetary(
         "Write-Off Amount",
-        currency='currency_writeoff', digits='currency_writeoff',
+        currency='currency', digits='currency',
         readonly=True,
         states={
             'invisible': Eval('type') != 'writeoff',
             })
-    currency_writeoff = fields.Many2One('currency.currency',
-        'Write-Off Currency', readonly=True, states={
-            'invisible': Eval('type') != 'writeoff',
-            })
     lines_to_pay = fields.Many2Many('account.move.line', None, None,
             'Lines to Pay', readonly=True)
     lines = fields.Many2Many('account.move.line', None, None, 'Lines',
         domain=[
             ('id', 'in', Eval('lines_to_pay')),
             ('reconciliation', '=', None),
             ],
@@ -3144,43 +3199,42 @@
     payment_lines = fields.Many2Many('account.move.line', None, None,
         'Payment Lines', readonly=True,
         states={
             'invisible': Eval('type') != 'writeoff',
             })
     company = fields.Many2One('company.company', 'Company', readonly=True)
     invoice = fields.Many2One('account.invoice', 'Invoice', readonly=True)
-    date = fields.Date('Date', readonly=True)
 
     @staticmethod
     def default_type():
         return 'partial'
 
-    @fields.depends('lines', 'amount', 'currency', 'currency_writeoff',
-        'invoice', 'payment_lines', 'date')
+    @fields.depends(
+        'lines', 'amount', 'currency', 'invoice', 'payment_lines', 'company')
     def on_change_lines(self):
-        Currency = Pool().get('currency.currency')
-
-        if self.currency and self.currency_writeoff:
-            with Transaction().set_context(date=self.date):
-                amount = Currency.compute(self.currency, self.amount,
-                    self.currency_writeoff)
-        else:
-            amount = self.amount
-
         self.amount_writeoff = Decimal('0.0')
         if not self.invoice:
             return
+
+        def balance(line):
+            if self.currency == line.second_currency:
+                return line.amount_second_currency
+            elif self.currency == self.company.currency:
+                return line.debit - line.credit
+            else:
+                return 0
+
         for line in self.lines:
-            self.amount_writeoff += line.debit - line.credit
+            self.amount_writeoff += balance(line)
         for line in self.payment_lines:
-            self.amount_writeoff += line.debit - line.credit
+            self.amount_writeoff += balance(line)
         if self.invoice.type == 'in':
-            self.amount_writeoff = - self.amount_writeoff - amount
+            self.amount_writeoff = - self.amount_writeoff - self.amount
         else:
-            self.amount_writeoff = self.amount_writeoff - amount
+            self.amount_writeoff = self.amount_writeoff - self.amount
 
 
 class PayInvoice(Wizard):
     'Pay Invoice'
     __name__ = 'account.invoice.pay'
     start = StateView('account.invoice.pay.start',
         'account_invoice.pay_start_view_form', [
@@ -3196,19 +3250,19 @@
     pay = StateTransition()
 
     @classmethod
     def __setup__(cls):
         super(PayInvoice, cls).__setup__()
         cls.__rpc__['create'].fresh_session = True
 
-    def get_reconcile_lines_for_amount(self, invoice, amount):
+    def get_reconcile_lines_for_amount(self, invoice, amount, currency):
         if invoice.type == 'in':
             amount *= -1
         return invoice.get_reconcile_lines_for_amount(
-            amount, party=self.start.payee)
+            amount, currency, party=self.start.payee)
 
     def default_start(self, fields):
         default = {}
         invoice = self.record
         if not invoice.alternative_payees:
             default['payee'] = invoice.party.id
         else:
@@ -3222,129 +3276,90 @@
         default['currency'] = invoice.currency.id
         default['amount'] = (invoice.amount_to_pay_today
             or invoice.amount_to_pay)
         default['invoice_account'] = invoice.account.id
         return default
 
     def transition_choice(self):
-        pool = Pool()
-        Currency = pool.get('currency.currency')
-
         invoice = self.record
-
-        with Transaction().set_context(date=self.start.date):
-            amount = Currency.compute(self.start.currency,
-                self.start.amount, invoice.company.currency)
-            amount_invoice = Currency.compute(
-                self.start.currency, self.start.amount, invoice.currency)
-        _, remainder = self.get_reconcile_lines_for_amount(invoice, amount)
-        if (remainder == Decimal('0.0')
-                and amount_invoice <= invoice.amount_to_pay):
+        amount = self.start.amount
+        currency = self.start.currency
+        _, remainder = self.get_reconcile_lines_for_amount(
+            invoice, amount, currency)
+        if remainder == Decimal('0.0') and amount <= invoice.amount_to_pay:
             return 'pay'
         return 'ask'
 
     def default_ask(self, fields):
-        pool = Pool()
-        Currency = pool.get('currency.currency')
-
         default = {}
         invoice = self.record
+        amount = self.start.amount
+        currency = self.start.currency
         default['lines_to_pay'] = [x.id for x in invoice.lines_to_pay
                 if not x.reconciliation]
 
-        default['amount'] = self.start.amount
-        default['date'] = self.start.date
-        default['currency'] = self.start.currency.id
+        default['amount'] = amount
+        default['currency'] = currency.id
         default['company'] = invoice.company.id
 
-        with Transaction().set_context(date=self.start.date):
-            amount = Currency.compute(self.start.currency,
-                self.start.amount, invoice.company.currency)
-            amount_invoice = Currency.compute(
-                self.start.currency, self.start.amount, invoice.currency)
-
-        if invoice.company.currency.is_zero(amount):
+        if currency.is_zero(amount):
             lines = invoice.lines_to_pay
         else:
-            lines, _ = self.get_reconcile_lines_for_amount(invoice, amount)
+            lines, _ = self.get_reconcile_lines_for_amount(
+                invoice, amount, currency)
         default['lines'] = [x.id for x in lines]
 
         for line_id in default['lines'][:]:
             if line_id not in default['lines_to_pay']:
                 default['lines'].remove(line_id)
 
         default['payment_lines'] = [x.id for x in invoice.payment_lines
                 if not x.reconciliation]
 
-        default['currency_writeoff'] = invoice.company.currency.id
         default['invoice'] = invoice.id
 
-        if (amount_invoice > invoice.amount_to_pay
-                or invoice.company.currency.is_zero(amount)):
+        if amount >= invoice.amount_to_pay or currency.is_zero(amount):
             default['type'] = 'writeoff'
         return default
 
     def transition_pay(self):
         pool = Pool()
-        Currency = pool.get('currency.currency')
         MoveLine = pool.get('account.move.line')
         Lang = pool.get('ir.lang')
 
         invoice = self.record
+        amount = self.start.amount
+        currency = self.start.currency
 
-        with Transaction().set_context(date=self.start.date):
-            amount = Currency.compute(self.start.currency,
-                self.start.amount, invoice.company.currency)
-            amount_invoice = Currency.compute(
-                self.start.currency, self.start.amount, invoice.currency)
-
-        reconcile_lines, remainder = \
-            self.get_reconcile_lines_for_amount(invoice, amount)
-
-        amount_second_currency = None
-        second_currency = None
-        if self.start.currency != invoice.company.currency:
-            amount_second_currency = self.start.amount
-            second_currency = self.start.currency
+        reconcile_lines, remainder = (
+            self.get_reconcile_lines_for_amount(invoice, amount, currency))
 
         overpayment = 0
-        overpayment_second_currency = 0
-        if (0 <= invoice.amount_to_pay < amount_invoice
-                or amount_invoice < invoice.amount_to_pay <= 0):
+        if (0 <= invoice.amount_to_pay < amount
+                or amount < invoice.amount_to_pay <= 0):
             if self.ask.type == 'partial':
                 lang = Lang.get()
                 raise PayInvoiceError(
                     gettext('account_invoice'
                         '.msg_invoice_pay_amount_greater_amount_to_pay',
                         invoice=invoice.rec_name,
                         amount_to_pay=lang.currency(
                             invoice.amount_to_pay, invoice.currency)))
             else:
                 if not invoice.amount_to_pay:
                     raise PayInvoiceError(
                         gettext('account_invoice.msg_invoice_overpay_paid',
                             invoice=invoice.rec_name))
-                with Transaction().set_context(date=self.start.date):
-                    overpayment = Currency.compute(
-                        invoice.currency,
-                        amount_invoice - invoice.amount_to_pay,
-                        invoice.company.currency)
-                    if second_currency:
-                        overpayment_second_currency = Currency.compute(
-                            invoice.currency,
-                            amount_invoice - invoice.amount_to_pay,
-                            second_currency)
+                overpayment = amount - invoice.amount_to_pay
 
         lines = []
-        if not invoice.company.currency.is_zero(amount):
-            lines = invoice.pay_invoice(amount,
-                self.start.payment_method, self.start.date,
-                self.start.description, amount_second_currency,
-                second_currency, overpayment, overpayment_second_currency,
-                party=self.start.payee)
+        if not currency.is_zero(amount):
+            lines = invoice.pay_invoice(
+                amount, self.start.payment_method, self.start.date,
+                self.start.description, overpayment, party=self.start.payee)
 
         if remainder:
             if self.ask.type != 'partial':
                 to_reconcile = {l for l in self.ask.lines}
                 to_reconcile.update(
                     l for l in invoice.payment_lines
                     if not l.reconciliation
```

### Comparing `trytond_account_invoice-6.6.5/invoice.xml` & `trytond_account_invoice-6.8.0/invoice.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/invoice.xml` & `trytond_account_invoice-6.8.0/invoice.xml`

```diff
@@ -119,14 +119,54 @@
     <record model="ir.action.act_window.domain" id="act_invoice_in_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_invoice_in_form"/>
     </record>
     <menuitem parent="menu_invoices" action="act_invoice_in_form" sequence="10" id="menu_invoice_in_form"/>
+    <record model="ir.action.act_window" id="act_invoice_relate">
+      <field name="name">Invoices</field>
+      <field name="res_model">account.invoice</field>
+      <field name="domain" eval="[                 If(Eval('active_model') == 'party.party',                 ('party', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_invoice_relate_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="invoice_view_tree"/>
+      <field name="act_window" ref="act_invoice_relate"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_invoice_relate_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="invoice_view_form"/>
+      <field name="act_window" ref="act_invoice_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_invoice_relate_pending">
+      <field name="name">Pending</field>
+      <field name="sequence" eval="10"/>
+      <field name="domain" eval="[('state', 'not in', ['paid', 'cancelled'])]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_invoice_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_invoice_relate_paid">
+      <field name="name">Paid</field>
+      <field name="sequence" eval="20"/>
+      <field name="domain" eval="[('state', '=', 'paid')]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_invoice_relate"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_invoice_relate_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_invoice_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_invoice_relate_keyword_party">
+      <field name="keyword">form_relate</field>
+      <field name="model">party.party,-1</field>
+      <field name="action" ref="act_invoice_relate"/>
+    </record>
     <record model="ir.model.access" id="access_invoice">
       <field name="model" search="[('model', '=', 'account.invoice')]"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
```

### Comparing `trytond_account_invoice-6.6.5/locale/bg.po` & `trytond_account_invoice-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,19 @@
 msgid "Currency Date"
 msgstr "Текуща дата"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Описание"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Адрес за фактура"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Дата на фактура"
@@ -307,14 +312,24 @@
 msgstr "Описание"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Фактура"
 
 #, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Описание"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Партньор"
+
+#, fuzzy
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Състояние на фактура"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Данъци на фактура"
@@ -398,26 +413,18 @@
 msgid "Write-Off Amount"
 msgstr "Сума за отписване"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Фирма"
 
-msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Валута при плащане"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Валута на отписване"
-
 #, fuzzy
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Дата"
+msgctxt "field:account.invoice.pay.ask,currency:"
+msgid "Currency"
+msgstr "Валута"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Фактура"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -819,27 +826,27 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Всичко фактури"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Фактури на доставчик"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Всичко фактури"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -905,14 +912,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Проверен"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Платен"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -937,18 +968,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -1002,28 +1033,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/ca.po` & `trytond_account_invoice-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr "Data moneda"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descripció"
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Té mètode de pagament"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Adreça de facturació"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Data factura"
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Descripció de la factura"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Tercer"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Estat de la factura"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Impostos de la factura"
@@ -376,24 +388,16 @@
 msgstr "Import del desajust"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Moneda de pagament"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Moneda del desajust"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -767,26 +771,26 @@
 msgid "Delegate Lines to Pay"
 msgstr "Delegar línies a pagar"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Factures"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Factures"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Factures de proveïdor"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Factures de client"
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Factures"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Mètodes de pagament de factura"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Terminis de pagament"
@@ -841,14 +845,40 @@
 msgstr "Comptabilitzada"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validada"
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Pagada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr "Pendent"
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+"Els assentaments \"%(moves)s\" tenen com origen les factures "
+"comptabilitzades \"%(invoices)s\"."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+"Al cancel·lar-les es conciliaran els apunts i es pagaran les factures. "
+"Potser voleu cancel·lar les factures primer."
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr "Per tancar el període heu de contabilitzar les factures \"%(invoices)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -879,21 +909,21 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Heu de cancel·lar la factura \"%(invoice)s\" per poder-la eliminar."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "No podeu la factura \"%(invoice)s\" perquè està numerada."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"No podeu afegir una línia a la factura \"%(invoice)s\" perquè està "
-"comptabilitzada, pagada o cancel·lada."
+"No podeu afegir línies a la factura \"%(invoice)s\" perquè no està en estat "
+"esborrany."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "No podeu modificar la línia \"%(line)s\" perquè la seva factura "
@@ -965,33 +995,25 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "La factura \"%(invoice)s\" genera una data de pagament \"%(date)s\" en el "
 "passat."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"No podeu utilitzar el mateix compte \"%(account)s\" a la factura "
-"\"%(invoice)s\" i a la línia \"%(line)s\"."
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "La factura \"%(invoice)s\" és similar a la factura \"%(similar)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"No podeu afegir impostos a la factura \"%(invoice)s\" perquè està "
-"comptabilitzada, pagada o cancel·lada."
+"No podeu afegir impostos a la factura \"%(invoice)s\" perquè no està en "
+"estat esborrany."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
 "Els impostos de la factura \"%(invoice)s\" no són correctes, heu de tornar a"
```

### Comparing `trytond_account_invoice-6.6.5/locale/cs.po` & `trytond_account_invoice-6.8.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -297,14 +302,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Invoice"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr ""
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -386,23 +400,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
+msgid "Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
@@ -474,31 +480,29 @@
 msgid "Debit Account"
 msgstr ""
 
 msgctxt "field:account.invoice.payment.method,journal:"
 msgid "Journal"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.payment.method,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:account.invoice.payment_term,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.payment_term,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,currency:"
 msgid "Currency"
@@ -789,26 +793,27 @@
 msgid "Delegate Lines to Pay"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Payment Terms"
@@ -865,14 +870,37 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -897,18 +925,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -962,28 +990,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
@@ -1109,15 +1131,14 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
-#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1286,15 +1307,14 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:account.invoice:"
 msgid "Invoice"
```

### Comparing `trytond_account_invoice-6.6.5/locale/de.po` & `trytond_account_invoice-6.8.0/locale/de.po`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr "Währungsdatum"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Beschreibung"
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Hat Zahlungsart"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Rechnungsadresse"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Rechnungsdatum"
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Rechnung"
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Rechnungsbeschreibung"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Partei"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Rechnungsstatus"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Steuern Rechnung"
@@ -376,25 +388,17 @@
 msgstr "Konto Ausbuchung"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
+msgid "Currency"
 msgstr "Währung"
 
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Währung Ausbuchung"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Datum"
-
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Rechnung"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
 msgstr "Positionen"
@@ -445,15 +449,15 @@
 
 msgctxt "field:account.invoice.pay.start,payees:"
 msgid "Payees"
 msgstr "Parteien für Zahlungsverkehr"
 
 msgctxt "field:account.invoice.pay.start,payment_method:"
 msgid "Payment Method"
-msgstr "Zahlungsmethode"
+msgstr "Zahlungsart"
 
 msgctxt "field:account.invoice.payment.method,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.invoice.payment.method,credit_account:"
 msgid "Credit Account"
@@ -734,15 +738,15 @@
 
 msgctxt "model:account.invoice.pay.start,name:"
 msgid "Pay Invoice"
 msgstr "Zahlung erfassen"
 
 msgctxt "model:account.invoice.payment.method,name:"
 msgid "Payment Method"
-msgstr "Zahlungsmethode"
+msgstr "Zahlungsart"
 
 msgctxt "model:account.invoice.payment_term,name:"
 msgid "Payment Term"
 msgstr "Zahlungsbedingung"
 
 msgctxt "model:account.invoice.payment_term.line,name:"
 msgid "Payment Term Line"
@@ -768,26 +772,26 @@
 msgid "Delegate Lines to Pay"
 msgstr "Zahlbare Positionen delegieren"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Rechnungen"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Rechnungen"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Lieferantenrechnungen"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Kundenrechnungen"
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Rechnungen"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Zahlungsarten"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Zahlungsbedingungen"
@@ -842,14 +846,41 @@
 msgstr "Festgeschrieben"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Geprüft"
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Bezahlt"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr "Ausstehend"
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+"Die Buchungssätze \"%(moves)s\" haben die festgeschriebenen Rechnungen "
+"\"%(invoices)s\" als Herkunft."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+"Die Stornierung wird zur Abstimmung der Buchungssätze und damit zur "
+"Bezahlung der zugehörigen Rechnungen führen. Um dies zu vermeiden sollten "
+"die Rechnungen zuerst annulliert werden."
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 "Um die Buchungszeiträume schließen zu können, müssen zuerst die Rechnungen "
 "\"%(invoices)s\" festgeschrieben werden."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
@@ -887,21 +918,21 @@
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht gelöscht werden, da ihr bereits eine "
 "Nummer zugewiesen wurde."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Zu Rechnung \"%(invoice)s\" kann keine Position mehr hinzugefügt werden, da "
-"sie festgeschrieben, bezahlt oder annulliert ist."
+"sie nicht mehr im Entwurfsstatus ist."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "Position \"%(line)s\" kann nicht verändert werden, da die zugehörige "
@@ -977,33 +1008,25 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "Die Rechnung \"%(invoice)s\" produziert ein Zahlungsdatum \"%(date)s\" in "
 "der Vergangenheit."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"Auf Rechnung \"%(invoice)s\" und Position \"%(lines)s\" kann nicht dasselbe "
-"Konto \"%(account)s\" verwendet werden."
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "Die Rechnungen \"%(invoices)s\" ist ähnlich zu Rechnung \"%(similar)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Zu Rechnung \"%(invoice)s\" kann keine Steuer hinzugefügt werden, da sie "
-"bereits festgeschrieben, bezahlt oder annulliert ist."
+"mehr im Entwurfsstatus ist."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
 "Die Steuern auf Rechnung \"%(invoice)s\" sind falsch. Die Rechnung muss "
```

### Comparing `trytond_account_invoice-6.6.5/locale/es.po` & `trytond_account_invoice-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr "Fecha moneda"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descripción"
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Tiene método de pago"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Dirección de facturación"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Fecha factura"
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Descripción de la factura"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Tercero"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Estado de la factura"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Impuestos de factura"
@@ -376,24 +388,16 @@
 msgstr "Importe del desajuste"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Moneda de pago"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Moneda del desajuste"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Fecha"
+msgid "Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -767,26 +771,26 @@
 msgid "Delegate Lines to Pay"
 msgstr "Delegar lineas a pagar"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Facturas"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Facturas"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Facturas de proveedor"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Facturas de cliente"
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Facturas"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Métodos de pago de factura"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Plazos de pago"
@@ -841,14 +845,40 @@
 msgstr "Contabilizada"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validada"
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Pagada"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr "Pendiente"
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+"Los asientos \"(moves)s\" tiene como origen las facturas contabilizadas "
+"\"%(facturas)s\"."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+"Al cancelar-los se conciliaran los apuntes i se pagaran las facturas. Quizas"
+" queréis cancelar las facturas primero."
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr "Para cerrar los periodos debe contabilizar las facturas \"%(facturas)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -878,21 +908,21 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Para eliminar la factura \"%(invoice)s\" debe cancelarla."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "No puede eliminar la factura \"%(invoice)s\" porque está numerada."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"No puede añadir una linea a la factura \"%(invoice)s\" porque está "
-"contabilizada, pagada o cancelada."
+"No puede añadir lineas a la factura \"%(invoice)s\" porque no está en estado"
+" borrador."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "No puede modificar la línea \"%(line)s\" porque su factura \"%(invoice)s\" "
@@ -964,33 +994,25 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "La factura \"%(invoice)s\" genera una fecha de pago \"%(date)s\" en el "
 "pasado."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"No puede usar la misma cuenta \"%(account)s\" en la factura \"%(invoice)s\" "
-"y en la línea \"%(line)s\"."
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "La factura \"%(invoices)s\" es similar a la factura \"%(similar)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"No puede añadir impuestos a la factura \"%(invoice)s\" porque está "
-"contabilizada, pagada o cancelada."
+"No puede añadir impuestos a la factura \"%(invoice)s\" porque no está en "
+"estado borrador."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
 "Los impuestos en la factura \"%(invoice)s\" no son válidos, debe grabar de "
```

### Comparing `trytond_account_invoice-6.6.5/locale/es_419.po` & `trytond_account_invoice-6.8.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Prueba de término de pago"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -295,14 +300,23 @@
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Informe de factura"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr ""
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -384,23 +398,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
+msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,lines:"
@@ -775,26 +781,27 @@
 msgid "Delegate Lines to Pay"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Informe de factura"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -851,14 +858,36 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -887,18 +916,18 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "No puede agregar el impuesto a la factura \"%(invoice)s\" porque está "
 "contabilizada, pagada o cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -960,29 +989,23 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "No puede agregar el impuesto a la factura \"%(invoice)s\" porque está "
 "contabilizada, pagada o cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/et.po` & `trytond_account_invoice-6.8.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr "Valuuta kuupäev"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Kulum"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Maksemeetod"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Arve aadress"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Arve kuupäev"
@@ -297,14 +302,24 @@
 msgid "Description"
 msgstr "Kulum"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Arve"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Kulum"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Osapool"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Arve staatus"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Arve maksud"
@@ -387,25 +402,18 @@
 msgid "Write-Off Amount"
 msgstr "Mahakandmise väärtus"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Tasumise valuuta"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Mahakandmise valuuta"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Kuupäev"
+msgid "Currency"
+msgstr "Valuuta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Arve"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -781,26 +789,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "Tasumisele kuuluvad read"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Arved"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Arved"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Ostuarved"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Müügiarved"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Arved"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Arve tasumise meetodid"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Maksetingimused"
@@ -856,14 +865,38 @@
 msgstr "Postitatud"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Kontrollitud"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Kõik"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Tasutud"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -891,18 +924,19 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Arve \"%(arve)te\" kustutamiseks tuleb see tühistada."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Arvet \"%(arve)id\" ei saa kustutada, kuna sellel on number."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Arvele \"%(arve)tele\" ei saa lisada rida, kuna see on postitatud, tasutud "
 "või tühistatud."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -972,31 +1006,23 @@
 " väärtus"
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"Arvel \"%(arve)tele\" ja real \"%(rida)del\" ei saa kasutada sama kontot "
-"\"%(konto)sid\""
-
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "Arve \"%(arve)te\" kustutamiseks tuleb see tühistada."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Maksu ei saa lisada arvelt \"%(arve)tele\", kuna see on postitatud, tasutud "
 "või tühistatud."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/fa.po` & `trytond_account_invoice-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr "تاریخ ارز"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "شرح"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "روش پرداخت"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "آدرس صورتحساب"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "تاریخ صورت حساب"
@@ -298,14 +303,24 @@
 msgid "Description"
 msgstr "شرح"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "صورت حساب"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "شرح"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "نهاد/سازمان"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "وضعیت صورت حساب"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "مالیات های صورتحساب"
@@ -388,25 +403,18 @@
 msgid "Write-Off Amount"
 msgstr "مقدار نوسان"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "شرکت"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "واحد پول پرداخت"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "نوسانات واحد پول"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "تاریخ"
+msgid "Currency"
+msgstr "واحد پول"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "صورت حساب"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -782,26 +790,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "خطوط پرداخت"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "صورتحساب ها"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "صورتحساب ها"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "صورت حسابهای تامین کننده"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "صورتحساب های مشتری"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "صورتحساب ها"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "روش پرداخت صورتحساب"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "دوره های پرداخت"
@@ -857,14 +866,38 @@
 msgstr "ارسال شده"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "تایید شده"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "همه"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "پرداخت شده"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -897,18 +930,19 @@
 msgstr "برای حذف صورتحساب : \"%(invoice)s\" شما باید آنرا لغو کنید."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 "شما نمیتوانید صورتحساب : \"%(invoice)s\" را حذف کنید چراکه آن یک شماره دارد."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "شما نمیتوانید یک سطر به صورتحساب : \"٪s\" اضافه کنید زیرا آن ارسال، پرداخت و"
 " یا لغو شده است."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -981,31 +1015,23 @@
 "صورتحساب باشد."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"شما نمیتوانید از همان حساب : \"%(account)s\" بر صورتحساب : \"%(invoice)s\" و"
-" روی سطر:\"%(lines)s\" استفاده کنید."
-
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "برای حذف صورتحساب : \"%(invoice)s\" شما باید آنرا لغو کنید."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "شما نمیتوانید مالیات را به صورتحساب\"٪s\" اضافه کنید زیرا آن ارسال، پرداخت و"
 " یا لغو شده است."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/fi.po` & `trytond_account_invoice-6.8.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -297,14 +302,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Invoice"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr ""
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -386,23 +400,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
+msgid "Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
@@ -474,29 +480,31 @@
 msgid "Debit Account"
 msgstr ""
 
 msgctxt "field:account.invoice.payment.method,journal:"
 msgid "Journal"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.payment.method,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:account.invoice.payment_term,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.payment_term,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:account.invoice.payment_term.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.payment_term.line,currency:"
 msgid "Currency"
@@ -787,26 +795,27 @@
 msgid "Delegate Lines to Pay"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Payment Terms"
@@ -863,14 +872,37 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -895,18 +927,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -960,28 +992,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/fr.po` & `trytond_account_invoice-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr "Date du taux de change"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Description"
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "A des méthodes de paiement"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Adresse de facturation"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Date de facturation"
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr "Description"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Facture"
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Description de la facture"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Tiers"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "État de la facture"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Taxes de le facture"
@@ -376,24 +388,16 @@
 msgstr "Compte de pertes et profits"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Devise du paiement"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Devise de pertes et profits"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Date"
+msgid "Currency"
+msgstr "Devise"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Facture"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -767,26 +771,26 @@
 msgid "Delegate Lines to Pay"
 msgstr "Déléguer les lignes à payer"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Factures"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Factures"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Factures fournisseur"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Factures client"
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Factures"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Méthodes de paiement de facture"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Conditions de paiement"
@@ -817,15 +821,15 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_in_domain_draft"
 msgid "Draft"
 msgstr "Brouillons"
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_in_domain_posted"
 msgid "Posted"
-msgstr "Postées"
+msgstr "Comptabilisés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_in_domain_validated"
 msgid "Validated"
 msgstr "Validées"
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_out_domain_all"
@@ -834,47 +838,74 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_out_domain_draft"
 msgid "Draft"
 msgstr "Brouillons"
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_out_domain_posted"
 msgid "Posted"
-msgstr "Postées"
+msgstr "Comptabilisés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validées"
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Toutes"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Payées"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr "En attentes"
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+"Les mouvements \"%(moves)s\" ont pour origine les factures comptabilisées "
+"\"%(invoices)s\"."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+"Les annuler réconciliera les lignes de mouvement et paiera ainsi les "
+"factures. Vous voudrez peut-être d'abord annuler les factures."
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
-"Pour clôturer les périodes, vous devez poster les factures « %(invoices)s »."
+"Pour clôturer les périodes, vous devez comptabiliser les factures "
+"« %(invoices)s »."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
 "company \"%(company)s\"."
 msgstr ""
 "Vous ne pouvez pas effacer le tiers « %(party)s » tant qu'il a des factures "
 "en cours avec la société « %(company)s »."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "Vous ne pouvez pas rembourser la facture « %(invoice)s » car elle n'est pas "
-"postée."
+"comptabilisée."
 
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Vous ne pouvez pas annuler la facture client « %(invoice)s » car elle est "
-"postée et la configuration de la société ne le permet pas."
+"comptabilisée et la configuration de la société ne le permet pas."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
 msgid "The invoices \"%(invoices)s\" have an invoice date in the future."
 msgstr "La facture « %(invoice)s » a une date de facture dans le futur."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_cancel"
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
@@ -882,50 +913,50 @@
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 "Vous ne pouvez pas supprimer la facture « %(invoice)s » car elle a un "
 "numéro."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"Vous ne pouvez pas ajouter une ligne à la facture « %(invoice)s » car elle "
-"est postée, payée ou annulée."
+"Vous ne pouvez pas ajouter de lignes à la facture « %(invoice)s » car elle "
+"n'est plus dans l'état brouillon."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "Vous ne pouvez pas modifier la ligne « %(line)s » car sa facture "
-"« %(invoice)s » est postée, payée ou annulée."
+"« %(invoice)s » est comptabilisée, payée ou annulée."
 
 msgctxt "model:ir.message,text:msg_invoice_line_tax_unique"
 msgid "A tax can be added only once to an invoice line."
 msgstr ""
 "Une taxe ne peut être ajoutée qu'une seule fois à une ligne de facture."
 
 msgctxt "model:ir.message,text:msg_invoice_modify"
 msgid ""
 "You cannot modify invoice \"%(invoice)s\" because it is posted, paid or "
 "cancelled."
 msgstr ""
-"Vous ne pouvez pas modifier la facture « %(invoice)s » car elle est postée, "
-"payée ou annulée."
+"Vous ne pouvez pas modifier la facture « %(invoice)s » car elle est "
+"comptabilisée, payée ou annulée."
 
 msgctxt "model:ir.message,text:msg_invoice_no_sequence"
 msgid ""
 "To post invoice \"%(invoice)s\", you must define a sequence on fiscal year "
 "\"%(fiscalyear)s\"."
 msgstr ""
-"Pour poster la facture « %(invoice)s », vous devez définir une séquence sur "
-"l'année fiscale « %(fiscalyear)s »."
+"Pour comptabiliser la facture « %(invoice)s », vous devez définir une "
+"séquence sur l'année fiscale « %(fiscalyear)s »."
 
 msgctxt "model:ir.message,text:msg_invoice_number_after"
 msgid ""
 "To number the invoice \"%(invoice)s\", you must set an invoice date after "
 "\"%(date)s\" because the sequence \"%(sequence)s\" has already been used for"
 " invoice \"%(after_invoice)s\"."
 msgstr ""
@@ -969,34 +1000,26 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "La facture « %(invoice)s » génère une date de paiement « %(date)s » dans le "
 "passé."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"Vous ne pouvez pas utiliser le même compte « %(account)s » pour la facture "
-"« %(invoice)s » et pour la ligne « %(lines)s »."
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 "La facture « %(invoice)s » est similaire à la facture « %(similar)s »."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"Vous ne pouvez pas ajouter une taxe à la facture « %(invoice)s » car elle "
-"est postée, payée ou annulée."
+"Vous ne pouvez pas ajouter de taxes à la facture « %(invoice)s » car elle "
+"n'est plus dans l'état brouillon."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
 "Les taxes sur la facture « %(invoice)s » sont invalides, vous devez "
@@ -1004,15 +1027,15 @@
 
 msgctxt "model:ir.message,text:msg_invoice_tax_modify"
 msgid ""
 "You cannot modify tax \"%(tax)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "Vous ne pouvez pas modifier la taxe « %(tax)s » car sa facture "
-"« %(invoice)s » est postée, payée ou annulée."
+"« %(invoice)s » est comptabilisée, payée ou annulée."
 
 msgctxt "model:ir.message,text:msg_payment_term_invalid_ratio_divisor"
 msgid "The ratio and divisor are not consistent on line \"%(line)s\"."
 msgstr ""
 "Le ratio et le diviseur ne sont pas cohérents sur la ligne « %(line)s »."
 
 msgctxt "model:ir.message,text:msg_payment_term_missing_last_remainder"
@@ -1033,15 +1056,15 @@
 
 msgctxt "model:ir.model.button,confirm:invoice_cancel_button"
 msgid "Are you sure you want to cancel the invoices?"
 msgstr "Êtes-vous sûr de vouloir annuler les factures ?"
 
 msgctxt "model:ir.model.button,confirm:invoice_post_button"
 msgid "Are you sure you want to post the invoices?"
-msgstr "Êtes-vous sûr de vouloir poster les factures ?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser les factures ?"
 
 msgctxt "model:ir.model.button,help:invoice_cancel_button"
 msgid "Cancel the invoice"
 msgstr "Annuler la facture"
 
 msgctxt "model:ir.model.button,help:invoice_validate_button"
 msgid "Also known as Pro Forma"
@@ -1061,15 +1084,15 @@
 
 msgctxt "model:ir.model.button,string:invoice_pay_button"
 msgid "Pay"
 msgstr "Payer"
 
 msgctxt "model:ir.model.button,string:invoice_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:invoice_process_button"
 msgid "Process"
 msgstr "Traiter"
 
 msgctxt "model:ir.model.button,string:invoice_reschedule_lines_to_pay_button"
 msgid "Reschedule"
@@ -1221,15 +1244,15 @@
 
 msgctxt "selection:account.invoice,state:"
 msgid "Paid"
 msgstr "Payée"
 
 msgctxt "selection:account.invoice,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.invoice,state:"
 msgid "Validated"
 msgstr "Validé"
 
 msgctxt "selection:account.invoice,type:"
 msgid "Customer"
```

### Comparing `trytond_account_invoice-6.6.5/locale/hu.po` & `trytond_account_invoice-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Megjegyzés"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Fizetési mód"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Számlázási cím"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Számla kelte"
@@ -291,14 +296,24 @@
 msgid "Description"
 msgstr "Leírás"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Számla"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Megjegyzés"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Ügyfél"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Számlázás állapota"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -379,25 +394,18 @@
 msgid "Write-Off Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Cég"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Dátum"
+msgid "Currency"
+msgstr "Pénznem"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Számla"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -775,26 +783,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "Fizetendő tételek"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Számlák"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Számlák"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Szállítói számlák"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Vevői számlák"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Számlák"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Számla fizetési módok"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Fizetési feltételek"
@@ -850,14 +859,38 @@
 msgstr "lekönyvelt"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "jóváhagyott"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "összes"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "fizetve"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -882,18 +915,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -947,28 +980,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/id.po` & `trytond_account_invoice-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,19 @@
 msgid "Currency Date"
 msgstr "Tanggal Mata Uang"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Deskripsi"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Metode pembayaran"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Alamat Faktur"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Tanggal Faktur"
@@ -292,14 +297,24 @@
 msgid "Description"
 msgstr "Deskripsi"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Faktur"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Deskripsi"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Pihak"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Status Faktur"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -380,25 +395,18 @@
 msgid "Write-Off Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Mata Uang Pembayaran"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Tanggal"
+msgid "Currency"
+msgstr "Mata Uang"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Faktur"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -771,26 +779,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "Baris yang Harus Dibayar"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Faktur-Faktur"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Faktur-Faktur"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Faktur Pemasok"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Faktur Pelanggan"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Faktur-Faktur"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr ""
@@ -846,14 +855,37 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Lunas"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -885,19 +917,20 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Untuk menghapus faktur \"%(invoice)s\" Anda harus membatalkannya."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Anda tidak dapat menghapus faktur \"%(invoice)s\" karena memiliki nomor."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
-msgstr ""
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
+msgstr "Anda tidak dapat menghapus faktur \"%(invoice)s\" karena memiliki nomor."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 
@@ -955,32 +988,27 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "Faktur \"%(invoice)s\" menghasilkan tanggal pembayaran \"%(date)s\" di masa "
 "lampau."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 "Faktur \"%(invoice)s\" menghasilkan tanggal pembayaran \"%(date)s\" di masa "
 "lampau."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
-msgstr ""
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
+msgstr "Anda tidak dapat menghapus faktur \"%(invoice)s\" karena memiliki nomor."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/it.po` & `trytond_account_invoice-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,19 @@
 msgid "Currency Date"
 msgstr "Data valuta"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descrizione"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Metodo di pagamento"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Indirizzo di fatturazione"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Data fattura"
@@ -300,14 +305,24 @@
 msgid "Description"
 msgstr "Descrizione"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Fattura"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Descrizione"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Controparti"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Stato fattura"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Imposte fattura"
@@ -390,25 +405,18 @@
 msgid "Write-Off Amount"
 msgstr "Importo Svalutazione"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Azienda"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Pagamento Valuta"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Svalutazione valuta"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Valuta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Fattura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -788,27 +796,28 @@
 msgid "Delegate Lines to Pay"
 msgstr "Righe pagamento"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Fatture"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Fatture"
-
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Fatture cliente"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Fatture"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Metodi di pagamento della fattura"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Termini di pagamento"
@@ -868,14 +877,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Tutti"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Pagato"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -904,18 +937,18 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Non puoi aggiungere/variare l'imposta nella fattura \"%(invoice)s\" perché è"
 " stata registrata, pagata o cancellata."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -977,29 +1010,23 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Non puoi aggiungere/variare l'imposta nella fattura \"%(invoice)s\" perché è"
 " stata registrata, pagata o cancellata."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/lo.po` & `trytond_account_invoice-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,19 @@
 msgid "Currency Date"
 msgstr "ວັນທີສະກຸນເງິນ"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "ເນື້ອໃນລາຍການ"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "ທີ່ຢູ່"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "ວັນທີໃບເກັບເງິນ"
@@ -307,14 +312,24 @@
 
 #, fuzzy
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "ໃບເກັບເງິນ"
 
 #, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "ເນື້ອໃນລາຍການ"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "ພາກສ່ວນ"
+
+#, fuzzy
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "ວັນທີໃບເກັບເງິນ"
 
 #, fuzzy
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
@@ -403,26 +418,18 @@
 msgid "Write-Off Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ"
 
-msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
 #, fuzzy
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "ວັນທີ:"
+msgctxt "field:account.invoice.pay.ask,currency:"
+msgid "Currency"
+msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "ໃບເກັບເງິນ"
 
 #, fuzzy
@@ -835,27 +842,27 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "ໃບເກັບເງິນ"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "ໃບເກັບເງິນຂອງຜູ້ສະໜອງ"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -923,14 +930,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "ກວດສອບແລ້ວ"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "ທັງໝົດ"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "ຈ່າຍແລ້ວ"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -955,18 +986,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -1020,28 +1051,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/lt.po` & `trytond_account_invoice-6.8.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr "Valiutos kurso data"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Aprašymas"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Mokėjimo būdas"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Juridinis adresas"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Sąskaitos faktūros data"
@@ -297,14 +302,24 @@
 msgid "Description"
 msgstr "Aprašymas"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Sąskaita faktūra"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Aprašymas"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Kontrahentas"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Sąskaitos faktūros būsena"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Sąskaitos faktūros mokesčiai"
@@ -387,25 +402,18 @@
 msgid "Write-Off Amount"
 msgstr "Nurašoma suma"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Organizacija"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Mokėjimo valiuta"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Nurašymo valiuta"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Valiuta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Sąskaita faktūra"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -781,26 +789,27 @@
 msgstr "Eilutės apmokėjimui"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Sąskaitos faktūros"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Sąskaitos faktūros"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Tiekėjų sąskaitos"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Sąskaitos pirkėjams"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Sąskaitos faktūros"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Sąskaitų faktūrų apmokėjimo būdai"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Mokėjimo sąlygos"
@@ -856,14 +865,38 @@
 msgstr "Įtraukta į apskaitą"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Patvirtinta"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Apmokėta"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -888,18 +921,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -953,28 +986,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/nl.po` & `trytond_account_invoice-6.8.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr "Wisselkoersdatum"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Omschrijving"
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Heeft Betalingsmethode"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Factuuradres"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Factuurdatum"
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr "Omschrijving"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Factuur"
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Factuur Omschrijving"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Relatie"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Factuur status"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Factuur belastingen"
@@ -376,24 +388,16 @@
 msgstr "Afboekingsbedrag"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Valuta betaling"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Valuta afboeking"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Datum"
+msgid "Currency"
+msgstr "Valuta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Factuur"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -767,26 +771,26 @@
 msgid "Delegate Lines to Pay"
 msgstr "Te betalen regels overdragen"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Facturen"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Facturen"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Leverancier facturen"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Klant facturen"
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Facturen"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Factuur betaalmethodes"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Betalingstermijnen"
@@ -841,14 +845,40 @@
 msgstr "Geboekt"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Bevestigd"
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Betaald"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr "In behandeling"
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+"De boekingen \"%(moves)s\" hebben de geboekte facturen \"%(invoices)s\" als "
+"bron."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+"Annuleren zal de boekingen afletteren en de facturen dus betalen. Misschien "
+"wilt u de facturen eerst annuleren."
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr "Om de periodes af te sluiten moet u de facturen \"%(invoices)s\" boeken."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -880,21 +910,21 @@
 msgstr "Om de factuur \"% (invoice)s\" te verwijderen, moet u deze annuleren."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 "U kunt factuur \"%(invoice)s\" niet verwijderen omdat deze een nummer heeft."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"U kunt geen regel toevoegen aan de factuur \"%(invoice)s\" omdat deze is "
-"geboekt, betaald of geannuleerd."
+"U kunt geen regels toevoegen aan de factuur \"%(invoice)s\" omdat deze niet "
+"langer in status concept staat."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "U kunt regel \"%(line)s\" niet wijzigen omdat de factuur \"%(invoice)s\" "
@@ -967,33 +997,25 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "De factuur \"%(invoice)s\" genereert een betalingsdatum \"%(date)s\" in het "
 "verleden."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-"U kunt niet dezelfde grootboekrekening \"%(account)s\" gebruiken voor de "
-"factuur \"%(invoice)s\" en de regel \"%(lines)s\"."
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "De factuur \"%(invoice)s\" is vergelijkbaar aan factuur \"%(similar)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
-"U kunt geen belasting toevoegen aan factuur \"%(invoice)s\" omdat deze reeds"
-" is geboekt, betaald of geannuleerd."
+"U kunt geen belastingen toevoegen aan factuur \"%(invoice)s\" omdat deze "
+"niet langer in status concept staat."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
 "De belastingen op de factuur \"%(invoice)s\" zijn niet geldig, u moet deze "
```

### Comparing `trytond_account_invoice-6.6.5/locale/pl.po` & `trytond_account_invoice-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Opis"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -297,14 +302,24 @@
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Faktura"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Opis"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Strona"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -388,25 +403,18 @@
 msgid "Write-Off Amount"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Firma"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Waluta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Faktura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -793,27 +801,27 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -879,14 +887,37 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -911,18 +942,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -976,28 +1007,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/pt.po` & `trytond_account_invoice-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr "Data da Moeda"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descrição"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Simulação do Prazo de Pagamento"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Endereço para faturamento"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Data da Fatura"
@@ -299,14 +304,24 @@
 msgid "Description"
 msgstr "Descrição"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Fatura"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Descrição"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Pessoa"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Estado da Fatura"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Tributos da Fatura"
@@ -389,25 +404,18 @@
 msgid "Write-Off Amount"
 msgstr "Montante de Perdas e Lucros"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Empresa"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Moeda do Pagamento"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Moeda das Perdas e Lucros"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Moeda"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Fatura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -792,28 +800,28 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -882,14 +890,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Pago"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -918,18 +950,18 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Você não pode adicionar a linha \"%(line)s\" à fatura \"%(invoice)s\" porque"
 " ela já foi confirmada, paga ou cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -991,29 +1023,23 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Você não pode adicionar a linha \"%(line)s\" à fatura \"%(invoice)s\" porque"
 " ela já foi confirmada, paga ou cancelada."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/ro.po` & `trytond_account_invoice-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,19 @@
 msgid "Currency Date"
 msgstr "Data Valută"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descriere"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Metodă Plata"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Adresa de facturare"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Data Factura"
@@ -289,14 +294,24 @@
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Descriere"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Parte"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Stare Factura"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Facturare Impozit"
@@ -377,25 +392,18 @@
 msgid "Write-Off Amount"
 msgstr "Sumă Prescriere"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Companie"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Plata Valută"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Prescriere Valută"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Data"
+msgid "Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -771,26 +779,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "Reprogramare Rânduri de Plata"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Facturi"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Facturi"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Facturi Furnizor"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Facturi Client"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Facturi"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Metode Plata Factura"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Termene de Plata"
@@ -845,14 +854,39 @@
 msgstr "Postat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validat"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Tot"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Plătit"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr "Pentru a închide perioadele trebuie postate facturile \"%(invoices)s\"."
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr "Pentru a închide perioadele trebuie postate facturile \"%(invoices)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -881,18 +915,19 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Pentru a şterge factura \"%(invoice)s\" trebuie anulata."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Nu se poate şterge factura \"%(invoice)s\" pentru că are un număr."
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că este "
 "postată, plătita sau anulată."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -960,30 +995,27 @@
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "Factura \"%(invoice)s\" genereaza data \"%(date)s\" de plata care este in "
 "trecut."
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "Facturile \"%(invoices)s\" au o data în viitor."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
+"Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că este "
+"postată, plătita sau anulată."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/ru.po` & `trytond_account_invoice-6.8.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,19 @@
 msgid "Currency Date"
 msgstr "Дата курса валюты"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Описание"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Адрес для инвойса"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Дата инвойса"
@@ -307,14 +312,24 @@
 msgstr "Описание"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Инвойс"
 
 #, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Описание"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Контрагент"
+
+#, fuzzy
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Состояние инвойса"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Налоги по инвойсу"
@@ -397,26 +412,18 @@
 msgid "Write-Off Amount"
 msgstr "Сумма списания"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Организация"
 
-msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Валюта оплаты"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Валюта списания"
-
 #, fuzzy
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Дата"
+msgctxt "field:account.invoice.pay.ask,currency:"
+msgid "Currency"
+msgstr "Валюта"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Инвойс"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -818,27 +825,27 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Инвойсы поставщиков"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -906,14 +913,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Утвержденный"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "Все"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Оплачен"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -942,18 +973,18 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Вы не можете добавить строчку \"%(line)s\" в инвойс \"%(invoice)s\" так как "
 "он \"Отправлен\", \"Оплачен\" или \"Отменен\"."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -1015,29 +1046,23 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Вы не можете добавить строчку \"%(line)s\" в инвойс \"%(invoice)s\" так как "
 "он \"Отправлен\", \"Оплачен\" или \"Отменен\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/sl.po` & `trytond_account_invoice-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 msgid "Currency Date"
 msgstr "Datum valute"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Opis"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Preizkus plačilnega roka"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Naslov plačnika"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "Datum računa"
@@ -299,14 +304,24 @@
 msgid "Description"
 msgstr "Opis"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Račun"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Opis"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "Partner"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Stanje računa"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "Davki računa"
@@ -389,25 +404,18 @@
 msgid "Write-Off Amount"
 msgstr "Znesek odpisa"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Družba"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "Valuta plačila"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "Valuta odpisa"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "Datum"
+msgid "Currency"
+msgstr "Valuta"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Račun"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -792,28 +800,28 @@
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
 #, fuzzy
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
@@ -882,14 +890,38 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "Plačano"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -918,18 +950,18 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Davka pri računu \"%(invoice)s\" ni možno dodati, ker je bodisi knjižen ali "
 "plačan bodisi preklican."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
@@ -991,29 +1023,23 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 "Davka pri računu \"%(invoice)s\" ni možno dodati, ker je bodisi knjižen ali "
 "plačan bodisi preklican."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
```

### Comparing `trytond_account_invoice-6.6.5/locale/tr.po` & `trytond_account_invoice-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,19 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "Test Payment Term"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -297,14 +302,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "Invoice"
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr ""
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -386,23 +400,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
+msgid "Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Invoice"
 
@@ -787,26 +793,27 @@
 msgid "Delegate Lines to Pay"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Invoices"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "Invoices"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Payment Terms"
@@ -863,14 +870,37 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "All"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -895,18 +925,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -960,28 +990,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
@@ -1107,14 +1131,15 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
+#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1283,14 +1308,15 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:account.invoice:"
 msgid "Invoice"
```

### Comparing `trytond_account_invoice-6.6.5/locale/uk.po` & `trytond_account_invoice-6.8.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 msgid "Currency Date"
 msgstr ""
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr ""
 
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr ""
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
@@ -287,14 +291,22 @@
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr ""
 
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr ""
+
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr ""
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr ""
@@ -376,23 +388,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr ""
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
+msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr ""
 
 msgctxt "field:account.invoice.pay.ask,lines:"
@@ -763,26 +767,26 @@
 msgid "Delegate Lines to Pay"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr ""
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr ""
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr ""
@@ -837,14 +841,36 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr ""
 
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr ""
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -869,18 +895,18 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
@@ -934,28 +960,22 @@
 "invoice amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
```

### Comparing `trytond_account_invoice-6.6.5/locale/zh_CN.po` & `trytond_account_invoice-6.8.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,19 @@
 msgid "Currency Date"
 msgstr "货币日期"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "描述"
 
+#, fuzzy
+msgctxt "field:account.invoice,has_payment_method:"
+msgid "Has Payment Method"
+msgstr "支付方式"
+
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "原始凭证地址"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
 msgstr "原始凭证日期"
@@ -291,14 +296,24 @@
 msgid "Description"
 msgstr "描述"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "原始凭证"
 
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_description:"
+msgid "Invoice Description"
+msgstr "描述"
+
+#, fuzzy
+msgctxt "field:account.invoice.line,invoice_party:"
+msgid "Party"
+msgstr "参与者"
+
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "原始凭证状态"
 
 msgctxt "field:account.invoice.line,invoice_taxes:"
 msgid "Invoice Taxes"
 msgstr "原始凭证税"
@@ -380,25 +395,18 @@
 msgid "Write-Off Amount"
 msgstr "核销金额"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "公司"
 
+#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
-msgid "Payment Currency"
-msgstr "支付货币"
-
-msgctxt "field:account.invoice.pay.ask,currency_writeoff:"
-msgid "Write-Off Currency"
-msgstr "核销货币"
-
-msgctxt "field:account.invoice.pay.ask,date:"
-msgid "Date"
-msgstr "日期"
+msgid "Currency"
+msgstr "货币"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "原始凭证"
 
 msgctxt "field:account.invoice.pay.ask,lines:"
 msgid "Lines"
@@ -776,26 +784,27 @@
 msgid "Delegate Lines to Pay"
 msgstr "待支付明细"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "发票"
 
-msgctxt "model:ir.action,name:act_invoice_form2"
-msgid "Invoices"
-msgstr "Invoices"
-
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Supplier Invoices"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Customer Invoices"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_invoice_relate"
+msgid "Invoices"
+msgstr "发票"
+
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "原始凭证付款方式"
 
 msgctxt "model:ir.action,name:act_payment_term_form"
 msgid "Payment Terms"
 msgstr "Payment Terms"
@@ -851,14 +860,38 @@
 msgstr "Posted"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "已验证"
 
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
+msgid "All"
+msgstr "全部"
+
+#, fuzzy
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
+msgid "Paid"
+msgstr "已支付"
+
+msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
+msgid "Pending"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move"
+msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
+msgid ""
+"Cancelling them will reconcile the move lines thus paying the invoices. You "
+"might want to cancel the invoices first."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending invoices with "
@@ -883,18 +916,19 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "删除原始凭证 \"%(invoice)s\" 之前必须先取消它。"
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "无法删除原始凭证 \"%(invoice)s\" ，因为它包含序号。"
 
-msgctxt "model:ir.message,text:msg_invoice_line_create"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
-"You cannot add a line to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr "无法给原始凭证 \"%(invoice)s\" 添加明细，因为它已经入账，付款或者取消。"
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr "无法更改明细 \"%(line)s\"，因为原始凭证 \"%(invoice)s\" 它已经入账，付款或者取消。"
@@ -954,29 +988,23 @@
 msgstr "原始凭证 \"%(invoice)s\" 上的付款明细金额不能大于凭证金额。"
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 
 #, fuzzy
-msgctxt "model:ir.message,text:msg_invoice_same_account_line"
-msgid ""
-"You cannot use the same account \"%(account)s\" on invoice \"%(invoice)s\" "
-"and on line \"%(line)s\"."
-msgstr "不能在原始凭证 \"%(invoice)s\" 和明细 \"%(invoice)s\"上使用相同的帐户 \"%(account)s\" 。"
-
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
 msgstr "删除原始凭证 \"%(invoice)s\" 之前必须先取消它。"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
-"You cannot add a tax to invoice \"%(invoice)s\" because it is posted, paid "
-"or cancelled."
+"You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
+" draft state."
 msgstr "无法给原始凭证 \"%(invoice)s\" 添加税，因为它已经入账，付款或者取消。"
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr "原始凭证 \"%(invoice)s\" 上的税款无效，必须再次保存以强制重新计算。"
```

### Comparing `trytond_account_invoice-6.6.5/message.xml` & `trytond_account_invoice-6.8.0/message.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/message.xml` & `trytond_account_invoice-6.8.0/message.xml`

```diff
@@ -23,17 +23,14 @@
     </record>
     <record model="ir.message" id="msg_invoice_number_after">
       <field name="text">To number the invoice &quot;%(invoice)s&quot;, you must set an invoice date after &quot;%(date)s&quot; because the sequence &quot;%(sequence)s&quot; has already been used for invoice &quot;%(after_invoice)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_invoice_modify">
       <field name="text">You cannot modify invoice &quot;%(invoice)s&quot; because it is posted, paid or cancelled.</field>
     </record>
-    <record model="ir.message" id="msg_invoice_same_account_line">
-      <field name="text">You cannot use the same account &quot;%(account)s&quot; on invoice &quot;%(invoice)s&quot; and on line &quot;%(line)s&quot;.</field>
-    </record>
     <record model="ir.message" id="msg_invoice_delete_cancel">
       <field name="text">To delete invoice &quot;%(invoice)s&quot; you must cancel it.</field>
     </record>
     <record model="ir.message" id="msg_invoice_delete_numbered">
       <field name="text">You cannot delete invoice &quot;%(invoice)s&quot; because it has a number.</field>
     </record>
     <record model="ir.message" id="msg_invoice_customer_cancel_move">
@@ -47,22 +44,22 @@
     </record>
     <record model="ir.message" id="msg_invoice_credit_refund_not_posted">
       <field name="text">You cannot refund invoice &quot;%(invoice)s&quot; because it is not posted.</field>
     </record>
     <record model="ir.message" id="msg_invoice_line_modify">
       <field name="text">You cannot modify line &quot;%(line)s&quot; because its invoice &quot;%(invoice)s&quot; is posted, paid or cancelled.</field>
     </record>
-    <record model="ir.message" id="msg_invoice_line_create">
-      <field name="text">You cannot add a line to invoice &quot;%(invoice)s&quot; because it is posted, paid or cancelled.</field>
+    <record model="ir.message" id="msg_invoice_line_create_draft">
+      <field name="text">You cannot add lines to invoice &quot;%(invoice)s&quot; because it is no longer in a draft state.</field>
     </record>
     <record model="ir.message" id="msg_invoice_tax_modify">
       <field name="text">You cannot modify tax &quot;%(tax)s&quot; because its invoice &quot;%(invoice)s&quot; is posted, paid or cancelled.</field>
     </record>
     <record model="ir.message" id="msg_invoice_tax_create">
-      <field name="text">You cannot add a tax to invoice &quot;%(invoice)s&quot; because it is posted, paid or cancelled.</field>
+      <field name="text">You cannot add taxes to invoice &quot;%(invoice)s&quot; because it is no longer in a draft state.</field>
     </record>
     <record model="ir.message" id="msg_invoice_line_tax_unique">
       <field name="text">A tax can be added only once to an invoice line.</field>
     </record>
     <record model="ir.message" id="msg_invoice_pay_amount_greater_amount_to_pay">
       <field name="text">You cannot add a partial payment on invoice &quot;%(invoice)s&quot; with an amount greater than the amount to pay &quot;%(amount_to_pay)s&quot;.</field>
     </record>
@@ -80,9 +77,15 @@
     </record>
     <record model="ir.message" id="msg_invoice_date_future">
       <field name="text">The invoices &quot;%(invoices)s&quot; have an invoice date in the future.</field>
     </record>
     <record model="ir.message" id="msg_invoice_similar">
       <field name="text">The invoice &quot;%(invoice)s&quot; is similar to invoice &quot;%(similar)s&quot;.</field>
     </record>
+    <record model="ir.message" id="msg_cancel_invoice_move">
+      <field name="text">The moves &quot;%(moves)s&quot; have the posted invoices &quot;%(invoices)s&quot; as origin.</field>
+    </record>
+    <record model="ir.message" id="msg_cancel_invoice_move_description">
+      <field name="text">Cancelling them will reconcile the move lines thus paying the invoices. You might want to cancel the invoices first.</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_invoice-6.6.5/party.py` & `trytond_account_invoice-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/payment_term.py` & `trytond_account_invoice-6.8.0/payment_term.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/payment_term.xml` & `trytond_account_invoice-6.8.0/payment_term.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/setup.py` & `trytond_account_invoice-6.8.0/setup.py`

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
@@ -37,39 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-dateutil', 'python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for invoicing',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
         'https://docs.tryton.org/projects/modules-account-invoice/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_invoice',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice',
     package_dir={'trytond.modules.account_invoice': '.'},
     packages=(
         ['trytond.modules.account_invoice']
         + ['trytond.modules.account_invoice.%s' % p for p in find_packages()]
         ),
@@ -106,24 +106,24 @@
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

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_credit_note.rst` & `trytond_account_invoice-6.8.0/tests/scenario_credit_note.rst`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
 
 Pay credit note::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('-220.00')
     >>> pay.form.amount = Decimal('-120.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.form.type = 'partial'
     >>> pay.form.amount
@@ -125,15 +125,15 @@
     1
     >>> pay.form.amount_writeoff
     Decimal('-100.00')
     >>> pay.execute('pay')
     >>> pay.state
     'end'
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('-100.00')
     >>> pay.form.amount = Decimal('-100.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ================
 Invoice Scenario
 ================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax, create_tax_code
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
@@ -29,15 +29,15 @@
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'BE0897290877'
     >>> company.party.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
     >>> period_ids = [p.id for p in fiscalyear.periods]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
@@ -163,14 +163,15 @@
     >>> tax_line.tax == tax
     True
     >>> tax_line.tax = None
     >>> tax_line.tax = tax
 
 Post invoice::
 
+    >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
     >>> invoice.tax_identifier.code
     'BE0897290877'
     >>> invoice.untaxed_amount
     Decimal('220.00')
@@ -215,15 +216,15 @@
     >>> credit = Wizard('account.invoice.credit', [invoice])
     >>> credit.form.with_refund = True
     >>> credit.form.invoice_date = invoice.invoice_date
     >>> credit.execute('credit')
     >>> invoice.reload()
     >>> invoice.state
     'cancelled'
-    >>> invoice.reconciled == today
+    >>> bool(invoice.reconciled)
     True
     >>> credit_note, = Invoice.find([
     ...     ('type', '=', 'out'), ('id', '!=', invoice.id)])
     >>> credit_note.state
     'paid'
     >>> all(line.taxes_date == today for line in credit_note.lines)
     True
@@ -260,24 +261,24 @@
     Decimal('20.00')
 
 Pay invoice::
 
     >>> invoice, = invoice.duplicate()
     >>> invoice.click('post')
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('240.00')
     >>> pay.form.amount = Decimal('120.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.state
     'end'
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('120.00')
     >>> pay.form.amount = Decimal('20.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.form.type = 'partial'
     >>> pay.form.amount
@@ -288,15 +289,15 @@
     0
     >>> len(pay.form.lines)
     1
     >>> pay.form.amount_writeoff
     Decimal('100.00')
     >>> pay.execute('pay')
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('-20.00')
     >>> pay.form.amount = Decimal('99.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.form.type = 'writeoff'
     >>> pay.form.writeoff = writeoff_method
@@ -364,15 +365,15 @@
     >>> invoice.party = party
     >>> invoice.payment_term = payment_term
     >>> line = invoice.lines.new()
     >>> line.product = product
     >>> line.quantity = 5
     >>> line.unit_price = Decimal('40')
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> invoice.tax_identifier
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 ===================================
 Invoice Scenario Alternate Currency
 ===================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.currency.tests.tools import get_currency
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + relativedelta(days=1)
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
@@ -40,19 +39,16 @@
     >>> rate.date = tomorrow
     >>> rate.rate = eur.rates[0].rate + Decimal('0.5')
     >>> eur.save()
 
 Create fiscal years::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=today))
+    ...     create_fiscalyear(company, (today, tomorrow)))
     >>> fiscalyear.click('create_period')
-    >>> next_fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=today + relativedelta(years=1)))
-    >>> next_fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> revenue = accounts['revenue']
     >>> expense = accounts['expense']
@@ -143,46 +139,25 @@
     Decimal('20.00')
     >>> invoice.untaxed_amount
     Decimal('420.00')
     >>> invoice.tax_amount
     Decimal('40.00')
     >>> invoice.total_amount
     Decimal('460.00')
+    >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
     >>> invoice.untaxed_amount
     Decimal('420.00')
     >>> invoice.tax_amount
     Decimal('40.00')
     >>> invoice.total_amount
     Decimal('460.00')
 
-Pay the invoice with rate change::
-
-    >>> pay = Wizard('account.invoice.pay', [invoice])
-    >>> pay.form.amount
-    Decimal('460.00')
-    >>> pay.form.payment_method = payment_method
-    >>> pay.form.date = tomorrow
-    >>> pay.execute('choice')
-    >>> pay.form.type = 'writeoff'
-    >>> pay.form.writeoff = writeoff
-    >>> pay.form.amount
-    Decimal('460.00')
-    >>> pay.form.currency == eur
-    True
-    >>> pay.form.amount_writeoff
-    Decimal('46.00')
-    >>> pay.form.currency_writeoff == currency
-    True
-    >>> pay.execute('pay')
-    >>> invoice.state
-    'paid'
-
 Create negative tax::
 
     >>> negative_tax = create_tax(Decimal('-.10'))
     >>> negative_tax.save()
 
 Create invoice with alternate currency and negative taxes::
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ==============================================
 Invoice Scenario Alternate Currency Lower Rate
 ==============================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.currency.tests.tools import get_currency
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
@@ -34,15 +34,15 @@
     >>> rate.date = today
     >>> rate.rate = Decimal('0.5')
     >>> eur.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
@@ -72,23 +72,24 @@
     >>> invoice.party = party
     >>> invoice.currency = eur
     >>> line = invoice.lines.new()
     >>> line.description = "Line"
     >>> line.account = accounts['revenue']
     >>> line.quantity = 5
     >>> line.unit_price = Decimal('80')
+    >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
     >>> invoice.total_amount
     Decimal('400.00')
 
 Pay the invoice::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('400.00')
     >>> pay.form.currency == eur
     True
     >>> pay.form.payment_method = payment_method
     >>> pay.form.date = today
     >>> pay.execute('choice')
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternative_payee.rst`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     Decimal('0.0')
     >>> party3.reload()
     >>> party3.receivable
     Decimal('10.00')
 
 Pay the invoice::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payee = party3
     >>> pay.form.amount = Decimal('10.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> invoice.state
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_customer_sequential.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 Customer Invoice Sequential
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
-    >>> from proteus import Model
+    >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
     >>> today = dt.date.today()
-    >>> past_year = today - relativedelta(years=1)
+    >>> past_year = today - dt.timedelta(days=365)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal years::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=past_year))
+    ...     create_fiscalyear(company, past_year))
     >>> fiscalyear.click('create_period')
-    >>> next_fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=today))
-    >>> next_fiscalyear.click('create_period')
+
+    >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
+    >>> renew_fiscalyear.execute('create_')
+    >>> next_fiscalyear, = renew_fiscalyear.actions[0]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
 Create party::
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_group_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_in_future.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 =================
 Invoice in Future
 =================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (create_company,
     ...     get_company)
     >>> from trytond.modules.account.tests.tools import (create_fiscalyear,
     ...     create_chart, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + datetime.timedelta(days=1)
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (today, tomorrow)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> revenue = accounts['revenue']
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_manual_tax.rst`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
     >>> period_ids = [p.id for p in fiscalyear.periods]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_overpayment.rst`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     >>> invoice.state
     'posted'
     >>> invoice.total_amount
     Decimal('100.00')
 
 Overpay the invoice with write-off::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount = Decimal('110.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.form.type = 'writeoff'
     >>> pay.form.writeoff = writeoff
     >>> pay.form.amount_writeoff
     Decimal('-10.00')
@@ -101,15 +101,15 @@
     >>> accounts['receivable'].balance
     Decimal('0.00')
 
 Overpay the invoice without write-off::
 
     >>> invoice, = invoice.duplicate()
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount = Decimal('110.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.form.type = 'overpayment'
     >>> pay.execute('pay')
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_reschedule_lines.rst`

 * *Files 11% similar despite different names*

```diff
@@ -70,16 +70,15 @@
     >>> len(invoice.lines_to_pay)
     1
     >>> invoice.amount_to_pay
     Decimal('10.00')
 
 Reschedule line::
 
-    >>> reschedule = Wizard(
-    ...     'account.invoice.lines_to_pay.reschedule', [invoice])
+    >>> reschedule = invoice.click('reschedule_lines_to_pay')
     >>> reschedule_lines, = reschedule.actions
     >>> reschedule_lines.form.total_amount
     Decimal('10.00')
     >>> reschedule_lines.form.start_date = period.end_date
     >>> reschedule_lines.form.frequency ='monthly'
     >>> reschedule_lines.form.number = 2
     >>> reschedule_lines.execute('preview')
@@ -93,15 +92,15 @@
     >>> len([l for l in invoice.lines_to_pay if not l.reconciliation])
     2
     >>> invoice.amount_to_pay
     Decimal('10.00')
 
 Pay the invoice::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.amount = Decimal('10.00')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 =========================
 Invoice Supplier Scenario
 =========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax, create_tax_code
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
     >>> period_ids = [p.id for p in fiscalyear.periods]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
@@ -239,9 +239,9 @@
 Cancel posted invoice::
 
     >>> invoice.click('cancel')
     >>> invoice.state
     'cancelled'
     >>> invoice.cancel_move is not None
     True
-    >>> invoice.reconciled == today
+    >>> bool(invoice.reconciled)
     True
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 ==========================
 Invoice Supplier Post Paid
 ==========================
 
 Imports::
-    >>> import datetime
+
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_tax_deductible.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-6.8.0/tests/scenario_invoice_with_credit.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ============================
 Invoice with credit Scenario
 ============================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax, create_tax_code
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
@@ -70,14 +68,15 @@
     >>> line.unit_price = Decimal('10.0000')
     >>> line.taxes.append(Tax(tax.id))
     >>> line = invoice.lines.new()
     >>> line.account = accounts['revenue']
     >>> line.quantity = -2
     >>> line.unit_price = Decimal('5.0000')
     >>> line.taxes.append(Tax(tax.id))
+    >>> invoice.invoice_date = fiscalyear.start_date
     >>> invoice.click('post')
 
     >>> invoice.untaxed_amount
     Decimal('40.00')
     >>> invoice.tax_amount
     Decimal('4.00')
     >>> invoice.total_amount
```

### Comparing `trytond_account_invoice-6.6.5/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-6.8.0/tests/scenario_renew_fiscalyear.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 =========================
 Renew Fiscalyear Scenario
 =========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
     >>> from trytond.modules.account_invoice.tests.tools \
     ...     import set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
-    >>> end_year = today + relativedelta(month=12, day=31)
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> InvoiceSequence = Model.get('account.fiscalyear.invoice_sequence')
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear = set_fiscalyear_invoice_sequences(fiscalyear)
     >>> fiscalyear.click('create_period')
     >>> inv_seq, = fiscalyear.invoice_sequences
     >>> seq = inv_seq.out_invoice_sequence
     >>> for period in fiscalyear.periods:
     ...     seq, = seq.duplicate()
     ...     _ = inv_seq.duplicate(default={
@@ -41,16 +40,16 @@
     ...             'out_invoice_sequence': seq.id,
     ...             'in_invoice_sequence': seq.id,
     ...             'out_credit_note_sequence': seq.id,
     ...             'in_credit_note_sequence': seq.id,
     ...             })
     >>> period = fiscalyear.periods.new()
     >>> period.name = 'Adjustment'
-    >>> period.start_date = end_year
-    >>> period.end_date = end_year
+    >>> period.start_date = fiscalyear.end_date
+    >>> period.end_date = fiscalyear.end_date
     >>> period.type = 'adjustment'
     >>> fiscalyear.save()
 
 Set the sequence number::
 
     >>> sequence = fiscalyear.post_move_sequence
     >>> sequence.number_next = 10
@@ -87,20 +86,20 @@
     [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
 
 
 Set the sequence name::
 
     >>> for seq in new_fiscalyear.invoice_sequences:
     ...     seq.out_invoice_sequence.name = ('Sequence %s' %
-    ...         new_fiscalyear.start_date.strftime('%Y'))
+    ...         new_fiscalyear.name)
     ...     seq.out_invoice_sequence.save()
 
 Renew fiscalyear and test sequence name is updated::
 
     >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
     >>> renew_fiscalyear.form.reset_sequences = True
     >>> renew_fiscalyear.execute('create_')
     >>> new_fiscalyear, = renew_fiscalyear.actions[0]
     >>> all(seq.out_invoice_sequence.name ==
-    ...         'Sequence %s' % new_fiscalyear.start_date.strftime('%Y')
+    ...         'Sequence %s' % new_fiscalyear.name
     ...     for seq in new_fiscalyear.invoice_sequences)
     True
```

### Comparing `trytond_account_invoice-6.6.5/tests/test_module.py` & `trytond_account_invoice-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/tests/tools.py` & `trytond_account_invoice-6.8.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice
-Version: 6.6.5
+Name: trytond_account_invoice
+Version: 6.8.0
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice
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
 
 ######################
 Account Invoice Module
 ######################
```

### Comparing `trytond_account_invoice-6.6.5/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -57,18 +57,20 @@
 ./locale/ro.po
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
+./tests/scenario_cancelling_invoice_move.rst
 ./tests/scenario_credit_note.rst
 ./tests/scenario_invoice.rst
 ./tests/scenario_invoice_alternate_currency.rst
 ./tests/scenario_invoice_alternate_currency_lower_rate.rst
+./tests/scenario_invoice_alternate_currency_rate_change.rst
 ./tests/scenario_invoice_alternative_payee.rst
 ./tests/scenario_invoice_customer_sequential.rst
 ./tests/scenario_invoice_group_line.rst
 ./tests/scenario_invoice_in_future.rst
 ./tests/scenario_invoice_manual_tax.rst
 ./tests/scenario_invoice_overpayment.rst
 ./tests/scenario_invoice_reschedule_lines.rst
@@ -152,18 +154,20 @@
 locale/ro.po
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
+tests/scenario_cancelling_invoice_move.rst
 tests/scenario_credit_note.rst
 tests/scenario_invoice.rst
 tests/scenario_invoice_alternate_currency.rst
 tests/scenario_invoice_alternate_currency_lower_rate.rst
+tests/scenario_invoice_alternate_currency_rate_change.rst
 tests/scenario_invoice_alternative_payee.rst
 tests/scenario_invoice_customer_sequential.rst
 tests/scenario_invoice_group_line.rst
 tests/scenario_invoice_in_future.rst
 tests/scenario_invoice_manual_tax.rst
 tests/scenario_invoice_overpayment.rst
 tests/scenario_invoice_reschedule_lines.rst
```

### Comparing `trytond_account_invoice-6.6.5/view/credit_start_form.xml` & `trytond_account_invoice-6.8.0/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_form.xml` & `trytond_account_invoice-6.8.0/view/invoice_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_line_form.xml` & `trytond_account_invoice-6.8.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_line_tree.xml` & `trytond_account_invoice-6.8.0/view/invoice_line_tree.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/view/invoice_line_tree.xml` & `trytond_account_invoice-6.8.0/view/invoice_line_tree.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tree>
   <field name="invoice" expand="1"/>
+  <field name="invoice_party" expand="1" optional="0"/>
   <field name="type" optional="1"/>
   <field name="product" expand="1" optional="0"/>
   <field name="summary" expand="1" optional="1"/>
-  <field name="account" expand="1" optional="0"/>
+  <field name="account" expand="1" optional="1"/>
   <field name="quantity" symbol="unit"/>
-  <field name="unit_price"/>
-  <field name="taxes" optional="0"/>
+  <field name="unit_price" optional="1"/>
+  <field name="taxes" optional="1"/>
   <field name="amount"/>
+  <field name="invoice_description" expand="1" optional="1"/>
 </tree>
```

### Comparing `trytond_account_invoice-6.6.5/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-6.8.0/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_sequence_form.xml` & `trytond_account_invoice-6.8.0/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_tax_form.xml` & `trytond_account_invoice-6.8.0/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-6.8.0/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/invoice_tree.xml` & `trytond_account_invoice-6.8.0/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/party_form.xml` & `trytond_account_invoice-6.8.0/view/party_form.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/view/party_form.xml` & `trytond_account_invoice-6.8.0/view/party_form.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <data>
   <xpath expr="//group[@id='links']" position="inside">
-    <link icon="tryton-invoice" name="account_invoice.act_invoice_form2" empty="hide"/>
+    <link icon="tryton-invoice" name="account_invoice.act_invoice_relate" empty="hide"/>
   </xpath>
   <xpath expr="/form/notebook/page[@id='accounting']/separator[@id='account']" position="before">
     <separator string="Payment Terms" colspan="4" id="payment_terms"/>
     <label name="customer_payment_term"/>
     <field name="customer_payment_term"/>
     <label name="supplier_payment_term"/>
     <field name="supplier_payment_term"/>
```

### Comparing `trytond_account_invoice-6.6.5/view/pay_ask_form.xml` & `trytond_account_invoice-6.8.0/view/pay_ask_form.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/view/pay_ask_form.xml` & `trytond_account_invoice-6.8.0/view/pay_ask_form.xml`

```diff
@@ -1,22 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="type"/>
   <field name="type" colspan="3"/>
   <label name="amount"/>
-  <field name="amount" symbol=""/>
-  <label name="currency"/>
-  <field name="currency"/>
+  <field name="amount"/>
+  <newline/>
   <label name="amount_writeoff"/>
   <field name="amount_writeoff"/>
-  <label name="currency_writeoff"/>
-  <field name="currency_writeoff" symbol=""/>
   <label name="writeoff"/>
   <field name="writeoff" widget="selection"/>
   <field name="lines" colspan="4" view_ids="account_invoice.move_line_view_list_to_pay"/>
   <field name="payment_lines" colspan="4" view_ids="account_invoice.move_line_view_list_payment"/>
   <field name="company" colspan="4" invisible="1"/>
   <field name="invoice" colspan="4" invisible="1"/>
-  <field name="date" colspan="4" invisible="1"/>
 </form>
```

### Comparing `trytond_account_invoice-6.6.5/view/pay_start_form.xml` & `trytond_account_invoice-6.8.0/view/pay_start_form.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_account_invoice-6.6.5/view/pay_start_form.xml` & `trytond_account_invoice-6.8.0/view/pay_start_form.xml`

```diff
@@ -1,18 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form cursor="amount">
   <label name="payee"/>
   <field name="payee"/>
-  <newline/>
   <label name="amount"/>
-  <field name="amount" symbol=""/>
-  <label name="currency"/>
-  <field name="currency"/>
+  <field name="amount"/>
   <label name="description"/>
   <field name="description" colspan="3"/>
   <label name="payment_method"/>
   <field name="payment_method" widget="selection"/>
   <label name="date"/>
   <field name="date"/>
 </form>
```

### Comparing `trytond_account_invoice-6.6.5/view/payment_method_form.xml` & `trytond_account_invoice-6.8.0/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/payment_term_form.xml` & `trytond_account_invoice-6.8.0/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/payment_term_line_form.xml` & `trytond_account_invoice-6.8.0/view/payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.6.5/view/payment_term_line_relativedelta_form.xml` & `trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_form.xml`

 * *Files identical despite different names*

