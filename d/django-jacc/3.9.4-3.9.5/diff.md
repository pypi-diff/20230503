# Comparing `tmp/django-jacc-3.9.4.tar.gz` & `tmp/django-jacc-3.9.5.tar.gz`

## Comparing `django-jacc-3.9.4.tar` & `django-jacc-3.9.5.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:45.000000 django-jacc-3.9.4/
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2021-07-12 15:07:39.000000 django-jacc-3.9.4/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)      174 2021-02-02 23:42:00.000000 django-jacc-3.9.4/requirements-dev.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)     7014 2021-07-12 15:07:39.000000 django-jacc-3.9.4/PKG-INFO
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:38.000000 django-jacc-3.9.4/htmlcov/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2349 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2375 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc_accountentry___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jquery.ba-throttle-debounce.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     4112 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_apps_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2347 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_management_commands___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     7025 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/style.css
--rw-rw-r--   0 jani      (1000) jani      (1000)    13665 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_management_commands_invoice_balance_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   146943 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_tests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jquery.hotkeys.js
--rw-rw-r--   0 jani      (1000) jani      (1000)      112 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/keybd_closed.png
--rw-rw-r--   0 jani      (1000) jani      (1000)     6301 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_helpers_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      112 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/keybd_open.png
--rw-rw-r--   0 jani      (1000) jani      (1000)     2365 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc_account___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2329 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_management___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_locale_fi___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    48331 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_settle_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2339 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_templates_admin___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    18620 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/coverage_html.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     6796 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jacc_forms_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   273289 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jacc_admin_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_templates___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_locale_en___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jquery.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)   164621 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_models_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jquery.isonscreen.js
--rw-rw-r--   0 jani      (1000) jani      (1000)    11561 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_management_commands_update_invoices_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    22039 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jacc_interests_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     2550 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/jquery.tablesorter.min.js
--rw-rw-r--   0 jani      (1000) jani      (1000)     2321 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/jacc_locale___init___py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     4634 2020-08-29 21:44:22.000000 django-jacc-3.9.4/htmlcov/manage_py.html
--rw-rw-r--   0 jani      (1000) jani      (1000)     9293 2021-01-04 05:13:02.000000 django-jacc-3.9.4/htmlcov/index.html
--rw-rw-r--   0 jani      (1000) jani      (1000)       53 2021-04-07 16:32:25.000000 django-jacc-3.9.4/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)       31 2021-07-12 15:07:23.000000 django-jacc-3.9.4/pyproject.toml
--rw-rw-r--   0 jani      (1000) jani      (1000)      929 2021-07-12 15:07:23.000000 django-jacc-3.9.4/setup.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/django_jacc.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)   646164 2021-07-12 15:07:38.000000 django-jacc-3.9.4/django_jacc.egg-info/SOURCES.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)     7014 2021-07-12 15:07:29.000000 django-jacc-3.9.4/django_jacc.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 14:03:44.000000 django-jacc-3.9.4/django_jacc.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2021-07-12 15:07:29.000000 django-jacc-3.9.4/django_jacc.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)       53 2021-07-12 15:07:29.000000 django-jacc-3.9.4/django_jacc.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        5 2021-07-12 15:07:29.000000 django-jacc-3.9.4/django_jacc.egg-info/top_level.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)     4576 2020-09-05 20:40:31.000000 django-jacc-3.9.4/README.md
--rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-26 16:13:29.000000 django-jacc-3.9.4/MANIFEST.in
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:41.000000 django-jacc-3.9.4/LICENSE.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      248 2020-05-26 15:11:48.000000 django-jacc-3.9.4/mypy.ini
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/
--rw-rw-r--   0 jani      (1000) jani      (1000)    36314 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/admin.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/templates/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/templates/admin/
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/templates/admin/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/accountentry/
--rw-rw-r--   0 jani      (1000) jani      (1000)      749 2020-09-01 23:33:32.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/accountentry/reverse_entry.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-09-01 20:02:28.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/accountentry/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/account/
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/account/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      774 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/templates/admin/jacc/account/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/templates/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    17499 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/tests.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:38.000000 django-jacc-3.9.4/jacc/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     5703 2021-04-24 00:45:32.000000 django-jacc-3.9.4/jacc/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    11474 2021-06-07 07:22:33.000000 django-jacc-3.9.4/jacc/locale/fi/LC_MESSAGES/django.po
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/locale/fi/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:38.000000 django-jacc-3.9.4/jacc/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1079 2021-04-24 00:45:32.000000 django-jacc-3.9.4/jacc/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     8418 2021-06-07 07:22:33.000000 django-jacc-3.9.4/jacc/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/locale/en/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/locale/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)      991 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/management/commands/update_invoices.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1413 2021-04-24 00:47:31.000000 django-jacc-3.9.4/jacc/management/commands/invoice_balance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/management/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      227 2021-04-07 16:33:20.000000 django-jacc-3.9.4/jacc/apps.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-12 15:07:39.000000 django-jacc-3.9.4/jacc/migrations/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2258 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0021_auto_20191209_2231.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      746 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0019_entrytype_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      475 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0003_auto_20171030_1933.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      458 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0013_auto_20180329_1052.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    16640 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0001_squashed_0014_auto_20180430_1506.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      442 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0020_auto_20191202_2332.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      383 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0004_auto_20171030_1935.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      415 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0009_accountentry_archived.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      544 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0008_auto_20180121_1705.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      812 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0012_auto_20180218_0638.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      614 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0011_auto_20180208_1146.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      522 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0002_auto_20171020_1331.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      503 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0006_account_name.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      486 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0026_alter_invoice_number.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      403 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0010_auto_20180201_0734.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.4/jacc/migrations/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1077 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0005_auto_20171030_1958.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      408 2021-04-24 00:47:31.000000 django-jacc-3.9.4/jacc/migrations/0024_account_notes.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1062 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0015_auto_20180505_1512.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      648 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0016_auto_20180505_1604.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      756 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0014_auto_20180430_1506.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2095 2021-03-11 21:56:53.000000 django-jacc-3.9.4/jacc/migrations/0023_accountentrynote.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      512 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0007_invoice_number.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1045 2021-07-09 18:10:30.000000 django-jacc-3.9.4/jacc/migrations/0025_alter_invoice_number.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      869 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0017_auto_20180807_1808.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      454 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/migrations/0018_auto_20181008_2322.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15109 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0001_initial.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4146 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/migrations/0022_auto_20200629_0346.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      506 2021-04-23 15:51:38.000000 django-jacc-3.9.4/jacc/helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      555 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/forms.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       44 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2560 2021-02-02 23:42:00.000000 django-jacc-3.9.4/jacc/interests.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    21844 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/models.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 15:11:48.000000 django-jacc-3.9.4/jacc/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)     9010 2021-07-12 15:07:23.000000 django-jacc-3.9.4/jacc/settle.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:23.000000 django-jacc-3.9.5/
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2021-07-27 18:37:17.000000 django-jacc-3.9.5/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)      174 2021-02-02 23:42:00.000000 django-jacc-3.9.5/requirements-dev.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7014 2021-07-27 18:37:17.000000 django-jacc-3.9.5/PKG-INFO
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:16.000000 django-jacc-3.9.5/htmlcov/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2349 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2375 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc_accountentry___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      731 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jquery.ba-throttle-debounce.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4112 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_apps_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2347 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_management_commands___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7025 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/style.css
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13665 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_management_commands_invoice_balance_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   146943 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_tests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3065 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jquery.hotkeys.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)      112 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/keybd_closed.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6301 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_helpers_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      112 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/keybd_open.png
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2365 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc_account___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2329 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_management___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_locale_fi___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    48331 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_settle_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2339 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_templates_admin___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18620 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/coverage_html.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6796 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jacc_forms_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   273289 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jacc_admin_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_templates___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2327 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_locale_en___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)   137549 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jquery.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)   164621 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_models_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1502 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jquery.isonscreen.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11561 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_management_commands_update_invoices_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22039 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jacc_interests_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2550 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12795 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/jquery.tablesorter.min.js
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2321 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/jacc_locale___init___py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4634 2020-08-29 21:44:22.000000 django-jacc-3.9.5/htmlcov/manage_py.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9293 2021-01-04 05:13:02.000000 django-jacc-3.9.5/htmlcov/index.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)       53 2021-04-07 16:32:25.000000 django-jacc-3.9.5/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)       31 2021-07-12 15:07:23.000000 django-jacc-3.9.5/pyproject.toml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      929 2021-07-27 18:37:00.000000 django-jacc-3.9.5/setup.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/django_jacc.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)   646164 2021-07-27 18:37:15.000000 django-jacc-3.9.5/django_jacc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7014 2021-07-27 18:37:07.000000 django-jacc-3.9.5/django_jacc.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 14:03:44.000000 django-jacc-3.9.5/django_jacc.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2021-07-27 18:37:07.000000 django-jacc-3.9.5/django_jacc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)       53 2021-07-27 18:37:07.000000 django-jacc-3.9.5/django_jacc.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        5 2021-07-27 18:37:07.000000 django-jacc-3.9.5/django_jacc.egg-info/top_level.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4576 2020-09-05 20:40:31.000000 django-jacc-3.9.5/README.md
+-rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-26 16:13:29.000000 django-jacc-3.9.5/MANIFEST.in
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:41.000000 django-jacc-3.9.5/LICENSE.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      248 2020-05-26 15:11:48.000000 django-jacc-3.9.5/mypy.ini
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    36314 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/admin.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/templates/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/templates/admin/
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/templates/admin/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/accountentry/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      749 2020-09-01 23:33:32.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/accountentry/reverse_entry.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-09-01 20:02:28.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/accountentry/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/account/
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/account/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      774 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/templates/admin/jacc/account/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/templates/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    17499 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/tests.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:16.000000 django-jacc-3.9.5/jacc/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5703 2021-04-24 00:45:32.000000 django-jacc-3.9.5/jacc/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11474 2021-06-07 07:22:33.000000 django-jacc-3.9.5/jacc/locale/fi/LC_MESSAGES/django.po
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/locale/fi/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:16.000000 django-jacc-3.9.5/jacc/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1079 2021-04-24 00:45:32.000000 django-jacc-3.9.5/jacc/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8418 2021-06-07 07:22:33.000000 django-jacc-3.9.5/jacc/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/locale/en/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/locale/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      991 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/management/commands/update_invoices.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1413 2021-04-24 00:47:31.000000 django-jacc-3.9.5/jacc/management/commands/invoice_balance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/management/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      227 2021-04-07 16:33:20.000000 django-jacc-3.9.5/jacc/apps.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2021-07-27 18:37:17.000000 django-jacc-3.9.5/jacc/migrations/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2258 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0021_auto_20191209_2231.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      746 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0019_entrytype_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      475 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0003_auto_20171030_1933.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      458 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0013_auto_20180329_1052.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    16640 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0001_squashed_0014_auto_20180430_1506.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      442 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0020_auto_20191202_2332.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      383 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0004_auto_20171030_1935.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      415 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0009_accountentry_archived.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      544 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0008_auto_20180121_1705.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      812 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0012_auto_20180218_0638.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      614 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0011_auto_20180208_1146.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      522 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0002_auto_20171020_1331.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      503 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0006_account_name.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      486 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0026_alter_invoice_number.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      403 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0010_auto_20180201_0734.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2020-05-21 16:43:41.000000 django-jacc-3.9.5/jacc/migrations/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1077 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0005_auto_20171030_1958.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      408 2021-04-24 00:47:31.000000 django-jacc-3.9.5/jacc/migrations/0024_account_notes.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1062 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0015_auto_20180505_1512.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      648 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0016_auto_20180505_1604.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      756 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0014_auto_20180430_1506.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2095 2021-03-11 21:56:53.000000 django-jacc-3.9.5/jacc/migrations/0023_accountentrynote.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      512 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0007_invoice_number.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1045 2021-07-09 18:10:30.000000 django-jacc-3.9.5/jacc/migrations/0025_alter_invoice_number.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      869 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0017_auto_20180807_1808.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      454 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/migrations/0018_auto_20181008_2322.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15109 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0001_initial.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4146 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/migrations/0022_auto_20200629_0346.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      506 2021-04-23 15:51:38.000000 django-jacc-3.9.5/jacc/helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      555 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/forms.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       44 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2560 2021-02-02 23:42:00.000000 django-jacc-3.9.5/jacc/interests.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    21862 2021-07-27 18:37:00.000000 django-jacc-3.9.5/jacc/models.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 15:11:48.000000 django-jacc-3.9.5/jacc/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9010 2021-07-12 15:07:23.000000 django-jacc-3.9.5/jacc/settle.py
```

### Comparing `django-jacc-3.9.4/PKG-INFO` & `django-jacc-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-jacc
-Version: 3.9.4
+Version: 3.9.5
 Summary: Simple double entry accounting system (debits/credits) for Django projects.
 Home-page: https://github.com/kajala/django-jacc
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 Description: django-jacc
         ===========
```

### Comparing `django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc_accountentry___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc_accountentry___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jquery.ba-throttle-debounce.min.js` & `django-jacc-3.9.5/htmlcov/jquery.ba-throttle-debounce.min.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_apps_py.html` & `django-jacc-3.9.5/htmlcov/jacc_apps_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_management_commands___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_management_commands___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/style.css` & `django-jacc-3.9.5/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_management_commands_invoice_balance_py.html` & `django-jacc-3.9.5/htmlcov/jacc_management_commands_invoice_balance_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_tests_py.html` & `django-jacc-3.9.5/htmlcov/jacc_tests_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jquery.hotkeys.js` & `django-jacc-3.9.5/htmlcov/jquery.hotkeys.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_helpers_py.html` & `django-jacc-3.9.5/htmlcov/jacc_helpers_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_templates_admin_jacc_account___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_templates_admin_jacc_account___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_management___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_management___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_locale_fi___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_locale_fi___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_settle_py.html` & `django-jacc-3.9.5/htmlcov/jacc_settle_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_templates_admin___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_templates_admin___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/coverage_html.js` & `django-jacc-3.9.5/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_forms_py.html` & `django-jacc-3.9.5/htmlcov/jacc_forms_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_admin_py.html` & `django-jacc-3.9.5/htmlcov/jacc_admin_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_templates___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_templates___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_locale_en___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_locale_en___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jquery.min.js` & `django-jacc-3.9.5/htmlcov/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_models_py.html` & `django-jacc-3.9.5/htmlcov/jacc_models_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jquery.isonscreen.js` & `django-jacc-3.9.5/htmlcov/jquery.isonscreen.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_management_commands_update_invoices_py.html` & `django-jacc-3.9.5/htmlcov/jacc_management_commands_update_invoices_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_interests_py.html` & `django-jacc-3.9.5/htmlcov/jacc_interests_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jquery.tablesorter.min.js` & `django-jacc-3.9.5/htmlcov/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/jacc_locale___init___py.html` & `django-jacc-3.9.5/htmlcov/jacc_locale___init___py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/manage_py.html` & `django-jacc-3.9.5/htmlcov/manage_py.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/htmlcov/index.html` & `django-jacc-3.9.5/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/setup.py` & `django-jacc-3.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jacc",
-    version="3.9.4",
+    version="3.9.5",
     author=u"Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="https://github.com/kajala/django-jacc",
     license="MIT licence, see LICENCE.txt",
     description="Simple double entry accounting system (debits/credits) for Django projects.",
```

### Comparing `django-jacc-3.9.4/django_jacc.egg-info/SOURCES.txt` & `django-jacc-3.9.5/django_jacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/django_jacc.egg-info/PKG-INFO` & `django-jacc-3.9.5/django_jacc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-jacc
-Version: 3.9.4
+Version: 3.9.5
 Summary: Simple double entry accounting system (debits/credits) for Django projects.
 Home-page: https://github.com/kajala/django-jacc
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 Description: django-jacc
         ===========
```

### Comparing `django-jacc-3.9.4/README.md` & `django-jacc-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/LICENSE.txt` & `django-jacc-3.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/admin.py` & `django-jacc-3.9.5/jacc/admin.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/templates/admin/jacc/accountentry/reverse_entry.html` & `django-jacc-3.9.5/jacc/templates/admin/jacc/accountentry/reverse_entry.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/templates/admin/jacc/account/change_form.html` & `django-jacc-3.9.5/jacc/templates/admin/jacc/account/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/tests.py` & `django-jacc-3.9.5/jacc/tests.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/locale/fi/LC_MESSAGES/django.mo` & `django-jacc-3.9.5/jacc/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/locale/fi/LC_MESSAGES/django.po` & `django-jacc-3.9.5/jacc/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/locale/en/LC_MESSAGES/django.mo` & `django-jacc-3.9.5/jacc/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/locale/en/LC_MESSAGES/django.po` & `django-jacc-3.9.5/jacc/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/management/commands/update_invoices.py` & `django-jacc-3.9.5/jacc/management/commands/update_invoices.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/management/commands/invoice_balance.py` & `django-jacc-3.9.5/jacc/management/commands/invoice_balance.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0021_auto_20191209_2231.py` & `django-jacc-3.9.5/jacc/migrations/0021_auto_20191209_2231.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0019_entrytype_identifier.py` & `django-jacc-3.9.5/jacc/migrations/0019_entrytype_identifier.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0001_squashed_0014_auto_20180430_1506.py` & `django-jacc-3.9.5/jacc/migrations/0001_squashed_0014_auto_20180430_1506.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0008_auto_20180121_1705.py` & `django-jacc-3.9.5/jacc/migrations/0008_auto_20180121_1705.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0012_auto_20180218_0638.py` & `django-jacc-3.9.5/jacc/migrations/0012_auto_20180218_0638.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0011_auto_20180208_1146.py` & `django-jacc-3.9.5/jacc/migrations/0011_auto_20180208_1146.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0002_auto_20171020_1331.py` & `django-jacc-3.9.5/jacc/migrations/0002_auto_20171020_1331.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0005_auto_20171030_1958.py` & `django-jacc-3.9.5/jacc/migrations/0005_auto_20171030_1958.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0015_auto_20180505_1512.py` & `django-jacc-3.9.5/jacc/migrations/0015_auto_20180505_1512.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0016_auto_20180505_1604.py` & `django-jacc-3.9.5/jacc/migrations/0016_auto_20180505_1604.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0014_auto_20180430_1506.py` & `django-jacc-3.9.5/jacc/migrations/0014_auto_20180430_1506.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0023_accountentrynote.py` & `django-jacc-3.9.5/jacc/migrations/0023_accountentrynote.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0007_invoice_number.py` & `django-jacc-3.9.5/jacc/migrations/0007_invoice_number.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0025_alter_invoice_number.py` & `django-jacc-3.9.5/jacc/migrations/0025_alter_invoice_number.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0017_auto_20180807_1808.py` & `django-jacc-3.9.5/jacc/migrations/0017_auto_20180807_1808.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0001_initial.py` & `django-jacc-3.9.5/jacc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/migrations/0022_auto_20200629_0346.py` & `django-jacc-3.9.5/jacc/migrations/0022_auto_20200629_0346.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/forms.py` & `django-jacc-3.9.5/jacc/forms.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/interests.py` & `django-jacc-3.9.5/jacc/interests.py`

 * *Files identical despite different names*

### Comparing `django-jacc-3.9.4/jacc/models.py` & `django-jacc-3.9.5/jacc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     notes = models.TextField(_("notes"), blank=True, default="")
 
     class Meta:
         verbose_name = _("account")
         verbose_name_plural = _("accounts")
 
     def __str__(self):
-        return "[{}] {}".format(self.id, self.name)
+        return "[{}] {}".format(self.id, self.name or self.type.name)
 
     def is_asset(self) -> bool:
         return self.type.is_asset
 
     is_asset.boolean = True  # type: ignore
     is_asset.short_description = _("asset")  # type: ignore
```

### Comparing `django-jacc-3.9.4/jacc/settle.py` & `django-jacc-3.9.5/jacc/settle.py`

 * *Files identical despite different names*

