# Comparing `tmp/trytond_account-6.6.3.tar.gz` & `tmp/trytond_account-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-6.6.3.tar", last modified: Wed May  3 17:07:12 2023, max compression
+gzip compressed data, was "trytond_account-6.8.0.tar", last modified: Mon May  1 11:44:33 2023, max compression
```

## Comparing `trytond_account-6.6.3.tar` & `trytond_account-6.8.0.tar`

### file list

```diff
@@ -1,247 +1,251 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.667924 trytond_account-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     9744 2023-05-03 17:07:08.000000 trytond_account-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-03 17:07:08.000000 trytond_account-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:48.000000 trytond_account-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_account-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-03 17:07:12.667924 trytond_account-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-13 16:52:41.000000 trytond_account-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3824 2023-05-03 16:22:12.000000 trytond_account-6.6.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   120952 2023-05-03 16:22:12.000000 trytond_account-6.6.3/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46631 2023-05-03 16:22:12.000000 trytond_account-6.6.3/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2022-12-19 12:02:48.000000 trytond_account-6.6.3/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-04-13 16:52:41.000000 trytond_account-6.6.3/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-05-03 16:22:12.000000 trytond_account-6.6.3/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6667 2023-05-03 16:22:12.000000 trytond_account-6.6.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-13 16:52:41.000000 trytond_account-6.6.3/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.657924 trytond_account-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-05-03 16:22:12.000000 trytond_account-6.6.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.657924 trytond_account-6.6.3/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/design/account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/design/fiscal-year.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/design/journal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6736 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/design/tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/design/template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.661258 trytond_account-6.6.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/create.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2022-12-19 12:02:48.000000 trytond_account-6.6.3/doc/usage/structure.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-04-13 16:52:41.000000 trytond_account-6.6.3/doc/usage/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1587 2023-05-03 16:22:12.000000 trytond_account-6.6.3/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24374 2023-05-03 16:22:12.000000 trytond_account-6.6.3/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-04-13 16:52:41.000000 trytond_account-6.6.3/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2022-12-19 12:02:48.000000 trytond_account-6.6.3/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81553 2023-04-13 16:52:41.000000 trytond_account-6.6.3/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.661258 trytond_account-6.6.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:48.000000 trytond_account-6.6.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-12-19 12:02:48.000000 trytond_account-6.6.3/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:48.000000 trytond_account-6.6.3/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:48.000000 trytond_account-6.6.3/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2022-12-19 12:02:48.000000 trytond_account-6.6.3/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13194 2023-05-03 16:22:12.000000 trytond_account-6.6.3/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11346 2023-05-03 16:22:12.000000 trytond_account-6.6.3/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.611257 trytond_account-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   126636 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125229 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   109836 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   128670 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125585 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114561 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122245 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133279 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   113610 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   127101 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   120474 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   112305 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118471 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   138201 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   129567 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125737 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117659 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   120951 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   124017 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   128523 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118530 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   109655 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   142243 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   121866 2023-05-03 16:22:12.000000 trytond_account-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2022-12-19 12:02:48.000000 trytond_account-6.6.3/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    15736 2023-05-03 16:22:12.000000 trytond_account-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2022-12-19 12:02:48.000000 trytond_account-6.6.3/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    99750 2023-05-03 16:22:12.000000 trytond_account-6.6.3/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26387 2023-05-03 16:22:12.000000 trytond_account-6.6.3/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14120 2023-05-03 16:22:12.000000 trytond_account-6.6.3/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6825 2022-12-19 12:02:48.000000 trytond_account-6.6.3/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14424 2023-05-03 16:22:12.000000 trytond_account-6.6.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-04-13 16:52:41.000000 trytond_account-6.6.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14623 2023-05-03 16:22:12.000000 trytond_account-6.6.3/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4677 2023-04-13 16:52:41.000000 trytond_account-6.6.3/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 17:07:12.667924 trytond_account-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4557 2023-05-03 16:22:12.000000 trytond_account-6.6.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70124 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.617924 trytond_account-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4654 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5233 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4815 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3159 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5029 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4902 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3981 2022-12-19 12:02:48.000000 trytond_account-6.6.3/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10929 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2628 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    68735 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_account-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4353 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2022-12-19 12:02:48.000000 trytond_account-6.6.3/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-03 16:22:12.000000 trytond_account-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.664591 trytond_account-6.6.3/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-03 17:07:11.000000 trytond_account-6.6.3/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    11430 2023-05-03 17:07:12.000000 trytond_account-6.6.3/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 17:07:11.000000 trytond_account-6.6.3/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-03 17:07:11.000000 trytond_account-6.6.3/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:32:23.000000 trytond_account-6.6.3/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-03 17:07:11.000000 trytond_account-6.6.3/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 17:07:11.000000 trytond_account-6.6.3/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2022-12-19 12:02:48.000000 trytond_account-6.6.3/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 17:07:12.654591 trytond_account-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1724 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      591 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-05-03 16:22:12.000000 trytond_account-6.6.3/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2022-12-19 12:02:48.000000 trytond_account-6.6.3/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-13 16:52:41.000000 trytond_account-6.6.3/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.691283 trytond_account-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10071 2023-05-01 11:03:09.000000 trytond_account-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:03:09.000000 trytond_account-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-01 11:44:33.691283 trytond_account-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-04-21 08:36:08.000000 trytond_account-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   125458 2023-04-30 10:46:36.000000 trytond_account-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-04-15 07:12:14.000000 trytond_account-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-01-16 14:00:20.000000 trytond_account-6.8.0/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-04-15 07:12:14.000000 trytond_account-6.8.0/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1088 2023-04-15 07:12:14.000000 trytond_account-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9401 2023-04-21 08:36:08.000000 trytond_account-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:14.000000 trytond_account-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.674616 trytond_account-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.681283 trytond_account-6.8.0/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/fiscal-year.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/journal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6736 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.681283 trytond_account-6.8.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/close.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/create.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/structure.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-04-15 07:12:14.000000 trytond_account-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25810 2023-04-28 07:46:16.000000 trytond_account-6.8.0/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-04-15 07:12:14.000000 trytond_account-6.8.0/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-04-15 07:12:14.000000 trytond_account-6.8.0/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81553 2023-04-15 07:12:14.000000 trytond_account-6.8.0/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.684616 trytond_account-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-01-16 14:00:20.000000 trytond_account-6.8.0/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13471 2023-04-15 07:12:14.000000 trytond_account-6.8.0/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-04-21 08:36:08.000000 trytond_account-6.8.0/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.644616 trytond_account-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   129951 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   128941 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   112944 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132434 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129284 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117838 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125584 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   136808 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   116831 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131223 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   124036 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   115678 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   121715 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   141931 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133225 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129526 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   120919 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   124236 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   127368 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131779 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   121797 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   112776 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   146125 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125354 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account-6.8.0/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    16493 2023-04-28 07:46:16.000000 trytond_account-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   114131 2023-04-21 08:36:08.000000 trytond_account-6.8.0/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27017 2023-04-21 08:36:08.000000 trytond_account-6.8.0/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14747 2023-04-28 07:46:16.000000 trytond_account-6.8.0/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-04-15 07:12:14.000000 trytond_account-6.8.0/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14382 2023-04-15 07:12:14.000000 trytond_account-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-04-15 07:12:14.000000 trytond_account-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15701 2023-04-21 08:36:08.000000 trytond_account-6.8.0/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4677 2023-04-15 07:12:14.000000 trytond_account-6.8.0/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:33.691283 trytond_account-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4529 2023-04-15 07:12:14.000000 trytond_account-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70888 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.651282 trytond_account-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4654 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3390 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4119 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4815 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4337 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5029 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4919 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3981 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2276 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10880 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2670 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    73136 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-04-15 07:12:14.000000 trytond_account-6.8.0/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 11:03:03.000000 trytond_account-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.687950 trytond_account-6.8.0/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    11872 2023-05-01 11:44:33.000000 trytond_account-6.8.0/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account-6.8.0/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-04-15 07:12:14.000000 trytond_account-6.8.0/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.674616 trytond_account-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1334 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      783 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1724 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      640 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/writeoff_tree.xml
```

### Comparing `trytond_account-6.6.3/CHANGELOG` & `trytond_account-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
-Version 6.6.3 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-02-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-02-05
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Support reconcile lines with currency exchange
+* Add reconcile and unreconcile from general ledger lines
+* Always raise exception when fiscal year or period are not found
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Add reversal option when cancelling move
+* Add cumulative balance to payable/receivable lines
+* Rename reconciliation name to number
+* Accrue and allocate rounding errors when there are multiple taxes
+* Use match pattern to find journal
+* Display general ledger information on account form
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add wizard to delegate move lines to another party
 * Support date range context for account type amount
 * Use context model for chart of accounts and taxes
```

### Comparing `trytond_account-6.6.3/COPYRIGHT` & `trytond_account-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/LICENSE` & `trytond_account-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/PKG-INFO` & `trytond_account-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account
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
 
 ##############
 Account Module
 ##############
```

### Comparing `trytond_account-6.6.3/__init__.py` & `trytond_account-6.8.0/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,23 +40,25 @@
         account.UpdateChartSucceed,
         account.AgedBalanceContext,
         account.AgedBalance,
         configuration.Configuration,
         configuration.ConfigurationDefaultAccount,
         configuration.DefaultTaxRule,
         configuration.Sequence,
+        configuration.Journal,
         period.Period,
         journal.Journal,
         journal.JournalSequence,
         journal.JournalCashContext,
         journal.JournalPeriod,
         move.Move,
         move.Reconciliation,
         configuration.ConfigurationTaxRounding,
         move.Line,
+        move.LineReceivablePayableContext,
         move.WriteOff,
         move.OpenJournalAsk,
         move.ReconcileLinesWriteOff,
         move.ReconcileStart,
         move.ReconcileShow,
         move.CancelMovesDefault,
         move.GroupLinesStart,
```

### Comparing `trytond_account-6.6.3/account.py` & `trytond_account-6.8.0/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 import operator
 from collections import defaultdict
 from decimal import Decimal
-from functools import wraps
 from itertools import zip_longest
 
 from dateutil.relativedelta import relativedelta
 from sql import Column, Literal, Null, Window
 from sql.aggregate import Count, Max, Min, Sum
 from sql.conditionals import Case, Coalesce
 
 from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import (
     Check, Index, ModelSQL, ModelView, Unique, fields, sequence_ordered, tree)
 from trytond.model.exceptions import AccessError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
-from trytond.pyson import Bool, Eval, If, PYSONEncoder
+from trytond.pyson import Bool, Eval, Id, If, PYSONEncoder
 from trytond.report import Report
 from trytond.tools import (
     grouped_slice, is_full_text, lstrip_wildcard, reduce_ids)
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access, inactive_records
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .common import ActivePeriodMixin, ContextCompanyMixin, PeriodMixin
 from .exceptions import (
-    AccountValidationError, ChartWarning, SecondCurrencyError)
-
-
-def inactive_records(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        with Transaction().set_context(active_test=False):
-            return func(*args, **kwargs)
-    return wrapper
+    AccountValidationError, ChartWarning, FiscalYearNotFoundError,
+    SecondCurrencyError)
 
 
 def TypeMixin(template=False):
 
     class Mixin:
         __slots__ = ()
         name = fields.Char('Name', required=True)
@@ -248,15 +240,16 @@
                 ],
             ])
     childs = fields.One2Many('account.account.type', 'parent', 'Children',
         domain=[
             ('company', '=', Eval('company', -1)),
             ])
     currency = fields.Function(fields.Many2One(
-        'currency.currency', 'Currency'), 'get_currency')
+        'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
     amount = fields.Function(Monetary(
             "Amount", currency='currency', digits='currency'),
         'get_amount')
     amount_cmp = fields.Function(Monetary(
             "Amount", currency='currency', digits='currency'),
         'get_amount_cmp')
 
@@ -266,14 +259,26 @@
     template_override = fields.Boolean('Override Template',
         help="Check to override template definition",
         states={
             'invisible': ~Bool(Eval('template', -1)),
             })
 
     @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        table = cls.__table__()
+        cls._sql_indexes.update({
+                # Index for receivable/payable balance
+                Index(
+                    table,
+                    (table.id, Index.Range()),
+                    where=table.receivable | table.payable),
+                })
+
+    @classmethod
     def __register__(cls, module_name):
         super().__register__(module_name)
         table_h = cls.__table_handler__(module_name)
 
         # Migration from 5.0: remove display_balance
         table_h.drop_column('display_balance')
 
@@ -290,14 +295,18 @@
         if self.parent:
             self.statement = self.parent.statement
 
     def get_currency(self, name):
         return self.company.currency.id
 
     @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
+    @classmethod
     def get_amount(cls, types, name):
         pool = Pool()
         Account = pool.get('account.account')
         GeneralLedger = pool.get('account.general_ledger.account')
         context = Transaction().context
 
         res = {}
@@ -421,16 +430,16 @@
         to_save = []
         childs = [self]
         while childs:
             for child in childs:
                 if child.template:
                     if not child.template_override:
                         if child.template.parent:
-                            parent = template2type[
-                                child.template.parent.id]
+                            parent = template2type.get(
+                                child.template.parent.id)
                         else:
                             parent = None
                         old_parent = (
                             child.parent.id if child.parent else None)
                         if parent != old_parent:
                             child.parent = parent
                             to_save.append(child)
@@ -556,14 +565,18 @@
                 field.domain = [
                     If(Eval('parent')
                         & Eval('_parent_parent.%s' % type_)
                         & Eval('_parent_parent.parent'),
                         ('id', '=', Eval('_parent_parent.%s' % type_)),
                         ()),
                     ]
+                field.states['required'] = (
+                    Eval('parent')
+                    & Eval('_parent_parent.%s' % type_)
+                    & Eval('_parent_parent.parent'))
 
                 cls.childs.domain.append(
                     If(Eval(type_) & Eval('parent'),
                         (type_, '=', Eval(type_)),
                         ()))
 
         @classmethod
@@ -841,26 +854,27 @@
     __name__ = 'account.account'
     _states = {
         'readonly': (Bool(Eval('template', -1))
             & ~Eval('template_override', False)),
         }
     company = fields.Many2One('company.company', 'Company', required=True,
             ondelete="RESTRICT")
-    currency = fields.Function(fields.Many2One('currency.currency',
-        'Currency'), 'get_currency')
-    second_currency = fields.Many2One('currency.currency',
-        'Secondary Currency', help='Force all moves for this account \n'
-        'to have this secondary currency.', ondelete="RESTRICT",
+    currency = fields.Function(fields.Many2One(
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
+    second_currency = fields.Many2One(
+        'currency.currency', "Second Currency", ondelete="RESTRICT",
         domain=[
             ('id', '!=', Eval('currency', -1)),
             ],
         states={
             'readonly': _states['readonly'],
             'invisible': ~Eval('deferral', False),
-            })
+            },
+        help="Force all moves for this account to have this second currency.")
     type = fields.Many2One(
         'account.account.type', "Type", ondelete='RESTRICT',
         states={
             'readonly': _states['readonly'],
             },
         domain=[
             ('company', '=', Eval('company')),
@@ -1007,14 +1021,18 @@
     def default_template_override(cls):
         return False
 
     def get_currency(self, name):
         return self.company.currency.id
 
     @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
+    @classmethod
     def get_balance(cls, accounts, name):
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         FiscalYear = pool.get('account.fiscalyear')
         cursor = Transaction().connection.cursor()
 
         table_a = cls.__table__()
@@ -1182,14 +1200,16 @@
         'general_ledger_balance', 'taxes']
 
     @fields.depends('parent', *(__on_change_parent_fields
             + ['_parent_parent.%s' % f for f in __on_change_parent_fields]))
     def on_change_parent(self):
         if not self.parent:
             return
+        if self.id is not None and self.id >= 0:
+            return
         for field in self.__on_change_parent_fields:
             if (not getattr(self, field)
                     or field in {'reconcile', 'deferral',
                         'party_required', 'general_ledger_balance'}):
                 setattr(self, field, getattr(self.parent, field))
 
     @classmethod
@@ -1408,14 +1428,28 @@
             if self.replaced_by:
                 return self.replaced_by.current(date=date)
             else:
                 return None
         else:
             return self
 
+    @classmethod
+    def view_attributes(cls):
+        return super().view_attributes() + [
+            ('//page[@id="general_ledger"]', 'states', {
+                    'invisible': ((Eval('id', -1) < 0)
+                        | ~Id('account', 'group_account').in_(
+                            Eval('context', {}).get('groups', []))),
+                    }),
+            ('//link[@name="account.act_general_ledger_account_party_form"]',
+                'states', {
+                    'invisible': ~Eval('party_required', False),
+                    }),
+            ]
+
 
 class AccountParty(ActivePeriodMixin, ModelSQL):
     "Account Party"
     __name__ = 'account.account.party'
     account = fields.Many2One('account.account', "Account")
     party = fields.Many2One(
         'party.party', "Party",
@@ -1449,15 +1483,16 @@
         'get_credit_debit')
     line_count = fields.Function(
         fields.Integer("Line Count"), 'get_credit_debit')
     second_currency = fields.Many2One(
         'currency.currency', "Secondary Currency")
 
     currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'get_currency')
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
 
     @classmethod
     def table_query(cls):
         pool = Pool()
         Line = pool.get('account.move.line')
         Account = pool.get('account.account')
         line = Line.__table__()
@@ -1613,14 +1648,18 @@
                 cls.get_credit_debit, deferral=None)
         else:
             return result
 
     def get_currency(self, name):
         return self.company.currency.id
 
+    @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
 
 class AccountDeferral(ModelSQL, ModelView):
     '''
     Account Deferral
 
     It is used to deferral the debit/credit of account by fiscal year.
     '''
@@ -1632,15 +1671,16 @@
         "Debit", currency='currency', digits='currency', required=True)
     credit = Monetary(
         "Credit", currency='currency', digits='currency', required=True)
     balance = fields.Function(Monetary(
             "Balance", currency='currency', digits='currency'),
         'get_balance')
     currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'get_currency')
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
     amount_second_currency = Monetary(
         "Amount Second Currency",
         currency='second_currency', digits='second_currency', required=True,
         states={
             'invisible': ~Eval('second_currency'),
             })
     line_count = fields.Integer("Line Count", required=True)
@@ -1736,14 +1776,18 @@
             if not isinstance(balance, Decimal):
                 balances[id_] = Decimal(str(balance))
         return balances
 
     def get_currency(self, name):
         return self.account.currency.id
 
+    @classmethod
+    def search_currency(cls, name, clause):
+        return [('account.' + clause[0], *clause[1:])]
+
     def get_second_currency(self, name):
         if self.account.second_currency:
             return self.account.second_currency.id
 
     def get_rec_name(self, name):
         return '%s - %s' % (self.account.rec_name, self.fiscalyear.rec_name)
 
@@ -1846,24 +1890,28 @@
     start_balance = fields.Function(Monetary(
             "Start Balance", currency='currency', digits='currency'),
         'get_account', searcher='search_account')
     end_balance = fields.Function(Monetary(
             "End Balance", currency='currency', digits='currency'),
         'get_account', searcher='search_account')
     currency = fields.Function(fields.Many2One(
-        'currency.currency', 'Currency'), 'get_currency')
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls._order.insert(0, ('account', 'ASC'))
 
     @classmethod
     def table_query(cls):
-        context = Transaction().context
+        pool = Pool()
+        LedgerAccountContext = pool.get(
+            'account.general_ledger.account.context')
+        context = LedgerAccountContext.get_context()
         Account = cls._get_account()
         account = Account.__table__()
         columns = []
         for fname, field in cls._fields.items():
             if not hasattr(field, 'set'):
                 if (isinstance(field, fields.Many2One)
                         and field.get_target() == Account):
@@ -1876,15 +1924,17 @@
             & (account.type != Null)
             & (account.closed != Literal(True)))
 
     @classmethod
     def get_period_ids(cls, name):
         pool = Pool()
         Period = pool.get('account.period')
-        context = Transaction().context
+        LedgerAccountContext = pool.get(
+            'account.general_ledger.account.context')
+        context = LedgerAccountContext.get_context()
 
         period = None
         if name.startswith('start_'):
             period_ids = []
             if context.get('start_period'):
                 period = Period(context['start_period'])
         elif name.startswith('end_'):
@@ -1919,30 +1969,36 @@
             if name.startswith('end_'):
                 # Always include ending period
                 period_ids.append(period.id)
         return period_ids
 
     @classmethod
     def get_dates(cls, name):
-        context = Transaction().context
+        pool = Pool()
+        LedgerAccountContext = pool.get(
+            'account.general_ledger.account.context')
+        context = LedgerAccountContext.get_context()
         if name.startswith('start_'):
             from_date = context.get('from_date')
             if from_date:
                 from_date -= datetime.timedelta(days=1)
             return None, from_date
         elif name.startswith('end_'):
             return None, context.get('to_date')
         return None, None
 
     @classmethod
     def get_account(cls, records, name):
+        pool = Pool()
+        LedgerAccountContext = pool.get(
+            'account.general_ledger.account.context')
         Account = cls._get_account()
 
         period_ids, from_date, to_date = None, None, None
-        context = Transaction().context
+        context = LedgerAccountContext.get_context()
         if context.get('start_period') or context.get('end_period'):
             period_ids = cls.get_period_ids(name)
         elif context.get('from_date') or context.get('end_date'):
             from_date, to_date = cls.get_dates(name)
         else:
             if name.startswith('start_'):
                 period_ids = []
@@ -1985,16 +2041,19 @@
 
         ids = [a.id for a in accounts
             if operand is not None and operator_(getattr(a, fname), operand)]
         return [('id', 'in', ids)]
 
     @classmethod
     def _debit_credit_context(cls):
+        pool = Pool()
+        LedgerAccountContext = pool.get(
+            'account.general_ledger.account.context')
         period_ids, from_date, to_date = None, None, None
-        context = Transaction().context
+        context = LedgerAccountContext.get_context()
         if context.get('start_period') or context.get('end_period'):
             start_period_ids = set(cls.get_period_ids('start_balance'))
             end_period_ids = set(cls.get_period_ids('end_balance'))
             period_ids = list(end_period_ids.difference(start_period_ids))
         elif context.get('from_date') or context.get('to_date'):
             from_date = context.get('from_date')
             to_date = context.get('to_date')
@@ -2034,14 +2093,18 @@
         ids = [a.id for a in accounts
             if operand is not None and operator_(getattr(a, name), operand)]
         return [('id', 'in', ids)]
 
     def get_currency(self, name):
         return self.company.currency.id
 
+    @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
     def get_rec_name(self, name):
         return self.account.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('account.rec_name',) + tuple(clause[1:])]
 
@@ -2105,31 +2168,41 @@
                 ()),
             ],
         states={
             'invisible': (Eval('start_period', False)
                 | Eval('end_period', False)),
             })
     company = fields.Many2One('company.company', 'Company', required=True)
-    posted = fields.Boolean('Posted Move', help="Only include posted moves.")
+    posted = fields.Boolean('Posted Moves', help="Only include posted moves.")
     journal = fields.Many2One(
         'account.journal', "Journal",
         context={
             'company': Eval('company', -1),
             },
         depends={'company'},
         help="Only include moves from the journal.")
 
     @classmethod
     def default_fiscalyear(cls):
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
+        Period = pool.get('account.period')
         context = Transaction().context
-        return context.get(
-            'fiscalyear',
-            FiscalYear.find(context.get('company'), exception=False))
+        if context.get('fiscalyear', -1) >= 0:
+            return context['fiscalyear']
+        elif context.get('period', -1) >= 0:
+            period = Period(context['period'])
+            return period.fiscalyear.id
+        else:
+            try:
+                fiscalyear = FiscalYear.find(
+                    context.get('company'), test_state=False)
+            except FiscalYearNotFoundError:
+                return None
+            return fiscalyear.id
 
     @classmethod
     def default_start_period(cls):
         return Transaction().context.get('start_period')
 
     @classmethod
     def default_end_period(cls):
@@ -2186,14 +2259,22 @@
             self.start_period = self.end_period = None
 
     @fields.depends('to_date')
     def on_change_to_date(self):
         if self.to_date:
             self.start_period = self.end_period = None
 
+    @classmethod
+    def get_context(cls, fields_names=None):
+        fields_names = fields_names.copy() if fields_names is not None else []
+        fields_names += [
+            'fiscalyear', 'start_period', 'end_period', 'from_date', 'to_date',
+            'company', 'posted', 'journal']
+        return cls.default_get(fields_names, with_rec_name=False)
+
 
 class GeneralLedgerAccountParty(_GeneralLedgerAccount):
     "General Ledger Account Party"
     __name__ = 'account.general_ledger.account.party'
 
     party = fields.Many2One(
         'party.party', "Party",
@@ -2276,40 +2357,47 @@
         "Internal Balance", currency='currency', digits='currency')
     balance = fields.Function(Monetary(
             "Balance", currency='currency', digits='currency'),
         'get_balance')
     origin = fields.Reference('Origin', selection='get_origin')
     description = fields.Char('Description')
     move_description = fields.Char('Move Description')
+    amount_second_currency = Monetary(
+        "Amount Second Currency",
+        currency='second_currency', digits='second_currency')
+    second_currency = fields.Many2One('currency.currency', 'Second Currency')
     reconciliation = fields.Many2One(
         'account.move.reconciliation', "Reconciliation")
     state = fields.Selection([
         ('draft', 'Draft'),
         ('posted', 'Posted'),
         ], "State", sort=False)
     state_string = state.translated('state')
     currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'get_currency')
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
 
     @classmethod
     def __setup__(cls):
         super(GeneralLedgerLine, cls).__setup__()
         cls.__access__.add('account')
         cls._order.insert(0, ('date', 'ASC'))
 
     @classmethod
     def table_query(cls):
         pool = Pool()
         Line = pool.get('account.move.line')
         Move = pool.get('account.move')
         LedgerAccount = pool.get('account.general_ledger.account')
+        LedgerLineContext = pool.get(
+            'account.general_ledger.line.context')
         Account = pool.get('account.account')
         transaction = Transaction()
         database = transaction.database
-        context = transaction.context
+        context = LedgerLineContext.get_context()
         line = Line.__table__()
         move = Move.__table__()
         account = Account.__table__()
         columns = []
         for fname, field in cls._fields.items():
             if hasattr(field, 'set'):
                 continue
@@ -2332,31 +2420,39 @@
             elif (not field_line
                     or fname == 'state'
                     or isinstance(field_line, fields.Function)):
                 column = Column(move, fname).as_(fname)
             else:
                 column = Column(line, fname).as_(fname)
             columns.append(column)
-        with Transaction().set_context(LedgerAccount._debit_credit_context()):
+        with Transaction().set_context(
+                context, **LedgerAccount._debit_credit_context()):
             line_query, fiscalyear_ids = Line.query_get(line)
         return line.join(move, condition=line.move == move.id
             ).join(account, condition=line.account == account.id
                 ).select(*columns, where=line_query)
 
     def get_currency(self, name):
         return self.company.currency.id
 
     @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
+    @classmethod
     def get_origin(cls):
         Line = Pool().get('account.move.line')
         return Line.get_origin()
 
     def get_balance(self, name):
+        pool = Pool()
+        LedgerLineContext = pool.get(
+            'account.general_ledger.line.context')
         transaction = Transaction()
-        context = transaction.context
+        context = LedgerLineContext.get_context()
         database = transaction.database
         balance = self.internal_balance
         if database.has_window_functions():
             if context.get('party_cumulate', False) and self.account_party:
                 balance += self.account_party.start_balance
             else:
                 balance += self.account.start_balance
@@ -2394,25 +2490,38 @@
                         # There can be more combinations of account-party in
                         # the database than from records
                         continue
                     for record_id in account_party_ids:
                         account_parties[record_id] = id_
         return account_parties
 
+    @classmethod
+    def reconcile(cls, *lines_list, **kwargs):
+        pool = Pool()
+        Line = pool.get('account.move.line')
+        lines_list = [Line.browse(l) for l in lines_list]
+        return Line.reconcile(*lines_list, **kwargs)
+
 
 class GeneralLedgerLineContext(GeneralLedgerAccountContext):
     'General Ledger Line Context'
     __name__ = 'account.general_ledger.line.context'
 
     party_cumulate = fields.Boolean('Cumulate per Party')
 
     @classmethod
     def default_party_cumulate(cls):
         return False
 
+    @classmethod
+    def get_context(cls, fields_names=None):
+        fields_names = fields_names.copy() if fields_names is not None else []
+        fields_names.append('party_cumulate')
+        return super().get_context(fields_names=fields_names)
+
 
 class GeneralLedger(Report):
     __name__ = 'account.general_ledger'
 
     @classmethod
     def get_context(cls, records, header, data):
         pool = Pool()
@@ -2472,15 +2581,15 @@
 
 
 class BalanceSheetContext(ModelView):
     'Balance Sheet Context'
     __name__ = 'account.balance_sheet.context'
     date = fields.Date('Date', required=True)
     company = fields.Many2One('company.company', 'Company', required=True)
-    posted = fields.Boolean('Posted Move', help="Only include posted moves.")
+    posted = fields.Boolean('Posted Moves', help="Only include posted moves.")
 
     @staticmethod
     def default_date():
         Date_ = Pool().get('ir.date')
         return Transaction().context.get('date', Date_.today())
 
     @staticmethod
@@ -2606,19 +2715,24 @@
                 ('to_date_cmp', '>=', Eval('from_date_cmp')),
                 ()),
             ],
         states={
             'invisible': ~Eval('comparison', False),
             })
 
-    @staticmethod
-    def default_fiscalyear():
-        FiscalYear = Pool().get('account.fiscalyear')
-        return FiscalYear.find(
-            Transaction().context.get('company'), exception=False)
+    @classmethod
+    def default_fiscalyear(cls):
+        pool = Pool()
+        FiscalYear = pool.get('account.fiscalyear')
+        try:
+            fiscalyear = FiscalYear.find(
+                cls.default_company(), test_state=False)
+        except FiscalYearNotFoundError:
+            return None
+        return fiscalyear.id
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @staticmethod
     def default_posted():
@@ -2766,15 +2880,16 @@
     term2 = Monetary(
         "Second Term", currency='currency', digits='currency')
     term3 = Monetary(
         "Third Term", currency='currency', digits='currency')
     balance = Monetary(
         "Balance", currency='currency', digits='currency')
     currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'get_currency')
+            'currency.currency', "Currency"),
+        'get_currency', searcher='search_currency')
 
     @classmethod
     def __setup__(cls):
         super(AgedBalance, cls).__setup__()
         cls._order.insert(0, ('party', 'ASC'))
 
     @classmethod
@@ -2888,14 +3003,18 @@
             return account_type.receivable
         else:
             return Literal(False)
 
     def get_currency(self, name):
         return self.company.currency.id
 
+    @classmethod
+    def search_currency(cls, name, clause):
+        return [('company.' + clause[0], *clause[1:])]
+
 
 class AgedBalanceReport(Report):
     __name__ = 'account.aged_balance'
 
     @classmethod
     def get_context(cls, records, header, data):
         pool = Pool()
@@ -3140,24 +3259,24 @@
             ])
     update = StateTransition()
     succeed = StateView('account.update_chart.succeed',
         'account.update_chart_succeed_view_form', [
             Button('OK', 'end', 'tryton-ok', default=True),
             ])
 
+    @check_access
     def default_start(self, fields):
         pool = Pool()
         Account = pool.get('account.account')
 
         defaults = {}
-        with Transaction().set_context(_check_access=True):
-            charts = Account.search([
-                    ('parent', '=', None),
-                    ('template', '!=', None),
-                    ], limit=2)
+        charts = Account.search([
+                ('parent', '=', None),
+                ('template', '!=', None),
+                ], limit=2)
         if len(charts) == 1:
             defaults['account'] = charts[0].id
         return defaults
 
     @inactive_records
     def transition_update(self):
         pool = Pool()
```

### Comparing `trytond_account-6.6.3/account.xml` & `trytond_account-6.8.0/account.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account-6.6.3/account.xml` & `trytond_account-6.8.0/account.xml`

```diff
@@ -546,14 +546,19 @@
       <field name="act_window" ref="act_general_ledger_account_party_form"/>
     </record>
     <record model="ir.action.keyword" id="act_general_ledger_account_party_form_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">account.general_ledger.account,-1</field>
       <field name="action" ref="act_general_ledger_account_party_form"/>
     </record>
+    <record model="ir.action.keyword" id="act_general_ledger_account_party_form_keyword_account">
+      <field name="keyword">form_relate</field>
+      <field name="model">account.account,-1</field>
+      <field name="action" ref="act_general_ledger_account_party_form"/>
+    </record>
     <record model="ir.action.wizard" id="act_general_ledger_account_party_open">
       <field name="name">Open General Ledger Account Parties</field>
       <field name="wiz_name">account.general_ledger.account.party.open</field>
     </record>
     <record model="ir.action.keyword" id="act_general_ledger_account_party_open_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">account.general_ledger.account.party,-1</field>
@@ -616,15 +621,19 @@
       <field name="act_window" ref="act_general_ledger_line_form"/>
     </record>
     <record model="ir.action.keyword" id="act_general_ledger_line_form_keyword">
       <field name="keyword">tree_open</field>
       <field name="model">account.general_ledger.account,-1</field>
       <field name="action" ref="act_general_ledger_line_form"/>
     </record>
-    <!-- TODO relate from account -->
+    <record model="ir.action.keyword" id="act_general_ledger_line_form_keyword_account">
+      <field name="keyword">form_relate</field>
+      <field name="model">account.account,-1</field>
+      <field name="action" ref="act_general_ledger_line_form"/>
+    </record>
     <record model="ir.rule.group" id="rule_group_general_ledger_line_companies">
       <field name="name">User in companies</field>
       <field name="model" search="[('model', '=', 'account.general_ledger.line')]"/>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_general_ledger_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
```

### Comparing `trytond_account-6.6.3/aged_balance.fodt` & `trytond_account-6.8.0/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/common.py` & `trytond_account-6.8.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/company.py` & `trytond_account-6.8.0/company.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     __name__ = 'company.company'
 
     @classmethod
     def write(cls, *args):
         pool = Pool()
         Move = pool.get('account.move')
         transaction = Transaction()
-        if (transaction.user
-                and transaction.context.get('_check_access')):
+        if transaction.user and transaction.check_access:
             actions = iter(args)
             for companies, values in zip(actions, actions):
                 if 'currency' in values:
                     moves = Move.search([
                             ('company', 'in', [c.id for c in companies]),
                             ],
                         limit=1, order=[])
```

### Comparing `trytond_account-6.6.3/configuration.py` & `trytond_account-6.8.0/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,35 +54,66 @@
             domain=[
                 ('company', 'in',
                     [Eval('context', {}).get('company', -1), None]),
                 ('sequence_type', '=',
                     Id('account',
                         'sequence_type_account_move_reconciliation')),
                 ]))
+    currency_exchange_journal = fields.MultiValue(fields.Many2One(
+            'account.journal', "Currency Exchange Journal",
+            domain=[
+                ('type', '=', 'write-off'),
+                ]))
+    currency_exchange_credit_account = fields.MultiValue(fields.Many2One(
+            'account.account', "Currency Exchange Credit Account",
+            domain=[
+                ('closed', '!=', True),
+                ('type.statement', '=', 'income'),
+                ('company', '=', Eval('context', {}).get('company', -1)),
+                ('second_currency', '=', None),
+                ]))
+    currency_exchange_debit_account = fields.MultiValue(fields.Many2One(
+            'account.account', "Currency Exchange Debit Account",
+            domain=[
+                ('closed', '!=', True),
+                ('type.statement', '=', 'income'),
+                ('company', '=', Eval('context', {}).get('company', -1)),
+                ('second_currency', '=', None),
+                ]))
 
     @classmethod
     def multivalue_model(cls, field):
         pool = Pool()
-        if field in {'default_account_receivable', 'default_account_payable'}:
+        if field in {
+                'default_account_receivable', 'default_account_payable',
+                'currency_exchange_credit_account',
+                'currency_exchange_debit_account'}:
             return pool.get('account.configuration.default_account')
         if field in {'default_customer_tax_rule', 'default_supplier_tax_rule'}:
             return pool.get('account.configuration.default_tax_rule')
         if field == 'reconciliation_sequence':
             return pool.get('account.configuration.sequence')
+        elif field == 'currency_exchange_journal':
+            return pool.get('account.configuration.journal')
         return super(Configuration, cls).multivalue_model(field)
 
     @classmethod
     def default_tax_rounding(cls, **pattern):
         return cls.multivalue_model('tax_rounding').default_tax_rounding()
 
     @classmethod
     def default_reconciliation_sequence(cls, **pattern):
         return cls.multivalue_model(
             'reconciliation_sequence').default_reconciliation_sequence()
 
+    @classmethod
+    def default_currency_exchange_journal(cls, **pattern):
+        return cls.multivalue_model(
+            'currency_exchange_journal').default_currency_exchange_journal()
+
 
 class ConfigurationDefaultAccount(ModelSQL, CompanyValueMixin):
     "Account Configuration Default Account"
     __name__ = 'account.configuration.default_account'
     default_account_receivable = fields.Many2One(
         'account.account', "Default Account Receivable",
         domain=[
@@ -93,14 +124,30 @@
     default_account_payable = fields.Many2One(
         'account.account', "Default Account Payable",
         domain=[
             ('type.payable', '=', True),
             ('party_required', '=', True),
             ('company', '=', Eval('company', -1)),
             ])
+    currency_exchange_credit_account = fields.Many2One(
+        'account.account', "Currency Exchange Credit Account",
+        domain=[
+            ('closed', '!=', True),
+            ('type.statement', '=', 'income'),
+            ('company', '=', Eval('company', -1)),
+            ('second_currency', '=', None),
+            ])
+    currency_exchange_debit_account = fields.Many2One(
+        'account.account', "Currency Exchange Debit Account",
+        domain=[
+            ('closed', '!=', True),
+            ('type.statement', '=', 'income'),
+            ('company', '=', Eval('company', -1)),
+            ('second_currency', '=', None),
+            ])
 
 
 class DefaultTaxRule(ModelSQL, CompanyValueMixin):
     "Account Configuration Default Tax Rule"
     __name__ = 'account.configuration.default_tax_rule'
     default_customer_tax_rule = fields.Many2One(
         'account.tax.rule', "Default Customer Tax Rule",
@@ -163,7 +210,29 @@
         pool = Pool()
         ModelData = pool.get('ir.model.data')
         try:
             return ModelData.get_id(
                 'account', 'sequence_account_move_reconciliation')
         except KeyError:
             return None
+
+
+class Journal(ModelSQL, CompanyValueMixin):
+    "Account Configuration Journal"
+    __name__ = 'account.configuration.journal'
+    currency_exchange_journal = fields.Many2One(
+        'account.journal', "Currency Exchange Journal",
+        domain=[
+            ('type', '=', 'write-off'),
+            ],
+        context={
+            'company': Eval('company', -1),
+            })
+
+    @classmethod
+    def default_currency_exchange_journal(cls):
+        pool = Pool()
+        ModelData = pool.get('ir.model.data')
+        try:
+            return ModelData.get_id('account', 'journal_currency_exchange')
+        except KeyError:
+            return None
```

### Comparing `trytond_account-6.6.3/configuration.xml` & `trytond_account-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/conf.py` & `trytond_account-6.8.0/doc/conf.py`

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

### Comparing `trytond_account-6.6.3/doc/configuration.rst` & `trytond_account-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/account.rst` & `trytond_account-6.8.0/doc/design/account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/configuration.rst` & `trytond_account-6.8.0/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/fiscal-year.rst` & `trytond_account-6.8.0/doc/design/fiscal-year.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/journal.rst` & `trytond_account-6.8.0/doc/design/journal.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/move.rst` & `trytond_account-6.8.0/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/tax.rst` & `trytond_account-6.8.0/doc/design/tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/design/template.rst` & `trytond_account-6.8.0/doc/design/template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/reference.rst` & `trytond_account-6.8.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/setup.rst` & `trytond_account-6.8.0/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/close.rst` & `trytond_account-6.8.0/doc/usage/close.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/create.rst` & `trytond_account-6.8.0/doc/usage/create.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/process.rst` & `trytond_account-6.8.0/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/report.rst` & `trytond_account-6.8.0/doc/usage/report.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/structure.rst` & `trytond_account-6.8.0/doc/usage/structure.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/doc/usage/view.rst` & `trytond_account-6.8.0/doc/usage/view.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/exceptions.py` & `trytond_account-6.8.0/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,31 +65,31 @@
     pass
 
 
 class PostError(UserError):
     pass
 
 
-class MoveDatesError(ValidationError):
+class MoveTemplateExpressionError(UserError):
     pass
 
 
-class MoveTemplateExpressionError(UserError):
+class MoveTemplateKeywordValidationError(ValidationError):
     pass
 
 
 class CancelWarning(UserWarning):
     pass
 
 
 class ReconciliationError(ValidationError):
     pass
 
 
-class DeleteDelegatedWarning(UserWarning):
+class ReconciliationDeleteWarning(UserWarning):
     pass
 
 
 class CancelDelegatedWarning(UserWarning):
     pass
```

### Comparing `trytond_account-6.6.3/fiscalyear.py` & `trytond_account-6.8.0/fiscalyear.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from dateutil.relativedelta import relativedelta
 
+from trytond.cache import Cache
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Eval, Id
 from trytond.rpc import RPC
 from trytond.transaction import Transaction
@@ -47,14 +48,15 @@
             ('sequence_type', '=',
                 Id('account', 'sequence_type_account_move')),
             ('company', '=', Eval('company')),
             ])
     company = fields.Many2One(
         'company.company', "Company", required=True)
     icon = fields.Function(fields.Char("Icon"), 'get_icon')
+    _find_cache = Cache(__name__ + '.find', context=False)
 
     @classmethod
     def __setup__(cls):
         super(FiscalYear, cls).__setup__()
         cls._order.insert(0, ('start_date', 'DESC'))
         cls._transitions |= set((
                 ('open', 'close'),
@@ -160,14 +162,20 @@
             if years:
                 raise FiscalYearSequenceError(gettext(
                         'account.msg_fiscalyear_different_post_move_sequence',
                         first=fiscalyear.rec_name,
                         second=years[0].rec_name))
 
     @classmethod
+    def create(cls, vlist):
+        fiscalyears = super().create(vlist)
+        cls._find_cache.clear()
+        return fiscalyears
+
+    @classmethod
     def write(cls, *args):
         pool = Pool()
         Move = pool.get('account.move')
         actions = iter(args)
         for fiscalyears, values in zip(actions, actions):
             if values.get('post_move_sequence'):
                 for fiscalyear in fiscalyears:
@@ -179,20 +187,22 @@
                                     ('state', '=', 'posted'),
                                     ]):
                             raise AccessError(
                                 gettext('account.'
                                     'msg_change_fiscalyear_post_move_sequence',
                                     fiscalyear=fiscalyear.rec_name))
         super(FiscalYear, cls).write(*args)
+        cls._find_cache.clear()
 
     @classmethod
     def delete(cls, fiscalyears):
         Period = Pool().get('account.period')
         Period.delete([p for f in fiscalyears for p in f.periods])
         super(FiscalYear, cls).delete(fiscalyears)
+        cls._find_cache.clear()
 
     @classmethod
     def create_period(cls, fiscalyears, interval=1, end_day=31):
         '''
         Create periods for the fiscal years with month interval
         '''
         Period = Pool().get('account.period')
@@ -222,42 +232,64 @@
 
     @classmethod
     @ModelView.button_action('account.act_create_periods')
     def create_periods(cls, fiscalyears):
         pass
 
     @classmethod
-    def find(cls, company_id, date=None, exception=True):
+    def find(cls, company, date=None, test_state=True):
         '''
-        Return the fiscal year for the company_id
-            at the date or the current date.
-        If exception is set the function will raise an exception
-            if any fiscal year is found.
+        Return the fiscal year for the company at the date or the current date
+        or raise FiscalYearNotFoundError.
+        If test_state is true, it searches on non-closed fiscal years
         '''
         pool = Pool()
         Lang = pool.get('ir.lang')
         Date = pool.get('ir.date')
+        Company = pool.get('company.company')
 
+        company_id = int(company) if company is not None else None
         if not date:
             with Transaction().set_context(company=company_id):
                 date = Date.today()
-        fiscalyears = cls.search([
-            ('start_date', '<=', date),
-            ('end_date', '>=', date),
-            ('company', '=', company_id),
-            ], order=[('start_date', 'DESC')], limit=1)
-        if not fiscalyears:
-            if exception:
-                lang = Lang.get()
+        key = (company_id, date)
+        fiscalyear = cls._find_cache.get(key, -1)
+        if fiscalyear is not None and fiscalyear < 0:
+            clause = [
+                ('start_date', '<=', date),
+                ('end_date', '>=', date),
+                ('company', '=', company_id),
+                ]
+            fiscalyears = cls.search(
+                clause, order=[('start_date', 'DESC')], limit=1)
+            if fiscalyears:
+                fiscalyear, = fiscalyears
+            else:
+                fiscalyear = None
+            cls._find_cache.set(key, int(fiscalyear) if fiscalyear else None)
+        elif fiscalyear is not None:
+            fiscalyear = cls(fiscalyear)
+        found = fiscalyear and (not test_state or fiscalyear.state == 'open')
+        if not found:
+            lang = Lang.get()
+            if company is not None and not isinstance(company, Company):
+                company = Company(company)
+            if not fiscalyear:
                 raise FiscalYearNotFoundError(
                     gettext('account.msg_no_fiscalyear_date',
-                        date=lang.strftime(date)))
+                        date=lang.strftime(date),
+                        company=company.rec_name if company else ''))
             else:
-                return None
-        return fiscalyears[0].id
+                raise FiscalYearNotFoundError(
+                    gettext('account.msg_no_open_fiscalyear_date',
+                        date=lang.strftime(date),
+                        fiscalyear=fiscalyear.rec_name,
+                        company=company.rec_name if company else ''))
+        else:
+            return fiscalyear
 
     def get_deferral(self, account):
         'Computes deferrals for accounts'
         pool = Pool()
         Currency = pool.get('currency.currency')
         Deferral = pool.get('account.account.deferral')
 
@@ -393,16 +425,15 @@
             ('closed', '!=', True),
             ('company', '=', Eval('company', -1)),
             ('deferral', '=', True),
             ])
 
     @fields.depends('fiscalyear')
     def on_change_with_company(self, name=None):
-        if self.fiscalyear:
-            return self.fiscalyear.company.id
+        return self.fiscalyear.company if self.fiscalyear else None
 
 
 class BalanceNonDeferral(Wizard):
     'Balance Non-Deferral'
     __name__ = 'account.fiscalyear.balance_non_deferral'
     start = StateView('account.fiscalyear.balance_non_deferral.start',
         'account.fiscalyear_balance_non_deferral_start_view_form', [
@@ -647,9 +678,10 @@
             if p.type == 'standard')
         if interval.is_integer():
             FiscalYear.create_period([fiscalyear], interval, end_day)
         return fiscalyear
 
     def do_create_(self, action):
         fiscalyear = self.create_fiscalyear()
+        fiscalyear.save()
         action['views'].reverse()
         return action, {'res_id': fiscalyear.id}
```

### Comparing `trytond_account-6.6.3/fiscalyear.xml` & `trytond_account-6.8.0/fiscalyear.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/general_journal.fodt` & `trytond_account-6.8.0/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/general_ledger.fodt` & `trytond_account-6.8.0/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/icons/LICENSE` & `trytond_account-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/journal.py` & `trytond_account-6.8.0/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from decimal import Decimal
 
 from sql.aggregate import Sum
 
 from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import (
-    DeactivableMixin, ModelSQL, ModelView, Unique, Workflow, fields)
+    DeactivableMixin, MatchMixin, ModelSQL, ModelView, Unique, Workflow,
+    fields, sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Id
 from trytond.tools import (
@@ -21,15 +22,17 @@
 
 STATES = {
     'readonly': Eval('state') == 'close',
 }
 
 
 class Journal(
-        DeactivableMixin, ModelSQL, ModelView, CompanyMultiValueMixin):
+        DeactivableMixin, MatchMixin,
+        sequence_ordered('matching_sequence', "Matching Sequence"),
+        ModelSQL, ModelView, CompanyMultiValueMixin):
     'Journal'
     __name__ = 'account.journal'
     name = fields.Char('Name', size=None, required=True, translate=True)
     code = fields.Char('Code', size=None)
     type = fields.Selection([
             ('general', "General"),
             ('revenue', "Revenue"),
@@ -150,14 +153,20 @@
                 result['debit'][journal_id] = company.currency.round(debit)
                 result['credit'][journal_id] = company.currency.round(credit)
                 result['balance'][journal_id] = company.currency.round(
                     debit - credit)
         return result
 
     @classmethod
+    def find(cls, pattern):
+        for journal in cls.search([]):
+            if journal.match(pattern):
+                return journal
+
+    @classmethod
     def write(cls, *args):
         pool = Pool()
         Move = pool.get('account.move')
         actions = iter(args)
         for journals, values in zip(actions, actions):
             if 'type' in values:
                 for sub_journals in grouped_slice(journals):
```

### Comparing `trytond_account-6.6.3/journal.xml` & `trytond_account-6.8.0/journal.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account-6.6.3/journal.xml` & `trytond_account-6.8.0/journal.xml`

```diff
@@ -190,9 +190,14 @@
       <field name="type">general</field>
     </record>
     <record model="account.journal" id="journal_miscellaneous">
       <field name="name">Miscellaneous</field>
       <field name="code">MISC</field>
       <field name="type">general</field>
     </record>
+    <record model="account.journal" id="journal_currency_exchange">
+      <field name="name">Currency Exchange</field>
+      <field name="code">EXC</field>
+      <field name="type">write-off</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_account-6.6.3/locale/bg.po` & `trytond_account-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,17 @@
 msgid "Replaced By"
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Десен"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Втора валута"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Начална дата"
 
@@ -594,32 +595,44 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Дата"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Публикувано движение"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Дата"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Публикувано движение"
 
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Разнодна сметка по подразбиране"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Приходна сметка по подразбиране"
@@ -644,14 +657,24 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Фирма"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Разнодна сметка по подразбиране"
 
 #, fuzzy
 msgctxt ""
@@ -673,14 +696,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Правило за данък на доставчик"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Фирма"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -942,15 +974,15 @@
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Дневник"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Публикувано движение"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Начален период"
 
@@ -1045,14 +1077,19 @@
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Разходна сметка"
 
 #, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Сума в допълнителна валута"
+
+#, fuzzy
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Баланс"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
@@ -1113,14 +1150,19 @@
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Съгласуване"
 
 #, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Втора валута"
+
+#, fuzzy
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Състояние"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
@@ -1148,15 +1190,15 @@
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Публикувано движение"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Начален период"
 
@@ -1246,14 +1288,19 @@
 msgid "Currency"
 msgstr "Валута"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Дебит"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Съгласувания"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Име"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Последователност"
@@ -1357,14 +1404,18 @@
 msgstr "Състояние"
 
 #, fuzzy
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Описание"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Сметка"
 
 #, fuzzy
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1447,14 +1498,19 @@
 msgid "Party"
 msgstr "Партньор"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Период"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Съгласуване"
@@ -1501,14 +1557,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Дневник"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Разходен"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "За получаване"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Съгласуване"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1685,17 +1756,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Редове"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Име"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Номер"
 
 #, fuzzy
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
@@ -1815,14 +1887,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
@@ -2539,18 +2616,17 @@
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 "Позволява редове от тази сметка\n"
 "да бъдат съгласувани"
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Всички движение по тази сметка\n"
 "задължително да имат втора валута"
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
@@ -2667,14 +2743,18 @@
 msgid "Only include posted moves."
 msgstr "Показване само на публикувани движения"
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Сумата изразена във втора валута"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2862,14 +2942,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Настройване на сметка"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Настройване на сметка"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Настройване на сметка"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2937,14 +3022,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2989,14 +3079,18 @@
 msgid "Delegate Lines"
 msgstr "Затваряне на редове"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3472,31 +3566,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Разходен"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "За получаване"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3714,38 +3791,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3810,14 +3901,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4295,18 +4392,17 @@
 msgstr "Фирма:"
 
 #, fuzzy
 msgctxt "report:account.account.type.statement:"
 msgid "Date:"
 msgstr "Дата:"
 
-#, fuzzy
 msgctxt "report:account.account.type.statement:"
 msgid "Fiscal Year:"
-msgstr "Финансова година"
+msgstr "Финансова година:"
 
 #, fuzzy
 msgctxt "report:account.account.type.statement:"
 msgid "From Date:"
 msgstr "От дата:"
 
 #, fuzzy
@@ -5001,25 +5097,50 @@
 msgstr "Наследници"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Обща информация"
 
 #, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
+#, fuzzy
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Условия"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Сметка на кредитно известие"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Валута"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Основна сметка"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Фактура"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Дневник"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Движение"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Партньор"
 
@@ -5098,14 +5219,19 @@
 msgstr "Месеци"
 
 #, fuzzy
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Друга информация"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Баланс"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Кредит"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Дебит"
```

### Comparing `trytond_account-6.6.3/locale/ca.po` & `trytond_account-6.8.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -103,16 +103,16 @@
 msgstr "Substituït per"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Dreta"
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Moneda secundària"
+msgid "Second Currency"
+msgstr "Segona moneda"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data inicial"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -523,29 +523,41 @@
 msgstr "Data"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Compte haver diferències de canvi"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Compte deure diferències de canvi"
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Diari diferències de canvi"
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Compte a pagar per defecte"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Compte a cobrar per defecte"
@@ -566,14 +578,24 @@
 msgid "Tax Rounding"
 msgstr "Arrodoniment d'impostos"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Compte haver diferències de canvi"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Compte deure diferències de canvi"
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Compte a pagar per defecte"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -589,14 +611,22 @@
 msgstr "Regla d'impost de client per defecte"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regla d'impost de proveïdor per defecte"
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Empresa"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Diari diferències de canvi"
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Seqüència de reconciliació"
@@ -822,15 +852,15 @@
 msgstr "Des de la data"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Diari"
 
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Període inicial"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -905,14 +935,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Compte del tercer"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Import segona moneda"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -961,14 +995,18 @@
 msgid "Party Required"
 msgstr "Tercer obligatori"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliació"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Segona moneda"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -990,15 +1028,15 @@
 msgstr "Diari"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Suma per tercer"
 
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Període inicial"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1073,14 +1111,18 @@
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Deure"
 
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Seqüència de coincidència"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Seqüència"
@@ -1173,14 +1215,18 @@
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descripció"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "Inverteix"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Import"
@@ -1257,14 +1303,18 @@
 msgid "Party"
 msgstr "Tercer"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Tercer obligatori"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Saldo a pagar/a cobrar"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Període"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliació"
@@ -1305,14 +1355,26 @@
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Diari"
 
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "A pagar"
+
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "A cobrar"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Conciliat"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Descripció"
@@ -1461,17 +1523,17 @@
 msgid "Delegate To"
 msgstr "Delegat a"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Línies"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nom"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Número"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1573,14 +1635,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Monedes"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Data"
@@ -2230,20 +2296,18 @@
 msgstr "Només mostra el saldo en el llibre major."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Permet conciliar els apunts d'aquest compte."
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
-"Força l'ús d'aquesta moneda secundària \n"
-"a tots els assentaments d'aquest compte."
+"Força a tots els assentaments d'aquest compte a tenir aquesta moneda "
+"secundària."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Impost per defecte per a l'entrada manual\n"
@@ -2347,14 +2411,18 @@
 msgid "Only include posted moves."
 msgstr "Mostra només assentaments comptabilitzats."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "També conegut com el número de foli."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr "Inverteix deure i haber."
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "L'import expressat en la segona moneda."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Establiu una data per fer el apunt pagable o cobrable."
@@ -2537,14 +2605,18 @@
 msgid "Account Configuration Default Account"
 msgstr "Configuració de comptes per defecte"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configuració de regles d'impost per defecte"
 
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configuració diari comptable"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configuració seqüències comptables"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Configuració comptable de l'arrodoniment d'impostos"
@@ -2605,14 +2677,18 @@
 msgid "Journal"
 msgstr "Diari"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Efectiu"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Diferències de canvi"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Despesa"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Miscel·lània"
@@ -2653,14 +2729,18 @@
 msgid "Delegate Lines"
 msgstr "Línies delegades"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Agrupa línies"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Context apunts a cobrar/a pagar"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reprogramar apunts"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Reprogramar apunts"
@@ -3065,29 +3145,14 @@
 msgid "Test Tax"
 msgstr "Prova impost"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Actualitza pla comptable des de plantilla"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Tot"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "A pagar"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "A cobrar"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Ja existeix un pla de comptes per l'empresa \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr "No podeu tancar el compte \"%(account)s\" perquè té apunts."
@@ -3354,23 +3419,15 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "El període del assentament \"%(move)s\" està tancat.\n"
 "Voleu utilitzar el període actual per cancel·lar l'assentament?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"La data del assentament \"%(move)s\" està fora del període. Heu de canviar "
-"la data o el període."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "El valor \"%(value)s\" de \"%(expression)s\" de la plantilla "
 "\"%(template)s\" no és un número."
 
@@ -3378,21 +3435,49 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "No s'ha pogut avaluar l'expressió \"%(expression)s\" de la plantilla \"%(template)s\" amb error:\n"
 "\"%(error)s\""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr "El nom de la parula clau \"%(name)s\" no és un identificador vàlid."
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
-msgstr "Per continuar heu de crear un exercici fiscal per la data \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+"Per continuar heu de crear un exercici fiscal per la data \"%(date)s\" i "
+"l'empresa \"%(company)s\"."
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"Per continuar heu de reobrir l'exercici fiscal \"%(fiscalyear)s\" de "
+"l'empresa \"%(company)s\" per la data \"%(date)s\"."
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr ""
+"Per continuar heu de reobrir el període \"%(period)s\" de l'empresa "
+"\"%(company)s\" per la data \"%(date)s\"."
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
-msgstr "Per continuar heu de crear un període per la data \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
+msgstr ""
+"Per continuar heu de crear un període per la data \"%(date)s\" i la empresa "
+"\"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "El compte només pot tenir un tipus deure o haver."
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
 msgid ""
@@ -3476,14 +3561,22 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "La conciliació: \"%(reconciliation)s\" s'ha delegat a la línia \"%(line)s\".\n"
 "És possible que s'hagi de cancel·lar l'assentament \"%(move)s\"."
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"La conciliació: \"%(reconciliation)s\" s'ha delegat a la línia \"%(line)s\".\n"
+"És possible que s'hagi de cancel·lar l'assentament \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "No podeu conciliar l'apunt \"%(line)s\" amb altres apunts perquè el compte "
 "\"%(account1)s\" és diferent de \"%(account2)s\"."
@@ -4548,23 +4641,43 @@
 msgid "Children"
 msgstr "Fills"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informació general"
 
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Llibre major"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Terminis"
 
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Compte haver"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Diferències de canvi"
+
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Compte deure"
+
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Diari"
+
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Assentament"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Tercer"
 
@@ -4633,14 +4746,18 @@
 msgstr "mesos"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Informació addicional"
 
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Haver"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Deure"
```

### Comparing `trytond_account-6.6.3/locale/cs.po` & `trytond_account-6.8.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr ""
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr ""
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:account.account,taxes:"
@@ -567,27 +567,40 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Aged Balance"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Account Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
+
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_receivable:"
@@ -611,14 +624,24 @@
 msgid "Tax Rounding"
 msgstr ""
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -634,14 +657,22 @@
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr ""
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -882,17 +913,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Journals"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -973,14 +1005,18 @@
 msgstr "Accounts"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Account Types"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr ""
@@ -1031,14 +1067,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliation Lines"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr ""
@@ -1061,17 +1101,18 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1148,14 +1189,19 @@
 msgstr ""
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
+#, fuzzy
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Namu"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr ""
@@ -1253,14 +1299,18 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr ""
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Accounts"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1340,14 +1390,19 @@
 msgstr ""
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
+#, fuzzy
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periods"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
@@ -1391,14 +1446,29 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Journals"
 
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Payable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Receivable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Reconcile Lines"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr ""
@@ -1560,18 +1630,17 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Namu"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr ""
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1682,14 +1751,18 @@
 msgid "Account"
 msgstr "Accounts"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr ""
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr ""
@@ -2364,17 +2437,15 @@
 msgstr ""
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
@@ -2473,14 +2544,18 @@
 msgid "Only include posted moves."
 msgstr ""
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2666,14 +2741,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Account Configuration"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Account Configuration"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Account Configuration"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2741,14 +2821,18 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr ""
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2794,14 +2878,18 @@
 msgid "Delegate Lines"
 msgstr "Reconcile Lines"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3253,29 +3341,14 @@
 msgid "Test Tax"
 msgstr "Test Tax"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3492,38 +3565,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3588,14 +3675,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4704,22 +4797,46 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Open Chart of Accounts"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Accounts"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Journals"
+
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr ""
@@ -4790,14 +4907,19 @@
 msgid "months"
 msgstr ""
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Aged Balance"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr ""
```

### Comparing `trytond_account-6.6.3/locale/de.po` & `trytond_account-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 msgstr "Ersetzt durch"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Rechts"
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Fremdwährung"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Startdatum"
 
 msgctxt "field:account.account,taxes:"
@@ -523,29 +523,41 @@
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Wechselkursdifferenzen Habenkonto"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Wechselkursdifferenzen Sollkonto"
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Journal Wechselkursdifferenzen"
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Standardkonto Verbindlichkeiten"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Standardkonto Forderungen"
@@ -566,14 +578,24 @@
 msgid "Tax Rounding"
 msgstr "Steuerrundung"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Wechselkursdifferenzen Habenkonto"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Wechselkursdifferenzen Sollkonto"
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Standardkonto Verbindlichkeiten"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -589,14 +611,22 @@
 msgstr "Standardsteuerregel Kunde"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Standardsteuerregel Lieferant"
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Unternehmen"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Journal Wechselkursdifferenzen"
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Nummernkreis Abstimmung"
@@ -822,15 +852,15 @@
 msgstr "Startdatum"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Journal"
 
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Von Buchungszeitraum"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -905,14 +935,18 @@
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Personenkonto"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Fremdwährungsbetrag"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Unternehmen"
@@ -961,14 +995,18 @@
 msgid "Party Required"
 msgstr "Partei erforderlich"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Abstimmung"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Fremdwährung"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Unternehmen"
@@ -990,15 +1028,15 @@
 msgstr "Journal"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Pro Partei kumulieren"
 
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Von Buchungszeitraum"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1073,14 +1111,18 @@
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Soll"
 
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Matching Reihenfolge"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Nummernkreis"
@@ -1173,14 +1215,18 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Beschreibung"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "Storno"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Betrag"
@@ -1257,14 +1303,18 @@
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Partei erforderlich"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Verbindlichkeiten/Forderungen Saldo"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Buchungszeitraum"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Abstimmung"
@@ -1305,14 +1355,26 @@
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Journal"
 
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Verbindlichkeiten"
+
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Forderungen"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Abgestimmt"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Beschreibung"
@@ -1461,17 +1523,17 @@
 msgid "Delegate To"
 msgstr "Delegieren an"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Positionen"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Name"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Nummer"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1573,14 +1635,18 @@
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Währungen"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Datum"
@@ -2230,20 +2296,16 @@
 msgstr "Nur Salden in Kontenblättern anzeigen."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Buchungszeilen dieses Kontos können abgestimmt werden."
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
-msgstr ""
-"Für alle Buchungen auf dieses Konto\n"
-"diese Fremdwährung verwenden."
+msgid "Force all moves for this account to have this second currency."
+msgstr "Für alle Buchungen auf dieses Konto diese Fremdwährung verwenden."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Standardsteuer für manuell erstellte Buchungszeilen\n"
@@ -2349,14 +2411,18 @@
 msgid "Only include posted moves."
 msgstr "Nur festgeschriebene Buchungssätze berücksichtigen."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Auch bekannt als Folio Nummer."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr "Soll und Haben umkehren."
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 "Der Betrag in einer Fremdwährung (bezogen auf die Währung des Unternehmens)."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2543,14 +2609,18 @@
 msgid "Account Configuration Default Account"
 msgstr "Einstellungen Buchhaltung Standardkonto"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Einstellungen Buchhaltung Standardsteuerregeln"
 
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Einstellungen Buchhaltung Journal"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Einstellungen Buchhaltung Nummernkreis"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Einstellungen Steuerrundung"
@@ -2611,14 +2681,18 @@
 msgid "Journal"
 msgstr "Journal"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Zahlungsverkehr"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Währungsumrechnung"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Aufwand"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Divers"
@@ -2659,14 +2733,18 @@
 msgid "Delegate Lines"
 msgstr "Buchungszeilen delegieren"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Positionen gruppieren"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Forderungen/Verbindlichkeiten Positionen Kontext"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Buchungspositionen neu planen"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Buchungspositionen neu planen"
@@ -3071,29 +3149,14 @@
 msgid "Test Tax"
 msgstr "Steuertest"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Kontenplan von Vorlage aktualisieren"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Alle"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Verbindlichkeiten"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Forderungen"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Es existiert bereits ein Kontenplan für das Unternehmen \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3390,24 +3453,15 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "Der Buchungszeitraum von Buchungssatz \"%(move)s\" ist geschlossen.\n"
 "Soll stattdessen der aktuelle Buchungszeitraum verwendet werden, um den Buchungssatz zu stornieren?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"Das Datum von Buchungssatz \"%(move)s\" liegt außerhalb des "
-"Buchungszeitraums. Es muss entweder das Datum oder der Buchungszeitraum "
-"gewechselt werden."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "Der Wert \"%(value)s\" von \"%(expression)s\" von Vorlage \"%(template)s\" "
 "ist keine Nummer."
 
@@ -3415,25 +3469,49 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "Die Auswertung des Ausdrucks \"%(expression)s\" von Vorlage \"%(template)s\" ist fehlgeschlagen:\n"
 "\"%(error)s\""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr "Der Name \"%(name)s\" des Bezeichners ist kein erlaubter Identifikator."
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr ""
-"Um fortzufahren, muss für das Datum \"%(date)s\" ein Geschäftsjahr erstellt "
-"werden."
+"Um fortzufahren, muss für das Datum \"%(date)s\" und das Unternehmen "
+"\"%(company)s\" ein Geschäftsjahr erstellt werden."
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"Um fortzufahren, muss das Geschäftsjahr \"%(fiscalyear)s\" des Unternehmens "
+"\"%(company)s\" für das Datum \"%(date)s\" wieder geöffnet werden."
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr ""
+"Um fortzufahren, muss der Buchungszeitraum \"%(period)s\" des Unternehmens "
+"\"%(company)s\" für das Datum \"%(date)s\" wieder geöffnet werden."
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
-"Um fortzufahren, muss für das Datum \"%(date)s\" ein Buchungszeitraum "
-"erstellt werden."
+"Um fortzufahren, muss für das Datum \"%(date)s\" und das Unternehmen "
+"\"%(company)s\" ein Buchungszeitraum erstellt werden."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 "Auf einem Konto darf nur entweder ein Haben-Typ oder ein Soll-Typ gesetzt "
 "werden."
 
@@ -3524,14 +3602,22 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Die Abstimmung \"%(reconciliation)s\" wurde an Buchungszeile \"%(line)s\" übertragen.\n"
 "Es muss gegebenenfalls der Buchungssatz \"%(move)s\" annulliert werden."
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"Die Abstimmung \"%(reconciliation)s\" ist mit der Ausbuchungszeile \"%(line)s\" verknüpft.\n"
+"Es muss gegebenenfalls der Buchungssatz \"%(move)s\" annulliert werden."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Abstimmung von Zeile \"%(line)s\" ist nicht möglich, weil das verwendete "
 "Konto \"%(account1)s\" unterschiedlich zu Konto \"%(account2)s\" ist."
@@ -3731,15 +3817,15 @@
 msgctxt ""
 "model:ir.sequence.type,name:sequence_type_account_move_reconciliation"
 msgid "Account Move Reconciliation"
 msgstr "Buchungssatz Abstimmung"
 
 msgctxt "model:ir.ui.menu,name:menu_account"
 msgid "Financial"
-msgstr "Buchhaltung"
+msgstr "Rechnungswesen"
 
 msgctxt "model:ir.ui.menu,name:menu_account_configuration"
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
@@ -4605,23 +4691,43 @@
 msgid "Children"
 msgstr "Untergeordnet (Konten)"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Allgemein"
 
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Kontenblätter"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Zeiträume"
 
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Habenkonto"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Währungsumrechnung"
+
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Sollkonto"
+
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Rechnung"
 
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Journal"
+
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Buchungssatz"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Partei"
 
@@ -4690,14 +4796,18 @@
 msgstr "Monate"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Sonstiges"
 
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Haben"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Soll"
```

### Comparing `trytond_account-6.6.3/locale/es.po` & `trytond_account-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,16 @@
 msgstr "Reemplazado por"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Derecha"
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Moneda secundaria"
+msgid "Second Currency"
+msgstr "Segunda moneda"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Fecha inicial"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -523,29 +523,41 @@
 msgstr "Fecha"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Fecha"
 
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Fecha"
 
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cuenta haber diferencias de cambio"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Cuenta debe diferencias de cambio"
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Diario diferencias de cambio"
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cuenta a pagar por defecto"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Cuenta a cobrar por defecto"
@@ -566,14 +578,24 @@
 msgid "Tax Rounding"
 msgstr "Redondeo de impuestos"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cuenta haber diferencias de cambio"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Cuenta debe diferencias de cambio"
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cuenta a pagar por defecto"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -589,14 +611,22 @@
 msgstr "Regla de impuesto de cliente por defecto"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regla de impuesto de proveedor por defecto"
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Empresa"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Diario diferencias de cambio"
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Secuencia de reconciliación"
@@ -822,15 +852,15 @@
 msgstr "Desde la fecha"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Diario"
 
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Periodo inicial"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -905,14 +935,18 @@
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Cuenta del tercero"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Importe segunda moneda"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -961,14 +995,18 @@
 msgid "Party Required"
 msgstr "Tercero obligatorio"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliación"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Segunda moneda"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -990,15 +1028,15 @@
 msgstr "Diario"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Sumar por tercero"
 
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Periodo inicial"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1073,14 +1111,18 @@
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debe"
 
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Secuencia de coincidencias"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Secuencia"
@@ -1173,14 +1215,18 @@
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descripción"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "Invertir"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Importe"
@@ -1257,14 +1303,18 @@
 msgid "Party"
 msgstr "Tercero"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Tercero obligatorio"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Saldo a pagar/a cobrar"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periodo"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliación"
@@ -1305,14 +1355,26 @@
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Diario"
 
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "A pagar"
+
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "A cobrar"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Conciliado"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Descripción"
@@ -1461,17 +1523,17 @@
 msgid "Delegate To"
 msgstr "Delegada a"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Apuntes"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nombre"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Número"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1573,14 +1635,18 @@
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Monedas"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Fecha"
@@ -2228,20 +2294,17 @@
 msgstr "Sólo muestra el saldo en el libro mayor."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Permite conciliar los apuntes de esta cuenta."
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
-"Fuerza el uso de esta moneda secundaria \n"
-"en todos los asientos de esta cuenta."
+"Fuerza todos los asientos de esta cuenta a tener esta moneda secundaria."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Impuesto por defecto para la introducción manual\n"
@@ -2345,14 +2408,18 @@
 msgid "Only include posted moves."
 msgstr "Muestra solo asientos contabilizados."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "También conocido como el número de folio."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr "Invertir debe y haber."
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "El importe expresado en la segunda moneda."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Establecer una fecha para hacer el apunte pagable o cobrable."
@@ -2537,14 +2604,18 @@
 msgid "Account Configuration Default Account"
 msgstr "Configuración de cuentas por defecto"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configuración de reglas de impuesto por defecto"
 
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configuración diario contable"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configuración secuencias contables"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Configuración contable del redondeo de impuestos"
@@ -2605,14 +2676,18 @@
 msgid "Journal"
 msgstr "Diario"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Efectivo"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Diferencias de cambio"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Gastos"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Misceláneas"
@@ -2653,14 +2728,18 @@
 msgid "Delegate Lines"
 msgstr "Lineas delegadas"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Agrupar líneas"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Contexto apuntes a cobrar/a pagar"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reprogramar apuntes"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Reprogramar apuntes"
@@ -3065,29 +3144,14 @@
 msgid "Test Tax"
 msgstr "Probar impuesto"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Actualizar plan de cuentas desde plantilla"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Todo"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "A pagar"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "A cobrar"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Ya existe un plan de cuentas para la empresa \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr "No se puede cerrar la cuenta \"%(account)s\" porque tiene apuntes."
@@ -3354,23 +3418,15 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "El periodo del asiento \"%(move)s\" está cerrado.\n"
 "¿Desea utilizar el periodo actual para cancelar el asiento?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"La fecha del asiento \"%(move)s\" está fuera del periodo, debe cambiar la "
-"fecha o el periodo."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "El valor \"%(value)s\" de \"%(expression)s\" de la plantilla "
 "\"%(template)s\" no es un número."
 
@@ -3378,22 +3434,49 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "Error al evaluar la expresión \"%(expression)s\" de la plantilla \"%(template)s\" con error:\n"
 "\"%(error)s\""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr "El nombre de la palabra clave \"%(name)s\" no és un identificador vàlido."
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr ""
-"Para continuar, debe crear un ejercicio fiscal para la fecha \"%(date)s\"."
+"Para continuar debe crear un ejercicio fiscal para la fecha \"%(date)s\" de "
+"la empresa \"%(company)s\"."
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"Para continuar deb reabrir el ejercicio fiscal \"%(fiscalyear)s\" de la "
+"empresa para la fecha \"%(date)s\"."
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr ""
+"Para continuar debe reabrir el período \"%(period)s\" de la empresa "
+"\"%(company)s\" para la fecha \"%(date)s\"."
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
-msgstr "Para continuar, debe crear un periodo para la fecha \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
+msgstr ""
+"Para continuar debe crear un periodo para la fecha \"%(date)s\" y la empresa"
+" \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "La cuenta solo puede tener un tipo debe o haber."
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
 msgid ""
@@ -3480,14 +3563,22 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "La conciliación \"%(reconciliation)s\" se ha delegado a la línea \"%(line)s\".\n"
 "Es posible que se necesite cancelar su asiento \"%(move)s\"."
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"La conciliación \"%(reconciliation)s\" se ha delegado a la línea \"%(line)s\".\n"
+"Es posible que se necesite cancelar su asiento \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "No puede conciliar el apunte \"%(line)s\" porque la cuenta \"%(account1)s\" "
 "es diferente de \"%(account2)s\"."
@@ -3894,15 +3985,15 @@
 
 msgctxt "model:res.group,name:group_account_admin"
 msgid "Account Administration"
 msgstr "Administración de contabilidad"
 
 msgctxt "model:res.group,name:group_account_party"
 msgid "Accounting Party"
-msgstr "Comptable de terceros"
+msgstr "Contabilidad de terceros"
 
 msgctxt "report:account.account.type.statement:"
 msgid "/"
 msgstr "/"
 
 msgctxt "report:account.account.type.statement:"
 msgid ":"
@@ -4552,23 +4643,43 @@
 msgid "Children"
 msgstr "Hijos"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Información general"
 
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Libro mayor"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Plazos"
 
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Cuenta haber"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Diferencias de cambio"
+
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Cuenta debe"
+
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Diario"
+
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Asiento"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Tercero"
 
@@ -4637,14 +4748,18 @@
 msgstr "meses"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Información adicional"
 
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Haber"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debe"
```

### Comparing `trytond_account-6.6.3/locale/es_419.po` & `trytond_account-6.8.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr ""
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr ""
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:account.account,taxes:"
@@ -564,29 +564,43 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Fecha"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asiento Contabilizado"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Fecha"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Asiento contabilizado"
+msgid "Posted Moves"
+msgstr "Asiento Contabilizado"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cuenta Crédito"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cuenta por Pagar por Defecto"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -609,14 +623,25 @@
 msgid "Tax Rounding"
 msgstr ""
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr ""
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cuenta Crédito"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cuenta por Pagar por Defecto"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -632,14 +657,22 @@
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr ""
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -876,16 +909,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Libro Diario"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asiento Contabilizado"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 #, fuzzy
@@ -973,14 +1007,18 @@
 msgstr "Cuenta"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Cuenta por pagar"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr ""
@@ -1032,14 +1070,18 @@
 msgstr "Tercero requerido"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Líneas de conciliación de asientos contables"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr ""
@@ -1061,17 +1103,18 @@
 msgid "Journal"
 msgstr "Libro Diario"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Acumular por tercero"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Asiento contabilizado"
+msgid "Posted Moves"
+msgstr "Asiento Contabilizado"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1149,14 +1192,19 @@
 msgstr ""
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Débito"
 
 #, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Líneas de conciliación de asientos contables"
+
+#, fuzzy
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nombre"
 
 #, fuzzy
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
@@ -1256,14 +1304,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descripción"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr ""
@@ -1343,14 +1395,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Tercero requerido"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periods"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
@@ -1396,14 +1452,29 @@
 msgstr "Descripción"
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Libro Diario"
 
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Por pagar"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Por cobrar"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Líneas de conciliación de asientos contables"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1571,17 +1642,17 @@
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Líneas"
 
 #, fuzzy
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nombre"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Número de contabilización"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.template,date:"
@@ -1692,14 +1763,18 @@
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr ""
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
@@ -2389,19 +2464,18 @@
 msgstr "Mostrar sólo el saldo en el informe del libro mayor"
 
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Permite conciliar las líneas de asiento de esta cuenta."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
-msgstr ""
+msgid "Force all moves for this account to have this second currency."
+msgstr "Permite conciliar las líneas de asiento de esta cuenta."
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
@@ -2505,14 +2579,18 @@
 msgid "Only include posted moves."
 msgstr ""
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2704,14 +2782,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configuración contable"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configuración contable"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configuración contable"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2775,14 +2858,18 @@
 msgid "Journal"
 msgstr "Libro diario"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr ""
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr ""
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr ""
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2824,14 +2911,19 @@
 msgid "Delegate Lines"
 msgstr "Cuenta Débito"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Contexto de las líneas del libro mayor"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr ""
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr ""
@@ -3284,31 +3376,14 @@
 msgid "Test Tax"
 msgstr "Test de Impuesto"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Por pagar"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Por cobrar"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3536,38 +3611,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3638,14 +3727,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "No puede conciliar la línea \"%(line)s\" porque la cuenta \"%(account1)s\" "
@@ -4769,24 +4864,48 @@
 msgid "Children"
 msgstr "Hijos"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Línea de libro mayor"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Cuenta Crédito"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Cuenta Débito"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Libro Diario"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Línea de asiento"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr ""
 
@@ -4857,14 +4976,19 @@
 msgid "months"
 msgstr ""
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Crédito"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Débito"
```

### Comparing `trytond_account-6.6.3/locale/et.po` & `trytond_account-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:account.account,active:"
 msgid "Active"
 msgstr "Aktiivne"
 
 msgctxt "field:account.account,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Valuutasumma"
+msgstr "Summa valuutas"
 
 msgctxt "field:account.account,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.account,childs:"
 msgid "Children"
@@ -75,15 +75,15 @@
 
 msgctxt "field:account.account,left:"
 msgid "Left"
 msgstr "Vasak"
 
 msgctxt "field:account.account,line_count:"
 msgid "Line Count"
-msgstr ""
+msgstr "Ridu"
 
 msgctxt "field:account.account,name:"
 msgid "Name"
 msgstr "Nimetus"
 
 msgctxt "field:account.account,note:"
 msgid "Note"
@@ -105,17 +105,18 @@
 msgid "Replaced By"
 msgstr "Asendatud"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Parem"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Teine valuuta"
+msgid "Second Currency"
+msgstr "Sekundaarne Valuuta"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Alguskuupäev"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -556,28 +557,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Kuupäev"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Postitatud kanne"
+msgid "Posted Moves"
+msgstr "Postittaud kanded"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Kuupäev"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Postitatud kanne"
+msgid "Posted Moves"
+msgstr "Postittaud kanded"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreeditkonto"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Vaikimisi võlgade konto"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -602,14 +617,25 @@
 msgid "Tax Rounding"
 msgstr "Maksu ümardus"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreeditkonto"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Vaikimisi võlgade konto"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -629,14 +655,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Hankija maksu reegel"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Ettevõte"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -869,17 +904,18 @@
 msgstr "Alates kuupäevast"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Andmik"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Postitatud kanne"
+msgid "Posted Moves"
+msgstr "Postittaud kanded"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Algus-periood"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -969,14 +1005,19 @@
 msgstr "Konto"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Võlgade konto"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Summa valuutas"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Ettevõte"
@@ -1028,14 +1069,19 @@
 msgstr "Osapool vajalik"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Kontroll"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Sekundaarne Valuuta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Olek"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Ettevõte"
@@ -1057,17 +1103,18 @@
 msgid "Journal"
 msgstr "Andmik"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Kumulatiivselt osapoolte kaupa"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Postitatud kanne"
+msgid "Posted Moves"
+msgstr "Postittaud kanded"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Algus-periood"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1142,14 +1189,19 @@
 msgid "Currency"
 msgstr "Valuuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Deebet"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Saldeeri read"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nimetus"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Jada"
@@ -1242,14 +1294,18 @@
 msgid "State"
 msgstr "Olek"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Selgitus"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Väärtus"
@@ -1330,14 +1386,19 @@
 msgid "Party"
 msgstr "Osapool"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Osapool vajalik"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Kohustuste/nõuete read"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periood"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Kontroll"
@@ -1382,14 +1443,29 @@
 msgstr "Kulum"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Andmik"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Tasumine"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Laekumine"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Saldeeri"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valuuta"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1552,17 +1628,18 @@
 msgid "Delegate To"
 msgstr "Delegeeritud"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Read"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nimetus"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Number"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1666,14 +1743,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valuuta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Kuupäev"
@@ -1684,15 +1766,15 @@
 
 msgctxt "field:account.reconcile.show,lines:"
 msgid "Lines"
 msgstr "Read"
 
 msgctxt "field:account.reconcile.show,parties:"
 msgid "Parties"
-msgstr "Osapooled"
+msgstr "Partnerid"
 
 msgctxt "field:account.reconcile.show,party:"
 msgid "Party"
 msgstr "Osapool"
 
 msgctxt "field:account.reconcile.show,write_off:"
 msgid "Write Off"
@@ -2336,18 +2418,17 @@
 msgid "Display only the balance in the general ledger report."
 msgstr "Näita ainult pearaamatu aruande saldot."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Luba selle konto kande ridade kontroll."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Sunni kõigile selle konto kannetele \n"
 "see sekundaarne valuuta."
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
@@ -2463,14 +2544,18 @@
 msgstr "Näita ainult postitatud kannet"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Kasutusel ka kui on Folio number"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Väärtus väljendatud sekundaarses valuutas."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2661,14 +2746,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Konto seadistus vaikimisi konto"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Konto seadistus"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Konto seadistus"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Konto seadistus maksu ümardus"
@@ -2731,14 +2821,19 @@
 msgid "Journal"
 msgstr "Andmik"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Raha"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valuuta"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Kulu"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2781,14 +2876,19 @@
 msgstr "Delegeeritud"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Grupeeri read"
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Pearaamatu rea sisu"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Saldeeri read"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3220,29 +3320,14 @@
 msgid "Test Tax"
 msgstr "Testi maksu"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Uuenda kontoplaani vormi pealt"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Kõik"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Tasumine"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Laekumine"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "\"%(company)s\" jaoks on kontoplaan juba loodud."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3502,40 +3587,56 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "Kande \"%(kannete)\" periood on lukus.\n"
 "Kasuta käesolevat perioodi kande tühistamiseks?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"Kande \"%(kannete) kuupäev on perioodist väljaspool, muuda kuupäeva või "
-"perioodi."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr "Jätkamiseks, loo kuupäeva \"%(kuupäeva)de\" jaoks majandusaasta."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr "Jätkamiseks, loo kuupäeva \"%(kuupäeva)de\" jaoks majandusaasta."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "Jätkamiseks, loo kuupäeva \"%(kuupäeva)de\" jaoks periood."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "Jätkamiseks, loo kuupäeva \"%(kuupäeva)de\" jaoks periood."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "Ei sa määrata reale nii deebetit kui ka kreeditit."
 
@@ -3614,14 +3715,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4735,24 +4842,49 @@
 msgid "Children"
 msgstr "Alamkontod"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Üldinformatsioon"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Pearaamat"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Tingimused"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Kreeditkonto"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valuuta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Deebetkonto"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Arve"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Andmik"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Kanne"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Osapool"
 
@@ -4820,14 +4952,19 @@
 msgid "months"
 msgstr "Kuud"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Muu info"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Kreedit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Deebet"
```

### Comparing `trytond_account-6.6.3/locale/fa.po` & `trytond_account-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,18 @@
 msgid "Replaced By"
 msgstr "جایگزین شده توسط"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "راست"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "واحد پول دوم"
+msgid "Second Currency"
+msgstr "مقدارپول دوم"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "تاریخ شروع"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -568,28 +569,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "تاریخ"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "جابجایی ارسال شده"
+msgid "Posted Moves"
+msgstr "جابجایی ها ارسال شده"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "شرکت"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "تاریخ"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "جابجایی ارسال شده"
+msgid "Posted Moves"
+msgstr "جابجایی ها ارسال شده"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "حساب بستانکاری"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "حساب قابل پرداخت پیش فرض"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -614,14 +629,25 @@
 msgid "Tax Rounding"
 msgstr "گرد کردن مالیات"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "شرکت"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "حساب بستانکاری"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "حساب قابل پرداخت پیش فرض"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -641,14 +667,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "قانون مالیات تامین کننده"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "شرکت"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "شرکت"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -881,17 +916,18 @@
 msgstr "از تاریخ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "روزنامه"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "جابجایی ارسال شده"
+msgid "Posted Moves"
+msgstr "جابجایی ها ارسال شده"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "شروع دوره"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -981,14 +1017,19 @@
 msgstr "حساب"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "حساب پرداختی"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "مقدار ارز دوم"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "تراز"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "شرکت"
@@ -1040,14 +1081,19 @@
 msgstr "مورد نیاز نهاد/سازمان"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "تطبیق دادن"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "مقدارپول دوم"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "وضعیت"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "شرکت"
@@ -1069,17 +1115,18 @@
 msgid "Journal"
 msgstr "روزنامه"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "تقسیم بر هر نهاد/سازمان"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "جابجایی ارسال شده"
+msgid "Posted Moves"
+msgstr "جابجایی ها ارسال شده"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "شروع دوره"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1154,14 +1201,19 @@
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "بدهی"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "تطبیق دادن سطرها"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "ادامه"
@@ -1254,14 +1306,18 @@
 msgid "State"
 msgstr "وضعیت"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "شرح"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "حساب"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "مقدار"
@@ -1342,14 +1398,19 @@
 msgid "Party"
 msgstr "نهاد/سازمان"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "مورد نیاز نهاد/سازمان"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "خطوط پرداختی و دریافتی"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "دوره"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "تطبیق دادن"
@@ -1396,14 +1457,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "روزنامه"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "پرداختی"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "دریافتی"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "تطبیق"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1566,17 +1642,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "سطرها"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "نام"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "عدد"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "شرکت"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1680,14 +1757,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "شرکت"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "واحد پول"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "تاریخ"
@@ -2354,18 +2436,17 @@
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 "جابجایی سطرهای این حساب مجاز است\n"
 "برای تطبیق دادن."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "مجموع تمام جابجایی های این حساب\n"
 " برای داشتن ارز ثانویه."
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
@@ -2484,14 +2565,18 @@
 msgstr "نمایش فقط جابجایی ارسال شده"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "همچنین به عنوان شماره برگه شناخته می شود"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "مقدار بیان شده در یک ارز دوم"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2681,14 +2766,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "پیکربندی حساب : حساب پیش فرض"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "پیکربندی حساب"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "پیکربندی حساب"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "پیکربندی حساب : گردکردن مالیات"
@@ -2751,14 +2841,19 @@
 msgid "Journal"
 msgstr "روزنامه"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "نقدی"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "واحد پول"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "هزینه"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2801,14 +2896,19 @@
 msgstr "حساب بدهی"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "مفاد سطر دفتر کل"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "تطبیق دادن سطرها"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3240,29 +3340,14 @@
 msgid "Test Tax"
 msgstr "آزمایش مالیات"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "به روزرسانی نمودار حساب ها از روی الگو"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "همه"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "قابل پرداخت"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "قابل دریافت"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "یک نمودار حساب ها برای شرکت \"%s\" وجود دارد."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3528,40 +3613,56 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "دوره جابجایی:\"%(move)s\" بسته شده است.\n"
 "از دوره جاری برای لغو جابجایی استفاده می کنید؟"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"تاریخ جابجایی : \"%(move)s\" خارج از دوره است، شما باید تاریخ یا دوره را "
-"تغییر دهید."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr "برای ادامه، شما باید یک سال مالی برای تاریخ : \"%(date)s\" ایجاد کنید."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr "برای ادامه، شما باید یک سال مالی برای تاریخ : \"%(date)s\" ایجاد کنید."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "برای ادامه، شما باید یک دوره برای تاریخ : \"%(date)s\" ایجاد کنید."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "برای ادامه، شما باید یک دوره برای تاریخ : \"%(date)s\" ایجاد کنید."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "شما نمی توانید هر دو (بدهی و اعتباری) را در سطرتنظیم کنید."
 
@@ -3648,14 +3749,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "شما نمیتوانید سطر \"%s\" را مطابقت دهید، چراکه حساب \"%s\" با \"%s\" دارای "
 "تفاوت است."
@@ -4760,24 +4867,49 @@
 msgid "Children"
 msgstr "زیر مجموعه"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "اطلاعات عمومی"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "دفتر کل"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "مقررات"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "حساب بستانکاری"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "واحد پول"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "حساب بدهی"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "صورت حساب"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "روزنامه"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "جابجایی"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "نهاد/سازمان"
 
@@ -4847,14 +4979,19 @@
 msgid "months"
 msgstr "ماه ها"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "سایر اطلاعات"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "تراز"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "بستانکاری"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "بدهی"
```

### Comparing `trytond_account-6.6.3/locale/fi.po` & `trytond_account-6.8.0/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 #, fuzzy
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Oikea"
 
 #, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "toissijainen valuutta"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Aloitus päivä"
 
@@ -629,28 +629,41 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "eräpäivä"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Account Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Yritys"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
+
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_receivable:"
@@ -677,14 +690,24 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Yritys"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -704,14 +727,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Oletus verot"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Yritys"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Yritys"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -971,17 +1003,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Journals"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -1072,14 +1105,19 @@
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Account Types"
 
 #, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "arvo toisessa valuutassa"
+
+#, fuzzy
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "tase"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
@@ -1135,14 +1173,19 @@
 msgstr "osapuoli (vaaditaan)"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliation Lines"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "toissijainen valuutta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
@@ -1166,17 +1209,18 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1259,14 +1303,19 @@
 
 #, fuzzy
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debit"
 
 #, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
+#, fuzzy
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr ""
@@ -1369,14 +1418,18 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr ""
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Accounts"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1462,14 +1515,19 @@
 
 #, fuzzy
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "osapuoli (vaaditaan)"
 
 #, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
+#, fuzzy
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periods"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
@@ -1515,14 +1573,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Journals"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Payable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Receivable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Täsmäytys"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valuutta"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr ""
@@ -1691,18 +1764,17 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nimi"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Yritys"
 
 msgctxt "field:account.move.template,date:"
@@ -1820,14 +1892,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Yritys"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valuutta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuutta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr ""
@@ -2552,17 +2629,15 @@
 msgstr ""
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
@@ -2661,14 +2736,18 @@
 msgid "Only include posted moves."
 msgstr ""
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2855,14 +2934,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Account Configuration"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Account Configuration"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Account Configuration"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2930,14 +3014,19 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valuutta"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2983,14 +3072,18 @@
 msgid "Delegate Lines"
 msgstr "Reconcile Lines"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3443,29 +3536,14 @@
 msgid "Test Tax"
 msgstr "Test Tax"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3682,38 +3760,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3778,14 +3870,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4916,22 +5014,47 @@
 msgid "Children"
 msgstr "lapsi"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Open Chart of Accounts"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valuutta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Tili"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Journals"
+
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr ""
@@ -5008,14 +5131,19 @@
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "tase"
+
+#, fuzzy
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Credit"
 
 #, fuzzy
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debit"
```

### Comparing `trytond_account-6.6.3/locale/fr.po` & `trytond_account-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 msgstr "Remplacer par"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Droite"
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Devise secondaire"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Date de début"
 
 msgctxt "field:account.account,taxes:"
@@ -144,15 +144,15 @@
 
 msgctxt "field:account.account.context,fiscalyear:"
 msgid "Fiscal Year"
 msgstr "Année fiscale"
 
 msgctxt "field:account.account.context,posted:"
 msgid "Posted Moves"
-msgstr "Mouvements postés"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.account.deferral,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.account.deferral,amount_second_currency:"
 msgid "Amount Second Currency"
@@ -484,15 +484,15 @@
 
 msgctxt "field:account.aged_balance.context,date:"
 msgid "Date"
 msgstr "Date"
 
 msgctxt "field:account.aged_balance.context,posted:"
 msgid "Posted Move"
-msgstr "Mouvement posté"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.aged_balance.context,term1:"
 msgid "First Term"
 msgstr "Premier terme"
 
 msgctxt "field:account.aged_balance.context,term2:"
 msgid "Second Term"
@@ -523,28 +523,40 @@
 msgstr "Date"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Date"
 
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Date"
 
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
+
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Compte de crédit de change de devise"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Compte de débit de change de devise"
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Journal de change de devise"
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Compte fournisseur par défaut"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -566,14 +578,24 @@
 msgid "Tax Rounding"
 msgstr "Arrondi de taxe"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Société"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Compte de crédit de change de devise"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Compte de débit de change de devise"
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Compte fournisseur par défaut"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -589,14 +611,22 @@
 msgstr "Règle de taxe client par défaut"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Règle de taxe fournisseur par défaut"
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Société"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Journal de change de devise"
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Séquence de réconciliation"
@@ -651,15 +681,15 @@
 
 msgctxt "field:account.fiscalyear,periods:"
 msgid "Periods"
 msgstr "Périodes"
 
 msgctxt "field:account.fiscalyear,post_move_sequence:"
 msgid "Post Move Sequence"
-msgstr "Séquence des mouvements postés"
+msgstr "Séquence de comptabilisation des mouvements"
 
 msgctxt "field:account.fiscalyear,start_date:"
 msgid "Starting Date"
 msgstr "Date de début"
 
 msgctxt "field:account.fiscalyear,state:"
 msgid "State"
@@ -822,16 +852,16 @@
 msgstr "Date de début"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Journal"
 
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Période de début"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -905,14 +935,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Compte tiers"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Montant en devise secondaire"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Balance"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Société"
@@ -961,14 +995,18 @@
 msgid "Party Required"
 msgstr "Tiers requis"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Réconciliation"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Devise secondaire"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "État"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Société"
@@ -990,16 +1028,16 @@
 msgstr "Journal"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Cumuler par tiers"
 
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Période de début"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1035,15 +1073,15 @@
 
 msgctxt "field:account.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Date de début"
 
 msgctxt "field:account.income_statement.context,posted:"
 msgid "Posted Move"
-msgstr "Mouvement posté"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.income_statement.context,start_period:"
 msgid "Start Period"
 msgstr "Période de début"
 
 msgctxt "field:account.income_statement.context,start_period_cmp:"
 msgid "Start Period"
@@ -1073,14 +1111,18 @@
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Débit"
 
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Séquence de correspondance"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Séquence"
@@ -1159,28 +1201,32 @@
 
 msgctxt "field:account.move,period:"
 msgid "Period"
 msgstr "Période"
 
 msgctxt "field:account.move,post_date:"
 msgid "Post Date"
-msgstr "Date de postage"
+msgstr "Date de comptabilisation"
 
 msgctxt "field:account.move,post_number:"
 msgid "Post Number"
-msgstr "Numéro de postage"
+msgstr "Numéro de comptabilisation"
 
 msgctxt "field:account.move,state:"
 msgid "State"
 msgstr "État"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Description"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "Inversion"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Montant"
@@ -1257,14 +1303,18 @@
 msgid "Party"
 msgstr "Tiers"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Tiers requis"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Balance à payer/recevoir"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Période"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Réconciliation"
@@ -1305,14 +1355,26 @@
 msgid "Description"
 msgstr "Description"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Journal"
 
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Fournisseur"
+
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Client"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Réconciliées"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Description"
@@ -1461,17 +1523,17 @@
 msgid "Delegate To"
 msgstr "Déléguer à"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Lignes"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nom"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Numéro"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1547,15 +1609,15 @@
 
 msgctxt "field:account.period,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:account.period,post_move_sequence:"
 msgid "Post Move Sequence"
-msgstr "Séquence des mouvements postés"
+msgstr "Séquence de comptabilisation des mouvements"
 
 msgctxt "field:account.period,start_date:"
 msgid "Starting Date"
 msgstr "Date de début"
 
 msgctxt "field:account.period,state:"
 msgid "State"
@@ -1573,14 +1635,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Société"
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Devises"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Date"
@@ -2207,15 +2273,15 @@
 
 msgctxt "field:party.party.account,supplier_tax_rule:"
 msgid "Supplier Tax Rule"
 msgstr "Règle de taxe fournisseur"
 
 msgctxt "help:account.account,closed:"
 msgid "Check to prevent posting move on the account."
-msgstr "Cocher pour empêcher de poster des mouvements sur le compte."
+msgstr "Cocher pour empêcher de comptabiliser des mouvements sur le compte."
 
 msgctxt "help:account.account,credit_type:"
 msgid "The type used if not empty and debit < credit."
 msgstr "Le type utilisé si non vide et débit < crédit."
 
 msgctxt "help:account.account,debit_type:"
 msgid "The type used if not empty and debit > credit."
@@ -2226,20 +2292,17 @@
 msgstr "Afficher uniquement la balance dans le grand livre."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Autoriser la réconciliation des lignes de mouvement de ce compte."
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
-"Force tous les mouvements pour ce compte \n"
-"à avoir cette devise secondaire."
+"Force tous les mouvements pour ce compte à avoir cette devise secondaire."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Taxe par défaut pour les lignes de mouvement manuelles\n"
@@ -2251,19 +2314,19 @@
 
 msgctxt "help:account.account.context,fiscalyear:"
 msgid "Leave empty for all open fiscal year."
 msgstr "Laissez vide pour toutes les années fiscales ouvertes."
 
 msgctxt "help:account.account.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.account.template,closed:"
 msgid "Check to prevent posting move on the account."
-msgstr "Cocher pour empêcher de poster des mouvements sur le compte."
+msgstr "Cocher pour empêcher de comptabiliser des mouvements sur le compte."
 
 msgctxt "help:account.account.template,general_ledger_balance:"
 msgid "Display only the balance in the general ledger report."
 msgstr "Afficher uniquement la balance dans le grand livre."
 
 msgctxt "help:account.account.template,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
@@ -2283,23 +2346,23 @@
 msgid "Check to allow booking debt via supplier invoice."
 msgstr ""
 "Cochez pour autoriser l'enregistrement de dette via des factures "
 "fournisseurs."
 
 msgctxt "help:account.aged_balance.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.balance_sheet.comparison.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.balance_sheet.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.configuration,default_customer_tax_rule:"
 msgid "Default customer tax rule for new parties."
 msgstr "Règle de taxe client par défaut pour les nouveaux tiers."
 
 msgctxt "help:account.configuration,default_supplier_tax_rule:"
 msgid "Default supplier tax rule for new parties."
@@ -2327,32 +2390,36 @@
 
 msgctxt "help:account.general_ledger.account.context,journal:"
 msgid "Only include moves from the journal."
 msgstr "Inclure seulement les mouvements du journal."
 
 msgctxt "help:account.general_ledger.account.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.general_ledger.line.context,journal:"
 msgid "Only include moves from the journal."
 msgstr "Inclure seulement les mouvements du journal."
 
 msgctxt "help:account.general_ledger.line.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.income_statement.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Aussi connu comme numéro de folio."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr "Débit et crédit inversés."
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Le montant exprimé dans la devise secondaire."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Fixez une date pour rendre la ligne payable ou recevable."
@@ -2536,14 +2603,18 @@
 msgid "Account Configuration Default Account"
 msgstr "Configuration comptable Compte par défaut"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configuration comptable Règle de taxe par défaut"
 
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configuration comptable Journal"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configuration comptable Séquence"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Configuration comptable de l'arrondi de taxe"
@@ -2604,14 +2675,18 @@
 msgid "Journal"
 msgstr "Journal"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Espèces"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Change de devises"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Charge"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Divers"
@@ -2652,14 +2727,18 @@
 msgid "Delegate Lines"
 msgstr "Déléguer les lignes"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Grouper les lignes"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Contexte des lignes à payer/recevoir"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Re-planifier les lignes"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Re-planifier les lignes"
@@ -3064,29 +3143,14 @@
 msgid "Test Tax"
 msgstr "Tester une taxe"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Mise à jour d'un plan comptable depuis un modèle"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Toutes"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "À payer"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "À recevoir"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Un plan comptable existe déjà pour la société « %(company)s »."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3132,24 +3196,25 @@
 "annulation dissociera les lignes."
 
 msgctxt "model:ir.message,text:msg_change_fiscalyear_post_move_sequence"
 msgid ""
 "You cannot change the post move sequence on fiscal year \"%(fiscalyear)s\" "
 "because it contains posted moves."
 msgstr ""
-"Vous ne pouvez pas changer la séquence des mouvements postés de l'année "
-"fiscale « %(fiscalyear)s » car elle contient des mouvements postés."
+"Vous ne pouvez pas changer la séquence de comptabilisation des mouvements de"
+" l'année fiscale « %(fiscalyear)s » car elle contient des mouvements "
+"comptabilisés."
 
 msgctxt "model:ir.message,text:msg_change_period_post_move_sequence"
 msgid ""
 "You cannot change the post move sequence in period \"%(period)s\" because it"
 " has posted moves."
 msgstr ""
-"Vous ne pouvez pas changer la séquence des mouvements postés de la période "
-"« %(period)s » car elle contient des mouvements postés."
+"Vous ne pouvez pas changer la séquence de comptabilisation des mouvements de"
+" la période « %(period)s » car elle contient des mouvements comptabilisés."
 
 msgctxt "model:ir.message,text:msg_close_fiscalyear_account_balance_not_zero"
 msgid ""
 "To close the fiscal year, the balance of account \"%(account)s\" must be "
 "zero."
 msgstr ""
 "Pour clôture l'année fiscale, la balance du compte « %(account)s » doit être"
@@ -3170,16 +3235,16 @@
 msgstr ""
 "Pour clôturer la période « %(period)s », vous devez solder le compte inactif"
 " « %(account)s »."
 
 msgctxt "model:ir.message,text:msg_close_period_non_posted_moves"
 msgid "To close period \"%(period)s\" you must post the moves \"%(moves)s\"."
 msgstr ""
-"Pour clôturer la période « %(period)s », vous devez poster les mouvements "
-"« %(moves)s »."
+"Pour clôturer la période « %(period)s », vous devez comptabiliser les "
+"mouvements « %(moves)s »."
 
 msgctxt "model:ir.message,text:msg_company_change_currency"
 msgid ""
 "You cannot change the currency of a company which is associated with account"
 " moves."
 msgstr ""
 "Vous ne pouvez pas modifier la devise d'une société associée à des "
@@ -3229,16 +3294,16 @@
 
 msgctxt "model:ir.message,text:msg_fiscalyear_different_post_move_sequence"
 msgid ""
 "The fiscal years \"%(first)s\" and \"%(second)s\" cannot have the same post "
 "move sequence, you must use different sequences."
 msgstr ""
 "Les années fiscales « %(first)s » et « %(second)s » ne peuvent pas avoir la "
-"même séquence des mouvements postés, vous devez utiliser des séquences "
-"différentes."
+"même séquence de comptabilisation des mouvements, vous devez utiliser des "
+"séquences différentes."
 
 msgctxt "model:ir.message,text:msg_fiscalyear_overlap"
 msgid ""
 "The fiscal years \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 "Les années fiscales « %(first)s » et « %(second)s » se chevauchent, vous "
@@ -3272,15 +3337,15 @@
 
 msgctxt "model:ir.message,text:msg_journal_account_moves"
 msgid ""
 "You cannot change the type of journal \"%(journal)s\" because it has posted "
 "moves."
 msgstr ""
 "Vous ne pouvez pas changer le type du journal « %(journal)s » car elle "
-"contient des mouvements postés."
+"contient des mouvements comptabilisés."
 
 msgctxt "model:ir.message,text:msg_journal_period_unique"
 msgid "You can create only one journal per period."
 msgstr "Vous ne pouvez créer qu'un seul journal par période."
 
 msgctxt "model:ir.message,text:msg_line_already_reconciled"
 msgid "You cannot reconcile already reconciled line \"%(line)s\"."
@@ -3346,24 +3411,24 @@
 msgstr ""
 "Vous ne pouvez pas ajouter/modifier/supprimer des lignes sur la relation "
 "journal - période clôturée « %(journal_period)s »."
 
 msgctxt "model:ir.message,text:msg_modify_line_posted_move"
 msgid "You cannot modify line \"%(line)s\" from posted move \"%(move)s\"."
 msgstr ""
-"Vous ne pouvez pas modifier la ligne « %(line)s » du mouvement posté "
+"Vous ne pouvez pas modifier la ligne « %(line)s » du mouvement comptabilisé "
 "« %(move)s »."
 
 msgctxt "model:ir.message,text:msg_modify_line_reconciled"
 msgid "You cannot modify reconciled line \"%(line)s\"."
 msgstr "Vous ne pouvez pas modifier le ligne réconciliée « %(line)s »."
 
 msgctxt "model:ir.message,text:msg_modify_posted_moved"
 msgid "You cannot modify posted move \"%(move)s\"."
-msgstr "Vous ne pouvez pas modifier le mouvement posté « %(move)s »."
+msgstr "Vous ne pouvez pas modifier le mouvement comptabilisé « %(move)s »."
 
 msgctxt "model:ir.message,text:msg_modify_tax_line_closed_period"
 msgid "You cannot add/modify/delete tax lines in closed period \"%(period)s\"."
 msgstr ""
 "Vous ne pouvez ajouter/modifier/supprimer des lignes de taxe sur la période "
 "clôturée « %(period)s »."
 
@@ -3371,23 +3436,15 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "La période du mouvement « %(move)s » est close.\n"
 "Utiliser la période courante pour annuler le mouvement ?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"La date du mouvement « %(move)s » est en dehors de la période, vous devez "
-"changé la date ou la période."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "La valeur « %(value)s » de « %(expression)s » du modèle « %(template)s » "
 "n'est pas un nombre."
 
@@ -3395,24 +3452,49 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "Échec de l'évaluation de l'expression « %(expression)s » du modèle « %(template)s » avec erreur :\n"
 "« %(error)s »"
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr "Le nom « %(name)s » du mot-clé n'est pas un identifiant valide."
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr ""
-"Pour continuer, vous devez créer une année fiscale pour la date "
-"« %(date)s »."
+"Pour continuer, vous devez créer une année fiscale pour la date « %(date)s »"
+" et la société « %(company)s »."
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"Pour continuer, vous devez rouvrir l'année fiscale « %(fiscalyear)s » de la "
+"société « %(company)s » pour la date « %(date)s »."
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr ""
+"Pour continuer, vous devez rouvrir la période « %(period)s » de la société "
+"« %(company)s » pour la date « %(date)s »."
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
-"Pour continuer, vous devez créer une période pour la date « %(date)s »."
+"Pour continuer, vous devez créer une période pour la date « %(date)s » et la"
+" société « %(company)s »."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 "Un compte ne peut avoir qu'un seul des types de débit ou de crédit définis."
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3468,29 +3550,30 @@
 "utiliser des dates différentes."
 
 msgctxt "model:ir.message,text:msg_period_same_sequence"
 msgid ""
 "You cannot use the same post move sequence for the periods \"%(first)s\" and"
 " \"%(second)s\" because they are from different fiscal years."
 msgstr ""
-"Vous ne pouvez pas utiliser la même séquence des mouvements postés pour les "
-"périodes « %(first)s » et « %(second)s » car elles viennent d'années "
-"fiscales différentes."
+"Vous ne pouvez pas utiliser la même séquence de comptabilisation des "
+"mouvements pour les périodes « %(first)s » et « %(second)s » car elles "
+"viennent d'années fiscales différentes."
 
 msgctxt "model:ir.message,text:msg_post_empty_move"
 msgid "To post move \"%(move)s\", you must fill in its lines."
-msgstr "Pour poster le mouvement « %(move)s », vous devez remplir ces lignes."
+msgstr ""
+"Pour comptabiliser le mouvement « %(move)s », vous devez remplir ces lignes."
 
 msgctxt "model:ir.message,text:msg_post_unbalanced_move"
 msgid ""
 "To post move \"%(move)s\", you must balance all its lines debits and "
 "credits."
 msgstr ""
-"Pour poster le mouvement « %(move)s », vous devez balancer tous les débits "
-"et crédits des ces lignes."
+"Pour comptabiliser le mouvement « %(move)s », vous devez balancer tous les "
+"débits et crédits des ces lignes."
 
 msgctxt "model:ir.message,text:msg_reconciliation_account_not_reconcile"
 msgid ""
 "To reconcile line \"%(line)s\", you must set its account \"%(account)s\" as "
 "reconcilable."
 msgstr ""
 "Pour réconcilier la ligne « %(line)s », vous devez rendre son compte "
@@ -3500,14 +3583,22 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "La réconciliation « %(reconciliation)s » est déléguée à la ligne « %(line)s ».\n"
 "Vous devrez peut-être annuler son mouvement « %(move)s »."
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"La réconciliation « %(reconciliation)s » est liée à la ligne de pertes et profits « %(line)s ».\n"
+"Vous devrez peut-être annuler son mouvement « %(move)s »."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Vous ne pouvez pas réconcilier la ligne « %(line)s » avec les autres car son"
 " compte « %(account1)s » est différent de « %(account2)s »."
@@ -3603,15 +3694,15 @@
 
 msgctxt "model:ir.model.button,string:fiscalyear_reopen_button"
 msgid "Re-Open"
 msgstr "Rouvrir"
 
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
 msgstr "Fermer"
 
 msgctxt "model:ir.model.button,string:period_lock_button"
 msgid "Lock"
@@ -4145,15 +4236,15 @@
 
 msgctxt "report:account.move.general_journal:"
 msgid "Origin:"
 msgstr "Origine :"
 
 msgctxt "report:account.move.general_journal:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisés"
 
 msgctxt "report:account.move.general_journal:"
 msgid "Print Date:"
 msgstr "Date d'impression :"
 
 msgctxt "report:account.move.general_journal:"
 msgid "User:"
@@ -4321,15 +4412,15 @@
 
 msgctxt "selection:account.general_ledger.line,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.general_ledger.line,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.journal,type:"
 msgid "Cash"
 msgstr "Espèces"
 
 msgctxt "selection:account.journal,type:"
 msgid "Expense"
@@ -4361,15 +4452,15 @@
 
 msgctxt "selection:account.move,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.move,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.move.line,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.move.line,state:"
 msgid "Valid"
@@ -4575,23 +4666,43 @@
 msgid "Children"
 msgstr "Enfants"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Information générale"
 
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Grand livre"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Termes"
 
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Compte de crédit"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Change de devises"
+
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Compte de débit"
+
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Facture"
 
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Journal"
+
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Mouvement"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Tiers"
 
@@ -4660,14 +4771,18 @@
 msgstr "mois"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Autre information"
 
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Balance"
+
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Crédit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Débit"
```

### Comparing `trytond_account-6.6.3/locale/hu.po` & `trytond_account-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 msgid "Replaced By"
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Jobb oldalon"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Deviza pénznem"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Kezdődátum"
 
 msgctxt "field:account.account,taxes:"
@@ -537,29 +538,43 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Dátum"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Lekönyvelt bizonylatok"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Cég"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Dátum"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Lekönyvelt bizonylatok"
 
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Követel forgalom"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Alapértelmezett kötelezettségek számla"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Alapértelmezett követelések számla"
@@ -581,14 +596,25 @@
 msgid "Tax Rounding"
 msgstr "Adó kerekítése"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Cég"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Követel forgalom"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Alapértelmezett kötelezettségek számla"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -605,14 +631,23 @@
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Szállítók alapértelmezett adószabálya"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Cég"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Cég"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -839,16 +874,17 @@
 msgid "From Date"
 msgstr "Ettől"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Napló"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Lekönyvelt bizonylatok"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Kezdőperiódus"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -924,14 +960,19 @@
 msgstr "Számla"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Account Types"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Összeg devizában"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Egyenleg"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Cég"
@@ -981,14 +1022,19 @@
 msgid "Party Required"
 msgstr "Ügyfél megadása kötelező"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Egyeztetés"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Deviza pénznem"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Állapot"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Cég"
@@ -1009,16 +1055,17 @@
 msgid "Journal"
 msgstr "Napló"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Egyenleg ügyfelenként"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Lekönyvelt bizonylatok"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Kezdőperiódus"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1094,14 +1141,19 @@
 msgid "Currency"
 msgstr "Pénznem"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Tartozik"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Sorszámozás"
@@ -1194,14 +1246,18 @@
 msgid "State"
 msgstr "Állapot"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Megjegyzés"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Számla"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Összeg"
@@ -1281,14 +1337,19 @@
 msgid "Party"
 msgstr "Ügyfél"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Ügyfél megadása kötelező"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Kötelezettség/követelés tételek"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periódus"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Egyeztetés"
@@ -1333,14 +1394,29 @@
 msgstr "Megjegyzés"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Napló"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Kötelezettségek"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Követelések"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Egyeztetés"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Pénznem"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1503,17 +1579,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Sorok"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Név"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Sorszám"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Cég"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1616,14 +1693,19 @@
 msgstr "Számla"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Cég"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Pénznem"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Pénznem"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Dátum"
@@ -2286,19 +2368,19 @@
 msgstr "Csak a főkönyv jelentésben mutasson egyenleget."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 "Engedélyezi, hogy a számlára könyvelt tételeket le lehessen egyeztetni."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
+"Engedélyezi, hogy a számlára könyvelt tételeket le lehessen egyeztetni."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Az alapértelmezett adót akkor használja, ha kézzel könyvel a „költségek” "
@@ -2408,14 +2490,18 @@
 msgid "Only include posted moves."
 msgstr "Csak lekönyvelt bizonylatokat vegyen figyelembe."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Az összeg devizában."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2604,14 +2690,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Account Configuration"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Általános beállítások"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Általános beállítások"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2676,14 +2767,19 @@
 msgid "Journal"
 msgstr "Napló"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Pénztár"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Pénznem"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Költségek"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2726,14 +2822,18 @@
 msgid "Delegate Lines"
 msgstr "Tartozik forgalom"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Tételek csoportosítása"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3166,29 +3266,14 @@
 msgid "Test Tax"
 msgstr "Adószámítás szimuláció"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Számlatükör frissítése sablon alapján"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "összes"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "kötelezettségek"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "követelések"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "A „%(company)s” cég rendelkezik már egy számlatükörrel."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3408,39 +3493,58 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr ""
 "A továbblépés előtt hozzon létre egy üzleti évet a „%(date)s” dátumhoz."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"A továbblépés előtt hozzon létre egy üzleti évet a „%(date)s” dátumhoz."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "A továbblépés előtt hozzon létre egy periódust a „%(date)s” dátumhoz."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "A továbblépés előtt hozzon létre egy periódust a „%(date)s” dátumhoz."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3510,14 +3614,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4622,24 +4732,49 @@
 msgid "Children"
 msgstr "Alárendelt rekordok"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Általános információ"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Főkönyv"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Fizetési feltétel"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Követel forgalom"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Pénznem"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Tartozik forgalom"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Számla"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Napló"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Tétel"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Ügyfél"
 
@@ -4707,14 +4842,19 @@
 msgid "months"
 msgstr "Hónap"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Egyéb info"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Egyenleg"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Követel"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Tartozik"
```

### Comparing `trytond_account-6.6.3/locale/id.po` & `trytond_account-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,18 @@
 msgid "Replaced By"
 msgstr "Digantikan Oleh"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Kanan"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Mata Uang Sekunder"
+msgid "Second Currency"
+msgstr "Mata Uang Kedua"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Tanggal Awal"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -527,29 +528,43 @@
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Tanggal"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Membukukan Perpindahan"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Tanggal"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Membukukan Perpindahan"
 
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Akun Kredit"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr ""
@@ -570,14 +585,25 @@
 msgid "Tax Rounding"
 msgstr "Pembulatan Pajak"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Akun Kredit"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -593,14 +619,23 @@
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Perusahaan"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr ""
@@ -828,15 +863,15 @@
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Membukukan Perpindahan"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Periode Awal"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -913,14 +948,19 @@
 msgstr "Akun"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Akun utang"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Jumlah Mata Uang Kedua"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Perusahaan"
@@ -970,14 +1010,19 @@
 msgid "Party Required"
 msgstr "Diperlukan Pihak"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Mata Uang Kedua"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Perusahaan"
@@ -1000,15 +1045,15 @@
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Membukukan Perpindahan"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Periode Awal"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1084,14 +1129,19 @@
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debit"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Urutan"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Urutan"
@@ -1184,14 +1234,18 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Deskripsi"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Akun"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Jumlah"
@@ -1271,14 +1325,19 @@
 msgid "Party"
 msgstr "Pihak"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Diperlukan Pihak"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Baris Utang/Piutang"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periode"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
@@ -1322,14 +1381,28 @@
 msgid "Description"
 msgstr "Deskripsi"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Utang"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Piutang"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr ""
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Deskripsi"
@@ -1481,17 +1554,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Baris"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nama"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Nomor"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1593,14 +1667,19 @@
 msgid "Account"
 msgstr "Akun"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
+#, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Mata Uang"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Tanggal"
@@ -2250,17 +2329,15 @@
 msgstr "Tampilkan hanya saldo dalam laporan buku besar."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
@@ -2359,14 +2436,18 @@
 msgid "Only include posted moves."
 msgstr ""
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2544,14 +2625,19 @@
 msgstr ""
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Konfigurasi Akun Aturan Pajak Standar"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Konfigurasi Akun"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Konfigurasi Akun"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2613,14 +2699,19 @@
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Kas"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Mata Uang"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Biaya"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2663,14 +2754,18 @@
 msgid "Delegate Lines"
 msgstr "Akun Debit"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr ""
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr ""
@@ -3088,29 +3183,14 @@
 msgid "Test Tax"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Utang"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Piutang"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Bagan akun sudah ada bagi perusahaan \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3355,40 +3435,60 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+"Untuk melanjutkan, Anda harus membuat tahun fiskal untuk tanggal "
+"\"%(date)s\"."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
 msgstr ""
 "Untuk melanjutkan, Anda harus membuat tahun fiskal untuk tanggal "
 "\"%(date)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "Untuk melanjutkan, Anda harus membuat periode untuk tanggal \"%(date)s\"."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "Untuk melanjutkan, Anda harus membuat periode untuk tanggal \"%(date)s\"."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3453,14 +3553,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4542,24 +4648,49 @@
 msgid "Children"
 msgstr "Cabang"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informasi Umum"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Buku Besar"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Akun Kredit"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Mata Uang"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Akun Debit"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Faktur"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Jurnal"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Perpindahan"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Pihak"
 
@@ -4625,14 +4756,19 @@
 msgid "months"
 msgstr ""
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Info Lain"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Kredit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debit"
```

### Comparing `trytond_account-6.6.3/locale/it.po` & `trytond_account-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,18 @@
 msgid "Replaced By"
 msgstr "Sostituito da"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Destra"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Valuta secondaria"
+msgid "Second Currency"
+msgstr "Seconda valuta"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data inizio"
 
 msgctxt "field:account.account,taxes:"
@@ -564,28 +565,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Movimento registrato"
+msgid "Posted Moves"
+msgstr "Movimenti registrati"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Azienda"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Movimento registrato"
+msgid "Posted Moves"
+msgstr "Movimenti registrati"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Conto AVERE"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Conto di debito predefinito"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -611,14 +626,25 @@
 msgstr ""
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Azienda"
 
 #, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Conto AVERE"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Conto di debito predefinito"
 
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
@@ -639,14 +665,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regola Imposta Fornitore"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Azienda"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Azienda"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -887,17 +922,18 @@
 msgstr "Dalla data"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Registro"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Movimento registrato"
+msgid "Posted Moves"
+msgstr "Movimenti registrati"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Periodo Iniziale"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -987,14 +1023,19 @@
 msgstr "Conto"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Conto Fornitore"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Importo della valuta secondaria"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Azienda"
@@ -1046,14 +1087,19 @@
 msgstr "Indicazione controparte obbligatoria"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Riconciliazione"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Seconda valuta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Stato"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Azienda"
@@ -1075,17 +1121,18 @@
 msgid "Journal"
 msgstr "Registro"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Movimento registrato"
+msgid "Posted Moves"
+msgstr "Movimenti registrati"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Periodo Iniziale"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1160,14 +1207,19 @@
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "DARE"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Sequenza"
@@ -1262,14 +1314,18 @@
 msgid "State"
 msgstr "Stato"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descrizione"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Conto"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Importo"
@@ -1350,14 +1406,19 @@
 msgid "Party"
 msgstr "Controparte"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Indicazione controparte obbligatoria"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periodo"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Riconciliazione"
@@ -1404,14 +1465,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Registro"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Pagabile"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Da ricevere"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Riconciliazione"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1576,17 +1652,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Righe"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nome"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Numero"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Azienda"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1692,14 +1769,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Azienda"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valuta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
@@ -2404,18 +2486,17 @@
 msgstr "Indica solo il saldo nel libro Mastro"
 
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Registrazione di movimenti consentita"
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Forza tutti i movimenti di questo conto \n"
 "ad avere questa seconda valuta."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
@@ -2531,14 +2612,18 @@
 msgstr "Mostra solo movimento registrato"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Definita anche numero di Folio"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2730,14 +2815,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configurazione Conto"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configurazione Conto"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configurazione Conto"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2802,14 +2892,19 @@
 msgid "Journal"
 msgstr "Registro"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Contanti"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valuta"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Spesa"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2851,14 +2946,18 @@
 msgid "Delegate Lines"
 msgstr "Conto DARE"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3322,29 +3421,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Crea Prospetto Contabile da Modello"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Tutti"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Pagabile"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Da ricevere"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3569,38 +3653,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3668,14 +3766,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4841,25 +4945,50 @@
 msgid "Children"
 msgstr "Figlio"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informazioni generali"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Mastro"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Termini"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Conto AVERE"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valuta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Conto DARE"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Fattura"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Registro"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Movimento"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Controparte"
 
@@ -4936,14 +5065,19 @@
 msgid "months"
 msgstr "Mesi"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Altre Info"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "AVERE"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "DARE"
```

### Comparing `trytond_account-6.6.3/locale/lo.po` & `trytond_account-6.8.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,17 @@
 msgid "Replaced By"
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "ຂວາ"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "ສະກຸນເງິນທີສອງ"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "ວັນທີເລີ່ມ"
 
@@ -572,28 +573,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "ວັນທີ"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "ເຄື່ອນໄຫວປະກາດແລ້ວ"
+msgid "Posted Moves"
+msgstr "ການເຄື່ອນໄຫວທີ່ປະກາດແລ້ວ"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ / ອົງກອນ"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "ວັນທີ"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "ເຄື່ອນໄຫວປະກາດແລ້ວ"
+msgid "Posted Moves"
+msgstr "ການເຄື່ອນໄຫວທີ່ປະກາດແລ້ວ"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "ບັນຊີ ມີ"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "ບັນຊີຕ້ອງສົ່ງເດີມ"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -620,14 +635,25 @@
 
 #, fuzzy
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ/ຫ້ອງການ"
 
 #, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "ບັນຊີ ມີ"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "ບັນຊີຕ້ອງສົ່ງເດີມ"
 
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
@@ -648,14 +674,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "ສູດຄິດໄລ່ອາກອນຜູ້ສະໜອງ"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "ສຳນັກງານ/ຫ້ອງການ"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ/ຫ້ອງການ"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -898,17 +933,18 @@
 msgstr "ແຕ່ວັນທີ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "ບັນຊີປະຈໍາວັນ"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "ເຄື່ອນໄຫວປະກາດແລ້ວ"
+msgid "Posted Moves"
+msgstr "ການເຄື່ອນໄຫວທີ່ປະກາດແລ້ວ"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "ເລີ່ມໄລຍະ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -999,14 +1035,19 @@
 msgstr "ບັນຊີ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "ບັນຊີໜີ້ຕ້ອງສົ່ງ"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "ມູນຄ່າສະກຸນເງິນທີສອງ"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "ດຸນດ່ຽງ"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ / ອົງກອນ"
@@ -1058,14 +1099,19 @@
 msgstr "ຕ້ອງການໃຫ້ມີພາກສ່ວນ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "ການພິສູດຍອດ"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "ສະກຸນເງິນທີສອງ"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "ສະຖານະ"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ / ອົງກອນ"
@@ -1088,17 +1134,18 @@
 msgid "Journal"
 msgstr "ບັນຊີປະຈໍາວັນ"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "ລວມສະສົມຕໍ່ພາກສ່ວນ"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "ເຄື່ອນໄຫວປະກາດແລ້ວ"
+msgid "Posted Moves"
+msgstr "ການເຄື່ອນໄຫວທີ່ປະກາດແລ້ວ"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "ເລີ່ມໄລຍະ"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1178,14 +1225,19 @@
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "ໜີ້"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "ລຳດັບ"
@@ -1282,14 +1334,18 @@
 msgid "State"
 msgstr "ສະຖານະ"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "ເນື້ອໃນລາຍການ"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "ບັນຊີ"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "ມູນຄ່າ"
@@ -1370,14 +1426,19 @@
 msgid "Party"
 msgstr "ພາກສ່ວນ"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "ຕ້ອງການໃຫ້ມີພາກສ່ວນ"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "ໄລຍະ"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "ການພິສູດຍອດ"
@@ -1424,14 +1485,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "ບັນຊີປະຈໍາວັນ"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "ຕ້ອງຈ່າຍ"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "ຕ້ອງຮັບ"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "ພິສູດຍອດ"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1601,17 +1677,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "ລາຍການ"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "ຊື່"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "ເລກທີ"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ/ຫ້ອງການ"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1716,14 +1793,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "ສຳນັກງານ/ຫ້ອງການ"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "ວັນທີ"
@@ -2418,18 +2500,17 @@
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 "ອະນຸຍາດເອົາລາຍການຂອງບັນຊີນີ້\n"
 "ໃຫ້ສາມາດທຽບຍອດໄດ້."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr "ບັງຄັບການເຄື່ອນໄຫວທັງໝົດສໍາລັບບັນຊີນີ້ ໃຫ້ມີສະກຸນເງິນທີສອງ."
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
@@ -2544,14 +2625,18 @@
 msgstr "ສະແດງບັນຊີເຄື່ອນໄຫວທີ່ປະກາດແລ້ວເທົ່ານັ້ນ"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "ນອກຈາກນັ້ນຍັງຮູ້ຈັກໃນນາມ ເລກປະຈຳເອກະສານນັ້ນໆ"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "ມູນຄ່າເປັນສະກຸນເງິນທີສອງ"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2741,14 +2826,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "ບັນຊີການກຳນົດການປັບໂຕມົນເລກພາສີ"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "ການກຳນົດຄ່າບັນຊີ"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "ການກຳນົດຄ່າບັນຊີ"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "ບັນຊີການກຳນົດການປັບໂຕມົນເລກພາສີ"
@@ -2813,14 +2903,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2865,14 +2960,19 @@
 msgstr "ບັນຊີ ໜີ້"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "ບໍລິບົດລາຍການບັນຊີແຍກປະເພດທົ່ວໄປ"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3348,32 +3448,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3601,38 +3683,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3703,14 +3799,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "ທ່ານບໍ່ສາມາດກວດສອບຍອດລາຍການ \"%(line)s\" ໄດ້ ເພາະວ່າບັນຊີມັນ \"%(party1)s\" "
@@ -4881,24 +4983,49 @@
 msgid "Children"
 msgstr "ລູກຮ່ວງ"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "ຂໍ້ມູນທົ່ວໄປ"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "ງວດ"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "ບັນຊີ ມີ"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "ບັນຊີ ໜີ້"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "ໃບເກັບເງິນ"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "ບັນຊີປະຈໍາວັນ"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "ເຄື່ອນໄຫວ"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "ພາກສ່ວນ"
 
@@ -4970,14 +5097,19 @@
 msgid "months"
 msgstr "ເດືອນ"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "ຂໍ້ມູນອື່ນໆ"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "ດຸນດ່ຽງ"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "ມີ"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "ໜີ້"
```

### Comparing `trytond_account-6.6.3/locale/lt.po` & `trytond_account-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 msgid "Replaced By"
 msgstr "Pakeičiančioji"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Dešinė"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Antroji valiuta"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Pradžios data"
 
 msgctxt "field:account.account,taxes:"
@@ -554,28 +555,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Įtraukta į apskaitą operacija"
+msgid "Posted Moves"
+msgstr "Įtrauktos į apskaitą operacijos"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Įtraukta į apskaitą operacija"
+msgid "Posted Moves"
+msgstr "Įtrauktos į apskaitą operacijos"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreditinė koresponduojanti sąskaita"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Numatytoji koresponduojanti sąskaita mokėtinoms sumoms"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -598,14 +613,25 @@
 msgid "Tax Rounding"
 msgstr "Mokesčių apvalinimas"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Organizacija"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreditinė koresponduojanti sąskaita"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Numatytoji koresponduojanti sąskaita mokėtinoms sumoms"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -622,14 +648,23 @@
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Numatytoji tiekėjo mokesčių taisyklė"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Organizacija"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -859,17 +894,18 @@
 msgstr "Pradinė data"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Žurnalas"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Įtraukta į apskaitą operacija"
+msgid "Posted Moves"
+msgstr "Įtrauktos į apskaitą operacijos"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Pradinis periodas"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -959,14 +995,19 @@
 msgstr "Koresponduojanti sąskaita"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Mokėtinų sumų koresponduojanti sąskaita"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Koresponduojančios sąskaitos antroji valiuta"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Balansas"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Organizacija"
@@ -1018,14 +1059,19 @@
 msgstr "Būtinas kontrahentas"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Sudengimas"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Antroji valiuta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Būsena"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Organizacija"
@@ -1047,17 +1093,18 @@
 msgid "Journal"
 msgstr "Žurnalas"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Sumuojama kontrahentui"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Įtraukta į apskaitą operacija"
+msgid "Posted Moves"
+msgstr "Įtrauktos į apskaitą operacijos"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Pradinis periodas"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1132,14 +1179,19 @@
 msgid "Currency"
 msgstr "Valiuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debetas"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Sudengimo eilutės"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Numeruotė"
@@ -1232,14 +1284,18 @@
 msgid "State"
 msgstr "Būsena"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Aprašymas"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Koresponduojanti sąskaita"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Suma"
@@ -1320,14 +1376,19 @@
 msgid "Party"
 msgstr "Kontrahentas"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Būtinas kontrahentas"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Mokėtinos/Gautinos eilutės"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periodas"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Sudengimas"
@@ -1372,14 +1433,29 @@
 msgstr "Aprašymas"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Žurnalas"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Mokėtinas"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Gautinas"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Sudengimas"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1543,17 +1619,18 @@
 msgid "Delegate To"
 msgstr "Deleguota"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Eilutės"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Pavadinimas"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Numeris"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1657,14 +1734,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valiuta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Data"
@@ -2327,18 +2409,17 @@
 msgid "Display only the balance in the general ledger report."
 msgstr "Didžiosios knygos ataskaitoje rodyti tik balansą."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Leisti šios koresponduojančios sąskaitos eilučių suderinimą."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Visoms operacijoms šioje koresponduojančioje \n"
 "sąskaitoje priskirti šią papildomą valiutą."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
@@ -2451,14 +2532,18 @@
 msgid "Only include posted moves."
 msgstr "Rodyti tik įtrauktas į apskaitą operacijas."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Dar žinomas kaip Folio numeris."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Suma antrąja valiuta."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2642,14 +2727,19 @@
 "Koresponduojančių sąskaitų valdymas - numatytoji koresponduojanti sąskaita"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Koresponduojančios sąskaitos numatytoji mokesčių taisyklė"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Koresponduojančių sąskaitų valdymas"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Koresponduojančių sąskaitų valdymas"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Koresponduojančių sąskaitų valdymas - mokesčių apvalinimas"
@@ -2711,14 +2801,19 @@
 msgid "Journal"
 msgstr "Žurnalas"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Kasa"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valiuta"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Išlaidos"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2761,14 +2856,19 @@
 msgstr "Deleguota"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Grupuoti eilutes"
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Didžiosios knygos eilutės kontekstas"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Sudengimo eilutės"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3198,29 +3298,14 @@
 msgid "Test Tax"
 msgstr "Tikrinti mokestį"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Atnaujinti koresponduojančių sąskaitų planą pagal šabloną"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Viskas"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Mokėtina"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Gautina"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Organizacija \"%(company)s\" jau turi sąskaitų planą."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3484,40 +3569,56 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "Operacijos \"%(move)s\" periodas yra uždarytas.\n"
 "Ar naudoti dabartinį periodą, kad panaikinti šią operaciją?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"Operacijos \"%(move)s\" data yra už periodo ribų, jūs turite pakeisti datą "
-"arba periodą."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr "Norint tęsti, reikia datai \"%(date)s\" sukurti finansinius metus."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
 msgstr "Norint tęsti, reikia datai \"%(date)s\" sukurti finansinius metus."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "Norint tęsti, reikia datai \"%(date)s\" sukurti periodą."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "Norint tęsti, reikia datai \"%(date)s\" sukurti periodą."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "Negalima vienoje eilutėje pasirinkti debetą ir kreditą vienu metu."
 
@@ -3609,14 +3710,23 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Sudengimas \"%(reconciliation)s\" yra nukreiptas į eilutę \"%(line)s\".\n"
 "Gali prisireikti panaikinti operaciją \"%(move)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"Sudengimas \"%(reconciliation)s\" yra nukreiptas į eilutę \"%(line)s\".\n"
+"Gali prisireikti panaikinti operaciją \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Negalima sudengti eilutės \"%(line)s\" su kitomis, nes jos koresponduojanti "
 "sąskaita \"%(account1)s\" skiriasi nuo \"%(account2)s\"."
@@ -4761,24 +4871,49 @@
 msgid "Children"
 msgstr "Dukterinės"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Pagrindinė informacija"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Didžioji knyga"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Sąlygos"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Kreditinė koresponduojanti sąskaita"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valiuta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Debetinė koresponduojanti sąskaita"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Sąskaita faktūra"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Žurnalas"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Operacija"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Kontrahentas"
 
@@ -4850,14 +4985,19 @@
 msgid "months"
 msgstr "Mėnesiai"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Kita informacija"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Balansas"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Kreditas"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debetas"
```

### Comparing `trytond_account-6.6.3/locale/nl.po` & `trytond_account-6.8.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 msgstr "Vervangen door"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Rechts"
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Secundaire valuta"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Start datum"
 
 msgctxt "field:account.account,taxes:"
@@ -523,28 +523,40 @@
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
+
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Valuta Wisselkoers Credit Grootboekrekening"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Valuta Wisselkoers Debet Grootboekrekening"
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Valuta Wisselkoers Dagboek"
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Standaard grootboekrekening crediteuren"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -566,14 +578,24 @@
 msgid "Tax Rounding"
 msgstr "Fiscale afronding"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Valuta Wisselkoers Credit Grootboekrekening"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr "Valuta Wisselkoers Debet Grootboekrekening"
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Standaard grootboekrekening crediteuren"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -589,14 +611,22 @@
 msgstr "Standaard belastingregel klanten"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Standaard belastingregel leveranciers"
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Bedrijf"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr "Valuta Wisselkoers Dagboek"
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Afletter reeks"
@@ -822,16 +852,16 @@
 msgstr "Start datum"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Dagboek"
 
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Begin periode"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -905,14 +935,18 @@
 msgid "Account"
 msgstr "Grootboekrekening"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Crediteuren"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Bedrag Secundaire Valuta"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Balans"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Bedrijf"
@@ -961,14 +995,18 @@
 msgid "Party Required"
 msgstr "Relatie verplicht"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Aflettering"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Secundaire Valuta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Bedrijf"
@@ -990,16 +1028,16 @@
 msgstr "Dagboek"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Salderen per relatie"
 
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Begin periode"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1073,14 +1111,18 @@
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debet"
 
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Vergelijking Reeks"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Reeks"
@@ -1173,14 +1215,18 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Omschrijving"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "Terugboeking"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Grootboekrekening"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Bedrag"
@@ -1257,14 +1303,18 @@
 msgid "Party"
 msgstr "Relatie"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Relatie verplicht"
 
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Te betalen / Te ontvangen Balans"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periode"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Aflettering"
@@ -1305,14 +1355,26 @@
 msgid "Description"
 msgstr "Omschrijving"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Dagboek"
 
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Betalen"
+
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Ontvangen"
+
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Afgeletterd"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Omschrijving"
@@ -1461,17 +1523,17 @@
 msgid "Delegate To"
 msgstr "Delegeren aan"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Regels"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Naam"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Nummer"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1573,14 +1635,18 @@
 msgid "Account"
 msgstr "Grootboekrekening"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valuta's"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Datum"
@@ -2226,20 +2292,18 @@
 msgstr "Geef alleen de balans weer van het grootboek."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Sta afletteren van boekingen op deze rekening toe."
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
-"Forceer alle boekingen voor deze rekening \n"
-"om deze secundaire valuta te gebruiken."
+"Forceer alle boekingen voor deze grootboekrekening om deze secundaire valuta"
+" te gebruiken."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 "Standaard belasting voor handmatig coderen van boekingen\n"
@@ -2342,14 +2406,18 @@
 msgid "Only include posted moves."
 msgstr "Alleen bevestigde boekingen weergeven."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Ook bekend als Folio-nummer."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr "Debet en credit wisselen."
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Het bedrag uitgedrukt in een secundaire valuta."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Datum om de regel als betaalbaar of te ontvangen in te stellen."
@@ -2534,14 +2602,18 @@
 msgid "Account Configuration Default Account"
 msgstr "Grootboekrekening configuratie standaard grootboekrekening"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Grootboekrekening configuratie standaard belastingregel"
 
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Grootboekrekening Configuratie Dagboek"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Grootboekrekening configuratie reeks"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Beheer afronding fiscale berekening"
@@ -2602,14 +2674,18 @@
 msgid "Journal"
 msgstr "Dagboek"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Kas"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valuta Wisselkoers"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Kosten"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Diversen"
@@ -2650,14 +2726,18 @@
 msgid "Delegate Lines"
 msgstr "Draag regels over"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Regels groeperen"
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Ontvangen / Betalen regels Context"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Regels herplannen"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Regels herplannen"
@@ -3062,29 +3142,14 @@
 msgid "Test Tax"
 msgstr "Test belasting"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Grootboekschema actualiseren"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Alles"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Te betalen"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Te ontvangen"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Er bestaat al een rekeningschema voor bedrijf \"% (company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3361,23 +3426,15 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "De periode van boeking \"%(move)s\" is afgesloten.\n"
 "Moet de huidige periode gebruikt worden om de boeking te annuleren?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"De boekingsdatum \"%(move)s\" valt buiten de periode, pas de datum of "
-"periode aan."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "De waarde \"%(value)s\" van \"%(expression)s\" van template \"%(template)s\""
 " is geen nummer."
 
@@ -3385,22 +3442,49 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "Evaluatie van expressie \"%(expression)s\" van template \"%(template)s\" faalde met error:\n"
 "\"%(error)s\""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr "Het trefwoord \"%(name)s\" is geen geldige identificator."
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr ""
-"Om door te gaan moet u een fiscaal jaar aanmaken voor de datum \"%(date)s\"."
+"Om door te gaan moet u een fiscaal jaar aanmaken voor de datum \"%(date)s\" "
+"en bedrijf \"%(company)s\"."
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+"Om door te gaan moet u het fiscaal jaar \"%(fiscalyear)s\" van bedrijf "
+"\"%(company)s\" voor de datum \"%(date)s\" heropenen."
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr ""
+"Om door te gaan moet u de periode \"%(period)s\" van bedrijf \"%(company)s\""
+" voor de datum \"%(date)s\" heropenen."
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
-msgstr "Om door te gaan moet u een periode aanmaken voor de datum \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
+msgstr ""
+"Om door te gaan moet u een periode aanmaken voor de datum \"%(date)s\" en "
+"bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 "Alleen één van de debet of credit soorten kan op een grootboekrekening "
 "ingesteld worden."
 
@@ -3491,14 +3575,22 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Het afletteren \"%(reconciliation)s is gedelegeerd naar de regel \"%(line)s\".\n"
 "Indien nodig kunt u de boeking \"%(move)s\" annuleren."
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"Het afletteren \"%(reconciliation)s is gekoppeld aan de afboek regel \"%(line)s\".\n"
+"Indien nodig kunt u de boeking \"%(move)s\" annuleren."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "U kunt de regel \"%(line)s\" niet afletteren, omdat de grootboekrekening "
 "\"%(account1)s niet overeenkomt met \"%(account2)s\"."
@@ -3595,15 +3687,15 @@
 
 msgctxt "model:ir.model.button,string:move_post_button"
 msgid "Post"
 msgstr "Boeken"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
-msgstr "Afsluiten"
+msgstr "Sluiten"
 
 msgctxt "model:ir.model.button,string:period_lock_button"
 msgid "Lock"
 msgstr "Vergrendel"
 
 msgctxt "model:ir.model.button,string:period_reopen_button"
 msgid "Re-Open"
@@ -4563,23 +4655,43 @@
 msgid "Children"
 msgstr "Onderliggend"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Algemene informatie"
 
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Grootboek"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Voorwaarden"
 
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Credit grootboekrekening"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valuta Wisselkoers"
+
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Debet grootboekrekening"
+
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Factuur"
 
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Dagboek"
+
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Boeking"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Relatie"
 
@@ -4648,14 +4760,18 @@
 msgstr "maanden"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Overige informatie"
 
 msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Balans"
+
+msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Credit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debet"
```

### Comparing `trytond_account-6.6.3/locale/pl.po` & `trytond_account-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 msgid "Replaced By"
 msgstr "Zastąpione przez"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "W prawo"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Druga waluta"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data rozpoczęcia"
 
 msgctxt "field:account.account,taxes:"
@@ -566,28 +567,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Zaksięgowany dowód"
+msgid "Posted Moves"
+msgstr "Zaksięgowane dowody"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Firma"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Zaksięgowany dowód"
+msgid "Posted Moves"
+msgstr "Zaksięgowane dowody"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Konto Ma"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Domyślne konto zobowiązań"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -610,14 +625,25 @@
 msgid "Tax Rounding"
 msgstr ""
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Firma"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Konto Ma"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Domyślne konto zobowiązań"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -635,14 +661,23 @@
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Firma"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Firma"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -881,17 +916,18 @@
 msgstr "Od dnia"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Rejestr"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Zaksięgowany dowód"
+msgid "Posted Moves"
+msgstr "Zaksięgowane dowody"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -982,14 +1018,19 @@
 msgstr "Konto"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Konto zobowiązań"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Wartość w drugiej walucie"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Bilans"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Firma"
@@ -1041,14 +1082,19 @@
 msgstr "Wymagana strona"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliation Lines"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Druga waluta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Firma"
@@ -1071,17 +1117,18 @@
 msgid "Journal"
 msgstr "Rejestr"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Zaksięgowany dowód"
+msgid "Posted Moves"
+msgstr "Zaksięgowane dowody"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1162,14 +1209,19 @@
 msgid "Currency"
 msgstr "Waluta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Wn"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Sekwencja"
@@ -1262,14 +1314,18 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Opis"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Wartość"
@@ -1350,14 +1406,19 @@
 msgid "Party"
 msgstr "Strona"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Wymagana strona"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Okres"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
@@ -1405,14 +1466,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Rejestr"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Zobowiązania"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Należności"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Uzgodnienie"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Waluta"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1583,17 +1659,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Zapisy księgowe"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nazwa"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Numer dowodu"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Firma"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1697,14 +1774,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Firma"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Waluta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Waluta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Data"
@@ -2394,19 +2476,18 @@
 msgid "Display only the balance in the general ledger report."
 msgstr ""
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Pozwala uzgadniać zapisy księgowe dla tego konta."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
-msgstr ""
+msgid "Force all moves for this account to have this second currency."
+msgstr "Pozwala uzgadniać zapisy księgowe dla tego konta."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
 
@@ -2513,14 +2594,18 @@
 msgid "Only include posted moves."
 msgstr "Pokaż tylko zaksięgowany dowód"
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2703,14 +2788,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Konfiguracja kont"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Konfiguracja kont"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Konfiguracja kont"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2777,14 +2867,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Waluta"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2830,14 +2925,18 @@
 msgid "Delegate Lines"
 msgstr "Konto Wn"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3319,32 +3418,14 @@
 msgid "Test Tax"
 msgstr "Test Tax"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Zobowiązania"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Należności"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3577,38 +3658,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 #, fuzzy
@@ -3679,14 +3774,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Nie można uzgodnić zapisu \"%(line)s\" ponieważ konto \"%(account1)s\" różni"
@@ -4837,24 +4938,49 @@
 msgid "Children"
 msgstr "Konta podrzędne"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informacje ogólne"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Terminy"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Konto Ma"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Waluta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Konto Wn"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Faktura"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Rejestr"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Dowód księgowy"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Strona"
 
@@ -4923,14 +5049,19 @@
 msgid "months"
 msgstr "Miesiące"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Inne informacje"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Bilans"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Ma"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Wn"
```

### Comparing `trytond_account-6.6.3/locale/pt.po` & `trytond_account-6.8.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -106,17 +106,18 @@
 msgid "Replaced By"
 msgstr "Substituído por"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Direita"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Moeda secundária"
+msgid "Second Currency"
+msgstr "Moeda Secundária"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data de início"
 
 msgctxt "field:account.account,taxes:"
@@ -568,28 +569,42 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Lançamento Confirmado"
+msgid "Posted Moves"
+msgstr "Lançamentos postados"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Lançamento Confirmado"
+msgid "Posted Moves"
+msgstr "Lançamentos postados"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Conta de Crédito"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Conta a Pagar Padrão"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -612,14 +627,25 @@
 msgid "Tax Rounding"
 msgstr "Arrendondamento de Impostos"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Empresa"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Conta de Crédito"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Conta a Pagar Padrão"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -637,14 +663,23 @@
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regra Imposto de Fornecedor"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Empresa"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Empresa"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -879,17 +914,18 @@
 msgstr "Da data"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Diário"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Lançamento Confirmado"
+msgid "Posted Moves"
+msgstr "Lançamentos postados"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Período Inicial"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -979,14 +1015,19 @@
 msgstr "Conta"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Conta a pagar"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Valor da Moeda Secundária"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -1038,14 +1079,19 @@
 msgstr "Entidade Obrigatória"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliação"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Moeda Secundária"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -1067,17 +1113,18 @@
 msgid "Journal"
 msgstr "Diário"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Cumulativo por Entidade"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Lançamento Confirmado"
+msgid "Posted Moves"
+msgstr "Lançamentos postados"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Início do Período"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1152,14 +1199,19 @@
 msgid "Currency"
 msgstr "Moeda"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Débito"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Sequência"
@@ -1252,14 +1304,18 @@
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descrição"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Conta"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Montante"
@@ -1340,14 +1396,19 @@
 msgid "Party"
 msgstr "Pessoa"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Pessoa obrigatória"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Período"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Conciliação"
@@ -1394,14 +1455,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Diário"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "A Pagar"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "A Receber"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Reconciliar"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Moeda"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1572,17 +1648,18 @@
 msgid "Delegate To"
 msgstr "Delegar A"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Linhas"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Nome"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Número"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1686,14 +1763,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Empresa"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Moeda"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Moeda"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Data"
@@ -2380,18 +2462,17 @@
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 "Permitir que as linhas de lançamentos desta conta\n"
 "seja reconciliadas."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Forçar os lançamentos dessa conta\n"
 "a ter essa moeda secundária"
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
@@ -2510,14 +2591,18 @@
 msgstr "Exibir apenas lançamentos confirmados"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Também conhecido como número de Folio"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "O valor expresso na moeda secundária"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2710,14 +2795,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configuração da Conta Conta Padrão"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configuração de Conta"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Configuração de Conta"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Configuração da Conta Arredondamento de Tributos"
@@ -2782,14 +2872,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Moeda"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2834,14 +2929,19 @@
 msgstr "Delegar A"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Agrupar Linhas"
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Contexto da Linha do Livro Razão"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3317,32 +3417,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3572,38 +3654,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3674,14 +3770,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Você não pode reconciliar a linha \"%(line)s\" porque sua conta "
@@ -4847,24 +4949,49 @@
 msgid "Children"
 msgstr "Filhos"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informação Geral"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Prazos"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Conta de Crédito"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Moeda"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Conta de Débito"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Fatura"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Diário"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Lançamento"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Pessoa"
 
@@ -4934,14 +5061,19 @@
 msgid "months"
 msgstr "Meses"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Outras Informações"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Crédito"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Débito"
```

### Comparing `trytond_account-6.6.3/locale/ro.po` & `trytond_account-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,18 @@
 msgid "Replaced By"
 msgstr "Înlocuit de"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Dreapta"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
-msgstr "Monedă Secundară"
+msgid "Second Currency"
+msgstr "Valută Secundara"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Data Inițierii"
 
 msgctxt "field:account.account,taxes:"
 msgid "Default Taxes"
@@ -136,20 +137,18 @@
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.account-account.tax,tax:"
 msgid "Tax"
 msgstr "Impozit"
 
-#, fuzzy
 msgctxt "field:account.account.context,company:"
 msgid "Company"
 msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.account.context,fiscalyear:"
 msgid "Fiscal Year"
 msgstr "An Fiscal"
 
 #, fuzzy
 msgctxt "field:account.account.context,posted:"
 msgid "Posted Moves"
@@ -513,50 +512,60 @@
 msgid "Type"
 msgstr "Tip"
 
 msgctxt "field:account.aged_balance.context,unit:"
 msgid "Unit"
 msgstr "Unitate"
 
-#, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,company:"
 msgid "Company"
 msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,comparison:"
 msgid "Comparison"
 msgstr "Comparație"
 
-#, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Mișcare postata"
+msgid "Posted Moves"
+msgstr "Mișcari Postate"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Mișcare postata"
+msgid "Posted Moves"
+msgstr "Mișcari Postate"
+
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cont Credit"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cont Implicit Furnizor"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -578,14 +587,25 @@
 msgid "Tax Rounding"
 msgstr "Rotunjire Impozit"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Companie"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Cont Credit"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Cont Implicit Furnizor"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -601,14 +621,23 @@
 msgstr "Regula Implicita de Impozitare al Clientului"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Regula Implicita de Impozitare al Furnizorului"
 
+#, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Companie"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Secvenţa de Reconciliere"
@@ -834,17 +863,18 @@
 msgid "From Date"
 msgstr "Din data"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr "Mișcare postata"
+msgid "Posted Moves"
+msgstr "Mișcari Postate"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Perioada inceput"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -918,14 +948,19 @@
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Cont Parte"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Suma Valută Secundara"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Sold"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Companie"
@@ -974,14 +1009,19 @@
 msgid "Party Required"
 msgstr "Parte obligatorie"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliere"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valută Secundara"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Stare"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Companie"
@@ -1002,17 +1042,18 @@
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Cumulare pe Parte"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr "Mișcare postata"
+msgid "Posted Moves"
+msgstr "Mișcari Postate"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Perioada inceput"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1086,14 +1127,19 @@
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debit"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Secvenţa de Reconciliere"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Secvenţă"
@@ -1186,14 +1232,19 @@
 msgid "State"
 msgstr "Stare"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Descriere"
 
+#, fuzzy
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "fiecare"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Suma"
@@ -1272,14 +1323,19 @@
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Parte obligatorie"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Rânduri Client/Furnizor"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Perioadă"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliere"
@@ -1300,20 +1356,18 @@
 msgid "State"
 msgstr "Stare"
 
 msgctxt "field:account.move.line,tax_lines:"
 msgid "Tax Lines"
 msgstr "Rânduri Impozit"
 
-#, fuzzy
 msgctxt "field:account.move.line.delegate.start,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.move.line.delegate.start,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 #, fuzzy
 msgctxt "field:account.move.line.delegate.start,party:"
 msgid "Party"
@@ -1324,24 +1378,37 @@
 msgstr "Descriere"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Furnizor"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Client"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Reconciliere"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valută"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,terms:"
 msgid "Terms"
@@ -1353,25 +1420,22 @@
 msgstr "Suma"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.start,currency:"
 msgid "Currency"
 msgstr "Valută"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,frequency:"
 msgid "Frequency"
 msgstr "Frecvență"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,interval:"
 msgid "Interval"
 msgstr "Interval"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.start,number:"
 msgid "Number"
 msgstr "Număr"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.start,start_date:"
 msgid "Start Date"
@@ -1388,15 +1452,14 @@
 msgstr "Suma"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.term,currency:"
 msgid "Currency"
 msgstr "Valută"
 
-#, fuzzy
 msgctxt "field:account.move.line.reschedule.term,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.move.line.template,account:"
 msgid "Account"
 msgstr "Cont"
@@ -1493,17 +1556,18 @@
 msgid "Delegate To"
 msgstr "Delegat la"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Rânduri"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Denumire"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Număr"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1605,14 +1669,19 @@
 msgid "Account"
 msgstr "Cont"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Companie"
 
+#, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valută"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Data"
@@ -1639,15 +1708,15 @@
 
 msgctxt "field:account.reconcile.show,write_off_amount:"
 msgid "Amount"
 msgstr "Suma"
 
 msgctxt "field:account.reconcile.start,automatic:"
 msgid "Automatic"
-msgstr ""
+msgstr "Automat"
 
 #, fuzzy
 msgctxt "field:account.reconcile.start,only_balanced:"
 msgid "Only Balanced"
 msgstr "Sold Final"
 
 msgctxt "field:account.tax,amount:"
@@ -1795,40 +1864,35 @@
 msgid "Template"
 msgstr "Șablon"
 
 msgctxt "field:account.tax.code,template_override:"
 msgid "Override Template"
 msgstr "Suprascriere șablon"
 
-#, fuzzy
 msgctxt "field:account.tax.code.context,company:"
 msgid "Company"
 msgstr "Companie"
 
 #, fuzzy
 msgctxt "field:account.tax.code.context,end_period:"
 msgid "End Period"
 msgstr "Sfârșit de Perioada"
 
-#, fuzzy
 msgctxt "field:account.tax.code.context,fiscalyear:"
 msgid "Fiscal Year"
 msgstr "An Fiscal"
 
-#, fuzzy
 msgctxt "field:account.tax.code.context,method:"
 msgid "Method"
 msgstr "Metodă"
 
-#, fuzzy
 msgctxt "field:account.tax.code.context,period:"
 msgid "Period"
 msgstr "Perioadă"
 
-#, fuzzy
 msgctxt "field:account.tax.code.context,periods:"
 msgid "Periods"
 msgstr "Perioade"
 
 #, fuzzy
 msgctxt "field:account.tax.code.context,start_period:"
 msgid "Start Period"
@@ -2267,18 +2331,17 @@
 msgid "Display only the balance in the general ledger report."
 msgstr "Afişare numai sold în registru general."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Permite reconciliere al randurilr al contului."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Obligatoriu pentru toate mişcările pe acest cont\n"
 "să aiba o valută secundară."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
@@ -2386,27 +2449,30 @@
 msgid "Only include posted moves."
 msgstr "Include numai mişcări postate."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Cunoscut şi că Numărul Folio."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Sumă exprimata în valută secundară."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
 
 msgctxt "help:account.move.line,second_currency:"
 msgid "The second currency."
 msgstr "Valută secundara."
 
-#, fuzzy
 msgctxt "help:account.move.line.reschedule.start,interval:"
 msgid "The length of each period, in months."
 msgstr "Lungimea fiecărei perioade, în luni."
 
 msgctxt "help:account.move.line.template,amount:"
 msgid "A python expression that will be evaluated with the keywords."
 msgstr "O expresie python care va fi evaluata cu cuvintele cheie."
@@ -2582,14 +2648,19 @@
 msgid "Account Configuration Default Account"
 msgstr "Configurare Implicita pentru Cont"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Configurare Implicita pentru Reguli de Impozitare"
 
+#, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Configurare"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Secvență Configurare Cont"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Configurare Rotunjire Impozit"
@@ -2650,21 +2721,26 @@
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valută"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Cheltuiala"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
-msgstr ""
+msgstr "Diverse"
 
 msgctxt "model:account.journal,name:journal_revenue"
 msgid "Revenue"
 msgstr "Venituri"
 
 msgctxt "model:account.journal,name:journal_stock"
 msgid "Stock"
@@ -2700,14 +2776,19 @@
 msgstr "Delegat la"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Grup de Rânduri"
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Registru General Context Rând"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconciliere Rânduri"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3075,15 +3156,14 @@
 msgid "Tax Lines"
 msgstr "Rânduri Impozit"
 
 msgctxt "model:ir.action,name:act_tax_list"
 msgid "Taxes"
 msgstr "Impozite"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_tax_rule_form"
 msgid "Rules"
 msgstr "Reguli"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_tax_rule_template_form"
 msgid "Tax Rules"
@@ -3125,29 +3205,14 @@
 msgid "Test Tax"
 msgstr "Proba Impozit"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Actualizare Plan de Conturi de la Șablon"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Tot"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Clienți"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Client"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "Un plan de conturi exista deja pentru compania \"%(company)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3415,40 +3480,56 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "Perioada mișcării \"%(move)s\" este închisă. \n"
 "Folosiți perioada curentă pentru a anula mișcarea?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"Data mișcării \"%(move)s\" este în afara perioadei, trebuie schimbată data "
-"sau perioada."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr "Pentru a continua, trebuie creat anul fiscal pentru data \"%(date)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr "Pentru a continua, trebuie creat anul fiscal pentru data \"%(date)s\"."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "Pentru a continua, trebuie creată perioada pentru data \"%(date)s\"."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "Pentru a continua, trebuie creată perioada pentru data \"%(date)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "Nu puteți seta debit și credit pe rând."
 
@@ -3535,14 +3616,23 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Reconcilierea \"%(reconciliation)s\" este corelată cu rândul \"%(line)s\".\n"
 "Posibil să fie nevoie de anularea mișcării \"%(move)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"Reconcilierea \"%(reconciliation)s\" este corelată cu rândul \"%(line)s\".\n"
+"Posibil să fie nevoie de anularea mișcării \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Nu puteți reconcilia rândul \"%(line)s\" cu altele pentru că contul "
 "\"%(account1)s\" este diferit de \"%(account2)s\"."
@@ -4624,22 +4714,47 @@
 msgid "Children"
 msgstr "Copii"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Informații Generale"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Registru General"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Termene"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Cont Credit"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valută"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Cont Debit"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Factura fiscala"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Jurnal"
+
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Mișcare"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Parte"
@@ -4710,14 +4825,19 @@
 msgid "months"
 msgstr "luni"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Alte Informații"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Sold"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Credit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debit"
```

### Comparing `trytond_account-6.6.3/locale/ru.po` & `trytond_account-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -109,16 +109,17 @@
 msgid "Replaced By"
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Правая сторона"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Вторичная валюта"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Дата начала"
 
@@ -594,32 +595,44 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Дата"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведенная операция"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Дата"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведенная операция"
 
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Счет кредиторов по умолчанию"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Счет дебиторов по умолчанию"
@@ -644,14 +657,24 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Организация"
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Счет кредиторов по умолчанию"
 
 #, fuzzy
 msgctxt ""
@@ -673,14 +696,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Правило налогов поставщика"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Организация"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Организация"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -942,15 +974,15 @@
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Журнал"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведенная операция"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Начальный период"
 
@@ -1045,14 +1077,19 @@
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Счет кредиторов"
 
 #, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Сумма во второй валюте"
+
+#, fuzzy
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Баланс"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
@@ -1113,14 +1150,19 @@
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Сверка"
 
 #, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Вторичная валюта"
+
+#, fuzzy
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Состояние"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
@@ -1148,15 +1190,15 @@
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведенная операция"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Начальный период"
 
@@ -1246,14 +1288,19 @@
 msgid "Currency"
 msgstr "Валюта"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Дебет"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Сверки"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Нумерация"
@@ -1354,14 +1401,18 @@
 msgstr "Состояние"
 
 #, fuzzy
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Описание"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Счет"
 
 #, fuzzy
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1442,14 +1493,19 @@
 msgid "Party"
 msgstr "Контрагент"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Период"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Сверка"
@@ -1496,14 +1552,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Журнал"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Подлежащий уплате"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Подлежащий получению"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Сверка"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1680,17 +1751,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Строки"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Наименование"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Номер"
 
 #, fuzzy
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Учет.орг."
 
 #, fuzzy
@@ -1810,14 +1882,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Организация"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Валюта"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Валюта"
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
@@ -2529,18 +2606,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Позволяет проводить сверку по проводкам этого счета"
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr "Все проводки для этого счета будут иметь вторичную валюту"
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
@@ -2654,14 +2730,18 @@
 msgstr "Показать только завершенные проводки"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Также известен как Folio Number"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Сумма в пересчете на вторичную валюту"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2849,14 +2929,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Конфигурация бухгалтерии"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Конфигурация бухгалтерии"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Конфигурация бухгалтерии"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2924,14 +3009,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Валюта"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2976,14 +3066,18 @@
 msgid "Delegate Lines"
 msgstr "Закрыть линии"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3459,32 +3553,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Все"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Подлежащий уплате"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Подлежащий получению"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3711,38 +3787,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3813,14 +3903,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Вы не можете сверить строку \"%(line)s\" так как её счет \"%(account1)s\" "
@@ -4997,25 +5093,50 @@
 msgstr "Подчиненый"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Основная информация"
 
 #, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
+#, fuzzy
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Сроки"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Счет сторно"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Валюта"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Корневой счет"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Инвойс"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Журнал"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Перемещение"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Контрагент"
 
@@ -5093,14 +5214,19 @@
 msgid "months"
 msgstr "Месяцев:"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Другая информация"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Баланс"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Кредит"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Дебет"
```

### Comparing `trytond_account-6.6.3/locale/sl.po` & `trytond_account-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,17 @@
 msgid "Replaced By"
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Desno"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Druga valuta"
 
 #, fuzzy
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Začetni datum"
 
@@ -572,29 +573,43 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Datum"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Samo knjiženo"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Družba"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Datum"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Samo knjiženo"
 
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreditni konto"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Privzeti obveznostni konto"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Privzeti terjatveni konto"
@@ -618,14 +633,25 @@
 msgid "Tax Rounding"
 msgstr "Zaokrožitev davka"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Družba"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Kreditni konto"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Privzeti obveznostni konto"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -645,14 +671,23 @@
 #, fuzzy
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Davčno pravilo dobavitelja"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Družba"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Družba"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -893,16 +928,17 @@
 msgstr "Od"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Dnevnik"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Samo knjiženo"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Od"
 
 #, fuzzy
@@ -994,14 +1030,19 @@
 msgstr "Konto"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Konto obveznosti"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Znesek v drugi valuti"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Družba"
@@ -1053,14 +1094,19 @@
 msgstr "Partner obvezen"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Uskladitev"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Druga valuta"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Stanje"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Družba"
@@ -1083,16 +1129,17 @@
 msgid "Journal"
 msgstr "Dnevnik"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Nabiranje po partnerju"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Samo knjiženo"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Od"
 
 #, fuzzy
@@ -1173,14 +1220,19 @@
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Debet"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Zap.št."
@@ -1273,14 +1325,18 @@
 msgid "State"
 msgstr "Stanje"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Opis"
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Znesek"
@@ -1361,14 +1417,19 @@
 msgid "Party"
 msgstr "Partner"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Partner obvezen"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Obdobje"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Uskladitev"
@@ -1415,14 +1476,29 @@
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Dnevnik"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Obveznosti"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Terjatve"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Uskladitev"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1592,17 +1668,18 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Postavke"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Naziv"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Številka"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Družba"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1706,14 +1783,19 @@
 
 #, fuzzy
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Družba"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Valuta"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Datum"
@@ -2399,18 +2481,17 @@
 msgstr "Prikaži samo bilanco na izpisu glavne knjige"
 
 #, fuzzy
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Dopušča usklajevanje knjiženih postavk tega konta."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr "Vsem vknjižbam za ta konto prisili uporabo te druge valute."
 
 #, fuzzy
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
@@ -2525,14 +2606,18 @@
 msgstr "Prikaži samo knjižene postavke"
 
 #, fuzzy
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Znana tudi kot 'Folio' številka"
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Znesek v drugotni valuti"
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
@@ -2721,14 +2806,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Konfiguracija privzetega konta"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Kontna konfiguracija"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Kontna konfiguracija"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Konfiguracija zaokroževanja davka"
@@ -2793,14 +2883,19 @@
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
 #, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Valuta"
+
+#, fuzzy
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2845,14 +2940,19 @@
 msgstr "Debetni konto"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Kontekst postavke glavne knjige"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3328,32 +3428,14 @@
 msgstr "Test Tax"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-#, fuzzy
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3581,38 +3663,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3683,14 +3779,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Postavke \"%(line)s\" ni možno uskladiti, ker je konto \"%(account1)s\" "
@@ -4859,24 +4961,49 @@
 msgid "Children"
 msgstr "Podšifre"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Splošno"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Roki"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Kreditni konto"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Valuta"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Debetni konto"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Račun"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Dnevnik"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Knjižba"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Partner"
 
@@ -4944,14 +5071,19 @@
 msgid "months"
 msgstr "Meseci"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Drugo"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Saldo"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Kredit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Debet"
```

### Comparing `trytond_account-6.6.3/locale/tr.po` & `trytond_account-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 msgstr ""
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr ""
 
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr ""
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:account.account,taxes:"
@@ -565,27 +565,40 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Aged Balance"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
-msgstr "Account Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
+msgstr "Account Moves"
+
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt "field:account.configuration,default_account_receivable:"
@@ -609,14 +622,24 @@
 msgid "Tax Rounding"
 msgstr ""
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr ""
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -632,14 +655,22 @@
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr ""
 
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -878,17 +909,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Journals"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
 msgid "To Date"
@@ -970,14 +1002,18 @@
 msgstr "Accounts"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Account Types"
 
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr ""
@@ -1028,14 +1064,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Reconciliation Lines"
 
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr ""
@@ -1058,17 +1098,18 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
-msgstr ""
+msgid "Posted Moves"
+msgstr "Account Moves"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr ""
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
 msgid "To Date"
@@ -1145,14 +1186,19 @@
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Reconciliation Lines"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr ""
@@ -1250,14 +1296,18 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr ""
 
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Accounts"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
@@ -1337,14 +1387,19 @@
 msgstr ""
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Payable/Receivable Lines"
+
+#, fuzzy
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Periods"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr ""
@@ -1388,14 +1443,29 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Journals"
 
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Payable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Receivable"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Reconcile Lines"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr ""
@@ -1556,16 +1626,16 @@
 msgid "Delegate To"
 msgstr ""
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr ""
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
 msgstr ""
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.move.template,date:"
@@ -1674,14 +1744,18 @@
 msgid "Account"
 msgstr "Accounts"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr ""
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr ""
@@ -2356,17 +2430,15 @@
 msgstr ""
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr ""
 
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
 "for journal types: \"expense\" and \"revenue\"."
 msgstr ""
@@ -2465,14 +2537,18 @@
 msgid "Only include posted moves."
 msgstr ""
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr ""
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr ""
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2658,14 +2734,19 @@
 
 #, fuzzy
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Account Configuration"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Account Configuration"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Account Configuration"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr ""
@@ -2733,14 +2814,18 @@
 msgid "Journal"
 msgstr "Journals"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Cash"
 
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr ""
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Expense"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2786,14 +2871,18 @@
 msgid "Delegate Lines"
 msgstr "Reconcile Lines"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr ""
 
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Reconcile Lines"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
@@ -3245,29 +3334,14 @@
 msgid "Test Tax"
 msgstr "Test Tax"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Update Chart of Accounts from Template"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "All"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Payable"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Receivable"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3484,38 +3558,52 @@
 
 msgctxt "model:ir.message,text:msg_move_cancel_closed_period"
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3580,14 +3668,20 @@
 
 msgctxt "model:ir.message,text:msg_reconciliation_delete_delegated"
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4690,22 +4784,46 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "General Ledger"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Open Chart of Accounts"
+
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Accounts"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Journals"
+
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr ""
@@ -4776,14 +4894,19 @@
 msgid "months"
 msgstr ""
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Aged Balance"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr ""
```

### Comparing `trytond_account-6.6.3/locale/uk.po` & `trytond_account-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,17 @@
 msgid "Replaced By"
 msgstr "Замінено на"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "Праворуч"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "Друга валюта"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "Початкова дата"
 
 msgctxt "field:account.account,taxes:"
@@ -526,30 +527,45 @@
 msgid "Date"
 msgstr "Дата"
 
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведена проводка"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "Компанія"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведена проводка"
 
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Кредитовий рахунок"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Кредит. заборгованість за умовчанням"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "Дебіт. заборгованість за умовчанням"
@@ -570,14 +586,25 @@
 msgid "Tax Rounding"
 msgstr "Округлення податків"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "Компанія"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "Кредитовий рахунок"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "Кредит. заборгованість за умовчанням"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -593,14 +620,23 @@
 msgstr "Правило оподаткування клієнтів за умовчанням"
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "Правило оподаткування постачальників за умовчанням"
 
+#, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "Компанія"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "Компанія"
 
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
 msgstr "Послідовність звірки"
@@ -825,16 +861,17 @@
 msgid "From Date"
 msgstr "З дати"
 
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "Журнал"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведена проводка"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "Початковий період"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -909,14 +946,19 @@
 msgid "Account"
 msgstr "Рахунок"
 
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "Особа рахунку"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "Сума у другій валюті"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "Баланс"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "Компанія"
@@ -965,14 +1007,19 @@
 msgid "Party Required"
 msgstr "Особа обов'язкова"
 
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Звірка"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "Друга валюта"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "Стан"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "Компанія"
@@ -993,16 +1040,17 @@
 msgid "Journal"
 msgstr "Журнал"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "Акумулювати для особи"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Проведена проводка"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "Початковий період"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1077,14 +1125,19 @@
 msgid "Currency"
 msgstr "Валюта"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "Дебет"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "Послідовність звірки"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "Назва"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "Послідовність"
@@ -1177,14 +1230,19 @@
 msgid "State"
 msgstr "Стан"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "Опис"
 
+#, fuzzy
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "кожні"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "Рахунок"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "Сума"
@@ -1261,14 +1319,19 @@
 msgid "Party"
 msgstr "Особа"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "Особа обов'язкова"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Рядки кредит./дебіт. заборгованості"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "Період"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "Звірка"
@@ -1312,14 +1375,29 @@
 msgid "Description"
 msgstr "Опис"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "Журнал"
 
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "Кредит. заборгованість"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "Дебіт. заборгованість"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "Звірити"
+
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "Валюта"
 
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
 msgstr "Опис"
@@ -1468,17 +1546,18 @@
 msgid "Delegate To"
 msgstr "Делегувати кому"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "Рядки"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "Назва"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "Номер"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "Компанія"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1580,14 +1659,19 @@
 msgid "Account"
 msgstr "Рахунок"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "Компанія"
 
+#, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "Валюта"
+
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "Валюта"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "Дата"
@@ -2240,18 +2324,17 @@
 msgid "Display only the balance in the general ledger report."
 msgstr "Відображати лише баланс у звіті головної книги."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "Дозволити звірку рядків проводок цього рахунку."
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "Примусово використати цю другу валюту \n"
 "для всіх проводок цього рахунку."
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
@@ -2358,14 +2441,18 @@
 msgid "Only include posted moves."
 msgstr "Включити лише проведені проводки."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "Також відомий як номер фоліо."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "Сума, виражена у другій валюті."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr "Встановіть дату, щоб зробити рядок кредиторським або дебіторським."
@@ -2546,14 +2633,19 @@
 msgid "Account Configuration Default Account"
 msgstr "Рахунок за умовчанням у налаштуванні рахунку"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "Правило оподаткування за умовчанням у налаштуванні рахунку"
 
+#, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "Налаштування рахунку"
+
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "Послідовність налаштування рахунку"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "Округлення податку у налаштуванні рахунку"
@@ -2614,14 +2706,19 @@
 msgid "Journal"
 msgstr "Журнал"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "Готівка"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "Валюта"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "Витрати"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr "Різне"
@@ -2663,14 +2760,19 @@
 msgid "Delegate Lines"
 msgstr "Делегувати кому"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "Групові рядки"
 
+#, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "Контекст рядка головної книги"
+
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "Перепланувати рядки"
 
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
 msgstr "Перепланувати рядки"
@@ -3080,29 +3182,14 @@
 msgid "Test Tax"
 msgstr "Тестовий податок"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "Оновити план рахунків із шаблону"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "Всі"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Кредит. заборгованість"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Дебіт. заборгованість"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "План рахунків вже існує для компанії \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
 msgstr ""
@@ -3377,23 +3464,16 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "Період проводки \"%(move)s\" закрито.\n"
 "Використати поточний період для скасування проводки?"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr ""
-"Дата проводки \"%(move)s\" знаходиться поза періодом, вам слід змінити дату "
-"або період."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+#, fuzzy
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 "Значення \"%(value)s\" виразу \"%(expression)s\" із шаблону \"%(template)s\""
 " не є числом."
 
@@ -3401,20 +3481,44 @@
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 "Помилка під час оцінки виразу \"%(expression)s\" із шаблону \"%(template)s\":\n"
 "\"%(error)s\""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
 msgstr "Щоб продовжити, вам слід створити фінансовий рік для дати \"%(date)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
+msgstr "Щоб продовжити, вам слід створити фінансовий рік для дати \"%(date)s\"."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "Щоб продовжити, вам слід створити період для дати \"%(date)s\"."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "Щоб продовжити, вам слід створити період для дати \"%(date)s\"."
 
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "Рахунок може мати лише один із встановлених типів дебету чи кредиту."
 
 msgctxt "model:ir.message,text:msg_open_fiscalyear_earlier"
@@ -3502,14 +3606,23 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "Звірка \"%(reconciliation)s\" делегована рядку \"%(line)s\".\n"
 "Можливо, вам слід скасувати його проводку \"%(move)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"Звірка \"%(reconciliation)s\" делегована рядку \"%(line)s\".\n"
+"Можливо, вам слід скасувати його проводку \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr ""
 "Ви не можете звірити рядок \"%(line)s\" з іншими, оскільки його рахунок "
 "\"%(account1)s\" відрізняється від \"%(account2)s\"."
@@ -4581,22 +4694,47 @@
 msgid "Children"
 msgstr "Діти"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "Головна інформація"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "Головна книга"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "Терміни"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "Кредитовий рахунок"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "Валюта"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "Дебетовий рахунок"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "Рахунок-фактура"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "Журнал"
+
 msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "Проводка"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "Особа"
@@ -4665,14 +4803,19 @@
 msgid "months"
 msgstr "місяці"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "Інша інформація"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "Баланс"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "Кредит"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "Дебет"
```

### Comparing `trytond_account-6.6.3/locale/zh_CN.po` & `trytond_account-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 msgid "Replaced By"
 msgstr "替换为"
 
 msgctxt "field:account.account,right:"
 msgid "Right"
 msgstr "右边"
 
+#, fuzzy
 msgctxt "field:account.account,second_currency:"
-msgid "Secondary Currency"
+msgid "Second Currency"
 msgstr "第二货币"
 
 msgctxt "field:account.account,start_date:"
 msgid "Start Date"
 msgstr "启用日期"
 
 msgctxt "field:account.account,taxes:"
@@ -536,29 +537,43 @@
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,date_cmp:"
 msgid "Date"
 msgstr "日期"
 
 #, fuzzy
 msgctxt "field:account.balance_sheet.comparison.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "已入账记账凭证"
 
 msgctxt "field:account.balance_sheet.context,company:"
 msgid "Company"
 msgstr "公司"
 
 msgctxt "field:account.balance_sheet.context,date:"
 msgid "Date"
 msgstr "日期"
 
+#, fuzzy
 msgctxt "field:account.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "已入账记账凭证"
 
+#, fuzzy
+msgctxt "field:account.configuration,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "贷方帐户"
+
+msgctxt "field:account.configuration,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
+msgctxt "field:account.configuration,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
 msgctxt "field:account.configuration,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "默认应付账款账户"
 
 msgctxt "field:account.configuration,default_account_receivable:"
 msgid "Default Account Receivable"
 msgstr "默认应收账款账户"
@@ -580,14 +595,25 @@
 msgid "Tax Rounding"
 msgstr "税额四舍五入"
 
 msgctxt "field:account.configuration.default_account,company:"
 msgid "Company"
 msgstr "公司"
 
+#, fuzzy
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_credit_account:"
+msgid "Currency Exchange Credit Account"
+msgstr "贷方帐户"
+
+msgctxt ""
+"field:account.configuration.default_account,currency_exchange_debit_account:"
+msgid "Currency Exchange Debit Account"
+msgstr ""
+
 msgctxt "field:account.configuration.default_account,default_account_payable:"
 msgid "Default Account Payable"
 msgstr "默认应付账款账户"
 
 msgctxt ""
 "field:account.configuration.default_account,default_account_receivable:"
 msgid "Default Account Receivable"
@@ -604,14 +630,23 @@
 
 msgctxt ""
 "field:account.configuration.default_tax_rule,default_supplier_tax_rule:"
 msgid "Default Supplier Tax Rule"
 msgstr "默认供应商税规则"
 
 #, fuzzy
+msgctxt "field:account.configuration.journal,company:"
+msgid "Company"
+msgstr "公司"
+
+msgctxt "field:account.configuration.journal,currency_exchange_journal:"
+msgid "Currency Exchange Journal"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.configuration.sequence,company:"
 msgid "Company"
 msgstr "公司"
 
 #, fuzzy
 msgctxt "field:account.configuration.sequence,reconciliation_sequence:"
 msgid "Reconciliation Sequence"
@@ -839,16 +874,17 @@
 msgstr "从日期"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.account.context,journal:"
 msgid "Journal"
 msgstr "日记账"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.account.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "已入账记账凭证"
 
 msgctxt "field:account.general_ledger.account.context,start_period:"
 msgid "Start Period"
 msgstr "期初"
 
 msgctxt "field:account.general_ledger.account.context,to_date:"
@@ -924,14 +960,19 @@
 msgstr "账户"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,account_party:"
 msgid "Account Party"
 msgstr "账户参与者"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr "第二货币金额"
+
 msgctxt "field:account.general_ledger.line,balance:"
 msgid "Balance"
 msgstr "余额"
 
 msgctxt "field:account.general_ledger.line,company:"
 msgid "Company"
 msgstr "公司"
@@ -982,14 +1023,19 @@
 msgstr "需要有参与者"
 
 #, fuzzy
 msgctxt "field:account.general_ledger.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "对账"
 
+#, fuzzy
+msgctxt "field:account.general_ledger.line,second_currency:"
+msgid "Second Currency"
+msgstr "第二货币"
+
 msgctxt "field:account.general_ledger.line,state:"
 msgid "State"
 msgstr "状态"
 
 msgctxt "field:account.general_ledger.line.context,company:"
 msgid "Company"
 msgstr "公司"
@@ -1011,16 +1057,17 @@
 msgid "Journal"
 msgstr "日记账"
 
 msgctxt "field:account.general_ledger.line.context,party_cumulate:"
 msgid "Cumulate per Party"
 msgstr "按参与者累计"
 
+#, fuzzy
 msgctxt "field:account.general_ledger.line.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "已入账记账凭证"
 
 msgctxt "field:account.general_ledger.line.context,start_period:"
 msgid "Start Period"
 msgstr "期初"
 
 msgctxt "field:account.general_ledger.line.context,to_date:"
@@ -1096,14 +1143,19 @@
 msgid "Currency"
 msgstr "货币"
 
 msgctxt "field:account.journal,debit:"
 msgid "Debit"
 msgstr "借方"
 
+#, fuzzy
+msgctxt "field:account.journal,matching_sequence:"
+msgid "Matching Sequence"
+msgstr "对帐明细"
+
 msgctxt "field:account.journal,name:"
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:account.journal,sequence:"
 msgid "Sequence"
 msgstr "序列"
@@ -1196,14 +1248,19 @@
 msgid "State"
 msgstr "状态"
 
 msgctxt "field:account.move.cancel.default,description:"
 msgid "Description"
 msgstr "描述"
 
+#, fuzzy
+msgctxt "field:account.move.cancel.default,reversal:"
+msgid "Reversal"
+msgstr "每"
+
 msgctxt "field:account.move.line,account:"
 msgid "Account"
 msgstr "账户"
 
 msgctxt "field:account.move.line,amount:"
 msgid "Amount"
 msgstr "数额"
@@ -1283,14 +1340,19 @@
 msgid "Party"
 msgstr "参与者"
 
 msgctxt "field:account.move.line,party_required:"
 msgid "Party Required"
 msgstr "需要有参与者"
 
+#, fuzzy
+msgctxt "field:account.move.line,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "应付账款/应收账款明细"
+
 msgctxt "field:account.move.line,period:"
 msgid "Period"
 msgstr "分期"
 
 msgctxt "field:account.move.line,reconciliation:"
 msgid "Reconciliation"
 msgstr "对账"
@@ -1335,14 +1397,29 @@
 msgstr "描述"
 
 msgctxt "field:account.move.line.group.start,journal:"
 msgid "Journal"
 msgstr "日记账"
 
 #, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,payable:"
+msgid "Payable"
+msgstr "应付账款"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,receivable:"
+msgid "Receivable"
+msgstr "应收账款"
+
+#, fuzzy
+msgctxt "field:account.move.line.receivable_payable.context,reconciled:"
+msgid "Reconciled"
+msgstr "允许对账"
+
+#, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,currency:"
 msgid "Currency"
 msgstr "货币"
 
 #, fuzzy
 msgctxt "field:account.move.line.reschedule.preview,description:"
 msgid "Description"
@@ -1506,17 +1583,18 @@
 msgid "Delegate To"
 msgstr "委托人"
 
 msgctxt "field:account.move.reconciliation,lines:"
 msgid "Lines"
 msgstr "明细"
 
-msgctxt "field:account.move.reconciliation,name:"
-msgid "Name"
-msgstr "名称"
+#, fuzzy
+msgctxt "field:account.move.reconciliation,number:"
+msgid "Number"
+msgstr "编号"
 
 msgctxt "field:account.move.template,company:"
 msgid "Company"
 msgstr "公司"
 
 msgctxt "field:account.move.template,date:"
 msgid "Date"
@@ -1619,14 +1697,19 @@
 msgstr "账户"
 
 msgctxt "field:account.reconcile.show,company:"
 msgid "Company"
 msgstr "公司"
 
 #, fuzzy
+msgctxt "field:account.reconcile.show,currencies:"
+msgid "Currencies"
+msgstr "货币"
+
+#, fuzzy
 msgctxt "field:account.reconcile.show,currency:"
 msgid "Currency"
 msgstr "货币"
 
 msgctxt "field:account.reconcile.show,date:"
 msgid "Date"
 msgstr "日期"
@@ -2284,18 +2367,17 @@
 msgid "Display only the balance in the general ledger report."
 msgstr "仅显示总分类帐报表中的余额."
 
 msgctxt "help:account.account,reconcile:"
 msgid "Allow move lines of this account to be reconciled."
 msgstr "允许对此帐户的记账凭证明细对账。"
 
+#, fuzzy
 msgctxt "help:account.account,second_currency:"
-msgid ""
-"Force all moves for this account \n"
-"to have this secondary currency."
+msgid "Force all moves for this account to have this second currency."
 msgstr ""
 "强制此帐户的所有记账凭证\n"
 "都拥有这种第二货币。"
 
 msgctxt "help:account.account,taxes:"
 msgid ""
 "Default tax for manual encoding of move lines\n"
@@ -2407,14 +2489,18 @@
 msgid "Only include posted moves."
 msgstr "只包括已入账的记账凭证."
 
 msgctxt "help:account.move,post_number:"
 msgid "Also known as Folio Number."
 msgstr "也称为登记号."
 
+msgctxt "help:account.move.cancel.default,reversal:"
+msgid "Reverse debit and credit."
+msgstr ""
+
 msgctxt "help:account.move.line,amount_second_currency:"
 msgid "The amount expressed in a second currency."
 msgstr "用第二种货币表示的金额."
 
 msgctxt "help:account.move.line,maturity_date:"
 msgid "Set a date to make the line payable or receivable."
 msgstr ""
@@ -2592,14 +2678,19 @@
 msgstr "账户设置-默认账户"
 
 msgctxt "model:account.configuration.default_tax_rule,name:"
 msgid "Account Configuration Default Tax Rule"
 msgstr "账户设置-默认税规则"
 
 #, fuzzy
+msgctxt "model:account.configuration.journal,name:"
+msgid "Account Configuration Journal"
+msgstr "账户设置"
+
+#, fuzzy
 msgctxt "model:account.configuration.sequence,name:"
 msgid "Account Configuration Sequence"
 msgstr "账户设置"
 
 msgctxt "model:account.configuration.tax_rounding,name:"
 msgid "Account Configuration Tax Rounding"
 msgstr "账户设置-税舍入"
@@ -2660,14 +2751,19 @@
 msgid "Journal"
 msgstr "日记账"
 
 msgctxt "model:account.journal,name:journal_cash"
 msgid "Cash"
 msgstr "现金"
 
+#, fuzzy
+msgctxt "model:account.journal,name:journal_currency_exchange"
+msgid "Currency Exchange"
+msgstr "货币"
+
 msgctxt "model:account.journal,name:journal_expense"
 msgid "Expense"
 msgstr "费用"
 
 msgctxt "model:account.journal,name:journal_miscellaneous"
 msgid "Miscellaneous"
 msgstr ""
@@ -2710,14 +2806,19 @@
 msgstr "委托人"
 
 msgctxt "model:account.move.line.group.start,name:"
 msgid "Group Lines"
 msgstr "明细汇总"
 
 #, fuzzy
+msgctxt "model:account.move.line.receivable_payable.context,name:"
+msgid "Receivable/Payable Line Context"
+msgstr "总分类帐明细内容"
+
+#, fuzzy
 msgctxt "model:account.move.line.reschedule.preview,name:"
 msgid "Reschedule Lines"
 msgstr "对账明细"
 
 #, fuzzy
 msgctxt "model:account.move.line.reschedule.start,name:"
 msgid "Reschedule Lines"
@@ -3145,29 +3246,14 @@
 msgid "Test Tax"
 msgstr "测试税"
 
 msgctxt "model:ir.action,name:wizard_update_chart"
 msgid "Update Chart of Accounts from Template"
 msgstr "从模板中更新账户一脸表"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_all"
-msgid "All"
-msgstr "全部"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "应付账款"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "应收账款"
-
 msgctxt "model:ir.message,text:msg_account_chart_exists"
 msgid "A chart of accounts already exists for company \"%(company)s\"."
 msgstr "公司 \"%(company)s\" 已经存在一个账户一览表."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_account_closed_lines"
 msgid "You cannot close account \"%(account)s\" because it has move lines."
@@ -3393,38 +3479,56 @@
 msgid ""
 "The period of move \"%(move)s\" is closed.\n"
 "Use the current period to cancel the move?"
 msgstr ""
 "记账凭证 \"%(move)s\" 对应的分期已经结账.\n"
 "使用当前分期来取消此记账凭证？"
 
-msgctxt "model:ir.message,text:msg_move_date_outside_period"
-msgid ""
-"The date of move \"%(move)s\" is outside the period, you must change the "
-"date or the period."
-msgstr "记账凭证 \"%(move)s\" 的日期不在分期之内，必须改变日期或者分期."
-
-msgctxt "model:ir.message,text:msg_move_template_expession_not_number"
+msgctxt "model:ir.message,text:msg_move_template_expression_not_number"
 msgid ""
 "The value \"%(value)s\" of \"%(expression)s\" from template \"%(template)s\""
 " is not a number."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_move_template_invalid_expression"
 msgid ""
 "Failed to evaluate expression \"%(expression)s\" from template \"%(template)s\" with error:\n"
 "\"%(error)s\""
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_template_keyword_name_not_identifier"
+msgid "The keyword name \"%(name)s\" is not a valid identifier."
+msgstr ""
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_fiscalyear_date"
-msgid "To continue, you must create a fiscal year for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a fiscal year for the date \"%(date)s\" and "
+"company \"%(company)s\"."
+msgstr "若要继续，必须为日期 \"%(date)s\" 创建会计年度。"
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_fiscalyear_date"
+msgid ""
+"To continue, you must reopen the fiscal year \"%(fiscalyear)s\" of company "
+"\"%(company)s\"for the date \"%(date)s\"."
 msgstr "若要继续，必须为日期 \"%(date)s\" 创建会计年度。"
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_no_open_period_date"
+msgid ""
+"To continue, you must reopen the period \"%(period)s\" of company "
+"\"%(company)s\" for the date \"%(date)s\"."
+msgstr "若要继续，必须为日期 \"%(date)s\" 创建分期。"
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_period_date"
-msgid "To continue, you must create a period for the date \"%(date)s\"."
+msgid ""
+"To continue, you must create a period for the date \"%(date)s\" and company "
+"\"%(company)s\"."
 msgstr "若要继续，必须为日期 \"%(date)s\" 创建分期。"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_only_one_debit_credit_types"
 msgid "Account can have only one of the debit or credit type set."
 msgstr "一条明细不能同时设置借方和贷方。"
 
@@ -3493,14 +3597,23 @@
 msgid ""
 "The reconciliation \"%(reconciliation)s\" is delegated to the line \"%(line)s\".\n"
 "You may need to cancel its move \"%(move)s\"."
 msgstr ""
 "对帐 \"%(reconciliation)s\" 已经委托给明细 \"%(line)s\".\n"
 "您可能需要取消其对应的记账凭证 \"%(move)s\"."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_reconciliation_delete_write_off"
+msgid ""
+"The reconciliation \"%(reconciliation)s\" is linked to the write-off line \"%(line)s\".\n"
+"You may need to cancel its move \"%(move)s\"."
+msgstr ""
+"对帐 \"%(reconciliation)s\" 已经委托给明细 \"%(line)s\".\n"
+"您可能需要取消其对应的记账凭证 \"%(move)s\"."
+
 msgctxt "model:ir.message,text:msg_reconciliation_different_accounts"
 msgid ""
 "You cannot reconcile line \"%(line)s\" with others because its account "
 "\"%(account1)s\" is different from \"%(account2)s\"."
 msgstr "不能将明细 \"%(line)s\" 与其他明细对帐，因为它的帐户\"%(account1)s\"与\"%(account2)s\"不同。"
 
 msgctxt "model:ir.message,text:msg_reconciliation_different_parties"
@@ -4608,24 +4721,49 @@
 msgid "Children"
 msgstr "子账户"
 
 msgctxt "view:account.account:"
 msgid "General Information"
 msgstr "一般信息"
 
+#, fuzzy
+msgctxt "view:account.account:"
+msgid "General Ledger"
+msgstr "总分类帐"
+
 msgctxt "view:account.aged_balance.context:"
 msgid "Terms"
 msgstr "条款"
 
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Credit Account"
+msgstr "贷方帐户"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Currency Exchange"
+msgstr "货币"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
+msgid "Debit Account"
+msgstr "借方帐户"
+
 msgctxt "view:account.configuration:"
 msgid "Invoice"
 msgstr "原始凭证"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
+msgid "Journal"
+msgstr "日记账"
+
+#, fuzzy
+msgctxt "view:account.configuration:"
 msgid "Move"
 msgstr "记账凭证"
 
 msgctxt "view:account.configuration:"
 msgid "Party"
 msgstr "参与者"
 
@@ -4693,14 +4831,19 @@
 msgid "months"
 msgstr "月"
 
 msgctxt "view:account.move.line.template:"
 msgid "Other Info"
 msgstr "其它信息"
 
+#, fuzzy
+msgctxt "view:account.move.line:"
+msgid "Balance"
+msgstr "余额"
+
 msgctxt "view:account.move.line:"
 msgid "Credit"
 msgstr "贷方"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
 msgstr "借方"
```

### Comparing `trytond_account-6.6.3/localize.xsl` & `trytond_account-6.8.0/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/message.xml` & `trytond_account-6.8.0/message.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_account-6.6.3/message.xml` & `trytond_account-6.8.0/message.xml`

```diff
@@ -1,14 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data grouped="1">
     <record model="ir.message" id="msg_no_period_date">
-      <field name="text">To continue, you must create a period for the date &quot;%(date)s&quot;.</field>
+      <field name="text">To continue, you must create a period for the date &quot;%(date)s&quot; and company &quot;%(company)s&quot;.</field>
+    </record>
+    <record model="ir.message" id="msg_no_open_period_date">
+      <field name="text">To continue, you must reopen the period &quot;%(period)s&quot; of company &quot;%(company)s&quot; for the date &quot;%(date)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_modify_delete_period_moves">
       <field name="text">You cannot modify or delete period &quot;%(period)s&quot; because it contains moves.</field>
     </record>
     <record model="ir.message" id="msg_create_period_closed_fiscalyear">
       <field name="text">You cannot create a period in fiscal year &quot;%(fiscalyear)s&quot; because it is closed.</field>
     </record>
@@ -48,15 +51,18 @@
     <record model="ir.message" id="msg_modify_tax_line_closed_period">
       <field name="text">You cannot add/modify/delete tax lines in closed period &quot;%(period)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_change_fiscalyear_post_move_sequence">
       <field name="text">You cannot change the post move sequence on fiscal year &quot;%(fiscalyear)s&quot; because it contains posted moves.</field>
     </record>
     <record model="ir.message" id="msg_no_fiscalyear_date">
-      <field name="text">To continue, you must create a fiscal year for the date &quot;%(date)s&quot;.</field>
+      <field name="text">To continue, you must create a fiscal year for the date &quot;%(date)s&quot; and company &quot;%(company)s&quot;.</field>
+    </record>
+    <record model="ir.message" id="msg_no_open_fiscalyear_date">
+      <field name="text">To continue, you must reopen the fiscal year &quot;%(fiscalyear)s&quot; of company &quot;%(company)s&quot;for the date &quot;%(date)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_fiscalyear_overlap">
       <field name="text">The fiscal years &quot;%(first)s&quot; and &quot;%(second)s&quot; overlap, you must use different dates.</field>
     </record>
     <record model="ir.message" id="msg_open_fiscalyear_earlier">
       <field name="text">The open fiscal year &quot;%(open)s&quot; can not be before the close fiscal year &quot;%(closed)s&quot;.</field>
     </record>
@@ -116,35 +122,39 @@
     </record>
     <record model="ir.message" id="msg_post_unbalanced_move">
       <field name="text">To post move &quot;%(move)s&quot;, you must balance all its lines debits and credits.</field>
     </record>
     <record model="ir.message" id="msg_modify_posted_moved">
       <field name="text">You cannot modify posted move &quot;%(move)s&quot;.</field>
     </record>
-    <record model="ir.message" id="msg_move_date_outside_period">
-      <field name="text">The date of move &quot;%(move)s&quot; is outside the period, you must change the date or the period.</field>
-    </record>
     <record model="ir.message" id="msg_move_cancel_closed_period">
       <field name="text">The period of move &quot;%(move)s&quot; is closed.
 Use the current period to cancel the move?</field>
     </record>
     <record model="ir.message" id="msg_move_template_invalid_expression">
       <field name="text">Failed to evaluate expression &quot;%(expression)s&quot; from template &quot;%(template)s&quot; with error:
 &quot;%(error)s&quot;</field>
     </record>
-    <record model="ir.message" id="msg_move_template_expession_not_number">
+    <record model="ir.message" id="msg_move_template_expression_not_number">
       <field name="text">The value &quot;%(value)s&quot; of &quot;%(expression)s&quot; from template &quot;%(template)s&quot; is not a number.</field>
     </record>
+    <record model="ir.message" id="msg_move_template_keyword_name_not_identifier">
+      <field name="text">The keyword name &quot;%(name)s&quot; is not a valid identifier.</field>
+    </record>
     <record model="ir.message" id="msg_write_reconciliation">
       <field name="text">You cannot modify any reconciliation.</field>
     </record>
     <record model="ir.message" id="msg_reconciliation_delete_delegated">
       <field name="text">The reconciliation &quot;%(reconciliation)s&quot; is delegated to the line &quot;%(line)s&quot;.
 You may need to cancel its move &quot;%(move)s&quot;.</field>
     </record>
+    <record model="ir.message" id="msg_reconciliation_delete_write_off">
+      <field name="text">The reconciliation &quot;%(reconciliation)s&quot; is linked to the write-off line &quot;%(line)s&quot;.
+You may need to cancel its move &quot;%(move)s&quot;.</field>
+    </record>
     <record model="ir.message" id="msg_reconciliation_line_not_valid">
       <field name="text">You cannot reconcile non-valid line &quot;%(line)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_reconciliation_different_accounts">
       <field name="text">You cannot reconcile line &quot;%(line)s&quot; with others because its account &quot;%(account1)s&quot; is different from &quot;%(account2)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_reconciliation_account_not_reconcile">
```

### Comparing `trytond_account-6.6.3/minimal_chart.xml` & `trytond_account-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_bg.xml` & `trytond_account-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_ca.xml` & `trytond_account-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_de.xml` & `trytond_account-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_en.xml` & `trytond_account-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_es.xml` & `trytond_account-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_fr.xml` & `trytond_account-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_nl.xml` & `trytond_account-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_pt.xml` & `trytond_account-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_ru.xml` & `trytond_account-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/minimal_chart_sl.xml` & `trytond_account-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/move.py` & `trytond_account-6.8.0/move.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import defaultdict
 from decimal import Decimal
 from itertools import chain, combinations, groupby, islice
 
 from dateutil.relativedelta import relativedelta
-from sql import Literal, Null
+from sql import Literal, Null, Window
 from sql.aggregate import Max, Sum
 from sql.conditionals import Case, Coalesce
 from sql.functions import Abs, CharLength, Round
 from sql.operators import Exists
 
 from trytond import backend
 from trytond.config import config
@@ -19,21 +19,21 @@
 from trytond.model.exceptions import AccessError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If, PYSONEncoder
 from trytond.report import Report
 from trytond.rpc import RPC
 from trytond.tools import grouped_slice, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import (
-    CancelDelegatedWarning, CancelWarning, DelegateLineError,
-    DeleteDelegatedWarning, GroupLineError, MoveDatesError, PostError,
+    CancelDelegatedWarning, CancelWarning, DelegateLineError, GroupLineError,
+    PeriodNotFoundError, PostError, ReconciliationDeleteWarning,
     ReconciliationError, RescheduleLineError)
 
 _MOVE_STATES = {
     'readonly': Eval('state') == 'posted',
     }
 _LINE_STATES = {
     'readonly': Eval('state') == 'valid',
@@ -51,14 +51,19 @@
         states=_MOVE_STATES)
     period = fields.Many2One('account.period', 'Period', required=True,
         domain=[
             ('company', '=', Eval('company', -1)),
             If(Eval('state') == 'draft',
                 ('state', '=', 'open'),
                 ()),
+            If(Eval('date'), [
+                    ('start_date', '<=', Eval('date')),
+                    ('end_date', '>=', Eval('date')),
+                    ],
+                []),
             ],
         states=_MOVE_STATES)
     journal = fields.Many2One('account.journal', 'Journal', required=True,
         states={
             'readonly': Eval('number') & Eval('journal'),
             },
         context={
@@ -143,112 +148,111 @@
         table, _ = tables[None]
         return [CharLength(table.post_number), table.post_number]
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
-    @staticmethod
-    def default_period():
+    @classmethod
+    def default_period(cls):
         Period = Pool().get('account.period')
-        return Period.find(Transaction().context.get('company'),
-            exception=False)
+        company = cls.default_company()
+        try:
+            period = Period.find(company)
+        except PeriodNotFoundError:
+            return None
+        return period.id
 
     @staticmethod
     def default_state():
         return 'draft'
 
     @classmethod
     def default_date(cls):
         pool = Pool()
         Period = pool.get('account.period')
         Date = pool.get('ir.date')
         today = Date.today()
         period_id = cls.default_period()
         if period_id:
             period = Period(period_id)
-            if today < period.start_date or today > period.end_date:
-                return period.start_date
-        return today
-
-    @fields.depends('period', 'journal', 'date', 'company')
-    def on_change_with_date(self):
-        pool = Pool()
-        Line = pool.get('account.move.line')
-        Date = pool.get('ir.date')
-        if self.company:
-            company_id = self.company.id
-        else:
-            company_id = Transaction().context.get('company')
-        with Transaction().set_context(company=company_id):
-            today = Date.today()
-        date = self.date
-        if date:
-            if self.period and not (
-                    self.period.start_date <= date <= self.period.end_date):
-                if (today >= self.period.start_date
-                        and today <= self.period.end_date):
-                    date = today
-                else:
-                    date = self.period.start_date
-                self.on_change_date()
-            return date
-        lines = Line.search([
-                ('journal', '=', self.journal),
-                ('period', '=', self.period),
-                ], order=[('id', 'DESC')], limit=1)
-        if lines:
-            date = lines[0].date
-        elif self.period:
-            if (today >= self.period.start_date
-                    and today <= self.period.end_date):
-                date = today
+            start_date = period.start_date
+            end_date = period.end_date
+            if start_date <= today <= end_date:
+                return today
+            elif start_date >= today:
+                return start_date
             else:
-                date = self.period.start_date
-        return date
+                end_date
 
-    @fields.depends('date', 'lines')
+    @fields.depends('date', 'period', 'company', 'lines')
     def on_change_date(self):
+        pool = Pool()
+        Period = pool.get('account.period')
+        context = Transaction().context
+        if self.date:
+            company = self.company or context.get('company')
+            if (not self.period
+                    or not (
+                        self.period.start_date <= self.date
+                        <= self.period.end_date)):
+                try:
+                    self.period = Period.find(company, date=self.date)
+                except PeriodNotFoundError:
+                    self.period = None
         for line in (self.lines or []):
             line.date = self.date
 
-    @fields.depends(methods=['on_change_with_date', 'on_change_date'])
+    @fields.depends(
+        'period', 'date', 'company', 'journal', methods=['on_change_date'])
     def on_change_period(self):
-        self.date = self.on_change_with_date()
-        self.on_change_date()
+        pool = Pool()
+        Date = pool.get('ir.date')
+        Line = pool.get('account.move.line')
+        context = Transaction().context
+        company_id = (
+            self.company.id if self.company else context.get('company'))
+        with Transaction().set_context(company=company_id):
+            today = Date.today()
+        if self.period:
+            start_date = self.period.start_date
+            end_date = self.period.end_date
+            if (not self.date
+                    or not (start_date <= self.date <= end_date)):
+                if start_date <= today <= end_date:
+                    self.date = today
+                else:
+                    lines = Line.search([
+                            ('company', '=', company_id),
+                            ('journal', '=', self.journal),
+                            ('period', '=', self.period),
+                            ],
+                        order=[('date', 'DESC')], limit=1)
+                    if lines:
+                        line, = lines
+                        self.date = line.date
+                    elif start_date >= today:
+                        self.date = start_date
+                    else:
+                        self.date = end_date
+            self.on_change_date()
 
     @classmethod
     def _get_origin(cls):
         'Return list of Model names for origin Reference'
         return ['account.fiscalyear', 'account.move']
 
     @classmethod
     def get_origin(cls):
         Model = Pool().get('ir.model')
         get_name = Model.get_name
         models = cls._get_origin()
         return [(None, '')] + [(m, get_name(m)) for m in models]
 
     @classmethod
-    def validate_fields(cls, moves, field_names):
-        super().validate_fields(moves, field_names)
-        cls.check_date(moves, field_names)
-
-    @classmethod
-    def check_date(cls, moves, field_names=None):
-        if field_names and not (field_names & {'date', 'period'}):
-            return
-        for move in moves:
-            if (move.date < move.period.start_date
-                    or move.date > move.period.end_date):
-                raise MoveDatesError(
-                    gettext('account.msg_move_date_outside_period',
-                        move=move.rec_name))
-
-    @classmethod
     def check_modify(cls, moves):
         'Check posted moves for modifications.'
         for move in moves:
             if move.state == 'posted':
                 raise AccessError(
                     gettext('account.msg_modify_posted_moved',
                         move=move.rec_name))
@@ -365,15 +369,15 @@
 
         Transaction().counter += 1
         for cache in Transaction().cache.values():
             if MoveLine.__name__ in cache:
                 cache_cls = cache[MoveLine.__name__]
                 cache_cls.clear()
 
-    def _cancel_default(self):
+    def _cancel_default(self, reversal=False):
         'Return default dictionary to cancel move'
         pool = Pool()
         Date = pool.get('ir.date')
         Period = pool.get('account.period')
         Warning = pool.get('res.user.warning')
 
         default = {
@@ -383,37 +387,41 @@
             key = '%s.cancel' % self
             if Warning.check(key):
                 raise CancelWarning(key,
                     gettext('account.msg_move_cancel_closed_period',
                         move=self.rec_name))
             with Transaction().set_context(company=self.company.id):
                 date = Date.today()
-            period_id = Period.find(self.company.id, date=date)
+            period = Period.find(self.company, date=date)
             default.update({
                     'date': date,
-                    'period': period_id,
+                    'period': period.id,
                     })
-        default['lines.debit'] = lambda data: data['debit'] * -1
-        default['lines.credit'] = lambda data: data['credit'] * -1
+        if reversal:
+            default['lines.debit'] = lambda data: data['credit']
+            default['lines.credit'] = lambda data: data['debit']
+        else:
+            default['lines.debit'] = lambda data: data['debit'] * -1
+            default['lines.credit'] = lambda data: data['credit'] * -1
         default['lines.amount_second_currency'] = (
             lambda data: data['amount_second_currency'] * -1
             if data['amount_second_currency']
             else data['amount_second_currency'])
         default['lines.tax_lines.amount'] = lambda data: data['amount'] * -1
         default['lines.origin'] = (
             lambda data: 'account.move.line,%s' % data['id'])
         return default
 
-    def cancel(self, default=None):
+    def cancel(self, default=None, reversal=False):
         'Return a cancel move'
         if default is None:
             default = {}
         else:
             default = default.copy()
-        default.update(self._cancel_default())
+        default.update(self._cancel_default(reversal=reversal))
         cancel_move, = self.copy([self], default=default)
         return cancel_move
 
     @classmethod
     @ModelView.button
     def post(cls, moves):
         pool = Pool()
@@ -471,29 +479,31 @@
         for move in moves:
             move.state = 'posted'
             if not move.post_number:
                 with Transaction().set_context(company=move.company.id):
                     move.post_date = Date.today()
                 move.post_number = move.period.post_move_sequence_used.get()
 
+        cls.save(moves)
+
         def keyfunc(line):
             return line.party, line.account
         to_reconcile = Line.browse(sorted(
                 [l for l in Line.browse(to_reconcile) if l.account.reconcile],
                 key=keyfunc))
-        for _, lines in groupby(to_reconcile, keyfunc):
-            Line.reconcile(list(lines))
-
-        cls.save(moves)
+        to_reconcile = [list(l) for _, l in groupby(to_reconcile, keyfunc)]
+        if to_reconcile:
+            Line.reconcile(*to_reconcile)
 
 
 class Reconciliation(ModelSQL, ModelView):
     'Account Move Reconciliation Lines'
     __name__ = 'account.move.reconciliation'
-    name = fields.Char('Name', size=None, required=True)
+    _rec_name = 'number'
+    number = fields.Char("Number", required=True)
     company = fields.Many2One('company.company', "Company", required=True)
     lines = fields.One2Many(
         'account.move.line', 'reconciliation', 'Lines',
         domain=[
             ('move.company', '=', Eval('company', -1)),
             ])
     date = fields.Date(
@@ -504,14 +514,15 @@
         domain=[
             ('move.company', '=', Eval('company', -1)),
             ],
         help="The line to which the reconciliation status is delegated.")
 
     @classmethod
     def __setup__(cls):
+        cls.number.search_unaccented = False
         super().__setup__()
         t = cls.__table__()
         cls._sql_indexes.add(Index(t, (t.date, Index.Range())))
 
     @classmethod
     def __register__(cls, module_name):
         cursor = Transaction().connection.cursor()
@@ -523,14 +534,18 @@
         move = Move.__table__()
         line = Line.__table__()
         line_h = Line.__table_handler__(module_name)
 
         date_exist = table.column_exist('date')
         company_exist = table.column_exist('company')
 
+        # Migration from 6.6: rename name to number
+        if table.column_exist('name') and not table.column_exist('number'):
+            table.column_rename('name', 'number')
+
         super(Reconciliation, cls).__register__(module_name)
 
         # Migration from 3.8: new date field
         if (not date_exist
                 and backend.TableHandler.table_exist(Line._table)
                 and Line.__table_handler__().column_exist('move')):
             cursor.execute(*sql_table.update(
@@ -548,33 +563,33 @@
                 .select(
                     move.company,
                     where=line.reconciliation == sql_table.id,
                     group_by=move.company))
             cursor.execute(*sql_table.update([sql_table.company], [value]))
 
     @classmethod
-    def order_name(cls, tables):
+    def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.name), table.name]
+        return [CharLength(table.number), table.number]
 
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def create(cls, vlist):
         pool = Pool()
         Configuration = pool.get('account.configuration')
         configuration = Configuration(1)
 
         vlist = [x.copy() for x in vlist]
         default_company = cls.default_company()
         for vals in vlist:
-            if 'name' not in vals:
-                vals['name'] = configuration.get_multivalue(
+            if 'number' not in vals:
+                vals['number'] = configuration.get_multivalue(
                     'reconciliation_sequence',
                     company=vals.get('company', default_company)).get()
 
         return super(Reconciliation, cls).create(vlist)
 
     @classmethod
     def write(cls, moves, values, *args):
@@ -587,21 +602,31 @@
 
     @classmethod
     def delete(cls, reconciliations):
         pool = Pool()
         Warning = pool.get('res.user.warning')
         for reconciliation in reconciliations:
             if reconciliation.delegate_to:
-                key = '%s.delete.delegated' % reconciliation
+                key = Warning.format('delete.delegated', [reconciliation])
                 if Warning.check(key):
-                    raise DeleteDelegatedWarning(key,
+                    raise ReconciliationDeleteWarning(key,
                         gettext('account.msg_reconciliation_delete_delegated',
                             reconciliation=reconciliation.rec_name,
                             line=reconciliation.delegate_to.rec_name,
                             move=reconciliation.delegate_to.move.rec_name))
+            for line in reconciliation.lines:
+                if line.move.journal.type == 'write-off':
+                    key = Warning.format('delete.write-off', [reconciliation])
+                    if Warning.check(key):
+                        raise ReconciliationDeleteWarning(key,
+                            gettext(
+                                'account.msg_reconciliation_delete_write_off',
+                                reconciliation=reconciliation.rec_name,
+                                line=line.rec_name,
+                                move=line.move.rec_name))
         super().delete(reconciliations)
 
     @classmethod
     def check_lines(cls, reconciliations):
         Lang = Pool().get('ir.lang')
         for reconciliation in reconciliations:
             debit = Decimal('0.0')
@@ -721,14 +746,89 @@
     def get_amount_currency(self, name):
         if self.second_currency:
             currency = self.second_currency
         else:
             currency = self.account.currency
         return currency.id
 
+    @classmethod
+    def get_payable_receivable_balance(cls, lines, name):
+        pool = Pool()
+        Account = pool.get('account.account')
+        AccountType = pool.get('account.account.type')
+        Move = pool.get('account.move')
+
+        transaction = Transaction()
+        database = transaction.database
+        context = transaction.context
+        cursor = transaction.connection.cursor()
+
+        line = cls.__table__()
+        account = Account.__table__()
+        account_type = AccountType.__table__()
+        move = Move.__table__()
+
+        balances = dict.fromkeys(map(int, lines))
+
+        for company, lines in groupby(lines, lambda l: l.company):
+            for sub_lines in grouped_slice(lines):
+                sub_lines = list(sub_lines)
+                where = account.company == company.id
+                where_type = Literal(False)
+                if context.get('receivable', True):
+                    where_type |= account_type.receivable
+                if context.get('payable', True):
+                    where_type |= account_type.payable
+                where &= where_type
+                if not context.get('reconciled'):
+                    if hasattr(cls, 'reconciliation'):
+                        where &= line.reconciliation == Null
+                    elif hasattr(cls, 'reconciled'):
+                        where &= ~line.reconciled
+
+                currency = Coalesce(line.second_currency, company.currency.id)
+                sign = Case(
+                    (account_type.statement == 'income', -1),
+                    else_=1)
+                balance = sign * Case(
+                    (line.amount_second_currency != Null,
+                        line.amount_second_currency),
+                    else_=line.debit - line.credit)
+                if database.has_window_functions():
+                    balance = Sum(balance,
+                        window=Window(
+                            [line.party, currency],
+                            order_by=[
+                                line.maturity_date.asc,
+                                move.date.desc,
+                                line.id.desc,
+                                ]))
+
+                party_where = Literal(False)
+                parties = {l.party for l in sub_lines}
+                if None in parties:
+                    party_where |= line.party == parties.discard(None)
+                party_where |= reduce_ids(line.party, map(int, parties))
+                where &= party_where
+
+                query = (line
+                    .join(move, condition=line.move == move.id)
+                    .join(account, condition=line.account == account.id)
+                    .join(
+                        account_type,
+                        condition=account.type == account_type.id)
+                    .select(
+                        line.id.as_('id'), balance.as_('balance'),
+                        where=where))
+                cursor.execute(*query.select(
+                        query.id, query.balance,
+                        where=reduce_ids(query.id, [l.id for l in sub_lines])))
+                balances.update(cursor)
+        return balances
+
     def get_rec_name(self, name):
         if self.debit > self.credit:
             return self.account.rec_name
         else:
             return '(%s)' % self.account.rec_name
 
     @classmethod
@@ -764,16 +864,17 @@
             ['OR',
                 ('end_date', '=', None),
                 ('end_date', '>=', Eval('date', None)),
                 ],
             ],
         context={
             'company': Eval('company', -1),
+            'period': Eval('period', -1),
             },
-        states=_states, depends={'company'})
+        states=_states, depends={'company', 'period'})
     move = fields.Many2One(
         'account.move', "Move", required=True,
         ondelete='CASCADE',
         states={
             'required': False,
             'readonly': (((Eval('state') == 'valid') | _states['readonly'])
                 & Bool(Eval('move'))),
@@ -817,15 +918,15 @@
             'readonly': _states['readonly'],
             },
         help='The amount expressed in a second currency.')
     second_currency = fields.Many2One('currency.currency', 'Second Currency',
             help='The second currency.',
         domain=[
             If(~Eval('second_currency_required'),
-                (),
+                ('id', '!=', Eval('currency', -1)),
                 ('id', '=', Eval('second_currency_required', -1))),
             ],
         states={
             'required': (Bool(Eval('amount_second_currency'))
                 | Bool(Eval('second_currency_required'))),
             'readonly': _states['readonly']
             })
@@ -866,27 +967,33 @@
         'account.move.reconciliation', 'delegate_to',
         "Reconciliations Delegated", readonly=True)
     tax_lines = fields.One2Many('account.tax.line', 'move_line', 'Tax Lines')
     move_state = fields.Function(
         fields.Selection('get_move_states', "Move State"),
         'on_change_with_move_state', searcher='search_move_field')
     currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'on_change_with_currency')
+            'currency.currency', "Currency"),
+        'on_change_with_currency', searcher='search_currency')
     amount = fields.Function(Monetary(
             "Amount", currency='amount_currency', digits='amount_currency'),
         'get_amount')
     amount_currency = fields.Function(fields.Many2One('currency.currency',
             'Amount Currency'), 'get_amount_currency')
     delegated_amount = fields.Function(Monetary(
             "Delegated Amount",
             currency='amount_currency', digits='amount_currency',
             states={
                 'invisible': ~Eval('reconciliation', False),
                 }),
         'get_delegated_amount')
+    payable_receivable_balance = fields.Function(
+        Monetary(
+            "Payable/Receivable Balance",
+            currency='amount_currency', digits='amount_currency'),
+        'get_payable_receivable_balance')
 
     del _states
 
     @classmethod
     def __setup__(cls):
         super(Line, cls).__setup__()
         cls.__access__.add('move')
@@ -925,39 +1032,52 @@
                 # Index for account.account.party
                 Index(
                     table,
                     (table.account, Index.Equality()),
                     (table.party, Index.Equality()),
                     (table.id, Index.Equality()),
                     where=table.party != Null),
+                # Index for receivable/payable balance
+                Index(
+                    table,
+                    (table.account, Index.Equality()),
+                    (table.party, Index.Equality()),
+                    where=table.reconciliation == Null),
                 })
 
     @classmethod
     def default_date(cls):
         '''
         Return the date of the last line for journal, period
         or the starting date of the period
         or today
         '''
         pool = Pool()
         Period = pool.get('account.period')
         Date = pool.get('ir.date')
+        context = Transaction().context
 
         date = Date.today()
         lines = cls.search([
-                ('journal', '=', Transaction().context.get('journal')),
-                ('period', '=', Transaction().context.get('period')),
-                ], order=[('id', 'DESC')], limit=1)
+                ('company', '=', context.get('company')),
+                ('journal', '=', context.get('journal')),
+                ('period', '=', context.get('period')),
+                ],
+            order=[('date', 'DESC')], limit=1)
         if lines:
-            date = lines[0].date
-        elif Transaction().context.get('period'):
-            period = Period(Transaction().context['period'])
-            date = period.start_date
-        if Transaction().context.get('date'):
-            date = Transaction().context['date']
+            line, = lines
+            date = line.date
+        elif context.get('period'):
+            period = Period(context['period'])
+            if period.start_date >= date:
+                date = period.start_date
+            else:
+                date = period.end_date
+        if context.get('date'):
+            date = context['date']
         return date
 
     @classmethod
     def default_move(cls):
         transaction = Transaction()
         context = transaction.context
         if context.get('journal') and context.get('period'):
@@ -998,16 +1118,19 @@
 
     @staticmethod
     def default_credit():
         return Decimal(0)
 
     @fields.depends('account')
     def on_change_with_currency(self, name=None):
-        if self.account:
-            return self.account.currency.id
+        return self.account.currency if self.account else None
+
+    @classmethod
+    def search_currency(cls, name, clause):
+        return [('account.company.' + clause[0], * clause[1:])]
 
     @classmethod
     def _get_origin(cls):
         'Return list of Model names for origin Reference'
         return ['account.move.line']
 
     @classmethod
@@ -1406,90 +1529,204 @@
                         gettext('account.msg_line_already_reconciled',
                             line=line.rec_name))
 
             lines = list(lines)
             reconcile_account = None
             reconcile_party = None
             amount = Decimal('0.0')
+            amount_second_currency = Decimal('0.0')
+            second_currencies = set()
             for line in lines:
                 amount += line.debit - line.credit
                 if not reconcile_account:
                     reconcile_account = line.account
                 if not reconcile_party:
                     reconcile_party = line.party
-            if amount:
+                if line.amount_second_currency is not None:
+                    amount_second_currency += line.amount_second_currency
+                second_currencies.add(line.second_currency)
+            company = reconcile_account.company
+
+            try:
+                second_currency, = second_currencies
+            except ValueError:
+                amount_second_currency = None
+                second_currency = None
+            if second_currency:
+                writeoff_amount = amount_second_currency
+                writeoff_currency = second_currency
+            else:
+                writeoff_amount = amount
+                writeoff_currency = company.currency
+            if writeoff_amount:
                 move = cls._get_writeoff_move(
-                    reconcile_account, reconcile_party, amount,
+                    reconcile_account, reconcile_party,
+                    writeoff_amount, writeoff_currency,
                     date, writeoff, description)
                 move.save()
-                lines += cls.search([
-                        ('move', '=', move.id),
-                        ('account', '=', reconcile_account.id),
-                        ('debit', '=', amount < Decimal('0.0') and - amount
-                            or Decimal('0.0')),
-                        ('credit', '=', amount > Decimal('0.0') and amount
-                            or Decimal('0.0')),
-                        ], limit=1)
+                for line in move.lines:
+                    if line.account == reconcile_account:
+                        lines.append(line)
+                        amount += line.debit - line.credit
+            if second_currency and amount:
+                move = cls._get_exchange_move(
+                    reconcile_account, reconcile_party, amount, date)
+                move.save()
+                for line in move.lines:
+                    if line.account == reconcile_account:
+                        lines.append(line)
+                        amount += line.debit - line.credit
+            assert not amount, f"{amount} must be zero"
             reconciliations.append({
                     'company': reconcile_account.company,
                     'lines': [('add', [x.id for x in lines])],
                     'date': max(l.date for l in lines),
                     'delegate_to': delegate_to,
                     })
         return Reconciliation.create(reconciliations)
 
     @classmethod
-    def _get_writeoff_move(cls, reconcile_account, reconcile_party, amount,
+    def _get_writeoff_move(
+            cls, reconcile_account, reconcile_party, amount, currency,
             date=None, writeoff=None, description=None):
         pool = Pool()
+        Currency = pool.get('currency.currency')
         Date = pool.get('ir.date')
         Period = pool.get('account.period')
         Move = pool.get('account.move')
         company = reconcile_account.company
         if not date:
             with Transaction().set_context(company=company.id):
                 date = Date.today()
-        period_id = Period.find(reconcile_account.company.id, date=date)
+        period = Period.find(reconcile_account.company, date=date)
         account = None
         journal = None
-        if writeoff:
+        if writeoff and writeoff.company == company:
             if amount >= 0:
                 account = writeoff.debit_account
             else:
                 account = writeoff.credit_account
             journal = writeoff.journal
 
+        if currency != company.currency:
+            amount_second_currency = amount
+            second_currency = currency
+            with Transaction().set_context(date=date):
+                amount = Currency.compute(
+                    currency, amount, company.currency)
+        else:
+            amount_second_currency = None
+            second_currency = None
+
         move = Move()
         move.company = company
         move.journal = journal
-        move.period = period_id
+        move.period = period
         move.date = date
         move.description = description
 
         lines = []
 
         line = cls()
         lines.append(line)
         line.account = reconcile_account
         line.party = reconcile_party
         line.debit = -amount if amount < 0 else 0
         line.credit = amount if amount > 0 else 0
+        if second_currency:
+            line.amount_second_currency = (
+                amount_second_currency).copy_sign(
+                    line.debit - line.credit)
+            line.second_currency = second_currency
 
         line = cls()
         lines.append(line)
         line.account = account
         line.party = (
             reconcile_party if account and account.party_required else None)
         line.debit = amount if amount > 0 else 0
         line.credit = -amount if amount < 0 else 0
+        if account.second_currency:
+            with Transaction().set_context(date=date):
+                line.amount_second_currency = Currency.compute(
+                    company.currency, amount,
+                    reconcile_account.second_currency).copy_sign(
+                        line.debit - line.credit)
+
+        move.lines = lines
+        return move
+
+    @classmethod
+    def _get_exchange_move(cls, account, party, amount, date=None):
+        pool = Pool()
+        Configuration = pool.get('account.configuration')
+        Date = pool.get('ir.date')
+        Move = pool.get('account.move')
+        Period = pool.get('account.period')
+
+        configuration = Configuration(1)
+        company = account.company
+        if not date:
+            with Transaction().set_context(company=company.id):
+                date = Date.today()
+
+        period_id = Period.find(company.id, date=date)
+
+        move = Move()
+        move.company = company
+        move.journal = configuration.get_multivalue(
+            'currency_exchange_journal', company=company.id)
+        move.period = period_id
+        move.date = date
+
+        lines = []
+
+        line = cls()
+        lines.append(line)
+        line.account = account
+        line.party = party
+        line.debit = -amount if amount < 0 else 0
+        line.credit = amount if amount > 0 else 0
+
+        line = cls()
+        lines.append(line)
+        line.debit = amount if amount > 0 else 0
+        line.credit = -amount if amount < 0 else 0
+        if line.credit:
+            line.account = configuration.get_multivalue(
+                'currency_exchange_credit_account', company=company.id)
+        else:
+            line.account = configuration.get_multivalue(
+                'currency_exchange_debit_account', company=company.id)
 
         move.lines = lines
         return move
 
 
+class LineReceivablePayableContext(ModelView):
+    "Receivable/Payable Line Context"
+    __name__ = 'account.move.line.receivable_payable.context'
+
+    reconciled = fields.Boolean("Reconciled")
+    receivable = fields.Boolean("Receivable")
+    payable = fields.Boolean("Payable")
+
+    @classmethod
+    def default_reconciled(cls):
+        return Transaction().context.get('reconciled', False)
+
+    @classmethod
+    def default_receivable(cls):
+        return Transaction().context.get('receivable', True)
+
+    @classmethod
+    def default_payable(cls):
+        return Transaction().context.get('payable', True)
+
+
 class WriteOff(DeactivableMixin, ModelSQL, ModelView):
     'Reconcile Write Off'
     __name__ = 'account.move.reconcile.write_off'
     company = fields.Many2One('company.company', "Company", required=True)
     name = fields.Char("Name", required=True, translate=True)
     journal = fields.Many2One('account.journal', "Journal", required=True,
         domain=[('type', '=', 'write-off')],
@@ -1527,19 +1764,24 @@
     __name__ = 'account.move.open_journal.ask'
     journal = fields.Many2One('account.journal', 'Journal', required=True)
     period = fields.Many2One('account.period', 'Period', required=True,
         domain=[
             ('state', '!=', 'close'),
             ])
 
-    @staticmethod
-    def default_period():
-        Period = Pool().get('account.period')
-        return Period.find(Transaction().context.get('company'),
-                exception=False)
+    @classmethod
+    def default_period(cls):
+        pool = Pool()
+        Period = pool.get('account.period')
+        company = Transaction().context.get('company')
+        try:
+            period = Period.find(company)
+        except PeriodNotFoundError:
+            return None
+        return period.id
 
 
 class OpenJournal(Wizard):
     'Open Journal'
     __name__ = 'account.move.open_journal'
     start = StateTransition()
     ask = StateView('account.move.open_journal.ask',
@@ -1664,63 +1906,86 @@
         required=True,
         domain=[
             ('company', '=', Eval('company')),
             ])
     date = fields.Date('Date', required=True)
     amount = Monetary(
         "Amount", currency='currency', digits='currency', readonly=True)
-    currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"),
-        'on_change_with_currency')
+    currency = fields.Many2One('currency.currency', "Currency", readonly=True)
     description = fields.Char('Description')
 
     @staticmethod
     def default_date():
         Date = Pool().get('ir.date')
         return Date.today()
 
-    @fields.depends('company')
-    def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
-
 
 class ReconcileLines(Wizard):
     'Reconcile Lines'
     __name__ = 'account.move.reconcile_lines'
     start = StateTransition()
     writeoff = StateView('account.move.reconcile_lines.writeoff',
         'account.reconcile_lines_writeoff_view_form', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Reconcile', 'reconcile', 'tryton-ok', default=True),
             ])
     reconcile = StateTransition()
 
+    @classmethod
+    def check_access(cls, models=None):
+        transaction = Transaction()
+        if transaction.user:
+            context = transaction.context
+            models = set() if models is None else models.copy()
+            models.update({'account.move.line', 'account.general_ledger.line'})
+            model = context.get('active_model')
+            if model and model not in models:
+                raise AccessError(gettext(
+                        'ir.msg_access_wizard_model_error',
+                        wizard=cls.__name__,
+                        model=model))
+        super().check_access()
+
     def get_writeoff(self):
         "Return writeoff amount and company"
         company = None
         amount = Decimal('0.0')
+        amount_second_currency = Decimal('0.0')
+        second_currencies = set()
         for line in self.records:
             amount += line.debit - line.credit
+            if line.amount_second_currency is not None:
+                amount_second_currency += line.amount_second_currency
+            second_currencies.add(line.second_currency)
             if not company:
                 company = line.account.company
-        return amount, company
+        try:
+            second_currency, = second_currencies
+        except ValueError:
+            second_currency = None
+        if second_currency:
+            amount = amount_second_currency
+            currency = second_currency
+        else:
+            currency = company.currency
+        return amount, currency, company
 
     def transition_start(self):
-        amount, company = self.get_writeoff()
+        amount, currency, company = self.get_writeoff()
         if not company:
             return 'end'
-        if company.currency.is_zero(amount):
+        if currency.is_zero(amount):
             return 'reconcile'
         return 'writeoff'
 
     def default_writeoff(self, fields):
-        amount, company = self.get_writeoff()
+        amount, currency, company = self.get_writeoff()
         return {
             'amount': amount,
+            'currency': currency.id,
             'company': company.id,
             }
 
     def transition_reconcile(self):
         self.model.reconcile(
             self.records,
             writeoff=getattr(self.writeoff, 'writeoff', None),
@@ -1731,14 +1996,29 @@
 
 class UnreconcileLines(Wizard):
     'Unreconcile Lines'
     __name__ = 'account.move.unreconcile_lines'
     start_state = 'unreconcile'
     unreconcile = StateTransition()
 
+    @classmethod
+    def check_access(cls, models=None):
+        transaction = Transaction()
+        if transaction.user:
+            context = transaction.context
+            models = set() if models is None else models.copy()
+            models.update({'account.move.line', 'account.general_ledger.line'})
+            model = context.get('active_model')
+            if model and model not in models:
+                raise AccessError(gettext(
+                        'ir.msg_access_wizard_model_error',
+                        wizard=cls.__name__,
+                        model=model))
+        super().check_access()
+
     def transition_unreconcile(self):
         self.make_unreconciliation(self.records)
         return 'end'
 
     @classmethod
     def make_unreconciliation(cls, lines):
         pool = Pool()
@@ -1802,155 +2082,218 @@
                         else_=False)
                     | Case((account_type.payable & ~account_type.receivable,
                             Sum(balance) > 0),
                         else_=False)
                     )))
         return [a for a, in cursor]
 
-    def get_parties(self, account, _balanced=False, party=None):
+    def get_parties(self, account, party=None):
         'Return a list party to reconcile for the account'
         pool = Pool()
         Line = pool.get('account.move.line')
         line = Line.__table__()
         cursor = Transaction().connection.cursor()
 
         if self.model and self.model.__name__ == 'account.move.line':
             lines = [l for l in self.records if not l.reconciliation]
             return list({l.party for l in lines if l.account == account})
 
-        balance = line.debit - line.credit
+        where = ((line.reconciliation == Null)
+            & (line.account == account.id))
+        if party:
+            where &= (line.party == party.id)
+        cursor.execute(*line.select(line.party,
+                where=where,
+                group_by=line.party))
+        return [p for p, in cursor]
+
+    def get_currencies(self, account, party, currency=None, _balanced=False):
+        "Return a list of currencies to reconcile for the account and party"
+        pool = Pool()
+        Line = pool.get('account.move.line')
+        line = Line.__table__()
+        cursor = Transaction().connection.cursor()
+
+        if self.model and self.model.__name__ == 'account.move.line':
+            lines = [l for l in self.records if not l.reconciliation]
+            return list({
+                    (l.second_currency or l.currency).id
+                    for l in lines
+                    if l.account == account and l.party == party})
+
+        balance = Case(
+            (line.second_currency != Null, line.amount_second_currency),
+            else_=line.debit - line.credit)
         if _balanced:
             having = Sum(balance) == 0
         else:
             having = ((
                     Sum(Case((balance > 0, 1), else_=0)) > 0)
                 & (Sum(Case((balance < 0, 1), else_=0)) > 0)
                 | Case((account.type.receivable, Sum(balance) < 0),
                     else_=False)
                 | Case((account.type.payable, Sum(balance) > 0),
                     else_=False)
                 )
         where = ((line.reconciliation == Null)
-            & (line.account == account.id))
-        if party:
-            where &= (line.party == party.id)
-        cursor.execute(*line.select(line.party,
+            & (line.account == account.id)
+            & (line.party == party.id if party else None))
+        currency_expr = Coalesce(line.second_currency, account.currency.id)
+        if currency:
+            where &= (currency_expr == currency.id)
+        cursor.execute(*line.select(
+                currency_expr,
                 where=where,
-                group_by=line.party,
+                group_by=line.second_currency,
                 having=having))
         return [p for p, in cursor]
 
+    @check_access
     def transition_next_(self):
         pool = Pool()
         Line = pool.get('account.move.line')
 
         def next_account():
             accounts = list(self.show.accounts)
             if not accounts:
                 return
             account = accounts.pop()
             self.show.account = account
-            self.show.parties = self.get_parties(account)
             self.show.accounts = accounts
+            self.show.parties = self.get_parties(account)
+            next_party()
             return account
 
         def next_party():
             parties = list(self.show.parties)
             if not parties:
                 return
             party = parties.pop()
             self.show.party = party
             self.show.parties = parties
+            self.show.currencies = self.get_currencies(
+                self.show.account, party)
             return party,
 
-        with Transaction().set_context(_check_access=True):
-            if getattr(self.show, 'accounts', None) is None:
-                self.show.accounts = self.get_accounts()
-                if not next_account():
-                    return 'end'
-            if getattr(self.show, 'parties', None) is None:
-                self.show.parties = self.get_parties(self.show.account)
+        def next_currency():
+            currencies = list(self.show.currencies)
+            if not currencies:
+                return
+            currency = currencies.pop()
+            self.show.currency = currency
+            self.show.currencies = currencies
+            return currency
+
+        if getattr(self.show, 'accounts', None) is None:
+            self.show.accounts = self.get_accounts()
+            if not next_account():
+                return 'end'
+        if getattr(self.show, 'parties', None) is None:
+            self.show.parties = self.get_parties(self.show.account)
+            if not next_party():
+                return 'end'
+        if getattr(self.show, 'currencies', None) is None:
+            self.show.currencies = self.get_currencies(
+                self.show.account, self.show.party)
 
+        while not next_currency():
             while not next_party():
                 if not next_account():
                     return 'end'
-            if self.start.automatic or self.start.only_balanced:
-                lines = self._default_lines()
-                if lines and self.start.automatic:
-                    while lines:
-                        Line.reconcile(lines)
-                        lines = self._default_lines()
-                    if not self.get_parties(
-                            self.show.account, party=self.show.party):
-                        return 'next_'
-                elif not lines and self.start.only_balanced:
+        if self.start.automatic or self.start.only_balanced:
+            lines = self._default_lines()
+            if lines and self.start.automatic:
+                while lines:
+                    Line.reconcile(lines)
+                    lines = self._default_lines()
+                if not self.get_parties(
+                        self.show.account, party=self.show.party):
                     return 'next_'
-            return 'show'
+            elif not lines and self.start.only_balanced:
+                return 'next_'
+        return 'show'
 
     def default_show(self, fields):
         pool = Pool()
         Date = pool.get('ir.date')
 
         defaults = {}
         defaults['accounts'] = [a.id for a in self.show.accounts]
         defaults['account'] = self.show.account.id
         defaults['company'] = self.show.account.company.id
         defaults['parties'] = [p.id for p in self.show.parties]
         defaults['party'] = self.show.party.id if self.show.party else None
-        defaults['currency'] = self.show.account.company.currency.id
+        defaults['currencies'] = [c.id for c in self.show.currencies]
+        defaults['currency'] = (
+            self.show.currency.id if self.show.currency else None)
         defaults['lines'] = list(map(int, self._default_lines()))
-        defaults['write_off_amount'] = Decimal(0)
+        defaults['write_off_amount'] = None
         with Transaction().set_context(company=self.show.account.company.id):
             defaults['date'] = Date.today()
         return defaults
 
     def _all_lines(self):
         'Return all lines to reconcile for the current state'
         pool = Pool()
         Line = pool.get('account.move.line')
         return Line.search([
                 ('account', '=', self.show.account.id),
                 ('party', '=',
                     self.show.party.id if self.show.party else None),
                 ('reconciliation', '=', None),
+                ['OR',
+                    [
+                        ('currency', '=', self.show.currency.id),
+                        ('second_currency', '=', None),
+                        ],
+                    ('second_currency', '=', self.show.currency.id),
+                    ],
                 ],
             order=[])
 
     def _line_sort_key(self, line):
         return [line.maturity_date or line.date]
 
     def _default_lines(self):
         'Return the larger list of lines which can be reconciled'
         if self.model and self.model.__name__ == 'account.move.line':
             requested = {
                 l for l in self.records
                 if l.account == self.show.account
-                and l.party == self.show.party}
+                and l.party == self.show.party
+                and (l.second_currency or l.currency) == self.show.currency}
         else:
             requested = None
+        currency = self.show.currency
 
-        currency = self.show.account.company.currency
+        def balance(line):
+            if line.second_currency == currency:
+                return line.amount_second_currency
+            elif line.currency == currency:
+                return line.debit - line.credit
+            else:
+                return 0
 
         all_lines = self._all_lines()
-        amount = sum((l.debit - l.credit) for l in all_lines)
+        amount = sum(map(balance, all_lines))
         if currency.is_zero(amount):
             return all_lines
 
         chunk = config.getint('account', 'reconciliation_chunk', default=10)
         # Combination is exponential so it must be limited to small number
         default = []
         for lines in grouped_slice(
                 sorted(all_lines, key=self._line_sort_key), chunk):
             lines = list(lines)
             best = None
             for n in range(len(lines), 1, -1):
                 for comb_lines in combinations(lines, n):
                     if requested and not requested.intersection(comb_lines):
                         continue
-                    amount = sum((l.debit - l.credit) for l in comb_lines)
+                    amount = sum(balance(l) for l in comb_lines)
                     if currency.is_zero(amount):
                         best = comb_lines
                         break
                 if best:
                     break
             if best:
                 default.extend(best)
@@ -1965,15 +2308,17 @@
 
         if self.show.lines:
             Line.reconcile(self.show.lines,
                 date=self.show.date,
                 writeoff=self.show.write_off,
                 description=self.show.description)
 
-        if self.get_parties(self.show.account, party=self.show.party):
+        if self.get_currencies(
+                self.show.account, self.show.party,
+                currency=self.show.currency):
             return 'show'
         return 'next_'
 
 
 class ReconcileStart(ModelView):
     "Reconcile"
     __name__ = 'account.reconcile.start'
@@ -2008,56 +2353,62 @@
         depends={'company'})
     party = fields.Many2One(
         'party.party', 'Party', readonly=True,
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
+    currencies = fields.Many2Many(
+        'currency.currency', None, None, "Currencies", readonly=True)
+    currency = fields.Many2One('currency.currency', "Currency", readonly=True)
     lines = fields.Many2Many('account.move.line', None, None, 'Lines',
         domain=[
             ('account', '=', Eval('account')),
             ('party', '=', Eval('party')),
             ('reconciliation', '=', None),
+            ['OR',
+                [
+                    ('currency', '=', Eval('currency', -1)),
+                    ('second_currency', '=', None),
+                    ],
+                ('second_currency', '=', Eval('currency', -1)),
+                ],
             ])
 
     _write_off_states = {
         'required': Bool(Eval('write_off_amount', 0)),
         'invisible': ~Eval('write_off_amount', 0),
         }
 
-    write_off_amount = fields.Function(Monetary(
-            "Amount", currency='currency', digits='currency',
-            states=_write_off_states),
-        'on_change_with_write_off_amount')
-    currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"),
-        'on_change_with_currency')
+    write_off_amount = Monetary(
+        "Amount", currency='currency', digits='currency', readonly=True,
+        states=_write_off_states)
     write_off = fields.Many2One(
         'account.move.reconcile.write_off', "Write Off",
         domain=[
             ('company', '=', Eval('company', -1)),
             ],
         states=_write_off_states)
     date = fields.Date('Date', states=_write_off_states)
     description = fields.Char('Description',
         states={
             'invisible': _write_off_states['invisible'],
             })
 
-    @fields.depends('lines', 'currency')
-    def on_change_with_write_off_amount(self, name=None):
-        amount = sum(((l.debit - l.credit) for l in self.lines), Decimal(0))
+    @fields.depends('lines', 'currency', 'company')
+    def on_change_lines(self):
+        amount = Decimal(0)
+        for line in self.lines:
+            if line.second_currency == self.currency:
+                amount += line.amount_second_currency
+            elif line.currency == self.currency:
+                amount += line.debit - line.credit
         if self.currency:
             amount = self.currency.round(amount)
-        return amount
-
-    @fields.depends('company')
-    def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        self.write_off_amount = amount
 
 
 class CancelMoves(Wizard):
     'Cancel Moves'
     __name__ = 'account.move.cancel'
     start_state = 'default'
     default = StateView('account.move.cancel.default',
@@ -2097,28 +2448,36 @@
 
         for move in moves:
             if moves_w_delegation.get(move):
                 # Skip further warnings
                 with Transaction().set_user(0):
                     Unreconcile.make_unreconciliation(moves_w_delegation[move])
             default = self.default_cancel(move)
-            cancel_move = move.cancel(default=default)
+            cancel_move = move.cancel(
+                default=default, reversal=self.default.reversal)
             to_reconcile = defaultdict(list)
             for line in move.lines + cancel_move.lines:
                 if line.account.reconcile:
                     to_reconcile[(line.account, line.party)].append(line)
             for lines in to_reconcile.values():
                 Line.reconcile(lines)
         return 'end'
 
 
 class CancelMovesDefault(ModelView):
     'Cancel Moves'
     __name__ = 'account.move.cancel.default'
     description = fields.Char('Description')
+    reversal = fields.Boolean(
+        "Reversal",
+        help="Reverse debit and credit.")
+
+    @classmethod
+    def default_reversal(cls):
+        return True
 
 
 class GroupLines(Wizard):
     "Group Lines"
     __name__ = 'account.move.line.group'
     start = StateView('account.move.line.group.start',
         'account.move_line_group_start_view_form', [
@@ -2213,15 +2572,15 @@
         Period = pool.get('account.period')
         Line = pool.get('account.move.line')
 
         company = grouping['company']
         if not date:
             with Transaction().set_context(company=company.id):
                 date = Date.today()
-        period = Period.find(company.id, date=date)
+        period = Period.find(company, date=date)
 
         move = Move()
         move.company = company
         move.date = date
         move.period = period
         move.journal = journal
 
@@ -2475,15 +2834,15 @@
         Move = pool.get('account.move')
         Period = pool.get('account.period')
 
         company = account.company
         if not date:
             with Transaction().set_context(company=company.id):
                 date = Date.today()
-        period = Period.find(company.id, date=date)
+        period = Period.find(company, date=date)
 
         move = Move()
         move.company = company
         move.date = date
         move.period = period
         move.journal = journal
 
@@ -2672,15 +3031,15 @@
         except ValueError:
             raise DelegateLineError(
                 gettext('account.msg_delegate_line_same_origins'))
 
         if not date:
             with Transaction().set_context(company=company.id):
                 date = Date.today()
-        period = Period.find(company.id, date=date)
+        period = Period.find(company, date=date)
 
         move = Move()
         move.company = company
         move.date = date
         move.period = period
         move.journal = journal
         move.origin = origin
```

### Comparing `trytond_account-6.6.3/move.xml` & `trytond_account-6.8.0/move.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account-6.6.3/move.xml` & `trytond_account-6.8.0/move.xml`

```diff
@@ -171,17 +171,24 @@
     </record>
     <record model="ir.ui.view" id="move_line_view_list_payable_receivable">
       <field name="model">account.move.line</field>
       <field name="type">tree</field>
       <field name="priority" eval="30"/>
       <field name="name">move_line_list_payable_receivable</field>
     </record>
+    <record model="ir.ui.view" id="move_line_view_list_reconcile">
+      <field name="model">account.move.line</field>
+      <field name="type">tree</field>
+      <field name="priority" eval="30"/>
+      <field name="name">move_line_list_reconcile</field>
+    </record>
     <record model="ir.action.act_window" id="act_move_line_form">
       <field name="name">Account Move Lines</field>
       <field name="res_model">account.move.line</field>
+      <field name="domain" eval="[('account', 'in', Eval('active_ids', [])), ('state', '=', 'valid')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_line_form_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="move_line_view_tree"/>
       <field name="act_window" ref="act_move_line_form"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_line_form_view2">
@@ -190,57 +197,52 @@
       <field name="act_window" ref="act_move_line_form"/>
     </record>
     <record model="ir.action.wizard" id="act_open_account">
       <field name="name">Open Move Account</field>
       <field name="wiz_name">account.move.open_account</field>
       <field name="model">account.account</field>
     </record>
-    <record model="ir.action.keyword" id="act_open_account_keyword">
+    <record model="ir.action.keyword" id="act_open_account_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">account.account,-1</field>
       <field name="action" ref="act_open_account"/>
     </record>
+    <record model="ir.action.keyword" id="act_open_account_keyword2">
+      <field name="keyword">form_relate</field>
+      <field name="model">account.account,-1</field>
+      <field name="action" ref="act_open_account"/>
+    </record>
     <record model="ir.action.act_window" id="act_move_line_payable_receivable">
       <field name="name">Payable/Receivable Lines</field>
       <field name="res_model">account.move.line</field>
-      <field name="domain" eval="[['OR', ('account.type.receivable', '=', True), ('account.type.payable', '=', True)], If(Eval('active_ids', []) == [Eval('active_id')], ('party', '=', Eval('active_id')), ('party', 'in', Eval('active_ids'))), ('company', '=', Eval('context', {}).get('company', -1))]" pyson="1"/>
-      <field name="search_value" eval="[('reconciliation', '=', None)]" pyson="1"/>
+      <field name="context_model">account.move.line.receivable_payable.context</field>
+      <field name="domain" eval="[('party', 'in', Eval('active_ids')), ('company', '=', Eval('context', {}).get('company', -1))]" pyson="1"/>
+      <field name="context_domain" eval="[['OR', If(Eval('receivable', True), ('account.type.receivable', '=', True), ('id', '&lt;', 0)), If(Eval('payable', True), ('account.type.payable', '=', True), ('id', '&lt;', 0))], If(Eval('reconciled', False), (), ('reconciliation', '=', None))]" pyson="1"/>
+      <field name="search_value"/>
       <field name="order" eval="[('maturity_date', 'ASC'), ('date', 'DESC'), ('id', 'DESC')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_line_payable_receivable_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="move_line_view_list_payable_receivable"/>
       <field name="act_window" ref="act_move_line_payable_receivable"/>
     </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_payable_receivable_domain_payable">
-      <field name="name">Payable</field>
-      <field name="sequence" eval="10"/>
-      <field name="domain" eval="[('account.type.payable', '=', True)]" pyson="1"/>
-      <field name="act_window" ref="act_move_line_payable_receivable"/>
-    </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_payable_receivable_domain_receivable">
-      <field name="name">Receivable</field>
-      <field name="sequence" eval="20"/>
-      <field name="domain" eval="[('account.type.receivable', '=', True)]" pyson="1"/>
-      <field name="act_window" ref="act_move_line_payable_receivable"/>
-    </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_payable_receivable_domain_all">
-      <field name="name">All</field>
-      <field name="sequence" eval="9999"/>
-      <field name="act_window" ref="act_move_line_payable_receivable"/>
-    </record>
     <record model="ir.action.keyword" id="act_move_line_payable_receivable_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_move_line_payable_receivable"/>
     </record>
     <record model="ir.action-res.group" id="act_move_line_payable-group_account">
       <field name="action" ref="act_move_line_payable_receivable"/>
       <field name="group" ref="group_account"/>
     </record>
+    <record model="ir.ui.view" id="move_line_receivable_payable_context_view_form">
+      <field name="model">account.move.line.receivable_payable.context</field>
+      <field name="type">form</field>
+      <field name="name">move_line_receivable_payable_context_form</field>
+    </record>
     <record model="ir.ui.view" id="open_journal_ask_view_form">
       <field name="model">account.move.open_journal.ask</field>
       <field name="type">form</field>
       <field name="name">open_journal_ask_form</field>
     </record>
     <record model="ir.action.wizard" id="act_open_journal">
       <field name="name">Open Journal</field>
@@ -256,32 +258,41 @@
       <field name="model">account.move.reconcile_lines.writeoff</field>
       <field name="type">form</field>
       <field name="name">reconcile_lines_writeoff_form</field>
     </record>
     <record model="ir.action.wizard" id="act_reconcile_lines">
       <field name="name">Reconcile Lines</field>
       <field name="wiz_name">account.move.reconcile_lines</field>
-      <field name="model">account.move.line</field>
+      <field name="model"/>
     </record>
     <record model="ir.action.keyword" id="act_reconcile_lines_keyword">
       <field name="keyword">form_action</field>
       <field name="model">account.move.line,-1</field>
       <field name="action" ref="act_reconcile_lines"/>
     </record>
-    <!-- TODO keyword general ledger -->
+    <record model="ir.action.keyword" id="act_reconcile_lines_keyword_general_ledger_line">
+      <field name="keyword">form_action</field>
+      <field name="model">account.general_ledger.line,-1</field>
+      <field name="action" ref="act_reconcile_lines"/>
+    </record>
     <record model="ir.action.wizard" id="act_unreconcile_lines">
       <field name="name">Unreconcile Lines</field>
       <field name="wiz_name">account.move.unreconcile_lines</field>
-      <field name="model">account.move.line</field>
+      <field name="model"/>
     </record>
     <record model="ir.action.keyword" id="act_unreconcile_lines_keyword">
       <field name="keyword">form_action</field>
       <field name="model">account.move.line,-1</field>
       <field name="action" ref="act_unreconcile_lines"/>
     </record>
+    <record model="ir.action.keyword" id="act_unreconcile_lines_keyword_general_ledger_line">
+      <field name="keyword">form_action</field>
+      <field name="model">account.general_ledger.line,-1</field>
+      <field name="action" ref="act_unreconcile_lines"/>
+    </record>
     <record model="ir.action.wizard" id="act_reconcile">
       <field name="name">Reconcile Accounts</field>
       <field name="wiz_name">account.reconcile</field>
       <field name="window" eval="True"/>
     </record>
     <menuitem parent="menu_processing" action="act_reconcile" sequence="20" id="menu_reconcile"/>
     <record model="ir.ui.view" id="reconcile_start_view_form">
```

### Comparing `trytond_account-6.6.3/move_template.py` & `trytond_account-6.8.0/move_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.tools import decistmt
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
-from .exceptions import MoveTemplateExpressionError
+from .exceptions import (
+    MoveTemplateExpressionError, MoveTemplateKeywordValidationError,
+    PeriodNotFoundError)
 
 
 class MoveTemplate(DeactivableMixin, ModelSQL, ModelView):
     'Account Move Template'
     __name__ = 'account.move.template'
     name = fields.Char('Name', required=True, translate=True)
     keywords = fields.One2Many('account.move.template.keyword', 'move',
@@ -64,15 +66,16 @@
 
 
 class MoveTemplateKeyword(sequence_ordered(), ModelSQL, ModelView):
     'Account Move Template Keyword'
     __name__ = 'account.move.template.keyword'
     name = fields.Char('Name', required=True)
     string = fields.Char('String', required=True, translate=True)
-    move = fields.Many2One('account.move.template', 'Move', required=True)
+    move = fields.Many2One(
+        'account.move.template', "Move", required=True, ondelete='CASCADE')
     type_ = fields.Selection([
             ('char', 'Char'),
             ('numeric', 'Numeric'),
             ('date', 'Date'),
             ('party', 'Party'),
             ], 'Type')
     required = fields.Boolean('Required')
@@ -82,14 +85,25 @@
             })
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('move')
 
+    @classmethod
+    def validate(cls, keywords):
+        for keyword in keywords:
+            keyword.check_name()
+
+    def check_name(self):
+        if self.name and not self.name.isidentifier():
+            raise MoveTemplateKeywordValidationError(
+                gettext('account.msg_name_not_valid',
+                    name=self.name))
+
     @staticmethod
     def default_required():
         return False
 
     def get_field(self):
         field = getattr(self, '_get_field_%s' % self.type_)()
         field.update({
@@ -154,15 +168,16 @@
             else:
                 yield k, v
 
 
 class MoveLineTemplate(ModelSQL, ModelView):
     'Account Move Line Template'
     __name__ = 'account.move.line.template'
-    move = fields.Many2One('account.move.template', 'Move', required=True)
+    move = fields.Many2One(
+        'account.move.template', "Move", required=True, ondelete='CASCADE')
     operation = fields.Selection([
             ('debit', 'Debit'),
             ('credit', 'Credit'),
             ], 'Operation', required=True)
     amount = fields.Char('Amount', required=True,
         help="A python expression that will be evaluated with the keywords.")
     account = fields.Many2One('account.account', 'Account', required=True,
@@ -201,24 +216,24 @@
         Line = pool.get('account.move.line')
         Keyword = pool.get('account.move.template.keyword')
 
         line = Line()
         try:
             amount = simple_eval(decistmt(self.amount),
                 functions={'Decimal': Decimal}, names=values)
-        except InvalidExpression as e:
+        except (InvalidExpression, SyntaxError) as e:
             raise MoveTemplateExpressionError(
                 gettext('account.msg_move_template_invalid_expression',
                     expression=values,
                     template=self.move.rec_name,
                     error=e)) from e
 
         if not isinstance(amount, Decimal):
             raise MoveTemplateExpressionError(
-                gettext('account.msg_move_template_expession_not_number',
+                gettext('account.msg_move_template_expression_not_number',
                     value=amount,
                     expression=self.move.name,
                     template=self.move.rec_name))
 
         amount = self.move.company.currency.round(amount)
         if self.operation == 'debit':
             line.debit = amount
@@ -241,15 +256,17 @@
 
         return line
 
 
 class TaxLineTemplate(ModelSQL, ModelView):
     'Account Tax Line Template'
     __name__ = 'account.tax.line.template'
-    line = fields.Many2One('account.move.line.template', 'Line', required=True)
+    line = fields.Many2One(
+        'account.move.line.template', "Line",
+        required=True, ondelete='CASCADE')
     amount = fields.Char('Amount', required=True,
         help="A python expression that will be evaluated with the keywords.")
     type = fields.Selection([
             ('tax', "Tax"),
             ('base', "Base"),
             ], "Type", required=True)
 
@@ -279,15 +296,15 @@
         pool = Pool()
         TaxLine = pool.get('account.tax.line')
 
         line = TaxLine()
         try:
             amount = simple_eval(decistmt(self.amount),
                 functions={'Decimal': Decimal}, names=values)
-        except InvalidExpression as e:
+        except (InvalidExpression, SyntaxError) as e:
             raise MoveTemplateExpressionError(
                 gettext('account.msg_template_invalid_expression',
                     expression=values,
                     template=self.line.rec_name,
                     error=e)) from e
 
         if not isinstance(amount, Decimal):
@@ -397,19 +414,23 @@
     period = fields.Many2One('account.period', 'Period', required=True,
         domain=[
             ('state', '!=', 'close'),
             ('fiscalyear.company.id', '=',
                 Eval('context', {}).get('company', 0)),
             ])
 
-    @staticmethod
-    def default_period():
+    @classmethod
+    def default_period(cls):
         pool = Pool()
         Period = pool.get('account.period')
         company = Transaction().context.get('company')
-        return Period.find(company, exception=False)
+        try:
+            period = Period.find(company)
+        except PeriodNotFoundError:
+            return None
+        return period.id
 
 
 class CreateMoveKeywords(ModelView):
     'Create Move from Template'
     __no_slots__ = True
     __name__ = 'account.move.template.create.keywords'
```

### Comparing `trytond_account-6.6.3/move_template.xml` & `trytond_account-6.8.0/move_template.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/party.py` & `trytond_account-6.8.0/party.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,17 +272,16 @@
                 'visual', If(Eval('receivable_today', 0) > 0, 'danger', '')),
             ('/tree/field[@name="payable_today"]',
                 'visual', If(Eval('payable_today', 0) < 0, 'warning', '')),
             ]
 
     @classmethod
     def copy(cls, parties, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             fields = [
                 'accounts',
                 'account_payable', 'account_receivable',
                 'customer_tax_rule', 'supplier_tax_rule']
             default_values = cls.default_get(fields, with_rec_name=False)
             for fname in fields:
                 default.setdefault(fname, default_values.get(fname))
```

### Comparing `trytond_account-6.6.3/party.xml` & `trytond_account-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/period.py` & `trytond_account-6.8.0/period.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
+from trytond.cache import Cache
 from trytond.const import OPERATORS
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Eval, Id
 from trytond.transaction import Transaction
@@ -46,14 +47,15 @@
             ('standard', 'Standard'),
             ('adjustment', 'Adjustment'),
             ], 'Type', required=True,
         states=_STATES)
     company = fields.Function(fields.Many2One('company.company', 'Company',),
         'on_change_with_company', searcher='search_company')
     icon = fields.Function(fields.Char("Icon"), 'get_icon')
+    _find_cache = Cache(__name__ + '.find', context=False)
 
     @classmethod
     def __setup__(cls):
         super(Period, cls).__setup__()
         t = cls.__table__()
         cls.__access__.add('fiscalyear')
         cls._sql_indexes.add(
@@ -89,16 +91,15 @@
 
     @staticmethod
     def default_type():
         return 'standard'
 
     @fields.depends('fiscalyear', '_parent_fiscalyear.company')
     def on_change_with_company(self, name=None):
-        if self.fiscalyear:
-            return self.fiscalyear.company.id
+        return self.fiscalyear.company if self.fiscalyear else None
 
     @classmethod
     def search_company(cls, name, clause):
         return [('fiscalyear.' + clause[0],) + tuple(clause[1:])]
 
     def get_icon(self, name):
         return {
@@ -176,47 +177,65 @@
             if periods:
                 raise PeriodSequenceError(
                     gettext('account.msg_period_same_sequence',
                         first=period.rec_name,
                         second=periods[0].rec_name))
 
     @classmethod
-    def find(cls, company_id, date=None, exception=True, test_state=True):
+    def find(cls, company, date=None, test_state=True):
         '''
-        Return the period for the company_id
-            at the date or the current date.
-        If exception is set the function will raise an exception
-            if no period is found.
-        If test_state is true, it will search on non-closed periods
+        Return the period for the company at the date or the current date
+        or raise PeriodNotFoundError.
+        If test_state is true, it searches on non-closed periods
         '''
         pool = Pool()
         Date = pool.get('ir.date')
         Lang = pool.get('ir.lang')
+        Company = pool.get('company.company')
 
+        company_id = int(company) if company is not None else None
         if not date:
             with Transaction().set_context(company=company_id):
                 date = Date.today()
-        clause = [
-            ('start_date', '<=', date),
-            ('end_date', '>=', date),
-            ('fiscalyear.company', '=', company_id),
-            ('type', '=', 'standard'),
-            ]
-        if test_state:
-            clause.append(('state', '=', 'open'))
-        periods = cls.search(clause, order=[('start_date', 'DESC')], limit=1)
-        if not periods:
-            if exception:
-                lang = Lang.get()
+        key = (company_id, date, test_state)
+        period = cls._find_cache.get(key, -1)
+        if period is not None and period < 0:
+            clause = [
+                ('start_date', '<=', date),
+                ('end_date', '>=', date),
+                ('fiscalyear.company', '=', company_id),
+                ('type', '=', 'standard'),
+                ]
+            periods = cls.search(
+                clause, order=[('start_date', 'DESC')], limit=1)
+            if periods:
+                period, = periods
+            else:
+                period = None
+            cls._find_cache.set(key, int(period) if period else None)
+        elif period is not None:
+            period = cls(period)
+        found = period and (not test_state or period.state == 'open')
+        if not found:
+            lang = Lang.get()
+            if company is not None and not isinstance(company, Company):
+                company = Company(company)
+            if not period:
                 raise PeriodNotFoundError(
                     gettext('account.msg_no_period_date',
-                        date=lang.strftime(date)))
+                        date=lang.strftime(date),
+                        company=company.rec_name if company else ''))
             else:
-                return None
-        return periods[0].id
+                raise PeriodNotFoundError(
+                    gettext('account.msg_no_open_period_date',
+                        date=lang.strftime(date),
+                        period=period.rec_name,
+                        company=company.rec_name if company else ''))
+        else:
+            return period
 
     @classmethod
     def _check(cls, periods):
         Move = Pool().get('account.move')
         moves = Move.search([
                 ('period', 'in', [p.id for p in periods]),
                 ], limit=1)
@@ -263,15 +282,17 @@
                 if fiscalyear.state != 'open':
                     raise AccessError(
                         gettext('account.msg_create_period_closed_fiscalyear',
                             fiscalyear=fiscalyear.rec_name))
                 if not vals.get('post_move_sequence'):
                     vals['post_move_sequence'] = (
                         fiscalyear.post_move_sequence.id)
-        return super(Period, cls).create(vlist)
+        periods = super(Period, cls).create(vlist)
+        cls._find_cache.clear()
+        return periods
 
     @classmethod
     def write(cls, *args):
         Move = Pool().get('account.move')
         actions = iter(args)
         args = []
         for periods, values in zip(actions, actions):
@@ -303,19 +324,21 @@
                                     ]):
                             raise AccessError(
                                 gettext('account'
                                     '.msg_change_period_post_move_sequence',
                                     period=period.rec_name))
             args.extend((periods, values))
         super(Period, cls).write(*args)
+        cls._find_cache.clear()
 
     @classmethod
     def delete(cls, periods):
         cls._check(periods)
         super(Period, cls).delete(periods)
+        cls._find_cache.clear()
 
     @classmethod
     @ModelView.button
     @Workflow.transition('close')
     def close(cls, periods):
         pool = Pool()
         JournalPeriod = pool.get('account.journal.period')
```

### Comparing `trytond_account-6.6.3/period.xml` & `trytond_account-6.8.0/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/setup.py` & `trytond_account-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
 name = 'trytond_account'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-dateutil', 'python-sql >= 0.7', 'simpleeval']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for accounting',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-account/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account',
     package_dir={'trytond.modules.account': '.'},
     packages=(
         ['trytond.modules.account']
         + ['trytond.modules.account.%s' % p for p in find_packages()]
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
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_account-6.6.3/tax.py` & `trytond_account-6.8.0/tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from collections import namedtuple
 from decimal import Decimal
-from itertools import groupby
+from itertools import cycle, groupby
 
 from sql import Literal
 from sql.aggregate import Sum
 from sql.conditionals import Case
 
 from trytond import backend
 from trytond.i18n import gettext
@@ -19,14 +19,15 @@
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If, PYSONEncoder
 from trytond.tools import cursor_dict, is_full_text, lstrip_wildcard
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateAction, StateView, Wizard
 
 from .common import ActivePeriodMixin, ContextCompanyMixin, PeriodMixin
+from .exceptions import PeriodNotFoundError
 
 KINDS = [
     ('sale', 'Sale'),
     ('purchase', 'Purchase'),
     ('both', 'Both'),
     ]
 
@@ -177,16 +178,15 @@
 
     @classmethod
     def default_template_override(cls):
         return False
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @classmethod
     def get_amount(cls, codes, name):
         result = {}
 
         parents = {}
         childs = cls.search([
@@ -553,39 +553,42 @@
     def default_method(cls):
         return 'period'
 
     @classmethod
     def default_period(cls):
         pool = Pool()
         Period = pool.get('account.period')
-        return Period.find(
-            cls.default_company(), exception=False, test_state=False)
+        try:
+            period = Period.find(cls.default_company(), test_state=False)
+        except PeriodNotFoundError:
+            return None
+        return period.id
 
     @fields.depends(
         'method', 'company',
         'fiscalyear', 'period', 'start_period', 'end_period')
     def on_change_with_periods(self):
         pool = Pool()
         Period = pool.get('account.period')
+        periods = []
         if self.method == 'fiscalyear' and self.fiscalyear:
-            return [
-                p.id for p in self.fiscalyear.periods if p.type == 'standard']
+            periods.extend(
+                p for p in self.fiscalyear.periods if p.type == 'standard')
         elif self.method == 'period' and self.period:
-            return [self.period.id]
+            periods.append(self.period)
         elif (self.method == 'periods'
                 and self.company
                 and self.start_period and self.end_period):
             periods = Period.search([
                     ('start_date', '>=', self.start_period.start_date),
                     ('start_date', '<=', self.end_period.start_date),
                     ('company', '=', self.company.id),
                     ('type', '=', 'standard'),
                     ])
-            return [p.id for p in periods]
-        return []
+        return periods
 
 
 class TaxTemplate(sequence_ordered(), ModelSQL, ModelView, DeactivableMixin):
     'Account Tax Template'
     __name__ = 'account.tax.template'
     name = fields.Char('Name', required=True)
     description = fields.Char('Description', required=True)
@@ -968,16 +971,15 @@
     def _amount_domain(cls):
         context = Transaction().context
         periods = context.get('periods', [])
         return [('move_line.move.period', 'in', periods)]
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @classmethod
     def copy(cls, taxes, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
@@ -1244,16 +1246,31 @@
         line['account'] = getattr(tax, '%s_account' % type_).id
 
         return _TaxKey(**line)
 
     def _round_taxes(self, taxes):
         if not self.currency:
             return
+
+        remainder = 0
         for taxline in taxes.values():
-            taxline['amount'] = self.currency.round(taxline['amount'])
+            rounded_amount = self.currency.round(taxline['amount'])
+            remainder += rounded_amount - taxline['amount']
+            taxline['amount'] = rounded_amount
+
+        # We need to compensate the rounding we did
+        remainder = self.currency.round(remainder, opposite=True)
+        if abs(remainder) >= self.currency.rounding:
+            offset_amount = self.currency.rounding.copy_sign(remainder)
+
+            for tax in cycle(taxes.values()):
+                tax['amount'] -= offset_amount
+                remainder -= offset_amount
+                if abs(remainder) < self.currency.rounding:
+                    break
 
     @fields.depends('company', methods=['_get_tax_context', '_round_taxes'])
     def _get_taxes(self):
         pool = Pool()
         Tax = pool.get('account.tax')
         Configuration = pool.get('account.configuration')
 
@@ -1263,27 +1280,29 @@
             tax_rounding = config.get_multivalue('tax_rounding')
             taxable_lines = [_TaxableLine(*params)
                 for params in self.taxable_lines]
             for line in taxable_lines:
                 assert all(t.company == self.company for t in line.taxes)
                 l_taxes = Tax.compute(Tax.browse(line.taxes), line.unit_price,
                     line.quantity, line.tax_date or self.tax_date)
+                current_taxes = {}
                 for tax in l_taxes:
                     taxline = self._compute_tax_line(**tax)
                     # Base must always be rounded per line as there will be one
                     # tax line per taxable_lines
                     if self.currency:
                         taxline['base'] = self.currency.round(taxline['base'])
                     if taxline not in taxes:
                         taxes[taxline] = taxline
                     else:
                         taxes[taxline]['base'] += taxline['base']
                         taxes[taxline]['amount'] += taxline['amount']
+                    current_taxes[taxline] = taxes[taxline]
                 if tax_rounding == 'line':
-                    self._round_taxes(taxes)
+                    self._round_taxes(current_taxes)
         if tax_rounding == 'document':
             self._round_taxes(taxes)
         return taxes
 
 
 class TaxLine(ModelSQL, ModelView):
     'Tax Line'
@@ -1351,21 +1370,20 @@
                         [table.type], ['base'],
                         where=(table.tax == tax)
                         & (table.code.in_(
                                 [invoice_base_code, credit_note_base_code]))))
 
     @fields.depends('move_line', '_parent_move_line.currency')
     def on_change_with_currency(self, name=None):
-        if self.move_line and self.move_line.currency:
-            return self.move_line.currency.id
+        return self.move_line.currency if self.move_line else None
 
     @fields.depends('_parent_move_line.account', 'move_line')
     def on_change_with_company(self, name=None):
         if self.move_line and self.move_line.account:
-            return self.move_line.account.company.id
+            return self.move_line.account.company
 
     def get_rec_name(self, name):
         name = super(TaxLine, self).get_rec_name(name)
         if self.tax:
             name = self.tax.rec_name
         return name
```

### Comparing `trytond_account-6.6.3/tax.xml` & `trytond_account-6.8.0/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_account_active.rst` & `trytond_account-6.8.0/tests/scenario_account_active.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_account_reconcile.rst` & `trytond_account-6.8.0/tests/scenario_account_reconcile.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-6.8.0/tests/scenario_account_reconcile_automatic.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_close_fiscalyear.rst` & `trytond_account-6.8.0/tests/scenario_close_fiscalyear.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 =================================
 Account Close Fiscalyear Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from dateutil.relativedelta import relativedelta
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
     >>> from trytond.modules.currency.tests.tools import get_currency
 
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
     >>> last_year = today - relativedelta(years=1)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
     >>> Account = Model.get('account.account')
```

### Comparing `trytond_account-6.6.3/tests/scenario_move_cancel.rst` & `trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,111 @@
-====================
-Move Cancel Scenario
-====================
+=========================================
+Account Reconciliation Alternate Currency
+=========================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> today = datetime.date.today()
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_fiscalyear, create_chart, get_accounts)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
+    >>> Configuration = Model.get('account.configuration')
+    >>> Journal = Model.get('account.journal')
+    >>> Move = Model.get('account.move')
+    >>> Party = Model.get('party.party')
+    >>> Reconciliation = Model.get('account.move.reconciliation')
+
+Create currencies::
+
+    >>> usd = get_currency('USD')
+    >>> eur = get_currency('EUR')
+
 Create company::
 
-    >>> _ = create_company()
-    >>> company = get_company()
+    >>> _ = create_company(currency=usd)
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear()
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
 
 Create chart of accounts::
 
-    >>> _ = create_chart(company)
-    >>> accounts = get_accounts(company)
-    >>> receivable = accounts['receivable']
-    >>> revenue = accounts['revenue']
+    >>> _ = create_chart()
+    >>> accounts = get_accounts()
 
-Create parties::
+Configure currency exchange::
 
-    >>> Party = Model.get('party.party')
-    >>> customer = Party(name='Customer')
-    >>> customer.save()
-    >>> party = Party(name='Party')
+    >>> currency_exchange_account, = (
+    ...     accounts['revenue'].duplicate(
+    ...         default={'name': "Currency Exchange"}))
+    >>> configuration = Configuration(1)
+    >>> configuration.currency_exchange_credit_account = (
+    ...     currency_exchange_account)
+    >>> configuration.save()
+
+Create party::
+
+    >>> party = Party(name="Party")
     >>> party.save()
 
-Create Move to cancel::
+Create moves to reconcile::
+
+    >>> journal_expense, = Journal.find([('code', '=', 'EXP')])
+    >>> journal_cash, = Journal.find([('code', '=', 'CASH')])
 
-    >>> Journal = Model.get('account.journal')
-    >>> Move = Model.get('account.move')
-    >>> journal_revenue, = Journal.find([
-    ...         ('code', '=', 'REV'),
-    ...         ])
-    >>> journal_cash, = Journal.find([
-    ...         ('code', '=', 'CASH'),
-    ...         ])
     >>> move = Move()
     >>> move.period = period
-    >>> move.journal = journal_revenue
+    >>> move.journal = journal_expense
     >>> move.date = period.start_date
     >>> line = move.lines.new()
-    >>> line.account = revenue
-    >>> line.credit = Decimal(42)
+    >>> line.account = accounts['expense']
+    >>> line.debit = Decimal('50.00')
     >>> line = move.lines.new()
-    >>> line.account = receivable
-    >>> line.debit = Decimal(32)
-    >>> line.party = customer
-    >>> line.second_currency = get_currency('EUR')
-    >>> line.amount_second_currency = Decimal(30)
+    >>> line.account = accounts['payable']
+    >>> line.party = party
+    >>> line.credit = Decimal('50.00')
+    >>> line.amount_second_currency = Decimal('-90.00')
+    >>> line.second_currency = eur
+    >>> move.save()
+    >>> reconcile1, = [l for l in move.lines if l.account == accounts['payable']]
+
+    >>> move = Move()
+    >>> move.period = period
+    >>> move.journal = journal_cash
+    >>> move.date = period.end_date
     >>> line = move.lines.new()
-    >>> line.account = receivable
-    >>> line.debit = Decimal(10)
+    >>> line.account = accounts['cash']
+    >>> line.credit = Decimal('45.00')
+    >>> line = move.lines.new()
+    >>> line.account = accounts['payable']
     >>> line.party = party
+    >>> line.debit = Decimal('45.00')
+    >>> line.amount_second_currency = Decimal('-90.00')
+    >>> line.second_currency = eur
     >>> move.save()
-    >>> revenue.reload()
-    >>> revenue.credit
-    Decimal('42.00')
-    >>> receivable.reload()
-    >>> receivable.debit
-    Decimal('42.00')
-
-Cancel Move::
-
-    >>> cancel_move = Wizard('account.move.cancel', [move])
-    >>> cancel_move.form.description = 'Cancel'
-    >>> cancel_move.execute('cancel')
-    >>> cancel_move.state
+    >>> reconcile2, = [l for l in move.lines if l.account == accounts['payable']]
+
+Reconcile lines::
+
+    >>> reconcile_lines = Wizard(
+    ...     'account.move.reconcile_lines', [reconcile1, reconcile2])
+    >>> reconcile_lines.state
     'end'
-    >>> move.reload()
-    >>> [bool(l.reconciliation) for l in move.lines if l.account == receivable]
-    [True, True]
-    >>> line, _ = [l for l in move.lines if l.account == receivable]
-    >>> cancel_move, = [l.move for l in line.reconciliation.lines
-    ...     if l.move != move]
-    >>> cancel_move.origin == move
-    True
-    >>> cancel_move.description
-    'Cancel'
-    >>> sorted([l.origin.id for l in cancel_move.lines]) == \
-    ...     sorted(map(int, move.lines))
+
+    >>> reconcile1.reconciliation == reconcile2.reconciliation != None
     True
-    >>> revenue.reload()
-    >>> revenue.credit
-    Decimal('0.00')
-    >>> receivable.reload()
-    >>> receivable.debit
-    Decimal('0.00')
+    >>> reconciliation, = Reconciliation.find([])
+    >>> len(reconciliation.lines)
+    3
+    >>> currency_exchange_account.reload()
+    >>> currency_exchange_account.balance
+    Decimal('-5.00')
```

### Comparing `trytond_account-6.6.3/tests/scenario_move_line_delegate.rst` & `trytond_account-6.8.0/tests/scenario_move_line_delegate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_move_line_group.rst` & `trytond_account-6.8.0/tests/scenario_move_line_group.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_move_line_reschedule.rst` & `trytond_account-6.8.0/tests/scenario_move_line_reschedule.rst`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     True
     >>> term3.date == period.end_date + relativedelta(months=2)
     True
     >>> term1.amount, term2.amount, term3.amount
     (Decimal('33.33'), Decimal('33.33'), Decimal('33.34'))
     >>> term1.amount = Decimal('40.00')
     >>> term2.amount = term3.amount = Decimal('30.00')
-    >>> term3.date += relativedelta(months=1)
+    >>> term3.date = period.end_date + relativedelta(months=3)
 
     >>> reschedule.execute('reschedule')
     >>> reschedule_move, = reschedule.actions[0]
     >>> reschedule_move.description
     'Split 3 months'
 
 Check receivable::
```

### Comparing `trytond_account-6.6.3/tests/scenario_move_template.rst` & `trytond_account-6.8.0/tests/scenario_move_template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/tests/scenario_renew_fiscalyear.rst` & `trytond_account-6.8.0/tests/scenario_renew_fiscalyear.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 =================================
 Account Renew Fiscalyear Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
-    >>> today = datetime.date.today()
-    >>> end_year = today + relativedelta(month=12, day=31)
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
 
@@ -26,16 +22,16 @@
 
 Create fiscal year::
 
     >>> fiscalyear = create_fiscalyear(company)
     >>> fiscalyear.click('create_period')
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
@@ -60,19 +56,19 @@
     >>> new_fiscalyear, = renew_fiscalyear.actions[0]
     >>> int(new_fiscalyear.post_move_sequence.number_next)
     1
 
 Set the sequence name::
 
     >>> sequence = new_fiscalyear.post_move_sequence
-    >>> sequence.name = 'Sequence %s' % new_fiscalyear.start_date.strftime('%Y')
+    >>> sequence.name = 'Sequence %s' % new_fiscalyear.name
     >>> sequence.save()
 
 Renew fiscalyear and test sequence name is updated::
 
     >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
     >>> renew_fiscalyear.form.reset_sequences = True
     >>> renew_fiscalyear.execute('create_')
     >>> new_fiscalyear, = renew_fiscalyear.actions[0]
     >>> new_fiscalyear.post_move_sequence.name == (
-    ...     'Sequence %s' % new_fiscalyear.start_date.strftime('%Y'))
+    ...     'Sequence %s' % new_fiscalyear.name)
     True
```

### Comparing `trytond_account-6.6.3/tests/scenario_reports.rst` & `trytond_account-6.8.0/tests/scenario_reports.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 ========================
 Account Reports Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear.click('create_period')
     >>> periods = fiscalyear.periods
     >>> period_1, period_3, period_5 = periods[0], periods[2], periods[4]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
```

### Comparing `trytond_account-6.6.3/tests/scenario_tax_code.rst` & `trytond_account-6.8.0/tests/scenario_tax_code.rst`

 * *Files 14% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     >>> tax_line.type = 'tax'
     >>> tax_line.tax = tax
     >>> move.save()
 
     >>> _ = move.duplicate()
 
     >>> cancel_move = Wizard('account.move.cancel', [move])
+    >>> cancel_move.form.reversal = False
     >>> cancel_move.execute('cancel')
 
 Check tax code::
 
     >>> TaxCode = Model.get('account.tax.code')
 
     >>> with config.set_context(periods=[period.id]):
```

### Comparing `trytond_account-6.6.3/tests/test_module.py` & `trytond_account-6.8.0/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from trytond.modules.account.exceptions import FiscalYearDatesError
 from trytond.modules.account.tax import TaxableMixin
 from trytond.modules.company.tests import (
     CompanyTestMixin, PartyCompanyCheckEraseMixin, create_company, set_company)
 from trytond.modules.currency.tests import create_currency
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 
 def create_chart(company, tax=False, chart='account.account_template_root_en'):
     pool = Pool()
     AccountTemplate = pool.get('account.account.template')
     TaxTemplate = pool.get('account.tax.template')
     TaxCodeTemplate = pool.get('account.tax.code.template')
@@ -651,14 +651,30 @@
                 ]
             move.save()
             Move.post([move])
             move_id = move.id
 
             self.assertEqual(move.state, 'posted')
 
+            # Move lines with debit = credit = 0 are automatically reconciled
+            move = Move()
+            move.period = period
+            move.journal = journal_revenue
+            move.date = period.start_date
+            move.lines = [
+                Line(account=revenue, credit=Decimal(0)),
+                Line(account=receivable, debit=Decimal(0), party=party),
+                ]
+            move.save()
+            Move.post([move])
+
+            lines = Line.browse([l.id for l in move.lines
+                    if l.account.reconcile])
+            self.assertTrue(all(bool(l.reconciliation) for l in lines))
+
             # Can not post an empty move
             with self.assertRaises(UserError):
                 move = Move()
                 move.period = period
                 move.journal = journal_revenue
                 move.date = period.start_date
                 move.save()
@@ -1150,14 +1166,116 @@
             taxes = taxable._get_taxes()
 
         tax, = taxes
         self.assertEqual(tax['base'], Decimal('100.00'))
         self.assertEqual(tax['amount'], Decimal('20.02'))
 
     @with_transaction()
+    def test_taxable_mixin_tax_residual_rounding(self):
+        "Test TaxableMixin for rounding with residual amount"
+        pool = Pool()
+        Account = pool.get('account.account')
+        Tax = pool.get('account.tax')
+        Configuration = pool.get('account.configuration')
+        currency = create_currency('cur')
+
+        company = create_company()
+        with set_company(company):
+            create_chart(company)
+
+            config = Configuration(1)
+            config.tax_rounding = 'line'
+            config.save()
+
+            tax_account, = Account.search([
+                    ('name', '=', 'Main Tax'),
+                    ])
+
+            tax1 = Tax()
+            tax1.name = tax1.description = "Tax 1"
+            tax1.type = 'percentage'
+            tax1.rate = Decimal('.1')
+            tax1.invoice_account = tax_account
+            tax1.credit_note_account = tax_account
+            tax1.save()
+            tax2 = Tax()
+            tax2.name = tax2.description = "Tax 2"
+            tax2.type = 'percentage'
+            tax2.rate = Decimal('.1')
+            tax2.invoice_account = tax_account
+            tax2.credit_note_account = tax_account
+            tax2.save()
+
+            taxable = self.Taxable(
+                currency=currency,
+                taxable_lines=[
+                    ([tax1, tax2], Decimal('1.0417'), 1, None),
+                    ],
+                company=company)
+
+            taxline_1, taxline_2 = taxable._get_taxes()
+            self.assertEqual(taxline_1['base'], Decimal('1.04'))
+            self.assertEqual(taxline_1['amount'], Decimal('.11'))
+            self.assertEqual(taxline_2['base'], Decimal('1.04'))
+            self.assertEqual(taxline_2['amount'], Decimal('.10'))
+
+    @with_transaction()
+    def test_taxable_mixin_tax_residual_rounding_negative_residual(self):
+        "Test TaxableMixin for rounding with negative residual amount"
+        pool = Pool()
+        Account = pool.get('account.account')
+        Tax = pool.get('account.tax')
+        Configuration = pool.get('account.configuration')
+        currency = create_currency('cur')
+
+        company = create_company()
+        with set_company(company):
+            create_chart(company)
+
+            config = Configuration(1)
+            config.tax_rounding = 'line'
+            config.save()
+
+            tax_account, = Account.search([
+                    ('name', '=', 'Main Tax'),
+                    ])
+
+            tax1 = Tax()
+            tax1.name = tax1.description = "Tax 1"
+            tax1.type = 'percentage'
+            tax1.rate = Decimal('.1')
+            tax1.invoice_account = tax_account
+            tax1.credit_note_account = tax_account
+            tax1.save()
+            tax2 = Tax()
+            tax2.name = tax2.description = "Tax 2"
+            tax2.type = 'percentage'
+            tax2.rate = Decimal('.1')
+            tax2.invoice_account = tax_account
+            tax2.credit_note_account = tax_account
+            tax2.save()
+
+            # -2.95 is the unit price of -3.54 with 20% tax included
+            taxable = self.Taxable(
+                currency=currency,
+                taxable_lines=[
+                    ([tax1], Decimal('30.00'), 1, None),
+                    ([tax1, tax2], Decimal('-2.95'), 1, None),
+                    ],
+                company=company)
+
+            taxline_1, taxline_2, taxline_3 = taxable._get_taxes()
+            self.assertEqual(taxline_1['base'], Decimal('30.00'))
+            self.assertEqual(taxline_1['amount'], Decimal('3.00'))
+            self.assertEqual(taxline_2['base'], Decimal('-2.95'))
+            self.assertEqual(taxline_2['amount'], Decimal('-0.29'))
+            self.assertEqual(taxline_3['base'], Decimal('-2.95'))
+            self.assertEqual(taxline_3['amount'], Decimal('-0.30'))
+
+    @with_transaction()
     def test_tax_compute_with_children_update_unit_price(self):
         "Test tax compute with children taxes modifying unit_price"
         pool = Pool()
         Account = pool.get('account.account')
         Date = pool.get('ir.date')
         Tax = pool.get('account.tax')
         today = Date.today()
@@ -1539,15 +1657,15 @@
                     tax.credit_note_account.template,
                     tax.template.credit_note_account)
 
         company = create_company()
         with set_company(company):
             create_chart(company, True)
 
-            with Transaction().set_context(active_test=False):
+            with inactive_records():
                 self.assertEqual(Type.search([], count=True), 16)
                 self.assertEqual(Account.search([], count=True), 7)
                 self.assertEqual(Tax.search([], count=True), 1)
 
                 check()
 
         with Transaction().set_user(0):
@@ -1611,15 +1729,15 @@
         with set_company(company):
             account, = Account.search([('parent', '=', None)])
             session_id, _, _ = UpdateChart.create()
             update_chart = UpdateChart(session_id)
             update_chart.start.account = account
             update_chart.transition_update()
 
-            with Transaction().set_context(active_test=False):
+            with inactive_records():
                 self.assertEqual(Type.search([], count=True), 17)
                 self.assertEqual(Account.search([], count=True), 8)
                 self.assertEqual(Tax.search([], count=True), 2)
 
                 check()
 
     @with_transaction()
@@ -1734,14 +1852,14 @@
             self.assertFalse(cash.active)
 
             session_id, _, _ = UpdateChart.create()
             update_chart = UpdateChart(session_id)
             update_chart.start.account = root
             update_chart.transition_update()
 
-            with Transaction().set_context(active_test=False):
+            with inactive_records():
                 self.assertEqual(
                     Account.search([('name', '=', 'Main Cash')], count=True),
                     1)
 
 
 del ModuleTestCase
```

### Comparing `trytond_account-6.6.3/tests/tools.py` & `trytond_account-6.8.0/tests/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 
 from dateutil.relativedelta import relativedelta
-from proteus import Model, Wizard
 
+from proteus import Model, Wizard
 from trytond.modules.company.tests.tools import get_company
 
 __all__ = ['create_fiscalyear', 'create_chart', 'get_accounts',
     'create_tax', 'create_tax_code']
 
 
 def create_fiscalyear(company=None, today=None, config=None):
-    "Create a fiscal year for the company on today"
+    "Create a fiscal year for the company on today or range"
     FiscalYear = Model.get('account.fiscalyear', config=config)
     Sequence = Model.get('ir.sequence', config=config)
     SequenceType = Model.get('ir.sequence.type', config=config)
 
     if not company:
         company = get_company(config=config)
 
     if not today:
         today = datetime.date.today()
+    if isinstance(today, datetime.date):
+        start_date = end_date = today
+    else:
+        start_date, end_date = today
+        today = start_date + (end_date - start_date) / 2
+    start_date = min(start_date, today - relativedelta(months=6, day=1))
+    end_date = max(end_date, today + relativedelta(months=5, day=31))
+    assert start_date <= end_date
 
     fiscalyear = FiscalYear(name=str(today.year))
-    fiscalyear.start_date = today + relativedelta(month=1, day=1)
-    fiscalyear.end_date = today + relativedelta(month=12, day=31)
+    fiscalyear.start_date = start_date
+    fiscalyear.end_date = end_date
     fiscalyear.company = company
 
     sequence_type, = SequenceType.find(
         [('name', '=', "Account Move")], limit=1)
     post_move_sequence = Sequence(
         name=str(today.year),
         sequence_type=sequence_type,
@@ -81,28 +89,31 @@
 
     accounts = {}
     for type in ['receivable', 'payable', 'revenue', 'expense']:
         try:
             accounts[type], = Account.find([
                     ('type.%s' % type, '=', True),
                     ('company', '=', company.id),
+                    ('closed', '!=', True),
                     ], limit=1)
         except ValueError:
             pass
     try:
         accounts['cash'], = Account.find([
                 ('company', '=', company.id),
                 ('name', '=', 'Main Cash'),
+                ('closed', '!=', True),
                 ], limit=1)
     except ValueError:
         pass
     try:
         accounts['tax'], = Account.find([
                 ('company', '=', company.id),
                 ('name', '=', 'Main Tax'),
+                ('closed', '!=', True),
                 ], limit=1)
     except ValueError:
         pass
     return accounts
 
 
 def create_tax(rate, company=None, config=None):
```

### Comparing `trytond_account-6.6.3/trial_balance.fodt` & `trytond_account-6.8.0/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/trytond_account.egg-info/PKG-INFO` & `trytond_account-6.8.0/trytond_account.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account
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
 
 ##############
 Account Module
 ##############
```

### Comparing `trytond_account-6.6.3/trytond_account.egg-info/SOURCES.txt` & `trytond_account-6.8.0/trytond_account.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_account_active.rst
 ./tests/scenario_account_reconcile.rst
 ./tests/scenario_account_reconcile_automatic.rst
 ./tests/scenario_account_reconciliation.rst
+./tests/scenario_account_reconciliation_alternate_currency.rst
+./tests/scenario_account_reconciliation_alternate_currency_write_off.rst
 ./tests/scenario_close_fiscalyear.rst
 ./tests/scenario_move_cancel.rst
 ./tests/scenario_move_line_delegate.rst
 ./tests/scenario_move_line_group.rst
 ./tests/scenario_move_line_reschedule.rst
 ./tests/scenario_move_template.rst
 ./tests/scenario_renew_fiscalyear.rst
@@ -178,14 +180,16 @@
 ./view/move_cancel_default_form.xml
 ./view/move_form.xml
 ./view/move_line_delegate_start_form.xml
 ./view/move_line_form.xml
 ./view/move_line_form_move.xml
 ./view/move_line_group_start_form.xml
 ./view/move_line_list_payable_receivable.xml
+./view/move_line_list_reconcile.xml
+./view/move_line_receivable_payable_context_form.xml
 ./view/move_line_reschedule_preview_form.xml
 ./view/move_line_reschedule_start_form.xml
 ./view/move_line_reschedule_term_list.xml
 ./view/move_line_template_form.xml
 ./view/move_line_template_list.xml
 ./view/move_line_tree.xml
 ./view/move_line_tree_move.xml
@@ -295,14 +299,16 @@
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_account_active.rst
 tests/scenario_account_reconcile.rst
 tests/scenario_account_reconcile_automatic.rst
 tests/scenario_account_reconciliation.rst
+tests/scenario_account_reconciliation_alternate_currency.rst
+tests/scenario_account_reconciliation_alternate_currency_write_off.rst
 tests/scenario_close_fiscalyear.rst
 tests/scenario_move_cancel.rst
 tests/scenario_move_line_delegate.rst
 tests/scenario_move_line_group.rst
 tests/scenario_move_line_reschedule.rst
 tests/scenario_move_template.rst
 tests/scenario_renew_fiscalyear.rst
@@ -366,14 +372,16 @@
 view/move_cancel_default_form.xml
 view/move_form.xml
 view/move_line_delegate_start_form.xml
 view/move_line_form.xml
 view/move_line_form_move.xml
 view/move_line_group_start_form.xml
 view/move_line_list_payable_receivable.xml
+view/move_line_list_reconcile.xml
+view/move_line_receivable_payable_context_form.xml
 view/move_line_reschedule_preview_form.xml
 view/move_line_reschedule_start_form.xml
 view/move_line_reschedule_term_list.xml
 view/move_line_template_form.xml
 view/move_line_template_list.xml
 view/move_line_tree.xml
 view/move_line_tree_move.xml
```

### Comparing `trytond_account-6.6.3/type_statement.fodt` & `trytond_account-6.8.0/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/account_deferral_form.xml` & `trytond_account-6.8.0/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/account_form.xml` & `trytond_account-6.8.0/view/account_type_form.xml`

 * *Files 17% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/account_form.xml` & `trytond_account-6.8.0/view/account_type_form.xml`

```diff
@@ -1,60 +1,36 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form col="6">
   <label name="name"/>
   <field name="name"/>
-  <label name="code"/>
-  <field name="code"/>
-  <group col="-1" colspan="2" id="checkboxes">
-    <label name="active"/>
-    <field name="active" xexpand="0" width="100"/>
-    <label name="template_override"/>
-    <field name="template_override" xexpand="0" width="100"/>
+  <label name="company"/>
+  <field name="company"/>
+  <label name="sequence"/>
+  <field name="sequence"/>
+  <label name="statement"/>
+  <group col="-1" id="statement">
+    <field name="statement"/>
+    <label name="assets"/>
+    <field name="assets"/>
   </group>
-  <notebook colspan="6">
-    <page string="General Information" id="general" col="6">
-      <label name="company"/>
-      <field name="company"/>
-      <label name="parent"/>
-      <field name="parent"/>
-      <newline/>
-      <label name="type"/>
-      <field name="type" colspan="5"/>
-      <label name="debit_type"/>
-      <field name="debit_type" colspan="5"/>
-      <label name="credit_type"/>
-      <field name="credit_type" colspan="5"/>
-      <label name="closed"/>
-      <field name="closed"/>
-      <label name="general_ledger_balance"/>
-      <field name="general_ledger_balance"/>
-      <newline/>
-      <label name="start_date"/>
-      <field name="start_date"/>
-      <label name="end_date"/>
-      <field name="end_date"/>
-      <label name="replaced_by"/>
-      <field name="replaced_by"/>
-      <label name="currency"/>
-      <field name="currency"/>
-      <label name="second_currency"/>
-      <field name="second_currency"/>
-      <newline/>
-      <label name="reconcile"/>
-      <field name="reconcile"/>
-      <label name="party_required"/>
-      <field name="party_required"/>
-      <field name="taxes" colspan="6"/>
-    </page>
-    <page string="Children" id="children">
-      <field name="childs" colspan="4"/>
-    </page>
-    <page name="deferrals">
-      <field name="deferrals"/>
-    </page>
-    <page name="note">
-      <field name="note"/>
-    </page>
-  </notebook>
+  <label name="parent"/>
+  <field name="parent"/>
+  <label name="template_override"/>
+  <field name="template_override"/>
+  <group colspan="6" col="-1" id="checkboxes">
+    <label name="receivable"/>
+    <field name="receivable" xexpand="0" width="25"/>
+    <label name="stock"/>
+    <field name="stock" xexpand="0" width="25"/>
+    <label name="payable"/>
+    <field name="payable" xexpand="0" width="25"/>
+    <label name="debt"/>
+    <field name="debt" xexpand="0" width="25"/>
+    <label name="revenue"/>
+    <field name="revenue" xexpand="0" width="25"/>
+    <label name="expense"/>
+    <field name="expense" xexpand="0" width="25"/>
+  </group>
+  <field name="childs" colspan="6"/>
 </form>
```

### Comparing `trytond_account-6.6.3/view/account_template_form.xml` & `trytond_account-6.8.0/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/account_type_form.xml` & `trytond_account-6.8.0/view/account_type_template_form.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/account_type_form.xml` & `trytond_account-6.8.0/view/account_type_template_form.xml`

```diff
@@ -1,36 +1,31 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="6">
+<form>
   <label name="name"/>
   <field name="name"/>
-  <label name="company"/>
-  <field name="company"/>
   <label name="sequence"/>
   <field name="sequence"/>
   <label name="statement"/>
   <group col="-1" id="statement">
     <field name="statement"/>
     <label name="assets"/>
     <field name="assets"/>
   </group>
   <label name="parent"/>
   <field name="parent"/>
-  <label name="template_override"/>
-  <field name="template_override"/>
-  <group colspan="6" col="-1" id="checkboxes">
+  <group colspan="4" col="-1" id="checkboxes">
     <label name="receivable"/>
     <field name="receivable" xexpand="0" width="25"/>
     <label name="stock"/>
     <field name="stock" xexpand="0" width="25"/>
     <label name="payable"/>
     <field name="payable" xexpand="0" width="25"/>
     <label name="debt"/>
     <field name="debt" xexpand="0" width="25"/>
     <label name="revenue"/>
     <field name="revenue" xexpand="0" width="25"/>
     <label name="expense"/>
     <field name="expense" xexpand="0" width="25"/>
   </group>
-  <field name="childs" colspan="6"/>
 </form>
```

### Comparing `trytond_account-6.6.3/view/aged_balance_context_form.xml` & `trytond_account-6.8.0/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/configuration_form.xml` & `trytond_account-6.8.0/view/move_line_template_form.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/configuration_form.xml` & `trytond_account-6.8.0/view/move_line_template_form.xml`

```diff
@@ -1,20 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
-  <separator id="party" string="Party" colspan="4"/>
-  <label name="default_account_receivable"/>
-  <field name="default_account_receivable"/>
-  <label name="default_account_payable"/>
-  <field name="default_account_payable"/>
-  <separator id="invoice" string="Invoice" colspan="4"/>
-  <label name="default_customer_tax_rule"/>
-  <field name="default_customer_tax_rule"/>
-  <label name="default_supplier_tax_rule"/>
-  <field name="default_supplier_tax_rule"/>
-  <label name="tax_rounding"/>
-  <field name="tax_rounding"/>
-  <separator id="move" string="Move" colspan="4"/>
-  <label name="reconciliation_sequence"/>
-  <field name="reconciliation_sequence"/>
+  <label name="account"/>
+  <field name="account"/>
+  <label name="move"/>
+  <field name="move"/>
+  <label name="operation"/>
+  <field name="operation"/>
+  <label name="amount"/>
+  <field name="amount"/>
+  <label name="description"/>
+  <field name="description" colspan="3"/>
+  <notebook colspan="4">
+    <page string="Other Info" id="info">
+      <label name="party"/>
+      <field name="party"/>
+    </page>
+    <page name="taxes">
+      <field name="taxes" colspan="4"/>
+    </page>
+  </notebook>
 </form>
```

### Comparing `trytond_account-6.6.3/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-6.8.0/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/fiscalyear_form.xml` & `trytond_account-6.8.0/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/general_ledger_account_context_form.xml` & `trytond_account-6.8.0/view/general_ledger_account_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/general_ledger_account_list.xml` & `trytond_account-6.8.0/view/general_ledger_account_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/general_ledger_line_list.xml` & `trytond_account-6.8.0/view/general_ledger_line_list.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/general_ledger_line_list.xml` & `trytond_account-6.8.0/view/general_ledger_line_list.xml`

```diff
@@ -9,9 +9,10 @@
   <field name="description" expand="1" optional="1"/>
   <field name="move_description" expand="1" optional="1"/>
   <field name="origin" optional="1"/>
   <field name="reconciliation" optional="1"/>
   <field name="state" optional="1"/>
   <field name="debit" sum="Debit" optional="0"/>
   <field name="credit" sum="Credit" optional="0"/>
+  <field name="amount_second_currency" optional="1"/>
   <field name="balance" optional="0"/>
 </tree>
```

### Comparing `trytond_account-6.6.3/view/income_statement_context_form.xml` & `trytond_account-6.8.0/view/income_statement_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_form.xml` & `trytond_account-6.8.0/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_line_form.xml` & `trytond_account-6.8.0/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_line_form_move.xml` & `trytond_account-6.8.0/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_line_list_payable_receivable.xml` & `trytond_account-6.8.0/view/move_line_list_payable_receivable.xml`

 * *Files 13% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/move_line_list_payable_receivable.xml` & `trytond_account-6.8.0/view/move_line_list_payable_receivable.xml`

```diff
@@ -2,14 +2,15 @@
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tree>
   <field name="company" expand="1" optional="1"/>
   <field name="maturity_date"/>
   <field name="party"/>
   <field name="amount"/>
+  <field name="payable_receivable_balance" string="Balance"/>
   <field name="move" optional="1"/>
   <field name="move_origin" optional="1"/>
   <field name="origin" optional="1"/>
   <field name="move_description" optional="1"/>
   <field name="description" optional="1"/>
   <field name="reconciliation" optional="1"/>
 </tree>
```

### Comparing `trytond_account-6.6.3/view/move_line_reschedule_start_form.xml` & `trytond_account-6.8.0/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_line_template_form.xml` & `trytond_account-6.8.0/view/tax_code_template_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/move_line_template_form.xml` & `trytond_account-6.8.0/view/tax_code_template_form.xml`

```diff
@@ -1,24 +1,28 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
+  <label name="name"/>
+  <field name="name"/>
+  <label name="code"/>
+  <field name="code"/>
   <label name="account"/>
   <field name="account"/>
-  <label name="move"/>
-  <field name="move"/>
-  <label name="operation"/>
-  <field name="operation"/>
-  <label name="amount"/>
-  <field name="amount"/>
-  <label name="description"/>
-  <field name="description" colspan="3"/>
+  <label name="parent"/>
+  <field name="parent"/>
+  <label name="start_date"/>
+  <field name="start_date"/>
+  <label name="end_date"/>
+  <field name="end_date"/>
   <notebook colspan="4">
-    <page string="Other Info" id="info">
-      <label name="party"/>
-      <field name="party"/>
+    <page name="lines">
+      <field name="lines" colspan="4"/>
     </page>
-    <page name="taxes">
-      <field name="taxes" colspan="4"/>
+    <page name="childs">
+      <field name="childs" colspan="4"/>
+    </page>
+    <page name="description">
+      <field name="description" colspan="4"/>
     </page>
   </notebook>
 </form>
```

### Comparing `trytond_account-6.6.3/view/move_line_tree.xml` & `trytond_account-6.8.0/view/move_line_tree.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/move_line_tree.xml` & `trytond_account-6.8.0/view/move_line_tree.xml`

```diff
@@ -7,14 +7,16 @@
   <field name="move_origin" expand="1" optional="1"/>
   <field name="origin" expand="1" optional="1"/>
   <field name="date"/>
   <field name="account" expand="1"/>
   <field name="party" expand="1"/>
   <field name="debit" sum="Debit"/>
   <field name="credit" sum="Credit"/>
+  <field name="amount_second_currency" symbol="" optional="1"/>
+  <field name="second_currency" optional="1"/>
   <field name="delegated_amount" optional="0"/>
   <field name="tax_lines" optional="1"/>
   <field name="description" expand="1" optional="1"/>
   <field name="move_description" expand="1" optional="1"/>
   <field name="reconciliation" optional="1"/>
   <field name="state"/>
   <field name="move_state" optional="0"/>
```

### Comparing `trytond_account-6.6.3/view/move_line_tree_move.xml` & `trytond_account-6.8.0/view/move_line_tree_move.xml`

 * *Files 21% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/move_line_tree_move.xml` & `trytond_account-6.8.0/view/move_line_tree_move.xml`

```diff
@@ -3,11 +3,13 @@
 this repository contains the full copyright notices and license terms. -->
 <tree editable="1">
   <field name="move"/>
   <field name="account" expand="1"/>
   <field name="party" expand="1"/>
   <field name="debit" sum="Debit"/>
   <field name="credit" sum="Credit"/>
+  <field name="amount_second_currency" symbol="" optional="1"/>
+  <field name="second_currency" optional="1"/>
   <field name="tax_lines" optional="1"/>
   <field name="description" expand="1" optional="1"/>
   <field name="reconciliation" optional="1"/>
 </tree>
```

### Comparing `trytond_account-6.6.3/view/move_template_form.xml` & `trytond_account-6.8.0/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_template_keyword_form.xml` & `trytond_account-6.8.0/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/move_tree.xml` & `trytond_account-6.8.0/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/party_form.xml` & `trytond_account-6.8.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/period_form.xml` & `trytond_account-6.8.0/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/reconcile_show_form.xml` & `trytond_account-6.8.0/view/reconcile_show_form.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/reconcile_show_form.xml` & `trytond_account-6.8.0/view/reconcile_show_form.xml`

```diff
@@ -4,15 +4,15 @@
 <form col="6">
   <label name="company"/>
   <field name="company"/>
   <label name="account"/>
   <field name="account"/>
   <label name="party"/>
   <field name="party"/>
-  <field name="lines" colspan="6"/>
+  <field name="lines" colspan="6" view_ids="account.move_line_view_list_reconcile"/>
   <separator name="write_off" colspan="6"/>
   <label name="write_off"/>
   <field name="write_off"/>
   <label name="date"/>
   <field name="date"/>
   <label name="write_off_amount"/>
   <field name="write_off_amount"/>
```

### Comparing `trytond_account-6.6.3/view/renew_fiscalyear_start_form.xml` & `trytond_account-6.8.0/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_code_context_form.xml` & `trytond_account-6.8.0/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_code_form.xml` & `trytond_account-6.8.0/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_code_template_form.xml` & `trytond_account-6.8.0/view/tax_rule_line_template_form.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_account-6.6.3/view/tax_code_template_form.xml` & `trytond_account-6.8.0/view/tax_rule_line_template_form.xml`

```diff
@@ -1,28 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
-  <label name="name"/>
-  <field name="name"/>
-  <label name="code"/>
-  <field name="code"/>
-  <label name="account"/>
-  <field name="account"/>
-  <label name="parent"/>
-  <field name="parent"/>
+  <label name="rule"/>
+  <field name="rule"/>
+  <newline/>
   <label name="start_date"/>
   <field name="start_date"/>
   <label name="end_date"/>
   <field name="end_date"/>
-  <notebook colspan="4">
-    <page name="lines">
-      <field name="lines" colspan="4"/>
-    </page>
-    <page name="childs">
-      <field name="childs" colspan="4"/>
-    </page>
-    <page name="description">
-      <field name="description" colspan="4"/>
-    </page>
-  </notebook>
+  <label name="group"/>
+  <field name="group"/>
+  <label name="origin_tax"/>
+  <field name="origin_tax"/>
+  <label name="tax"/>
+  <field name="tax"/>
+  <label name="sequence"/>
+  <field name="sequence"/>
+  <label name="keep_origin"/>
+  <field name="keep_origin"/>
 </form>
```

### Comparing `trytond_account-6.6.3/view/tax_form.xml` & `trytond_account-6.8.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_rule_form.xml` & `trytond_account-6.8.0/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_rule_line_form.xml` & `trytond_account-6.8.0/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_template_form.xml` & `trytond_account-6.8.0/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/tax_test_form.xml` & `trytond_account-6.8.0/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.6.3/view/writeoff_form.xml` & `trytond_account-6.8.0/view/writeoff_form.xml`

 * *Files identical despite different names*

