# Comparing `tmp/django-jbank-4.1.2.tar.gz` & `tmp/django-jbank-4.1.3.tar.gz`

## Comparing `django-jbank-4.1.2.tar` & `django-jbank-4.1.3.tar`

### file list

```diff
@@ -1,364 +1,366 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:14.000000 django-jbank-4.1.2/
--rw-rw-r--   0 jani      (1000) jani      (1000)      931 2023-03-27 06:59:59.000000 django-jbank-4.1.2/pyproject.toml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-04-05 11:04:17.000000 django-jbank-4.1.2/README.md
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2023-04-06 05:48:10.000000 django-jbank-4.1.2/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.1.2/LICENSE.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-04-06 05:48:10.000000 django-jbank-4.1.2/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      256 2022-07-02 11:10:09.000000 django-jbank-4.1.2/requirements-dev.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/django_jbank.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-04-06 05:48:02.000000 django-jbank-4.1.2/django_jbank.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-04-06 05:48:02.000000 django-jbank-4.1.2/django_jbank.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2023-04-06 05:48:02.000000 django-jbank-4.1.2/django_jbank.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.1.2/django_jbank.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        6 2023-04-06 05:48:02.000000 django-jbank-4.1.2/django_jbank.egg-info/top_level.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)   609015 2023-04-06 05:48:10.000000 django-jbank-4.1.2/django_jbank.egg-info/SOURCES.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/htmlcov/
--rw-rw-r--   0 jani      (1000) jani      (1000)    20396 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_pain002_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jquery.hotkeys.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     4577 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_apps_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jquery.tablesorter.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    20010 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    54955 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22199 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_import_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   463697 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_admin_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13564 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2756 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22245 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    26018 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    42120 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   152313 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_sepa_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   106957 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    77825 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_wsedi_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9556 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/manage_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4542 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22558 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/index.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    12322 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11994 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6940 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2533 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   155711 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_sepa_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    14174 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4582 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d1b4fb5372fdacae___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22201 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates_jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29198 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    21506 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates_admin___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29235 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2575 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank_statement___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22185 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    30153 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    82193 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_wsedi_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jquery.ba-throttle-debounce.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_payment_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    10869 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9846 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_files_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    39776 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_make_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24060 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_ecb_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4683 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    45984 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_csr_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    93373 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_tests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    53341 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_download_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   378796 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_models_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    93109 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_parsers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   348054 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_models_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    47349 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    10339 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_xmlsec1_examples_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    60842 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_parsers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   102362 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jquery.isonscreen.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     8921 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2551 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    17350 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wspki_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11825 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_files_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    42348 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_upload_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    28422 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   111921 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_tito_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24166 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    41408 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   132280 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_wspki_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4538 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_9798a7910e9d8d38___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9004 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/keybd_closed.png
--rw-rw-r--   0 jani      (1000) jani      (1000)     1732 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/favicon_32.png
--rw-rw-r--   0 jani      (1000) jani      (1000)    15523 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    61488 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   190062 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_camt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     7786 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13596 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    52753 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_xt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20188 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_reparse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9776 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_services_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    54239 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9769 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2505 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_views_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2531 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11551 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_ecb_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    11954 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_x509_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jquery.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    17982 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_export_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4504 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_f6e593a656d19133___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    44748 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    27154 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_to_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13619 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4514 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_de1059d8df3ce8de___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    35254 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    58311 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     8924 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   140727 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_wspki_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4474 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_views_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4526 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_367ac34b948d641d___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    29945 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13834 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_payment_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    23928 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6935 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    18044 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_euribor_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2599 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    27546 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2555 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     6546 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_apps_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   112238 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_tito_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20650 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/coverage_html.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    12429 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/style.css
--rw-rw-r--   0 jani      (1000) jani      (1000)    13993 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13624 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_app_req_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9003 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/keybd_open.png
--rw-rw-r--   0 jani      (1000) jani      (1000)    19907 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_pain001_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4520 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_c6b51be18eb0ec86___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4558 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d4f8c6455716e7bb___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    24383 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   105315 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_tests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    13538 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_ecb_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    20842 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   139457 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_camt_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22274 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_make_parse_format_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    25502 2023-03-27 06:36:02.000000 django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   386954 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_admin_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    28146 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_make_x509_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     8876 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_test_xp_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    18793 2021-06-23 23:14:44.000000 django-jbank-4.1.2/htmlcov/jbank_management_commands_reparse_svm_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.1.2/mypy.ini
--rw-rw-r--   0 jani      (1000) jani      (1000)      287 2020-09-02 13:51:57.000000 django-jbank-4.1.2/MANIFEST.in
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/pain001/
--rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.1.2/data/pain001/pain.001.001.03.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.1.2/data/ecb-rates-2019-08-15.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/pki/
--rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.1.2/data/pki/GetBankCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.1.2/data/pki/CreateCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.1.2/data/x509-data.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/finvoice/
--rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.1.2/data/finvoice/xsd-test.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/xm/
--rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.1.2/data/xm/camt_054_credit_notoification_example_finland.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/data/x509/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.1.2/data/x509/x509data.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.1.2/data/x509/appreq.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-02-14 22:34:42.000000 django-jbank-4.1.2/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      867 2023-04-06 05:47:52.000000 django-jbank-4.1.2/setup.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)     3440 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     9975 2022-12-30 01:32:15.000000 django-jbank-4.1.2/jbank/wsedi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    44606 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/models.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_ra.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      505 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/test_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/make_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/parse_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2021-09-14 00:17:15.000000 django-jbank-4.1.2/jbank/management/commands/test_app_req.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      859 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/xmlsec1_examples.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2338 2021-09-14 00:17:15.000000 django-jbank-4.1.2/jbank/management/commands/wsedi_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/test_payment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2021-09-09 00:31:49.000000 django-jbank-4.1.2/jbank/management/commands/wsedi_import.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/management/commands/wspki_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/test_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7189 2021-09-09 00:31:49.000000 django-jbank-4.1.2/jbank/management/commands/parse_xt.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2021-09-14 00:17:15.000000 django-jbank-4.1.2/jbank/management/commands/test_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7591 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/wsedi_download.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2945 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_xm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2021-09-09 00:31:49.000000 django-jbank-4.1.2/jbank/management/commands/reparse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_saldo.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/make_parse_format.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2021-09-14 00:17:15.000000 django-jbank-4.1.2/jbank/management/commands/parse_ecb_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/management/commands/parse_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      676 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/test_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4589 2022-12-09 16:27:19.000000 django-jbank-4.1.2/jbank/management/commands/make_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/reparse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2021-09-14 00:17:15.000000 django-jbank-4.1.2/jbank/management/commands/parse_euribor_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5375 2022-12-09 16:27:19.000000 django-jbank-4.1.2/jbank/management/commands/wsedi_upload.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2021-09-09 00:31:49.000000 django-jbank-4.1.2/jbank/management/commands/wsedi_export.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/management/commands/parse_aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/management/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/migrations/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0008_auto_20210512_2208.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0016_alter_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0004_statementfile.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0026_auto_20181205_0034.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0034_auto_20190815_2059.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0007_auto_20171102_2351.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0019_auto_20180209_0437.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0013_auto_20180126_0909.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0004_refund_attachment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0015_auto_20180208_0643.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0068_auto_20200717_2327.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0055_auto_20191130_2011.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0020_payout_due_date.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0069_auto_20200717_2333.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0047_wsedisoapcall_error.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0050_remove_wsedisoapcall_payout.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0041_auto_20191127_0559.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0039_auto_20191127_0156.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0037_auto_20191127_0132.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0008_auto_20171103_0007.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0024_auto_20180425_1704.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0048_wsediconnection_soap_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0028_auto_20190327_1830.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0066_wsediconnection_pin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0018_auto_20180208_1130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0053_wsediconnection_target_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0005_statementfile_created.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0025_auto_20181101_1430.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0027_auto_20190304_1913.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0036_wsediconnection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0015_ps_timestamp_fill.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0038_auto_20191127_0145.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0011_auto_20180126_0851.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0045_wsediconnection_receiver_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0051_payout_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0003_statement_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0007_auto_20210507_2122.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0012_auto_20180126_0858.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0003_auto_20200902_1354.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0001_initial.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0013_euriborrate.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0019_alter_payout_state.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0010_auto_20171226_1013.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0017_alter_statementrecord_name.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0059_auto_20200324_0234.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0049_wsediconnection_sender_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0014_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0046_auto_20191128_2242.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0022_accountbalance_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0020_accountbalance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0023_auto_20180419_1316.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0021_auto_20180209_0935.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0057_wsediconnection_enabled.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0043_wsedisoapcall.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0006_auto_20210318_2130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0029_auto_20190727_1352.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0064_auto_20200629_0344.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0062_auto_20200415_2300.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0005_auto_20201203_2308.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0061_auto_20200325_2204.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0060_auto_20200325_1906.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0063_auto_20200608_1827.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0033_auto_20190801_2121.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0052_auto_20191130_1927.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0009_auto_20171107_1847.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0058_auto_20200316_1949.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0016_auto_20180208_0724.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/migrations/0032_wsediconnection_use_sha256.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0006_auto_20171102_2341.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0021_alter_accountbalance_balance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0044_auto_20191128_2231.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0017_payoutparty_payouts_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0056_wsediconnection_debug_commands.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0002_auto_20171031_0356.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0030_auto_20190727_1633.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0067_wsediconnection_pki_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0014_payout_payoutstatus.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0025_auto_20230325_1014.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0035_auto_20190815_2137.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0040_wsediconnection_signing_key_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0002_auto_20200817_2217.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0054_wsediconnection_environment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0031_auto_20190727_1639.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0032_auto_20190727_1655.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/migrations/0022_auto_20180411_1814.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/migrations/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    19030 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/wspki.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.1.2/jbank/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)    11505 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      716 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/services.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22554 2023-04-06 05:44:34.000000 django-jbank-4.1.2/jbank/camt.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    26191 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/tests.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    52546 2023-04-06 05:47:52.000000 django-jbank-4.1.2/jbank/admin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6524 2021-07-06 23:33:19.000000 django-jbank-4.1.2/jbank/aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1257 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/ecb.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22601 2021-09-09 00:31:49.000000 django-jbank-4.1.2/jbank/sepa.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1189 2021-12-11 15:04:51.000000 django-jbank-4.1.2/jbank/x509_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    10249 2023-02-25 01:11:55.000000 django-jbank-4.1.2/jbank/parsers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5273 2023-02-26 05:09:42.000000 django-jbank-4.1.2/jbank/csr_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      235 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      819 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/files.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/admin/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/referencepaymentbatch/
--rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      690 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/mark_as_manually_settled.html
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/statement/
--rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/statement/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/statement/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/jbank/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/admin/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/templates/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_certificate_status_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_create_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/jbank/soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_renew_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/templates/jbank/application_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/jbank/application_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/jbank/encryption_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.1.2/jbank/templates/jbank/pki_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/jbank/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/templates/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-02-24 09:03:24.000000 django-jbank-4.1.2/jbank/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    26153 2023-02-24 09:03:24.000000 django-jbank-4.1.2/jbank/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-02-24 08:59:20.000000 django-jbank-4.1.2/jbank/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    21019 2023-02-24 09:03:24.000000 django-jbank-4.1.2/jbank/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-04-06 05:48:10.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/Makefile
--rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/encrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/sign3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/decrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/verify3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.1.2/jbank/xmlsec1-examples/sign3-sha256.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-03-27 06:59:59.000000 django-jbank-4.1.2/jbank/pain002.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.2/jbank/views.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1550 2021-12-20 09:39:29.000000 django-jbank-4.1.2/jbank/euribor.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    12672 2021-08-11 21:48:35.000000 django-jbank-4.1.2/jbank/tito.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       46 2021-07-06 21:13:32.000000 django-jbank-4.1.2/jbank/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:13.000000 django-jbank-4.1.3/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      931 2023-03-27 06:59:59.000000 django-jbank-4.1.3/pyproject.toml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-04-05 11:04:17.000000 django-jbank-4.1.3/README.md
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2023-05-03 19:07:09.000000 django-jbank-4.1.3/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.1.3/LICENSE.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-03 19:07:09.000000 django-jbank-4.1.3/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      256 2022-07-02 11:10:09.000000 django-jbank-4.1.3/requirements-dev.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/django_jbank.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1310 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.1.3/django_jbank.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        6 2023-05-03 19:07:01.000000 django-jbank-4.1.3/django_jbank.egg-info/top_level.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)   609127 2023-05-03 19:07:09.000000 django-jbank-4.1.3/django_jbank.egg-info/SOURCES.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/htmlcov/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20396 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_pain002_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.hotkeys.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4577 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_apps_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.tablesorter.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20010 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    54955 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22199 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_import_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   463697 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_admin_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13564 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2756 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22245 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26018 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    42120 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   152313 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_sepa_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   106957 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    77825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wsedi_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9556 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/manage_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4542 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22558 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/index.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12322 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11994 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6940 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2533 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   155711 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_sepa_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    14174 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4582 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d1b4fb5372fdacae___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22201 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29198 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    21506 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2543 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29235 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2575 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_statement___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22185 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    30153 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    82193 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_wsedi_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.ba-throttle-debounce.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_payment_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10869 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9846 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_files_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    39776 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24060 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_ecb_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4683 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    45984 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_csr_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93373 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_tests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    53341 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_download_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   378796 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_models_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93109 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_parsers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   348054 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_models_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    47349 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10339 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_xmlsec1_examples_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    60842 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_parsers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   102362 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.isonscreen.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8921 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2551 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    17350 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wspki_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11825 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_files_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    42348 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_upload_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    28422 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   111921 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tito_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24166 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    41408 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   132280 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_wspki_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4538 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_9798a7910e9d8d38___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9004 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/keybd_closed.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1732 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/favicon_32.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15523 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    61488 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   190062 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_camt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7786 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13596 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    52753 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20188 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9776 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_services_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    54239 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9769 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2505 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_views_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2531 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11551 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_ecb_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11954 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_x509_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jquery.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    17982 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_export_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4504 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_f6e593a656d19133___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    44748 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27154 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_to_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13619 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4514 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_de1059d8df3ce8de___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    35254 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    58311 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8924 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   140727 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wspki_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4474 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_views_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4526 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_367ac34b948d641d___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    29945 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13834 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_payment_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23928 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6935 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18044 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_euribor_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2599 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27546 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2555 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6546 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_apps_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   112238 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_tito_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20650 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/coverage_html.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12429 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/style.css
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13993 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13624 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_app_req_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9003 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/keybd_open.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19907 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_pain001_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4520 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_c6b51be18eb0ec86___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4558 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d4f8c6455716e7bb___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    24383 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   105315 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13538 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_ecb_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20842 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   139457 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_camt_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22274 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_parse_format_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    25502 2023-03-27 06:36:02.000000 django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   386954 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_admin_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    28146 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_make_x509_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8876 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_test_xp_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18793 2021-06-23 23:14:44.000000 django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_svm_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.1.3/mypy.ini
+-rw-rw-r--   0 jani      (1000) jani      (1000)      287 2020-09-02 13:51:57.000000 django-jbank-4.1.3/MANIFEST.in
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/pain001/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/pain001/pain.001.001.03.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/ecb-rates-2019-08-15.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/pki/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.1.3/data/pki/GetBankCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.1.3/data/pki/CreateCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.1.3/data/x509-data.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/finvoice/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/finvoice/xsd-test.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/xm/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.1.3/data/xm/camt_054_credit_notoification_example_finland.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/data/x509/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.1.3/data/x509/x509data.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.1.3/data/x509/appreq.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      139 2023-02-14 22:34:42.000000 django-jbank-4.1.3/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      867 2023-05-03 19:06:59.000000 django-jbank-4.1.3/setup.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3440 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11013 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/wsedi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    44747 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/models.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_ra.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      505 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/make_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/parse_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/test_app_req.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      859 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/xmlsec1_examples.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2338 2023-05-03 18:51:50.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_payment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_import.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/management/commands/wspki_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7308 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xt.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/test_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7591 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_download.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2935 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/reparse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_saldo.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/make_parse_format.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/parse_ecb_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/management/commands/parse_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      676 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/test_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4589 2022-12-09 16:27:19.000000 django-jbank-4.1.3/jbank/management/commands/make_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/reparse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2021-09-14 00:17:15.000000 django-jbank-4.1.3/jbank/management/commands/parse_euribor_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5375 2022-12-09 16:27:19.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_upload.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/management/commands/wsedi_export.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/management/commands/parse_aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/management/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/migrations/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0008_auto_20210512_2208.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0016_alter_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0004_statementfile.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0026_auto_20181205_0034.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0034_auto_20190815_2059.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0007_auto_20171102_2351.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0019_auto_20180209_0437.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0013_auto_20180126_0909.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0004_refund_attachment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0015_auto_20180208_0643.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0068_auto_20200717_2327.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0055_auto_20191130_2011.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0020_payout_due_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0069_auto_20200717_2333.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0047_wsedisoapcall_error.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0050_remove_wsedisoapcall_payout.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0041_auto_20191127_0559.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0039_auto_20191127_0156.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0037_auto_20191127_0132.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0008_auto_20171103_0007.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0024_auto_20180425_1704.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0048_wsediconnection_soap_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0028_auto_20190327_1830.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0066_wsediconnection_pin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0018_auto_20180208_1130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0053_wsediconnection_target_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0005_statementfile_created.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0025_auto_20181101_1430.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0027_auto_20190304_1913.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0036_wsediconnection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0015_ps_timestamp_fill.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0038_auto_20191127_0145.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0011_auto_20180126_0851.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0045_wsediconnection_receiver_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0051_payout_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0003_statement_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0007_auto_20210507_2122.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0012_auto_20180126_0858.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0003_auto_20200902_1354.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0001_initial.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0013_euriborrate.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0019_alter_payout_state.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0010_auto_20171226_1013.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0017_alter_statementrecord_name.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0059_auto_20200324_0234.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0049_wsediconnection_sender_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0014_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0046_auto_20191128_2242.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0022_accountbalance_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0020_accountbalance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0023_auto_20180419_1316.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0021_auto_20180209_0935.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0057_wsediconnection_enabled.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0043_wsedisoapcall.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0006_auto_20210318_2130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0029_auto_20190727_1352.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0064_auto_20200629_0344.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0062_auto_20200415_2300.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0005_auto_20201203_2308.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0061_auto_20200325_2204.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0060_auto_20200325_1906.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/migrations/0033_alter_statement_begin_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0063_auto_20200608_1827.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0033_auto_20190801_2121.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0052_auto_20191130_1927.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0009_auto_20171107_1847.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0058_auto_20200316_1949.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0016_auto_20180208_0724.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/migrations/0032_wsediconnection_use_sha256.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0006_auto_20171102_2341.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0021_alter_accountbalance_balance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0044_auto_20191128_2231.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0017_payoutparty_payouts_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0056_wsediconnection_debug_commands.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0002_auto_20171031_0356.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0030_auto_20190727_1633.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0067_wsediconnection_pki_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0014_payout_payoutstatus.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0025_auto_20230325_1014.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0035_auto_20190815_2137.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0040_wsediconnection_signing_key_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0002_auto_20200817_2217.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0054_wsediconnection_environment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0031_auto_20190727_1639.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0032_auto_20190727_1655.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/migrations/0022_auto_20180411_1814.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/migrations/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19043 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/wspki.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.1.3/jbank/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11505 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      716 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/services.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23260 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/camt.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26191 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/tests.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    52672 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/admin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6524 2021-07-06 23:33:19.000000 django-jbank-4.1.3/jbank/aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1257 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/ecb.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22601 2021-09-09 00:31:49.000000 django-jbank-4.1.3/jbank/sepa.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1189 2021-12-11 15:04:51.000000 django-jbank-4.1.3/jbank/x509_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10244 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/parsers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5273 2023-02-26 05:09:42.000000 django-jbank-4.1.3/jbank/csr_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      235 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      819 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/files.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      690 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/mark_as_manually_settled.html
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/statement/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/jbank/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/admin/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/templates/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_certificate_status_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_create_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/application_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/application_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/encryption_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.1.3/jbank/templates/jbank/pki_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/jbank/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/templates/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15825 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    26153 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-02-24 08:59:20.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    21019 2023-02-24 09:03:24.000000 django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2023-05-03 19:07:09.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/Makefile
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/encrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/sign3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/decrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/verify3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.1.3/jbank/xmlsec1-examples/sign3-sha256.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-03-27 06:59:59.000000 django-jbank-4.1.3/jbank/pain002.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:43.000000 django-jbank-4.1.3/jbank/views.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1562 2023-05-03 19:06:59.000000 django-jbank-4.1.3/jbank/euribor.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12672 2021-08-11 21:48:35.000000 django-jbank-4.1.3/jbank/tito.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       46 2021-07-06 21:13:32.000000 django-jbank-4.1.3/jbank/__init__.py
```

### Comparing `django-jbank-4.1.2/pyproject.toml` & `django-jbank-4.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/README.md` & `django-jbank-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/LICENSE.txt` & `django-jbank-4.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/PKG-INFO` & `django-jbank-4.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.1.2
+Version: 4.1.3
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
```

### Comparing `django-jbank-4.1.2/django_jbank.egg-info/PKG-INFO` & `django-jbank-4.1.3/django_jbank.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.1.2
+Version: 4.1.3
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
```

### Comparing `django-jbank-4.1.2/django_jbank.egg-info/SOURCES.txt` & `django-jbank-4.1.3/django_jbank.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6944,16 +6944,18 @@
 jbank/migrations/0029_auto_20190727_1352.py
 jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
 jbank/migrations/0030_auto_20190727_1633.py
 jbank/migrations/0031_auto_20190727_1639.py
 jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
 jbank/migrations/0032_auto_20190727_1655.py
 jbank/migrations/0032_wsediconnection_use_sha256.py
+jbank/migrations/0033_alter_statement_begin_date.py
 jbank/migrations/0033_auto_20190801_2121.py
 jbank/migrations/0034_auto_20190815_2059.py
+jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
 jbank/migrations/0035_auto_20190815_2137.py
 jbank/migrations/0036_wsediconnection.py
 jbank/migrations/0037_auto_20191127_0132.py
 jbank/migrations/0038_auto_20191127_0145.py
 jbank/migrations/0039_auto_20191127_0156.py
 jbank/migrations/0040_wsediconnection_signing_key_file.py
 jbank/migrations/0041_auto_20191127_0559.py
```

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_pain002_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_pain002_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jquery.hotkeys.js` & `django-jbank-4.1.3/htmlcov/jquery.hotkeys.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_apps_py.html` & `django-jbank-4.1.3/htmlcov/jbank_apps_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jquery.tablesorter.min.js` & `django-jbank-4.1.3/htmlcov/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_export_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_download_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_import_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_import_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_admin_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_admin_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_saldo_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_exec_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_svm_py.html` & `django-jbank-4.1.3/htmlcov/jbank_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_sepa_py.html` & `django-jbank-4.1.3/htmlcov/jbank_sepa_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_helpers_py.html` & `django-jbank-4.1.3/htmlcov/jbank_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_wsedi_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wsedi_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/manage_py.html` & `django-jbank-4.1.3/htmlcov/manage_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3___init___py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/index.html` & `django-jbank-4.1.3/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_xmlsec1_examples_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_aeb43_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_to_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_management___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_sepa_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_sepa_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_x509_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d1b4fb5372fdacae___init___py.html` & `django-jbank-4.1.3/htmlcov/d_d1b4fb5372fdacae___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wspki_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates_jbank___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates_jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_to_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates_admin___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates_admin___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank_statement___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_statement___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_x509_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_wsedi_py.html` & `django-jbank-4.1.3/htmlcov/jbank_wsedi_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jquery.ba-throttle-debounce.min.js` & `django-jbank-4.1.3/htmlcov/jquery.ba-throttle-debounce.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_payment_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_payment_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_xp_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_files_py.html` & `django-jbank-4.1.3/htmlcov/jbank_files_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_make_pain001_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_ecb_rates_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_ecb_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31___init___py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_csr_helpers_py.html` & `django-jbank-4.1.3/htmlcov/jbank_csr_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_tests_py.html` & `django-jbank-4.1.3/htmlcov/jbank_tests_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_download_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_download_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_models_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_models_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_parsers_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_parsers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_models_py.html` & `django-jbank-4.1.3/htmlcov/jbank_models_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_csr_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_xmlsec1_examples_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_xmlsec1_examples_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_parsers_py.html` & `django-jbank-4.1.3/htmlcov/jbank_parsers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_svm_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jquery.isonscreen.js` & `django-jbank-4.1.3/htmlcov/jquery.isonscreen.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_to_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wspki_exec_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wspki_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_files_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_files_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_upload_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_upload_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_svm_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_tito_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tito_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_import_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_wspki_py.html` & `django-jbank-4.1.3/htmlcov/jbank_wspki_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_9798a7910e9d8d38___init___py.html` & `django-jbank-4.1.3/htmlcov/d_9798a7910e9d8d38___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/keybd_closed.png` & `django-jbank-4.1.3/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/favicon_32.png` & `django-jbank-4.1.3/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_app_req_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_aeb43_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_camt_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_camt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_x509_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ra_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_xt_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_reparse_to_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_services_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_services_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_xt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_views_py.html` & `django-jbank-4.1.3/htmlcov/jbank_views_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_ecb_py.html` & `django-jbank-4.1.3/htmlcov/jbank_ecb_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_x509_helpers_py.html` & `django-jbank-4.1.3/htmlcov/jbank_x509_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jquery.min.js` & `django-jbank-4.1.3/htmlcov/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_wsedi_export_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_wsedi_export_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_f6e593a656d19133___init___py.html` & `django-jbank-4.1.3/htmlcov/d_f6e593a656d19133___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_upload_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_to_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_to_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_euribor_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_de1059d8df3ce8de___init___py.html` & `django-jbank-4.1.3/htmlcov/d_de1059d8df3ce8de___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_helpers_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_aeb43_py.html` & `django-jbank-4.1.3/htmlcov/jbank_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_test_svm_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_test_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_wspki_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_wspki_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_views_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_views_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_367ac34b948d641d___init___py.html` & `django-jbank-4.1.3/htmlcov/d_367ac34b948d641d___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_payment_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_payment_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_wsedi_exec_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_svm_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_euribor_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_euribor_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank_referencepaymentbatch___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_parse_xp_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_parse_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_templates_admin_jbank___init___py.html` & `django-jbank-4.1.3/htmlcov/jbank_templates_admin_jbank___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_apps_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_apps_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_tito_py.html` & `django-jbank-4.1.3/htmlcov/jbank_tito_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/coverage_html.js` & `django-jbank-4.1.3/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/style.css` & `django-jbank-4.1.3/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_aeb43_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_app_req_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_app_req_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/keybd_open.png` & `django-jbank-4.1.3/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_pain001_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_pain001_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_c6b51be18eb0ec86___init___py.html` & `django-jbank-4.1.3/htmlcov/d_c6b51be18eb0ec86___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d4f8c6455716e7bb___init___py.html` & `django-jbank-4.1.3/htmlcov/d_d4f8c6455716e7bb___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_make_parse_format_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_tests_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_tests_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_2442641f6b49fa31_ecb_py.html` & `django-jbank-4.1.3/htmlcov/d_2442641f6b49fa31_ecb_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_reparse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_camt_py.html` & `django-jbank-4.1.3/htmlcov/jbank_camt_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_make_parse_format_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_parse_format_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html` & `django-jbank-4.1.3/htmlcov/d_d9f236fb879a91e3_parse_ecb_rates_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_admin_py.html` & `django-jbank-4.1.3/htmlcov/jbank_admin_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_make_x509_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_make_x509_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_test_xp_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_test_xp_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/htmlcov/jbank_management_commands_reparse_svm_py.html` & `django-jbank-4.1.3/htmlcov/jbank_management_commands_reparse_svm_py.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/pain001/pain.001.001.03.xml` & `django-jbank-4.1.3/data/pain001/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/ecb-rates-2019-08-15.xml` & `django-jbank-4.1.3/data/ecb-rates-2019-08-15.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/pki/GetBankCertificate-res.xml` & `django-jbank-4.1.3/data/pki/GetBankCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/pki/CreateCertificate-res.xml` & `django-jbank-4.1.3/data/pki/CreateCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/x509-data.xml` & `django-jbank-4.1.3/data/x509-data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/finvoice/xsd-test.xml` & `django-jbank-4.1.3/data/finvoice/xsd-test.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/xm/camt_054_credit_notoification_example_finland.xml` & `django-jbank-4.1.3/data/xm/camt_054_credit_notoification_example_finland.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/x509/x509data.xml` & `django-jbank-4.1.3/data/x509/x509data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/data/x509/appreq.xml` & `django-jbank-4.1.3/data/x509/appreq.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/setup.py` & `django-jbank-4.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jbank",
-    version="4.1.2",
+    version="4.1.3",
     author="Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="",
     license="MIT licence, see LICENCE.txt",
     description="Finnish bank file format support for Django projects",
```

### Comparing `django-jbank-4.1.2/jbank/helpers.py` & `django-jbank-4.1.3/jbank/helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/wsedi.py` & `django-jbank-4.1.3/jbank/wsedi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # pylint: disable=logging-format-interpolation,logging-not-lazy,too-many-arguments,too-many-locals,too-many-statements,c-extension-no-member
 import base64
 import logging
 import traceback
-from datetime import date
+from datetime import date, timedelta, datetime
 from os.path import basename
 from typing import Callable, Optional
 import requests
 from django.conf import settings
 from django.template.loader import get_template
 from django.utils.timezone import now
 from django.utils.translation import gettext as _
 from lxml import etree  # type: ignore
 from zeep.wsse import BinarySignature  # type: ignore
+from zeep import ns
 from jbank.models import WsEdiConnection, WsEdiSoapCall
 
 logger = logging.getLogger(__name__)
 
 
 def wsedi_get(command: str, file_type: str, status: str, file_reference: str = "", verbose: bool = False) -> requests.Response:
     """
@@ -35,15 +36,15 @@
         url += "&file-type=" + file_type
     if status:
         url += "&status=" + status
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Token " + settings.WSEDI_TOKEN,
     }
-    res = requests.get(url, headers=headers)
+    res = requests.get(url, headers=headers, timeout=120)
     if res.status_code >= 300:
         logger.error(
             "wsedi_get(command={}, file_type={}, status={}, file_reference={}) response HTTP {}:\n".format(
                 command, file_type, status, file_reference, res.status_code
             )
             + res.text
         )
@@ -78,27 +79,43 @@
         "file-name": basename(file_name),
         "file-content": base64.b64encode(file_content.encode("utf8")).decode("ascii"),
     }
     headers = {
         "Content-Type": "application/x-www-form-urlencoded",
         "Authorization": "Token " + settings.WSEDI_TOKEN,
     }
-    res = requests.post(url, data=data, headers=headers)
+    res = requests.post(url, data=data, headers=headers, timeout=600)
     if res.status_code >= 300:
         logger.error(
             "wsedi_upload_file(command={}, file_type={}, file_name={}) response HTTP {}:\n".format(command, file_type, file_name, res.status_code) + res.text
         )
         raise Exception("WS-EDI {} HTTP {}".format(command, res.status_code))
     if verbose:
         logger.info(
             "wsedi_upload_file(command={}, file_type={}, file_name={}) response HTTP {}:\n".format(command, file_type, file_name, res.status_code) + res.text
         )
     return res
 
 
+def wsse_insert_timestamp(envelope: etree.Element, timestamp: datetime, expires_seconds: int = 3600):
+    """
+    Inserts <wsu:Timestamp> element to the beginning of <wsse:Security>.
+    """
+    soap_header = envelope.find("{http://schemas.xmlsoap.org/soap/envelope/}Header")
+    if soap_header is not None:
+        soap_security = soap_header.find("{http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd}Security")
+        if soap_security is not None:
+            soap_timestamp = etree.Element(etree.QName(ns.WSU, "Timestamp"), {etree.QName(ns.WSU, "Id"): "timestamp"})
+            soap_timestamp_created = etree.SubElement(soap_timestamp, etree.QName(ns.WSU, "Created"))
+            soap_timestamp_created.text = timestamp.isoformat()
+            soap_timestamp_expires = etree.SubElement(soap_timestamp, etree.QName(ns.WSU, "Expires"))
+            soap_timestamp_expires.text = (timestamp + timedelta(seconds=expires_seconds)).isoformat()
+            soap_security.insert(0, soap_timestamp)
+
+
 def wsedi_execute(  # noqa
     ws: WsEdiConnection,
     command: str,
     file_type: str = "",
     status: str = "",
     file_reference: str = "",  # noqa
     file_content: str = "",
@@ -177,33 +194,32 @@
         if verbose:
             logger.info("------------------------------------------------------ {} soap_body\n{}".format(call_str, soap_body))
 
         body_bytes = soap_body.encode()
         envelope = etree.fromstring(body_bytes)
         binary_signature = BinarySignature(ws.signing_key_full_path, ws.signing_cert_full_path)
         soap_headers: dict = {}
-        # print(f"BEFORE signing with {ws.signing_key_full_path} and {ws.signing_cert_full_path}")
-        # with open("/home/jani/Downloads/e.xml", "wb") as fp:
-        #     fp.write(etree.tostring(envelope))
-        # print(etree.tostring(envelope).decode())
         envelope, soap_headers = binary_signature.apply(envelope, soap_headers)
+        if ws.use_wsse_timestamp:
+            wsse_insert_timestamp(envelope, soap_call.created)
         signed_body_bytes = etree.tostring(envelope)
         if verbose:
-            logger.info("------------------------------------------------------ {} signed_body_bytes\n{}".format(call_str, signed_body_bytes))
+            logger.info("------------------------------------------------------ {} HTTP POST\n{}".format(call_str, ws.soap_endpoint))
+            logger.info(
+                "------------------------------------------------------ {} signed_body_bytes.decode()\n{}".format(call_str, signed_body_bytes.decode())
+            )
 
         http_headers = {
             "Connection": "Close",
             "Content-Type": "text/xml",
             "Method": "POST",
             "SOAPAction": "",
             "User-Agent": "Kajala WS",
         }
-        if verbose:
-            logger.info("HTTP POST {}".format(ws.soap_endpoint))
-        res = requests.post(ws.soap_endpoint, data=signed_body_bytes, headers=http_headers)
+        res = requests.post(ws.soap_endpoint, data=signed_body_bytes, headers=http_headers, timeout=600)
         if verbose:
             logger.info("------------------------------------------------------ {} HTTP response {}\n{}".format(call_str, res.status_code, res.text))
         if res.status_code >= 300:
             logger.error("------------------------------------------------------ {} HTTP response {}\n{}".format(call_str, res.status_code, res.text))
             raise Exception("WS-EDI {} HTTP {}".format(command, res.status_code))
 
         envelope = etree.fromstring(res.content)
```

### Comparing `django-jbank-4.1.2/jbank/models.py` & `django-jbank-4.1.3/jbank/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 class Statement(AccountEntrySourceFile):
     file = models.ForeignKey("StatementFile", blank=True, default=None, null=True, on_delete=models.CASCADE)
     account = models.ForeignKey(Account, related_name="+", on_delete=models.PROTECT)
     account_number = SafeCharField(_("account number"), max_length=32, db_index=True)
     statement_identifier = SafeCharField(_("statement identifier"), max_length=48, db_index=True, blank=True, default="")
     statement_number = models.SmallIntegerField(_("statement number"), db_index=True)
-    begin_date = models.DateField(_("begin date"), db_index=True)
+    begin_date = models.DateField(_("begin date"), db_index=True, null=True, default=None, blank=True)
     end_date = models.DateField(_("end date"), db_index=True)
     record_date = models.DateTimeField(_("record date"), db_index=True)
     customer_identifier = SafeCharField(_("customer identifier"), max_length=64, blank=True, default="")
     begin_balance_date = models.DateField(_("begin balance date"), null=True, blank=True, default=None)
     begin_balance = models.DecimalField(_("begin balance"), max_digits=10, decimal_places=2)
     record_count = models.IntegerField(_("record count"), null=True, default=None)
     currency_code = SafeCharField(_("currency code"), max_length=3)
@@ -736,14 +736,15 @@
     encryption_cert_file = models.FileField(verbose_name=_("encryption certificate file"), blank=True, upload_to="certs")
     encryption_key_file = models.FileField(verbose_name=_("encryption key file"), blank=True, upload_to="certs")
     old_signing_key_file = models.FileField(verbose_name=_("old signing key file"), blank=True, upload_to="certs", editable=False)
     old_encryption_key_file = models.FileField(verbose_name=_("old encryption key file"), blank=True, upload_to="certs", editable=False)
     bank_encryption_cert_file = models.FileField(verbose_name=_("bank encryption cert file"), blank=True, upload_to="certs")
     bank_signing_cert_file = models.FileField(verbose_name=_("bank signing cert file"), blank=True, upload_to="certs")
     use_sha256 = models.BooleanField(_("SHA-256"), blank=True, default=False)
+    use_wsse_timestamp = models.BooleanField(_("Use WS-Security timestamp"), blank=True, default=False)
     ca_cert_file = models.FileField(verbose_name=_("CA certificate file"), blank=True, upload_to="certs")
     debug_commands = SafeTextField(_("debug commands"), blank=True, help_text=_("wsedi.connection.debug.commands.help.text"))
     created = models.DateTimeField(_("created"), default=now, db_index=True, editable=False, blank=True)
     _signing_cert = None
 
     class Meta:
         verbose_name = _("WS-EDI connection")
```

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_ra.py` & `django-jbank-4.1.3/jbank/management/commands/parse_ra.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/make_x509.py` & `django-jbank-4.1.3/jbank/management/commands/make_x509.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/test_app_req.py` & `django-jbank-4.1.3/jbank/management/commands/test_app_req.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_svm.py` & `django-jbank-4.1.3/jbank/management/commands/parse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/xmlsec1_examples.py` & `django-jbank-4.1.3/jbank/management/commands/xmlsec1_examples.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wsedi_exec.py` & `django-jbank-4.1.3/jbank/management/commands/wsedi_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/test_payment.py` & `django-jbank-4.1.3/jbank/management/commands/test_payment.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wsedi_import.py` & `django-jbank-4.1.3/jbank/management/commands/wsedi_import.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wspki_exec.py` & `django-jbank-4.1.3/jbank/management/commands/wspki_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_to.py` & `django-jbank-4.1.3/jbank/management/commands/parse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_xt.py` & `django-jbank-4.1.3/jbank/management/commands/parse_xt.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import os
 from pprint import pprint
 
 from django.core.exceptions import ValidationError
 from django.core.management.base import CommandParser
 from django.db import transaction
 from jbank.camt import (
-    camt053_get_iban,
+    camt053_get_account_iban,
     camt053_create_statement,
     camt053_parse_statement_from_file,
-    CAMT053_STATEMENT_SUFFIXES,
+    CAMT053_FILE_SUFFIXES,
     camt053_get_unified_str,
+    camt053_get_account_currency,
 )
 from jbank.helpers import get_or_create_bank_account, save_or_store_media
 from jbank.files import list_dir_files
 from jbank.models import Statement, StatementFile, StatementRecord, StatementRecordDetail
 from jbank.parsers import parse_filename_suffix
 from jutil.command import SafeCommand
 
@@ -35,15 +36,15 @@
         parser.add_argument("--tag", type=str, default="")
         parser.add_argument("--parse-creditor-account-data", action="store_true", help="For data migration")
 
     def parse_creditor_account_data(self):  # pylint: disable=too-many-locals,too-many-branches
         for sf in StatementFile.objects.all():  # pylint: disable=too-many-nested-blocks
             assert isinstance(sf, StatementFile)
             full_path = sf.full_path
-            if os.path.isfile(full_path) and parse_filename_suffix(full_path).upper() in CAMT053_STATEMENT_SUFFIXES:
+            if os.path.isfile(full_path) and parse_filename_suffix(full_path).upper() in CAMT053_FILE_SUFFIXES:
                 logger.info("Parsing creditor account data of %s", full_path)
                 statement_data = camt053_parse_statement_from_file(full_path)
                 d_stmt = statement_data.get("BkToCstmrStmt", {}).get("Stmt", {})
                 d_ntry = d_stmt.get("Ntry", [])
                 recs = list(StatementRecord.objects.all().filter(statement__file=sf).order_by("id"))
                 if len(recs) != len(d_ntry):
                     raise ValidationError(f"Statement record counts do not match in id={sf.id} ({sf})")
@@ -87,15 +88,15 @@
             self.parse_creditor_account_data()
             return
 
         files = list_dir_files(options["path"], options["suffix"])
         for filename in files:
             plain_filename = os.path.basename(filename)
 
-            if parse_filename_suffix(plain_filename).upper() not in CAMT053_STATEMENT_SUFFIXES:
+            if parse_filename_suffix(plain_filename).upper() not in CAMT053_FILE_SUFFIXES:
                 print("Ignoring non-CAMT53 file {}".format(filename))
                 continue
 
             if options["resolve_original_filenames"]:
                 found = StatementFile.objects.filter(statement__name=plain_filename).first()
                 if found and not found.original_filename:
                     assert isinstance(found, StatementFile)
@@ -122,14 +123,15 @@
                     file = StatementFile(original_filename=filename, tag=options["tag"])
                     file.save()
                     save_or_store_media(file.file, filename)
                     file.save()
 
                     for data in [statement]:
                         if options["auto_create_accounts"]:
-                            account_number = camt053_get_iban(data)
+                            account_number = camt053_get_account_iban(data)
+                            currency = camt053_get_account_currency(data)
                             if account_number:
-                                get_or_create_bank_account(account_number)
+                                get_or_create_bank_account(account_number, currency)
 
                         camt053_create_statement(data, name=plain_filename, file=file)  # pytype: disable=not-callable
             else:
                 print("Skipping statement file {}".format(filename))
```

### Comparing `django-jbank-4.1.2/jbank/management/commands/test_pain001.py` & `django-jbank-4.1.3/jbank/management/commands/test_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wsedi_download.py` & `django-jbank-4.1.3/jbank/management/commands/wsedi_download.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_xm.py` & `django-jbank-4.1.3/jbank/management/commands/parse_xm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from pprint import pprint
 from django.core.management.base import CommandParser
 from django.db import transaction
-from jbank.camt import CAMT054_STATEMENT_SUFFIXES, camt054_parse_file, camt054_create_reference_payment_batch, camt054_parse_ntfctn_acct
+from jbank.camt import CAMT054_FILE_SUFFIXES, camt054_parse_file, camt054_create_reference_payment_batch, camt054_parse_ntfctn_acct
 from jbank.files import list_dir_files
 from jbank.helpers import save_or_store_media, get_or_create_bank_account
 from jbank.models import ReferencePaymentBatch, ReferencePaymentBatchFile
 from jbank.parsers import parse_filename_suffix
 from jutil.command import SafeCommand
 
 logger = logging.getLogger(__name__)
@@ -25,15 +25,15 @@
         parser.add_argument("--tag", type=str, default="")
 
     def do(self, *args, **options):  # pylint: disable=too-many-branches
         files = list_dir_files(options["path"])
         for filename in files:
             plain_filename = os.path.basename(filename)
 
-            if parse_filename_suffix(plain_filename).upper() not in CAMT054_STATEMENT_SUFFIXES:
+            if parse_filename_suffix(plain_filename).upper() not in CAMT054_FILE_SUFFIXES:
                 print("Ignoring non-camt.054 file {}".format(filename))
                 continue
 
             if options["delete_old"]:
                 ReferencePaymentBatch.objects.filter(name=plain_filename).delete()
 
             if options["test"]:
```

### Comparing `django-jbank-4.1.2/jbank/management/commands/reparse_svm.py` & `django-jbank-4.1.3/jbank/management/commands/reparse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_saldo.py` & `django-jbank-4.1.3/jbank/management/commands/parse_saldo.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/make_parse_format.py` & `django-jbank-4.1.3/jbank/management/commands/make_parse_format.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_ecb_rates.py` & `django-jbank-4.1.3/jbank/management/commands/parse_ecb_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_xp.py` & `django-jbank-4.1.3/jbank/management/commands/parse_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/test_xp.py` & `django-jbank-4.1.3/jbank/management/commands/test_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/make_pain001.py` & `django-jbank-4.1.3/jbank/management/commands/make_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/reparse_to.py` & `django-jbank-4.1.3/jbank/management/commands/reparse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_euribor_rates.py` & `django-jbank-4.1.3/jbank/management/commands/parse_euribor_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wsedi_upload.py` & `django-jbank-4.1.3/jbank/management/commands/wsedi_upload.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/wsedi_export.py` & `django-jbank-4.1.3/jbank/management/commands/wsedi_export.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/management/commands/parse_aeb43.py` & `django-jbank-4.1.3/jbank/management/commands/parse_aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0008_auto_20210512_2208.py` & `django-jbank-4.1.3/jbank/migrations/0008_auto_20210512_2208.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0016_alter_payoutstatus_timestamp.py` & `django-jbank-4.1.3/jbank/migrations/0016_alter_payoutstatus_timestamp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0004_statementfile.py` & `django-jbank-4.1.3/jbank/migrations/0004_statementfile.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py` & `django-jbank-4.1.3/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0026_auto_20181205_0034.py` & `django-jbank-4.1.3/jbank/migrations/0026_auto_20181205_0034.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0034_auto_20190815_2059.py` & `django-jbank-4.1.3/jbank/migrations/0034_auto_20190815_2059.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0007_auto_20171102_2351.py` & `django-jbank-4.1.3/jbank/migrations/0007_auto_20171102_2351.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0019_auto_20180209_0437.py` & `django-jbank-4.1.3/jbank/migrations/0019_auto_20180209_0437.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0013_auto_20180126_0909.py` & `django-jbank-4.1.3/jbank/migrations/0013_auto_20180126_0909.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py` & `django-jbank-4.1.3/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0015_auto_20180208_0643.py` & `django-jbank-4.1.3/jbank/migrations/0015_auto_20180208_0643.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0055_auto_20191130_2011.py` & `django-jbank-4.1.3/jbank/migrations/0055_auto_20191130_2011.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0069_auto_20200717_2333.py` & `django-jbank-4.1.3/jbank/migrations/0069_auto_20200717_2333.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0041_auto_20191127_0559.py` & `django-jbank-4.1.3/jbank/migrations/0041_auto_20191127_0559.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0039_auto_20191127_0156.py` & `django-jbank-4.1.3/jbank/migrations/0039_auto_20191127_0156.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0037_auto_20191127_0132.py` & `django-jbank-4.1.3/jbank/migrations/0037_auto_20191127_0132.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0008_auto_20171103_0007.py` & `django-jbank-4.1.3/jbank/migrations/0008_auto_20171103_0007.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0024_auto_20180425_1704.py` & `django-jbank-4.1.3/jbank/migrations/0024_auto_20180425_1704.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0048_wsediconnection_soap_endpoint.py` & `django-jbank-4.1.3/jbank/migrations/0048_wsediconnection_soap_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0018_auto_20180208_1130.py` & `django-jbank-4.1.3/jbank/migrations/0018_auto_20180208_1130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0005_statementfile_created.py` & `django-jbank-4.1.3/jbank/migrations/0005_statementfile_created.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0025_auto_20181101_1430.py` & `django-jbank-4.1.3/jbank/migrations/0025_auto_20181101_1430.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0027_auto_20190304_1913.py` & `django-jbank-4.1.3/jbank/migrations/0027_auto_20190304_1913.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0036_wsediconnection.py` & `django-jbank-4.1.3/jbank/migrations/0036_wsediconnection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py` & `django-jbank-4.1.3/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0011_auto_20180126_0851.py` & `django-jbank-4.1.3/jbank/migrations/0011_auto_20180126_0851.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0051_payout_connection.py` & `django-jbank-4.1.3/jbank/migrations/0051_payout_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0003_statement_account.py` & `django-jbank-4.1.3/jbank/migrations/0003_statement_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0007_auto_20210507_2122.py` & `django-jbank-4.1.3/jbank/migrations/0007_auto_20210507_2122.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0012_auto_20180126_0858.py` & `django-jbank-4.1.3/jbank/migrations/0012_auto_20180126_0858.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0001_initial.py` & `django-jbank-4.1.3/jbank/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0013_euriborrate.py` & `django-jbank-4.1.3/jbank/migrations/0013_euriborrate.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0019_alter_payout_state.py` & `django-jbank-4.1.3/jbank/migrations/0019_alter_payout_state.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.1.3/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0022_accountbalance_connection.py` & `django-jbank-4.1.3/jbank/migrations/0022_accountbalance_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0020_accountbalance.py` & `django-jbank-4.1.3/jbank/migrations/0020_accountbalance.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0021_auto_20180209_0935.py` & `django-jbank-4.1.3/jbank/migrations/0021_auto_20180209_0935.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0043_wsedisoapcall.py` & `django-jbank-4.1.3/jbank/migrations/0043_wsedisoapcall.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0006_auto_20210318_2130.py` & `django-jbank-4.1.3/jbank/migrations/0006_auto_20210318_2130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0029_auto_20190727_1352.py` & `django-jbank-4.1.3/jbank/migrations/0029_auto_20190727_1352.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0064_auto_20200629_0344.py` & `django-jbank-4.1.3/jbank/migrations/0064_auto_20200629_0344.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0062_auto_20200415_2300.py` & `django-jbank-4.1.3/jbank/migrations/0062_auto_20200415_2300.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0061_auto_20200325_2204.py` & `django-jbank-4.1.3/jbank/migrations/0061_auto_20200325_2204.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0060_auto_20200325_1906.py` & `django-jbank-4.1.3/jbank/migrations/0060_auto_20200325_1906.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.1.3/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0052_auto_20191130_1927.py` & `django-jbank-4.1.3/jbank/migrations/0052_auto_20191130_1927.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0009_auto_20171107_1847.py` & `django-jbank-4.1.3/jbank/migrations/0009_auto_20171107_1847.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0016_auto_20180208_0724.py` & `django-jbank-4.1.3/jbank/migrations/0016_auto_20180208_0724.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py` & `django-jbank-4.1.3/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0006_auto_20171102_2341.py` & `django-jbank-4.1.3/jbank/migrations/0006_auto_20171102_2341.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py` & `django-jbank-4.1.3/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0017_payoutparty_payouts_account.py` & `django-jbank-4.1.3/jbank/migrations/0017_payoutparty_payouts_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0002_auto_20171031_0356.py` & `django-jbank-4.1.3/jbank/migrations/0002_auto_20171031_0356.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py` & `django-jbank-4.1.3/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0014_payout_payoutstatus.py` & `django-jbank-4.1.3/jbank/migrations/0014_payout_payoutstatus.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0025_auto_20230325_1014.py` & `django-jbank-4.1.3/jbank/migrations/0025_auto_20230325_1014.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0002_auto_20200817_2217.py` & `django-jbank-4.1.3/jbank/migrations/0002_auto_20200817_2217.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/migrations/0031_auto_20190727_1639.py` & `django-jbank-4.1.3/jbank/migrations/0031_auto_20190727_1639.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/wspki.py` & `django-jbank-4.1.3/jbank/wspki.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
                 body_bytes.decode(),
             )
         debug_output = command in ws.debug_command_list or "ALL" in ws.debug_command_list
         if debug_output and soap_call.debug_request_full_path:
             with open(soap_call.debug_request_full_path, "wb") as fp:
                 fp.write(body_bytes)
 
-        res = requests.post(pki_endpoint, data=body_bytes, headers=http_headers)
+        res = requests.post(pki_endpoint, data=body_bytes, headers=http_headers, timeout=120)
         if verbose and res.status_code < 300:
             logger.info(
                 "------------------------------------------------------ HTTP response %s\n%s",
                 res.status_code,
                 format_xml_bytes(res.content).decode(),
             )
         if debug_output and soap_call.debug_response_full_path:
```

### Comparing `django-jbank-4.1.2/jbank/svm.py` & `django-jbank-4.1.3/jbank/svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/services.py` & `django-jbank-4.1.3/jbank/services.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/camt.py` & `django-jbank-4.1.3/jbank/camt.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,33 +25,41 @@
     ReferencePaymentBatch,
     ReferencePaymentRecord,
 )
 from jbank.parsers import parse_filename_suffix
 from jutil.xml import xml_to_dict
 
 
-CAMT053_STATEMENT_SUFFIXES = ("XML", "XT", "CAMT", "NDCAMT53L", "XML")
+CAMT053_FILE_SUFFIXES = ("XML", "XT", "CAMT", "NDCAMT53L", "XML", "NDARSTXMLO", "NDAREXXMLO", "053")
 
 CAMT053_ARRAY_TAGS = ["Bal", "Ntry", "NtryDtls", "TxDtls", "Strd", "Ustrd"]
 
 CAMT053_INT_TAGS = ["NbOfNtries", "NbOfTxs"]
 
-CAMT054_STATEMENT_SUFFIXES = ("XE", "XE", "CAMT", "NDCAMT54L", "XML")
+CAMT054_FILE_SUFFIXES = ("XE", "XE", "CAMT", "NDCAMT54L", "XML", "NDCAPXMLD54O", "NDARCRAXMLO", "054")
 
 CAMT054_ARRAY_TAGS = ["Ntfctn", "Othr", "Ntry", "NtryDtls", "PrtryAmt", "Chrgs", "AdrLine", "Strd", "Ustrd", "RfrdDocInf", "AddtlRmtInf"]
 
 CAMT054_INT_TAGS = ["NbOfNtries", "NbOfTxs"]
 
 logger = logging.getLogger(__name__)
 
 
 def camt053_get_iban(data: dict) -> str:
     return data.get("BkToCstmrStmt", {}).get("Stmt", {}).get("Acct", {}).get("Id", {}).get("IBAN", "")
 
 
+def camt053_get_account_iban(data: dict) -> str:
+    return data.get("BkToCstmrStmt", {}).get("Stmt", {}).get("Acct", {}).get("Id", {}).get("IBAN", "")
+
+
+def camt053_get_account_currency(data: dict) -> str:
+    return data.get("BkToCstmrStmt", {}).get("Stmt", {}).get("Acct", {}).get("Ccy") or ""
+
+
 def camt053_get_val(data: dict, key: str, default: Any = None, required: bool = True, name: str = "") -> Any:
     if key not in data:
         if required:
             raise ValidationError(_("camt.053 field {} missing").format(name if name else key))
         return default
     return data[key]
 
@@ -78,14 +86,22 @@
     s = camt053_get_val(data, key, None, True, name)
     val = parse_datetime(s)
     if val is None:
         raise ValidationError(_("camt.053 field {} type {} missing or invalid").format(name, "datetime") + ": {}".format(s))
     return val
 
 
+def camt053_get_date_or_none(data: Dict[str, Any], key: str, name: str = "") -> Optional[date]:
+    s = camt053_get_val(data, key, None, False, name)
+    if not s:
+        return None
+    val = parse_datetime(s)
+    return val.date()
+
+
 def camt053_get_int(data: Dict[str, Any], key: str, name: str = "") -> int:
     s = camt053_get_val(data, key, None, True, name)
     try:
         return int(s)
     except Exception:
         pass
     raise ValidationError(_("camt.053 field {} type {} missing or invalid").format(name, "int"))
@@ -112,18 +128,18 @@
         return val
     except Exception:
         pass
     raise ValidationError(_("camt.053 field {} type {} missing or invalid").format(name, "date") + ": {}".format(s))
 
 
 def camt053_parse_statement_from_file(filename: str) -> dict:
-    if parse_filename_suffix(filename).upper() not in CAMT053_STATEMENT_SUFFIXES:
+    if parse_filename_suffix(filename).upper() not in CAMT053_FILE_SUFFIXES:
         raise ValidationError(
             _('File {filename} has unrecognized ({suffixes}) suffix for file type "{file_type}"').format(
-                filename=filename, suffixes=", ".join(CAMT053_STATEMENT_SUFFIXES), file_type="camt.053"
+                filename=filename, suffixes=", ".join(CAMT053_FILE_SUFFIXES), file_type="camt.053"
             )
         )
     with open(filename, "rb") as fp:
         data = xml_to_dict(fp.read(), array_tags=CAMT053_ARRAY_TAGS, int_tags=CAMT053_INT_TAGS)
         return data
 
 
@@ -167,18 +183,19 @@
     """
     Creates camt.053 Statement from statement data parsed by camt053_parse_statement_from_file()
     :param statement_data: XML data in form of dict
     :param name: File name of the account statement
     :param file: Source statement file
     :return: Statement
     """
-    account_number = camt053_get_iban(statement_data)
+    account_number = camt053_get_account_iban(statement_data)
+    account_currency = camt053_get_account_currency(statement_data)
     if not account_number:
         raise ValidationError("{name}: ".format(name=name) + _("account.not.found").format(account_number=""))
-    accounts = list(Account.objects.filter(name=account_number))
+    accounts = list(Account.objects.filter(name=account_number, currency=account_currency))
     if len(accounts) != 1:
         raise ValidationError("{name}: ".format(name=name) + _("account.not.found").format(account_number=account_number) + " (" + str(len(accounts)) + ")")
     account = accounts[0]
     assert isinstance(account, Account)
 
     d_stmt = statement_data.get("BkToCstmrStmt", {}).get("Stmt", {})
     if not d_stmt:
@@ -193,16 +210,16 @@
         raise ValidationError("Bank account {} statement {} of processed already".format(account_number, name))
     stm = Statement(name=name, account=account, file=file)
     stm.account_number = stm.iban = account_number
     stm.bic = camt053_get_str(d_acct.get("Svcr", {}).get("FinInstnId", {}), "BIC", name="Stmt.Acct.Svcr.FinInstnId.BIC")
     stm.statement_identifier = camt053_get_str(d_stmt, "Id", name="Stmt.Id")
     stm.statement_number = camt053_get_str(d_stmt, "LglSeqNb", name="Stmt.LglSeqNb")
     stm.record_date = camt053_get_dt(d_stmt, "CreDtTm", name="Stmt.CreDtTm")
-    stm.begin_date = camt053_get_dt(d_frto, "FrDtTm", name="Stmt.FrDtTm").date()
-    stm.end_date = camt053_get_dt(d_frto, "ToDtTm", name="Stmt.ToDtTm").date()
+    stm.begin_date = camt053_get_date_or_none(d_frto, "FrDtTm", name="Stmt.FrDtTm")
+    stm.end_date = camt053_get_date_or_none(d_frto, "ToDtTm", name="Stmt.ToDtTm") or stm.record_date
     stm.currency_code = camt053_get_str(d_acct, "Ccy", name="Stmt.Acct.Ccy")
     if stm.currency_code != account.currency:
         raise ValidationError(
             _(
                 "Account currency {account_currency} does not match statement entry currency {statement_currency}".format(
                     statement_currency=stm.currency_code, account_currency=account.currency
                 )
@@ -385,18 +402,18 @@
         rec.full_clean()
         rec.save()
 
     return stm
 
 
 def camt054_parse_file(filename: str) -> dict:
-    if parse_filename_suffix(filename).upper() not in CAMT054_STATEMENT_SUFFIXES:
+    if parse_filename_suffix(filename).upper() not in CAMT054_FILE_SUFFIXES:
         raise ValidationError(
             _('File {filename} has unrecognized ({suffixes}) suffix for file type "{file_type}"').format(
-                filename=filename, suffixes=", ".join(CAMT054_STATEMENT_SUFFIXES), file_type="camt.054"
+                filename=filename, suffixes=", ".join(CAMT054_FILE_SUFFIXES), file_type="camt.054"
             )
         )
     with open(filename, "rb") as fp:
         data = xml_to_dict(fp.read(), array_tags=CAMT054_ARRAY_TAGS, int_tags=CAMT054_INT_TAGS)
         return data
```

### Comparing `django-jbank-4.1.2/jbank/tests.py` & `django-jbank-4.1.3/jbank/tests.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/admin.py` & `django-jbank-4.1.3/jbank/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,20 +236,22 @@
     def bic_code(self, obj):
         assert isinstance(obj, Statement)
         return iban_bic(obj.account_number)
 
     bic_code.short_description = "BIC"  # type: ignore
 
     def statement_date_short(self, obj):
+        assert isinstance(obj, Statement)
         return date_format(obj.end_date, "SHORT_DATE_FORMAT")
 
     statement_date_short.short_description = _("date")  # type: ignore
     statement_date_short.admin_order_field = "end_date"  # type: ignore
 
     def record_date_short(self, obj):
+        assert isinstance(obj, Statement)
         return date_format(obj.record_date, "SHORT_DATE_FORMAT")
 
     record_date_short.short_description = _("record date")  # type: ignore
     record_date_short.admin_order_field = "record_date"  # type: ignore
 
     def account_entry_list(self, obj):
         assert isinstance(obj, Statement)
@@ -1410,14 +1412,15 @@
                     "signing_key_file",
                     "encryption_cert_file",
                     "encryption_key_file",
                     "bank_encryption_cert_file",
                     "bank_signing_cert_file",
                     "ca_cert_file",
                     "use_sha256",
+                    "use_wsse_timestamp",
                 ]
             },
         ),
     )
 
     readonly_fields = (
         "id",
```

### Comparing `django-jbank-4.1.2/jbank/aeb43.py` & `django-jbank-4.1.3/jbank/aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/ecb.py` & `django-jbank-4.1.3/jbank/ecb.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/sepa.py` & `django-jbank-4.1.3/jbank/sepa.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/x509_helpers.py` & `django-jbank-4.1.3/jbank/x509_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/parsers.py` & `django-jbank-4.1.3/jbank/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     data["extra_data"] = line[i:]
 
     rec_len = data.get("record_length", record_length)
     if check_record_length and rec_len:
         data["extra_data"] = str(data["extra_data"]).strip()
         if i != rec_len and data["extra_data"] != "":
             raise ValidationError(
-                _("Line {line}: Record length ({record_length}) does not match length of " 'parsed data ({data_length}). Extra data: "{extra_data}"').format(
+                _("Line {line}: Record length ({record_length}) does not match length of parsed data ({data_length}). Extra data: {extra_data}").format(
                     line=line_number,
                     data_length=i + len(str(data["extra_data"])),
                     record_length=rec_len,
                     extra_data=data["extra_data"],
                 )
             )
     return data
```

### Comparing `django-jbank-4.1.2/jbank/csr_helpers.py` & `django-jbank-4.1.3/jbank/csr_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/files.py` & `django-jbank-4.1.3/jbank/files.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html` & `django-jbank-4.1.3/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/admin/jbank/mark_as_manually_settled.html` & `django-jbank-4.1.3/jbank/templates/admin/jbank/mark_as_manually_settled.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/admin/jbank/statement/change_form.html` & `django-jbank-4.1.3/jbank/templates/admin/jbank/statement/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_certificate_status_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_certificate_status_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_create_certificate_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_create_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/soap_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_soap_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_renew_certificate_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/application_request_template-sha256.xml` & `django-jbank-4.1.3/jbank/templates/jbank/application_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/application_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/application_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/encryption_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/encryption_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml` & `django-jbank-4.1.3/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/templates/jbank/pki_soap_template.xml` & `django-jbank-4.1.3/jbank/templates/jbank/pki_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/locale/fi/LC_MESSAGES/django.mo` & `django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/locale/fi/LC_MESSAGES/django.po` & `django-jbank-4.1.3/jbank/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/locale/en/LC_MESSAGES/django.mo` & `django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/locale/en/LC_MESSAGES/django.po` & `django-jbank-4.1.3/jbank/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/Makefile` & `django-jbank-4.1.3/jbank/xmlsec1-examples/Makefile`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/encrypt3.c` & `django-jbank-4.1.3/jbank/xmlsec1-examples/encrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/sign3.c` & `django-jbank-4.1.3/jbank/xmlsec1-examples/sign3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/decrypt3.c` & `django-jbank-4.1.3/jbank/xmlsec1-examples/decrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/verify3.c` & `django-jbank-4.1.3/jbank/xmlsec1-examples/verify3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/xmlsec1-examples/sign3-sha256.c` & `django-jbank-4.1.3/jbank/xmlsec1-examples/sign3-sha256.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/pain002.py` & `django-jbank-4.1.3/jbank/pain002.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.1.2/jbank/euribor.py` & `django-jbank-4.1.3/jbank/euribor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 logger = logging.getLogger(__name__)
 
 
 def fetch_latest_euribor_rates(commit: bool = False, verbose: bool = False) -> List[EuriborRate]:
     feed_url = (
         "https://www.suomenpankki.fi/WebForms/ReportViewerPage.aspx?report=/tilastot/markkina-_ja_hallinnolliset_korot/euribor_korot_today_xml_en&output=xml"
     )
-    res = requests.get(feed_url)
+    res = requests.get(feed_url, timeout=60)
     if verbose:
         logger.info("GET %s HTTP %s\n%s", feed_url, res.status_code, res.content)
     if res.status_code >= 300:
         raise Exception(f"Failed to load Euribor rate feed from {feed_url}")
     results = xml_to_dict(res.content)
     data = results["data"]["period_Collection"]["period"]
     rates: List[EuriborRate] = []
```

### Comparing `django-jbank-4.1.2/jbank/tito.py` & `django-jbank-4.1.3/jbank/tito.py`

 * *Files identical despite different names*

