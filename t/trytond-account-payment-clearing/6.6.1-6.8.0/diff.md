# Comparing `tmp/trytond_account_payment_clearing-6.6.1.tar.gz` & `tmp/trytond_account_payment_clearing-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_clearing-6.6.1.tar", last modified: Wed May  3 16:54:57 2023, max compression
+gzip compressed data, was "trytond_account_payment_clearing-6.8.0.tar", last modified: Mon May  1 11:39:34 2023, max compression
```

## Comparing `trytond_account_payment_clearing-6.6.1.tar` & `trytond_account_payment_clearing-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.924192 trytond_account_payment_clearing-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2126 2023-05-03 16:54:54.000000 trytond_account_payment_clearing-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-03 16:54:53.000000 trytond_account_payment_clearing-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-05-03 16:54:57.924192 trytond_account_payment_clearing-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.920859 trytond_account_payment_clearing-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.917526 trytond_account_payment_clearing-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2636 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2557 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2049 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2140 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2297 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15596 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:54:57.924192 trytond_account_payment_clearing-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4741 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8890 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/statement.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.917526 trytond_account_payment_clearing-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3467 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/tests/scenario_account_negative_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14647 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/tests/scenario_account_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5739 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-03 16:22:12.000000 trytond_account_payment_clearing-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.924192 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:54:57.000000 trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:54:57.920859 trytond_account_payment_clearing-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      594 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-13 16:52:41.000000 trytond_account_payment_clearing-6.6.1/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:49.000000 trytond_account_payment_clearing-6.6.1/view/succeed_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.544237 trytond_account_payment_clearing-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2188 2023-05-01 10:59:51.000000 trytond_account_payment_clearing-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 10:59:50.000000 trytond_account_payment_clearing-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2764 2023-05-01 11:39:34.544237 trytond_account_payment_clearing-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.540904 trytond_account_payment_clearing-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.537571 trytond_account_payment_clearing-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2636 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2557 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2654 2023-04-30 10:46:36.000000 trytond_account_payment_clearing-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2049 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2140 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2297 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:40.000000 trytond_account_payment_clearing-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15802 2023-04-21 08:36:08.000000 trytond_account_payment_clearing-6.8.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:39:34.544237 trytond_account_payment_clearing-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4664 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9757 2023-04-30 10:46:36.000000 trytond_account_payment_clearing-6.8.0/statement.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.540904 trytond_account_payment_clearing-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3398 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/scenario_account_negative_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14481 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/scenario_account_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5499 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 10:59:45.000000 trytond_account_payment_clearing-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.544237 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2764 2023-05-01 11:39:33.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-05-01 11:39:34.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:39:33.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-05-01 11:39:33.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-05-01 11:39:33.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:39:33.000000 trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:34.540904 trytond_account_payment_clearing-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      594 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-6.8.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-6.8.0/view/succeed_start_form.xml
```

### Comparing `trytond_account_payment_clearing-6.6.1/CHANGELOG` & `trytond_account_payment_clearing-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-05-03
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

### Comparing `trytond_account_payment_clearing-6.6.1/COPYRIGHT` & `trytond_account_payment_clearing-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/LICENSE` & `trytond_account_payment_clearing-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/PKG-INFO` & `trytond_account_payment_clearing-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_clearing
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for payment clearing
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_clearing
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment clearing
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
 
 Account Payment Clearing Module
 ###############################
 
 The account_payment_clearing module allows to generate account move when a
```

### Comparing `trytond_account_payment_clearing-6.6.1/__init__.py` & `trytond_account_payment_clearing-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/account.py` & `trytond_account_payment_clearing-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/doc/conf.py` & `trytond_account_payment_clearing-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_payment_clearing-6.6.1/locale/bg.po` & `trytond_account_payment_clearing-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/ca.po` & `trytond_account_payment_clearing-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/cs.po` & `trytond_account_payment_clearing-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/de.po` & `trytond_account_payment_clearing-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/es.po` & `trytond_account_payment_clearing-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/es_419.po` & `trytond_account_payment_clearing-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/et.po` & `trytond_account_payment_clearing-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/fa.po` & `trytond_account_payment_clearing-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/fi.po` & `trytond_account_payment_clearing-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/fr.po` & `trytond_account_payment_clearing-6.8.0/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:account.payment.journal,clearing_journal:"
 msgid "Clearing Journal"
 msgstr "Journal de compensation"
 
 msgctxt "field:account.payment.journal,clearing_posting_delay:"
 msgid "Clearing Posting Delay"
-msgstr "Délai postage de compensation"
+msgstr "Délai de comptabilisation de compensation"
 
 msgctxt "field:account.payment.succeed.start,date:"
 msgid "Date"
 msgstr "Date"
 
 msgctxt "help:account.payment,account:"
 msgid "Define the account to use for clearing move."
@@ -55,16 +55,16 @@
 msgstr "Tous les paiements du groupe sont réconciliés."
 
 msgctxt "help:account.payment.journal,clearing_posting_delay:"
 msgid ""
 "Post automatically the clearing moves after the delay.\n"
 "Leave empty for no posting."
 msgstr ""
-"Poste automatiquement les mouvements de compensation après le délai.\n"
-"Laissez vide pour ne pas poster."
+"Comptabilise automatiquement les mouvements de compensation après le délai.\n"
+"Laissez vide pour ne pas comptabiliser."
 
 msgctxt "model:account.payment.succeed.start,name:"
 msgid "Succeed Payment"
 msgstr "Réussir les paiements"
 
 msgctxt "model:ir.action,name:wizard_succeed"
 msgid "Succeed Payments"
@@ -72,15 +72,15 @@
 
 msgctxt "model:ir.model.button,string:payment_succeed_wizard_button"
 msgid "Succeed"
 msgstr "Réussir"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Post Clearing Moves"
-msgstr "Poster les mouvements de compensation"
+msgstr "Comptabiliser les mouvements de compensation"
 
 msgctxt "view:account.payment.journal:"
 msgid "Clearing"
 msgstr "Compensation"
 
 msgctxt "wizard_button:account.payment.succeed,start,end:"
 msgid "Cancel"
```

### Comparing `trytond_account_payment_clearing-6.6.1/locale/hu.po` & `trytond_account_payment_clearing-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/id.po` & `trytond_account_payment_clearing-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/it.po` & `trytond_account_payment_clearing-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/lo.po` & `trytond_account_payment_clearing-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/lt.po` & `trytond_account_payment_clearing-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/nl.po` & `trytond_account_payment_clearing-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/pl.po` & `trytond_account_payment_clearing-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/pt.po` & `trytond_account_payment_clearing-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/ro.po` & `trytond_account_payment_clearing-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/ru.po` & `trytond_account_payment_clearing-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/sl.po` & `trytond_account_payment_clearing-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/tr.po` & `trytond_account_payment_clearing-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/uk.po` & `trytond_account_payment_clearing-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/locale/zh_CN.po` & `trytond_account_payment_clearing-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/payment.py` & `trytond_account_payment_clearing-6.8.0/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,37 +5,42 @@
 
 from sql.aggregate import BoolAnd, Min
 from sql.conditionals import Coalesce
 
 from trytond import backend
 from trytond.model import ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Bool, Eval
+from trytond.pyson import Bool, Eval, TimeDelta
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 
 class Journal(metaclass=PoolMeta):
     __name__ = 'account.payment.journal'
     clearing_account = fields.Many2One('account.account', 'Clearing Account',
         domain=[
+            ('company', '=', Eval('company', -1)),
             ('type', '!=', None),
             ('closed', '!=', True),
             ('party_required', '=', False),
             ],
         states={
             'required': Bool(Eval('clearing_journal')),
             })
     clearing_journal = fields.Many2One('account.journal', 'Clearing Journal',
         states={
             'required': Bool(Eval('clearing_account')),
             })
     clearing_posting_delay = fields.TimeDelta(
         "Clearing Posting Delay",
+        domain=['OR',
+            ('clearing_posting_delay', '=', None),
+            ('clearing_posting_delay', '>=', TimeDelta()),
+            ],
         help="Post automatically the clearing moves after the delay.\n"
         "Leave empty for no posting.")
 
     @classmethod
     def cron_post_clearing_moves(cls, date=None):
         pool = Pool()
         Date = pool.get('ir.date')
@@ -238,15 +243,15 @@
             return self.clearing_move
 
         if date is None:
             date = Transaction().context.get('clearing_date')
         if date is None:
             with Transaction().set_context(company=self.company.id):
                 date = Date.today()
-        period = Period.find(self.company.id, date=date)
+        period = Period.find(self.company, date=date)
 
         local_currency = self.journal.currency == self.company.currency
         if not local_currency:
             with Transaction().set_context(date=self.date):
                 local_amount = Currency.compute(
                     self.journal.currency, self.amount, self.company.currency)
         else:
```

### Comparing `trytond_account_payment_clearing-6.6.1/payment.xml` & `trytond_account_payment_clearing-6.8.0/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/setup.py` & `trytond_account_payment_clearing-6.8.0/setup.py`

 * *Files 6% similar despite different names*

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
@@ -34,43 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_payment_clearing'
 
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
 
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_account_statement'),
     get_require_version('trytond_account_statement_rule'),
     get_require_version('trytond_account_invoice'),
-    'python-dateutil']
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module for payment clearing',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_payment_clearing'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment clearing',
     package_dir={'trytond.modules.account_payment_clearing': '.'},
     packages=(
         ['trytond.modules.account_payment_clearing']
         + ['trytond.modules.account_payment_clearing.%s' % p
             for p in find_packages()]
@@ -108,24 +107,24 @@
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

### Comparing `trytond_account_payment_clearing-6.6.1/statement.py` & `trytond_account_payment_clearing-6.8.0/statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,17 +202,18 @@
                 and l.payment.clearing_move
                 and l.payment.clearing_move.state == 'draft'])
 
 
 class StatementRuleLine(metaclass=PoolMeta):
     __name__ = 'account.statement.rule.line'
 
-    def _get_related_to(self, origin, keywords):
-        return super()._get_related_to(origin, keywords) | {
-            self._get_payment(origin, keywords),
+    def _get_related_to(self, origin, keywords, party=None, amount=0):
+        return super()._get_related_to(
+            origin, keywords, party=party, amount=amount) | {
+            self._get_payment(origin, keywords, party=party, amount=amount),
             self._get_payment_group(origin, keywords),
             }
 
     def _get_party_from(self, related_to):
         pool = Pool()
         Payment = pool.get('account.payment')
         party = super()._get_party_from(related_to)
@@ -225,25 +226,42 @@
         Payment = pool.get('account.payment')
         PaymentGroup = pool.get('account.payment.group')
         account = super()._get_account_from(related_to)
         if isinstance(related_to, (Payment, PaymentGroup)):
             account = related_to.journal.clearing_account
         return account
 
-    def _get_payment(self, origin, keywords):
+    def _get_payment(self, origin, keywords, party=None, amount=0):
         pool = Pool()
         Payment = pool.get('account.payment')
         if keywords.get('payment'):
-            payments = Payment.search([('rec_name', '=', keywords['payment'])])
+            domain = [
+                ('rec_name', '=', keywords['payment']),
+                ('company', '=', origin.company.id),
+                ('currency', '=', origin.currency.id),
+                ('state', 'in', ['processing', 'succeeded', 'failed']),
+                ('clearing_reconciled', '!=', True),
+                ]
+            if party:
+                domain.append(('party', '=', party.id))
+            if amount > 0:
+                domain.append(('kind', '=', 'receivable'))
+            elif amount < 0:
+                domain.append(('kind', '=', 'payable'))
+            payments = Payment.search(domain)
             if len(payments) == 1:
                 payment, = payments
                 return payment
 
     def _get_payment_group(self, origin, keywords):
         pool = Pool()
-        Payment = pool.get('account.payment.group')
+        PaymentGroup = pool.get('account.payment.group')
         if keywords.get('payment_group'):
-            groups, = Payment.search(
-                [('rec_name', '=', keywords['payment_group'])])
+            groups, = PaymentGroup.search([
+                    ('rec_name', '=', keywords['payment_group']),
+                    ('company', '=', origin.company.id),
+                    ('currency', '=', origin.currency.id),
+                    ('clearing_reconciled', '!=', True),
+                    ])
             if len(groups) == 1:
                 group, = groups
                 return group
```

### Comparing `trytond_account_payment_clearing-6.6.1/tests/scenario_account_negative_payment_clearing.rst` & `trytond_account_payment_clearing-6.8.0/tests/scenario_account_negative_payment_clearing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ==================================
 Negative Payment Clearing Scenario
 ==================================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment_clearing'])
 
 Create company::
 
@@ -95,15 +95,15 @@
     >>> process_payment.execute('process')
     >>> payment.reload()
     >>> payment.state
     'processing'
 
 Succeed payment::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
     >>> payment.clearing_move.state
     'draft'
     >>> payable.reload()
     >>> payable.balance
```

### Comparing `trytond_account_payment_clearing-6.6.1/tests/scenario_account_payment_clearing.rst` & `trytond_account_payment_clearing-6.8.0/tests/scenario_account_payment_clearing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 =========================
 Payment Clearing Scenario
 =========================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
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
-    >>> yesterday = today - relativedelta(days=1)
-    >>> first = today  + relativedelta(day=1)
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
+    >>> first = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment_clearing', 'account_statement'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (yesterday, first)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> receivable = accounts['receivable']
@@ -58,15 +58,15 @@
 
 Create payment journal::
 
     >>> PaymentJournal = Model.get('account.payment.journal')
     >>> payment_journal = PaymentJournal(name='Manual',
     ...     process_method='manual', clearing_journal=expense,
     ...     clearing_account=bank_clearing,
-    ...     clearing_posting_delay=datetime.timedelta(1))
+    ...     clearing_posting_delay=dt.timedelta(1))
     >>> payment_journal.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
     >>> supplier = Party(name='Supplier')
     >>> supplier.save()
@@ -105,17 +105,15 @@
     >>> process_payment.execute('process')
     >>> payment.reload()
     >>> payment.state
     'processing'
 
 Succeed payment::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
-    >>> succeed.form.date == today
-    True
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.form.date = first
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
     >>> payment.clearing_move.date == first
     True
     >>> payment.clearing_move.state
@@ -164,15 +162,15 @@
     >>> process_payment.execute('process')
     >>> payment.reload()
     >>> payment.state
     'processing'
 
 Succeed payment::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
     >>> payment.clearing_move.state
     'draft'
     >>> payable.reload()
     >>> payable.balance
@@ -189,15 +187,15 @@
     >>> payment.state
     'failed'
     >>> payment.clearing_move
     >>> payment.line.reconciliation
 
 Succeed payment and post clearing::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.form.date = yesterday
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
 
     >>> Cron = Model.get('ir.cron')
     >>> Company = Model.get('company.company')
@@ -226,15 +224,15 @@
     >>> line, = [l for l in clearing_move.lines
     ...     if l.account == payment.line.account]
     >>> bool(line.reconciliation)
     True
 
 Succeed payment to use on statement::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
 
 Create statement::
 
     >>> StatementJournal = Model.get('account.statement.journal')
@@ -370,15 +368,15 @@
     >>> process_payment.execute('process')
     >>> payment.reload()
     >>> payment.state
     'processing'
 
 Succeed payment::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
     >>> debit_line, = [l for l in payment.clearing_move.lines if l.debit > 0]
     >>> debit_line.debit
     Decimal('20.00')
     >>> debit_line.amount_second_currency
     Decimal('40.00')
 
@@ -412,15 +410,15 @@
     >>> process_payment.execute('process')
     >>> payment.reload()
     >>> payment.state
     'processing'
 
 Succeed payment::
 
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
     >>> credit_line, = [l for l in payment.clearing_move.lines if l.credit > 0]
     >>> credit_line.credit
     Decimal('50.00')
     >>> credit_line.amount_second_currency
     Decimal('-100.0')
```

### Comparing `trytond_account_payment_clearing-6.6.1/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst` & `trytond_account_payment_clearing-6.8.0/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 ======================================
 Payment Clearing Invoice Amount to Pay
 ======================================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.currency.tests.tools import get_currency
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
-    >>> first = today  + relativedelta(day=1)
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['account_payment_clearing', 'account_invoice'])
 
 Create company::
@@ -100,15 +96,15 @@
     >>> payment, = Payment.find()
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.reload()
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
 
     >>> invoice.reload()
     >>> invoice.amount_to_pay
     Decimal('0.00')
 
 Create an invoice and pay it::
@@ -133,15 +129,15 @@
     >>> payment, = Payment.find([('state', '=', 'draft')])
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.reload()
-    >>> succeed = Wizard('account.payment.succeed', [payment])
+    >>> succeed = payment.click('succeed_wizard')
     >>> succeed.execute('succeed')
 
     >>> invoice1.reload()
     >>> invoice1.amount_to_pay
     Decimal('0')
 
 Unreconcile the payment line and check the amount to pay::
```

### Comparing `trytond_account_payment_clearing-6.6.1/tox.ini` & `trytond_account_payment_clearing-6.8.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/account_payment_clearing/* -m unittest discover -s tests
-    coverage report --include=./**/account_payment_clearing/* --omit=*/tests/*
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

### Comparing `trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/PKG-INFO` & `trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-payment-clearing
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for payment clearing
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_clearing
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment clearing
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
 
 Account Payment Clearing Module
 ###############################
 
 The account_payment_clearing module allows to generate account move when a
```

### Comparing `trytond_account_payment_clearing-6.6.1/trytond_account_payment_clearing.egg-info/SOURCES.txt` & `trytond_account_payment_clearing-6.8.0/trytond_account_payment_clearing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/view/payment_form.xml` & `trytond_account_payment_clearing-6.8.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-6.6.1/view/payment_journal_form.xml` & `trytond_account_payment_clearing-6.8.0/view/payment_journal_form.xml`

 * *Files identical despite different names*

