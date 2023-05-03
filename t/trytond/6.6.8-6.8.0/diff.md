# Comparing `tmp/trytond-6.6.8.tar.gz` & `tmp/trytond-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-6.6.8.tar", last modified: Wed May  3 16:22:48 2023, max compression
+gzip compressed data, was "trytond-6.8.0.tar", last modified: Mon May  1 11:25:19 2023, max compression
```

## Comparing `trytond-6.6.8.tar` & `trytond-6.8.0.tar`

### file list

```diff
@@ -1,589 +1,597 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.782117 trytond-6.6.8/
--rw-r--r--   0 ced       (1000) ced       (1000)    37923 2023-05-03 16:22:44.000000 trytond-6.6.8/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-05-03 16:22:44.000000 trytond-6.6.8/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond-6.6.8/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2022-12-19 12:02:59.000000 trytond-6.6.8/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2626 2023-05-03 16:22:48.782117 trytond-6.6.8/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2022-12-19 12:02:59.000000 trytond-6.6.8/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.515447 trytond-6.6.8/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2888 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond
--rwxr-xr-x   0 ced       (1000) ced       (1000)      807 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond-admin
--rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond-console
--rwxr-xr-x   0 ced       (1000) ced       (1000)      889 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond-cron
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond-stat
--rwxr-xr-x   0 ced       (1000) ced       (1000)      898 2023-04-13 16:52:41.000000 trytond-6.6.8/bin/trytond-worker
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.515447 trytond-6.6.8/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.532114 trytond-6.6.8/doc/ref/
--rw-r--r--   0 ced       (1000) ced       (1000)    10224 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/backend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2452 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/cache.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2443 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/exceptions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31448 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/filestore.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/i18n.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    30579 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/models.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/pool.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/pyson.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/sendmail.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3139 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tests.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.535447 trytond-6.6.8/doc/ref/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/immutabledict.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1150 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/misc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/singleton.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/tools/timezone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/transaction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6056 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/ref/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.555448 trytond-6.6.8/doc/topics/
--rw-r--r--   0 ced       (1000) ced       (1000)     3717 2022-12-19 12:02:59.000000 trytond-6.6.8/doc/topics/access_rights.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2022-12-19 12:02:59.000000 trytond-6.6.8/doc/topics/actions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3751 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/backend_types.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14273 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/cron.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/domain.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/install.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/logs.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.555448 trytond-6.6.8/doc/topics/models/
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/models/fields_default_value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/models/fields_on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/models/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.558781 trytond-6.6.8/doc/topics/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/modules/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/pyson.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.558781 trytond-6.6.8/doc/topics/reports/
--rw-r--r--   0 ced       (1000) ced       (1000)     7765 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/reports/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2022-12-19 12:02:59.000000 trytond-6.6.8/doc/topics/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/start_server.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/task_queue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2880 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/testing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/translation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/triggers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/user_errors_warnings.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.558781 trytond-6.6.8/doc/topics/views/
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/views/extension.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    24473 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/views/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/topics/wizard.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.558781 trytond-6.6.8/doc/tutorial/
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.568781 trytond-6.6.8/doc/tutorial/module/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/anatomy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/default_values.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/domains.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/extend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/function_fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3935 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/model.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3722 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/states.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4745 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/table_query.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4773 2023-04-13 16:52:41.000000 trytond-6.6.8/doc/tutorial/module/workflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-03 16:22:48.782117 trytond-6.6.8/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5274 2023-04-13 16:52:41.000000 trytond-6.6.8/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-13 16:52:41.000000 trytond-6.6.8/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.582115 trytond-6.6.8/trytond/
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6290 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/admin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/application.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.582115 trytond-6.6.8/trytond/backend/
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4381 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/database.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.585448 trytond-6.6.8/trytond/backend/postgresql/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/postgresql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25952 2023-04-19 08:56:47.000000 trytond-6.6.8/trytond/backend/postgresql/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4312 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/backend/postgresql/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    25570 2023-04-19 08:56:47.000000 trytond-6.6.8/trytond/backend/postgresql/table.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.585448 trytond-6.6.8/trytond/backend/sqlite/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/sqlite/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20777 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/sqlite/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2209 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/backend/sqlite/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    16323 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/sqlite/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/backend/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9621 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16335 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6958 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/commandline.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6154 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/console.py
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31326 2023-04-13 17:20:35.000000 trytond-6.6.8/trytond/convert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/i18n.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.608782 trytond-6.6.8/trytond/ir/
--rw-r--r--   0 ced       (1000) ced       (1000)     3310 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    40399 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9920 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/action.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4059 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/attachment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4282 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/calendar_.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7391 2023-04-22 21:13:14.000000 trytond-6.6.8/trytond/ir/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/cron.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4525 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/email.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20559 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/error.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/error.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/export.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/export.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.608782 trytond-6.6.8/trytond/ir/fonts/
--rw-r--r--   0 ced       (1000) ced       (1000)     4384 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/fonts/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    58284 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/fonts/karla.ttf
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21152 2023-04-13 17:16:42.000000 trytond-6.6.8/trytond/ir/lang.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27227 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/lang.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.635449 trytond-6.6.8/trytond/ir/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    97303 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96664 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    83941 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98256 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97525 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    79052 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90670 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    99484 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    83616 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98237 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93192 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    83139 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93082 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88943 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88889 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96017 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96131 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93999 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88293 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    99735 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92244 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    83752 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   108492 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93039 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/message.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21563 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    55800 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14735 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/ir/model.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21140 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8376 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/module.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/note.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/queue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9475 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/queue_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-13 17:03:36.000000 trytond-6.6.8/trytond/ir/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10318 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11695 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4927 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5587 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/session.py
--rw-r--r--   0 ced       (1000) ced       (1000)    66706 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/ir/translation.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7726 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/translation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12039 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/trigger.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.642115 trytond-6.6.8/trytond/ir/ui/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/board.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    18063 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/board.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/calendar.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     3508 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/calendar.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     9660 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/form.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    32848 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/form.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/graph.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5214 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/graph.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2520 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/icon.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1521 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icon.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.645449 trytond-6.6.8/trytond/ir/ui/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-board.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-calendar.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-folder.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-form.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-graph.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-list.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-settings.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/icons/tryton-tree.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     9271 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2962 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/menu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3719 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/ir/ui/tree.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    12969 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/tree.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/ui/ui.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22383 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/view.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7956 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/ui/view.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.685449 trytond-6.6.8/trytond/ir/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_domain_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_domain_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_domain_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1698 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_act_window_view_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/ir/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/action_report_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_report_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_wizard_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/action_wizard_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/attachment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/attachment_form_preview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/attachment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/email_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/ir/view/error_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/error_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/export_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/export_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/icon_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/icon_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/lang_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/lang_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/lang_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_button_click_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_button_click_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/model_button_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_button_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_button_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_button_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      870 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_data_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/model_data_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_field_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_field_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      679 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_field_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/ir/view/model_field_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/model_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/model_print_model_graph_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_activate_upgrade_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_activate_upgrade_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/module_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_config_wizard_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_config_wizard_first_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/module_config_wizard_item_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_config_wizard_other_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_dependency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_dependency_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/module_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/module_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/note_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/note_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1064 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/rule_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/rule_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1620 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/ir/view/sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/sequence_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_clean_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_clean_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_export_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/translation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_set_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_set_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/translation_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1035 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/trigger_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/trigger_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_menu_favorite_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      279 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_menu_favorite_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      625 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_menu_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_menu_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_menu_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/ui_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/ir/view/ui_view_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_search_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_optional_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_optional_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_state_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_state_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_width_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/ir/view/ui_view_tree_width_list.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.692116 trytond-6.6.8/trytond/model/
--rw-r--r--   0 ced       (1000) ced       (1000)     1133 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/active.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1050 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/model/descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9337 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/dictschema.py
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/digits.py
--rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/model/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.698783 trytond-6.6.8/trytond/model/fields/
--rw-r--r--   0 ced       (1000) ced       (1000)     1286 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9577 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7104 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8246 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26532 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/model/fields/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7603 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/model/fields/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18715 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13834 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4288 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14468 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/model/fields/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8256 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7298 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/model/fields/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3517 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/fields/text.py
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/model/match.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17168 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4238 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    82947 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    83391 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34939 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1102 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/model/order.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/model/symbol.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/model/union.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/model/workflow.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.702116 trytond-6.6.8/trytond/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)    15965 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/modules/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9247 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/pool.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.702116 trytond-6.6.8/trytond/protocols/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/protocols/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8063 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/protocols/dispatcher.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5759 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/protocols/jsonrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8400 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/protocols/wrappers.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/protocols/xmlrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22275 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.702116 trytond-6.6.8/trytond/report/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/report/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19057 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/report/report.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.708783 trytond-6.6.8/trytond/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2674 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/group.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9576 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    55265 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/res/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.718783 trytond-6.6.8/trytond/res/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    15093 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15563 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13288 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15814 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15739 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12898 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14652 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15438 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/res/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13249 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16048 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14827 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13959 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14279 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16836 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15110 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15516 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/res/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15538 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14453 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15531 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15287 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14393 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13249 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17623 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14880 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/res/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2486 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/res/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)    43748 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/res/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8284 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.725450 trytond-6.6.8/trytond/res/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1153 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/user_application_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/user_application_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/user_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1511 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/res/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/res/view/user_form_preferences.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/res/view/user_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/user_warning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/res/view/user_warning_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3476 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4804 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/security.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4965 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3205 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/status.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.778784 trytond-6.6.8/trytond/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     2419 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/copy_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1989 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/export_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2213 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/field_function.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6725 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/tests/field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4696 2023-04-08 09:35:50.000000 trytond-6.6.8/trytond/tests/field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3123 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1489 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1224 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)        9 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/forbidden.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/import_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/import_data.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7180 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6484 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8349 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/modelview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/path.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)      971 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    34615 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6538 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_backend.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9021 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11016 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_copy.py
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14582 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_exportdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6048 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_depends.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2897 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10316 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24044 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14245 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11134 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16606 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20430 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9686 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20443 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8106 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15175 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3648 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_i18n.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19311 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_importdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15623 2023-04-13 16:52:41.000000 trytond-6.6.8/trytond/tests/test_ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_mixins.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13792 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4393 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_model_index.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47667 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28317 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23731 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3471 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      958 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_path.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_protocols.py
--rw-r--r--   0 ced       (1000) ced       (1000)    33898 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2326 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2413 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26679 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4323 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5020 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)    38151 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11788 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)    41333 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_tryton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_union.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11988 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3151 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/test_wsgi.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tests/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tests/workflow.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.782117 trytond-6.6.8/trytond/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/decimal_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17106 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tools/gevent.py
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/immutabledict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9313 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/misc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3893 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tools/singleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/string_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/tools/timezone.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tryton.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2022-12-19 12:02:59.000000 trytond-6.6.8/trytond/tryton.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2754 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/url.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.782117 trytond-6.6.8/trytond/wizard/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/wizard/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13781 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/wizard/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6372 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/worker.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9598 2023-04-13 16:52:42.000000 trytond-6.6.8/trytond/wsgi.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:22:48.582115 trytond-6.6.8/trytond.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2626 2023-05-03 16:22:47.000000 trytond-6.6.8/trytond.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    16050 2023-05-03 16:22:48.000000 trytond-6.6.8/trytond.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:22:47.000000 trytond-6.6.8/trytond.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 21:28:03.000000 trytond-6.6.8/trytond.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-05-03 16:22:47.000000 trytond-6.6.8/trytond.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-03 16:22:47.000000 trytond-6.6.8/trytond.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.690296 trytond-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    38579 2023-05-01 10:56:22.000000 trytond-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-05-01 10:56:22.000000 trytond-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-04-15 07:12:15.000000 trytond-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-05-01 11:25:19.690296 trytond-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-04-15 07:12:16.000000 trytond-6.8.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.546960 trytond-6.8.0/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2888 2023-04-15 07:12:16.000000 trytond-6.8.0/bin/trytond
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      807 2023-04-15 07:12:16.000000 trytond-6.8.0/bin/trytond-admin
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-04-15 07:12:15.000000 trytond-6.8.0/bin/trytond-console
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      889 2023-04-15 07:12:15.000000 trytond-6.8.0/bin/trytond-cron
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-04-15 07:12:16.000000 trytond-6.8.0/bin/trytond-stat
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond-6.8.0/bin/trytond-worker
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.546960 trytond-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.550294 trytond-6.8.0/doc/ref/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10247 2023-04-30 10:46:36.000000 trytond-6.8.0/doc/ref/backend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/cache.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/exceptions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31979 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/filestore.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/i18n.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31703 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/ref/models.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/pool.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/pyson.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1461 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/sendmail.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3139 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/tests.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.550294 trytond-6.8.0/doc/ref/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/tools/barcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-29 22:04:03.000000 trytond-6.8.0/doc/ref/tools/email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/tools/immutabledict.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/tools/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1313 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/tools/misc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/tools/qrcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/tools/singleton.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/tools/timezone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5510 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/ref/transaction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6056 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/ref/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/topics/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3717 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/access_rights.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/actions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4014 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/backend_types.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14772 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/cron.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/domain.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/install.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/logs.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/topics/models/
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/topics/models/fields_default_value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/models/fields_on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/models/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/topics/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/modules/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/pyson.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/topics/reports/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/topics/reports/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/start_server.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/task_queue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2880 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/testing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/translation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/triggers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/user_errors_warnings.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/topics/views/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/topics/views/extension.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    25050 2023-04-28 07:46:16.000000 trytond-6.8.0/doc/topics/views/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/topics/wizard.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.553627 trytond-6.8.0/doc/tutorial/
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.556960 trytond-6.8.0/doc/tutorial/module/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/tutorial/module/anatomy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/default_values.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/domains.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/extend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/tutorial/module/function_fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/tutorial/module/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3935 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/model.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/tutorial/module/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/states.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4746 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/tutorial/module/table_query.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-04-15 07:12:15.000000 trytond-6.8.0/doc/tutorial/module/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2023-04-21 08:36:08.000000 trytond-6.8.0/doc/tutorial/module/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4773 2023-04-15 07:12:16.000000 trytond-6.8.0/doc/tutorial/module/workflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:25:19.690296 trytond-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5418 2023-04-29 22:04:03.000000 trytond-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-04-29 22:04:03.000000 trytond-6.8.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.560294 trytond-6.8.0/trytond/
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-05-01 10:56:15.000000 trytond-6.8.0/trytond/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6777 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/admin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/application.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.563627 trytond-6.8.0/trytond/backend/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/backend/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4390 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/backend/database.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.563627 trytond-6.8.0/trytond/backend/postgresql/
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/backend/postgresql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26462 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/backend/postgresql/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3631 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/backend/postgresql/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    26758 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/backend/postgresql/table.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.563627 trytond-6.8.0/trytond/backend/sqlite/
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/backend/sqlite/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20773 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/backend/sqlite/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2209 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/backend/sqlite/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    16323 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/backend/sqlite/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/backend/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16982 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7095 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/commandline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6437 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2280 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/console.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31266 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/convert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/i18n.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.570294 trytond-6.8.0/trytond/ir/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3329 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    41248 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9920 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/action.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4059 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/attachment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/calendar_.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7783 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/ir/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/cron.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4525 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/email.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20472 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/ir/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/error.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/error.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/export.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.570294 trytond-6.8.0/trytond/ir/fonts/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/fonts/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/fonts/karla.ttf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    21357 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/ir/lang.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27227 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/lang.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.576961 trytond-6.8.0/trytond/ir/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   100724 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99739 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87078 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101295 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100595 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81805 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93862 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   102927 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86753 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101311 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96718 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86440 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96368 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92224 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92210 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99075 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99407 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97205 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92005 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103100 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95508 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86889 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   111911 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96295 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/ir/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/message.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21762 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    61326 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16085 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/model.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20966 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8376 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/module.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/note.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/queue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9445 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/queue_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6477 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10150 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11734 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/session.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    67166 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/ir/translation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/translation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12236 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/trigger.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.580294 trytond-6.8.0/trytond/ir/ui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/board.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    18063 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/board.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/ui/calendar.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     3508 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/calendar.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     9858 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/form.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    33494 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/form.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/graph.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5214 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/graph.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2520 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/icon.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/icon.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.583628 trytond-6.8.0/trytond/ir/ui/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/ui/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-board.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-calendar.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-folder.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-form.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-graph.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-list.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-settings.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/ui/icons/tryton-tree.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     9173 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/menu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3818 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/ir/ui/tree.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    13292 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/ir/ui/tree.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/ui.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22402 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/view.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7956 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/ui/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.606961 trytond-6.8.0/trytond/ir/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_domain_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_domain_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_domain_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1698 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/action_act_window_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_act_window_view_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_report_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_report_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/action_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/action_wizard_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/action_wizard_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/attachment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/attachment_form_preview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/attachment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/email_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/error_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/error_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/export_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/export_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/icon_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/icon_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/lang_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/lang_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/lang_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/model_button_click_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/model_button_click_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_button_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_button_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/model_button_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_button_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      870 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/model_data_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_data_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_field_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_field_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      679 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_field_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond-6.8.0/trytond/ir/view/model_field_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/model_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/model_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/view/model_log_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/ir/view/model_log_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/model_print_model_graph_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_activate_upgrade_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_activate_upgrade_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/module_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_config_wizard_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_config_wizard_first_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/module_config_wizard_item_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_config_wizard_other_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_dependency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_dependency_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/module_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/module_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/note_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/note_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1064 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/rule_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/rule_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1620 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/sequence_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_clean_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_clean_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/translation_export_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/translation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_set_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/translation_set_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/translation_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/trigger_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/trigger_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_menu_favorite_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      279 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_menu_favorite_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_menu_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_menu_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_menu_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_search_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_optional_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_optional_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_state_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_state_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_width_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/ir/view/ui_view_tree_width_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.613628 trytond-6.8.0/trytond/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1177 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/active.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/model/descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9337 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/dictschema.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/digits.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.620295 trytond-6.8.0/trytond/model/fields/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9577 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7104 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8280 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27311 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/model/fields/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7529 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/model/fields/function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18790 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14244 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16083 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/model/fields/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8320 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7628 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3517 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/fields/text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17168 2023-04-29 09:36:56.000000 trytond-6.8.0/trytond/model/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    86283 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/model/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    82807 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/model/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    36331 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/model/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/symbol.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/model/union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-04-28 07:46:16.000000 trytond-6.8.0/trytond/model/workflow.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.620295 trytond-6.8.0/trytond/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16062 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/modules/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9456 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/pool.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.623628 trytond-6.8.0/trytond/protocols/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/protocols/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8468 2023-04-27 20:01:07.000000 trytond-6.8.0/trytond/protocols/dispatcher.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5759 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/protocols/jsonrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9054 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/protocols/wrappers.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/protocols/xmlrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22275 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.623628 trytond-6.8.0/trytond/report/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/report/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19856 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/report/report.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.626961 trytond-6.8.0/trytond/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/res/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2674 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/group.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9576 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    39551 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/res/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.636962 trytond-6.8.0/trytond/res/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14621 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15011 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12816 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15227 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12426 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14090 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14966 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15436 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14355 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13372 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16364 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14553 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14944 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14961 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14922 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14815 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13921 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16986 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14333 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/res/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/res/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)    43825 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/res/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8284 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.640295 trytond-6.8.0/trytond/res/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/res/view/user_application_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/res/view/user_application_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/user_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1527 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1386 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/user_form_preferences.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/res/view/user_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/res/view/user_warning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/res/view/user_warning_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3644 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4804 2023-04-27 20:16:31.000000 trytond-6.8.0/trytond/security.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4965 2023-04-29 12:31:47.000000 trytond-6.8.0/trytond/sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3205 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/status.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.683629 trytond-6.8.0/trytond/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/copy_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1989 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/export_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_function.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7491 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/forbidden.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/import_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/import_data.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/tests/model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7377 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/tests/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7720 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8349 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/modelview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    34615 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6538 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_backend.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9968 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11841 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_copy.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14582 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_exportdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6048 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_depends.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3626 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10440 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25082 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15081 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12677 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16606 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23584 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9821 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20600 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15175 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3648 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_i18n.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19311 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_importdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16316 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/tests/test_ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_mixins.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13792 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4393 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_model_index.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/tests/test_model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51742 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/tests/test_modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31235 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24647 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_protocols.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    33898 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2413 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2023-04-30 10:46:36.000000 trytond-6.8.0/trytond/tests/test_routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26679 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4323 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5020 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    39952 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11788 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42503 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_tryton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11988 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/test_wsgi.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tests/workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tests/workflow.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.686962 trytond-6.8.0/trytond/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/barcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/decimal_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-04-29 22:04:03.000000 trytond-6.8.0/trytond/tools/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/gevent.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/immutabledict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9313 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/misc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3893 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1595 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/qrcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-01-16 14:00:21.000000 trytond-6.8.0/trytond/tools/singleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/string_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tools/timezone.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12661 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tryton.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/tryton.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/url.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.690296 trytond-6.8.0/trytond/wizard/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/wizard/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14525 2023-04-21 08:36:08.000000 trytond-6.8.0/trytond/wizard/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6882 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/worker.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9486 2023-04-15 07:12:16.000000 trytond-6.8.0/trytond/wsgi.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:25:19.560294 trytond-6.8.0/trytond.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-05-01 11:25:18.000000 trytond-6.8.0/trytond.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    16279 2023-05-01 11:25:19.000000 trytond-6.8.0/trytond.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:25:18.000000 trytond-6.8.0/trytond.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond-6.8.0/trytond.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 11:25:18.000000 trytond-6.8.0/trytond.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:25:18.000000 trytond-6.8.0/trytond.egg-info/top_level.txt
```

### Comparing `trytond-6.6.8/CHANGELOG` & `trytond-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 
-Version 6.6.8 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.7 - 2023-04-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.6 - 2023-03-03
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Support return instances for Function getter and on_change_with
+* Log events for ModelStorage
+* Use IDENTITY column for id columns in the postgresql backend
+* Use no breaking space to format number and date
+* Fallback to code to format currency without symbol
+* Add sort method to order like ModelStorage.search
 * Do not alter argument values of with_transaction decorator (#12108)
-
-Version 6.6.5 - 2023-02-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.4 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.3 - 2023-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-01-02
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2022-11-17
---------------------------
-* Bug fixes (see mercurial logs for details)
+* Support SMALLINT and REAL as backend types
+* Remove BigInteger field
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Add scroll time for calendar view
+* Allow cache size to be configured
+* Add local and global list of ignore context keys
+* Add functions in transaction for check access and active record
+* Add check_access and active_records attribute to Transaction
+* Add searchable and sortable methods on Field
+* Add support for barcode and QR code
+* Support reading string value of selection fields
+* Add ButtonActionException and RPCReturnException
+* Rename ModelStorage.count into ModelStorage.estimated_count
+* Add border type to images
+* Lock table on transaction start
+* Use EXISTS for search on O2M with many records
+* Replace target_search by use of count()
+* Manage domain on id in single value list as unique
+* Do not validate domain for empty fields
+* Warn about implicit save() of unsaved relation
+* Raise error message with record name and field in check_xml_record
+* Cache RPC call for class method selection
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add sql_id method to Reference field
 * Use declarative index definition for ModelSQL
 * Add configuration entries for unaccent and similarity functions
```

### Comparing `trytond-6.6.8/COPYRIGHT` & `trytond-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/LICENSE` & `trytond-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/PKG-INFO` & `trytond-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 6.6.8
+Version: 6.8.0
 Summary: Tryton server
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
-Project-URL: Source Code, https://hg.tryton.org/trytond
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: business application platform ERP
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -38,31 +38,33 @@
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
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: PostgreSQL
 Provides-Extra: graphviz
 Provides-Extra: Levenshtein
 Provides-Extra: BCrypt
 Provides-Extra: Argon2
 Provides-Extra: html2text
 Provides-Extra: weasyprint
 Provides-Extra: coroutine
 Provides-Extra: image
+Provides-Extra: barcode
+Provides-Extra: qrcode
 Provides-Extra: completion
 License-File: LICENSE
 
 trytond
 =======
 
 The server of Tryton.
```

### Comparing `trytond-6.6.8/bin/trytond` & `trytond-6.8.0/bin/trytond`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/bin/trytond-admin` & `trytond-6.8.0/bin/trytond-admin`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/bin/trytond-console` & `trytond-6.8.0/bin/trytond-console`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/bin/trytond-cron` & `trytond-6.8.0/bin/trytond-cron`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/bin/trytond-stat` & `trytond-6.8.0/bin/trytond-stat`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/bin/trytond-worker` & `trytond-6.8.0/bin/trytond-worker`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/conf.py` & `trytond-6.8.0/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,18 @@
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
 
     return info
```

### Comparing `trytond-6.6.8/doc/index.rst` & `trytond-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/backend.rst` & `trytond-6.8.0/doc/ref/backend.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 .. method:: Database.connect()
 
    Connect to the database and return the instance.
 
 .. method:: Database.get_connection([autocommit[, readonly]])
 
-   Retrieve a connection object as defined by :pep:249#connection.
+   Retrieve a connection object as defined by :pep:`249#connection`.
    If autocommit is set, the connection is committed after each statement.
    If readonly is set, the connection is read only.
 
 .. method:: Database.put_connection(connection[, close])
 
    Release the connection.
    If close is set, the connection is discarded.
@@ -61,17 +61,17 @@
 
 .. method:: Database.test([hostname])
 
    Return if the database is a Tryton database.
    If ``hostname`` is set, it checks also if it has the same configured
    hostname.
 
-.. method:: Database.nextid(connection, table)
+.. method:: Database.nextid(connection, table[, count])
 
-   Return the next ID for the ``table`` using the ``connection``.
+   Return the next ``count`` IDs for the ``table`` using the ``connection``.
 
    .. note:: It may return ``None`` for some database.
 
 .. method:: Database.setnextid(connection, table, value)
 
    Set the ``value`` as current ID to the ``table`` using the ``connection``.
 
@@ -168,16 +168,16 @@
 .. method:: Database.sequence_create(connection, name[, number_increment[, start_value]])
 
    Create a named sequence incremented by ``number_increment`` or ``1`` and
    starting at ``start_value`` or ``1`` using the ``connection``.
 
 .. method:: Database.sequence_update(connection, name[, number_increment[, start_value]])
 
-   Modify the named sequence with ``number_increment`` and ``start_value``using
-   the ``connection``.
+   Modify the named sequence with ``number_increment`` and ``start_value``
+   using the ``connection``.
 
 .. method:: Database.sequence_rename(connection, old_name, new_name)
 
    Rename the sequece from ``old_name`` to ``new_name`` using the
    ``connection``.
 
 .. method:: Database.sequence_delete(connection, name)
```

### Comparing `trytond-6.6.8/doc/ref/bus.rst` & `trytond-6.8.0/doc/ref/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/cache.rst` & `trytond-6.8.0/doc/ref/cache.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 .. _ref-cache:
 .. module:: trytond.cache
 
 Cache
 =====
 
-.. class:: Cache(name[, size_limit[, duration[, context]]])
+.. class:: Cache(name[, duration[, context[, context_ignored_keys]]])
 
    Use to cache values between server requests.
 
    The ``name`` should be unique and it's used to identify the cache.
    Usually ``<class_name>.<content_name>`` is used to make it unique.
 
-   The ``size_limit`` parameter can be used to limit the number of values
-   cached and it has ``1024`` as the default value.
-
    The ``duration`` parameter defines how long a cached value stays valid but
    if it is not set the value remains valid until it is cleared.
 
    And the ``context`` parameter is used to indicate if the cache depends on
    the user context and is ``True`` by default.
+   Keys specified in ``context_ignored_keys`` are ignored.
 
    The cache is cleaned on :class:`~trytond.transaction.Transaction` starts and
    resets on :class:`~trytond.transaction.Transaction` commit or rollback.
 
    .. warning::
 
        As there is no deepcopy of the values cached, they must never be mutated
        after being set in or retrieved from the cache.
 
+.. attribute:: Cache.size_limit
+
+   The maximal number of values cached.
+   The value comes from the entry with the same ``name`` under the ``cache``
+   section of the :ref:`configuration <topics-configuration>` using the
+   ``default`` entry as default value.
+
 .. attribute:: Cache.hit
 
    Count the number of times the cache returned a cached value.
 
 .. attribute:: Cache.miss
 
    Count the number of times the cache did not contain the key.
```

### Comparing `trytond-6.6.8/doc/ref/exceptions.rst` & `trytond-6.8.0/doc/ref/exceptions.rst`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 
    The exception raised when trying to access a record without the rights.
 
 .. exception:: AccessButtonError
 
    The exception raised when trying to execute a button without the rights.
 
+.. exception:: ButtonActionException
+
+   The exception raised to launch the ``action`` instead of executing the
+   button method.
+
+   The ``value`` attribute is the action value returned.
+
 .. exception:: ImportDataError
 
    The exception raises when importing data fails.
 
 .. exception:: ValidationError
 
    The base class for all record validation error.
```

### Comparing `trytond-6.6.8/doc/ref/fields.rst` & `trytond-6.8.0/doc/ref/fields.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
       model level.
 
 .. attribute:: Field.domain
 
    A :ref:`domain <topics-domain>` constraint that is applied on the field
    value.
 
+   The domain is enforced unless the field value is ``None``.
+
    .. note::
 
       For :class:`Reference` field it is a dictionary that contains the domain
       per model name.
 
 .. attribute:: Field.states
 
@@ -188,14 +190,22 @@
 
     Return a dictionary with the definition of the field.
 
 .. method:: Field.definition_translations(model, language)
 
     Return a list of translation sources used by :meth:`~Field.definition`.
 
+.. method:: Field.searchable(model)
+
+   Return True if the field is searchable.
+
+.. method:: Field.sortable(model)
+
+   Return True if the field is sortable.
+
 Default value
 =============
 
 See :ref:`default value <topics-fields_default_value>`
 
 Searching
 =========
@@ -246,21 +256,14 @@
 Integer
 -------
 
 .. class:: Integer(string[, \**options])
 
    An :py:class:`integer <int>` field.
 
-BigInteger
-----------
-
-.. class:: BigInteger(string[, \**options])
-
-   A long :py:class:`integer <int>` field.
-
 Char
 ----
 
 .. class:: Char(string[, size[, translate[, strip[, \**options]]]])
 
    A single line :py:class:`string <str>` field.
 
@@ -583,14 +586,30 @@
 
    Default value is ``True``.
 
 .. attribute:: Selection.help_selection
 
    A dictionary mapping the selection value with its help string.
 
+Class methods:
+
+.. classmethod:: Selection.get_selection(model, name, inst)
+
+   Returns a :py:class:`dictionary <dict>` mapping the selection value to its
+   human-readable value.
+
+.. classmethod:: Selection.get_selection_string(selection, value)
+
+   Returns the human-readable form of ``value`` in regard to ``selection``.
+   ``selection`` is acquired thanks to :meth:`Selection.get_selection`.
+   ..note::
+   This method should be used instead of relying on dictionary access
+   because this method take into account the internal representation of the
+   ``Selection`` value.
+
 Instance methods:
 
 .. method:: Selection.translated([name])
 
    Returns a descriptor for the translated value of the field.
 
    The descriptor must be used on the same class as the field.
@@ -618,14 +637,24 @@
 
    Same as :attr:`Selection.translate_selection`.
 
 .. attribute:: MultiSelection.help_selection
 
    Same as :attr:`Selection.help_selection`.
 
+Class methods:
+
+.. classmethod:: MultiSelection.get_selection(model, name, inst)
+
+   Same as :meth:`Selection.get_selection`
+
+.. classmethod:: MultiSelection.get_selection_string(selection, value)
+
+   Same as :meth:`Selection.get_selection_string`
+
 Instance methods:
 
 .. method:: MultiSelection.translated([name])
 
    Same as :meth:`Selection.translated` but returns a list of translated
    values.
 
@@ -688,15 +717,15 @@
 
    Return the SQL expression that extract the record ID of the column.
 
 
 Many2One
 --------
 
-.. class:: Many2One(model_name, string[, left[, right[, path[, ondelete[, datetime_field[, target_search[, search_order[, search_context[, \**options]]]]]]]]])
+.. class:: Many2One(model_name, string[, left[, right[, path[, ondelete[, datetime_field[, search_order[, search_context[, \**options]]]]]]]])
 
    A many-to-one relation field that refers to a record of the named model.
 
    A :py:class:`integer <int>` as :attr:`~trytond.model.Model.id` is used for
    low level APIs.
 
 :class:`Many2One` has some extra arguments:
@@ -763,31 +792,14 @@
    If set, the target record will be read at the date defined by the datetime
    field name of the record.
 
    It is usually used in combination with
    :attr:`~trytond.model.ModelSQL._history` to request a value for a given date
    and time on a historicized model.
 
-.. attribute:: Many2One.target_search
-
-   Define the kind of SQL query to use when searching on related target.
-
-   Allowed values are:
-
-      - ``subquery``: uses a subquery based on the ids.
-
-      - ``join``: adds a join on the main query.
-
-   ``join`` is the default value.
-
-   .. note::
-
-      ``join`` could improve the performance if the target has a huge amount of
-      records.
-
 .. attribute:: Many2One.search_order
 
    A :ref:`PYSON <ref-pyson>` expression defining the default order used to
    display search results in the clients.
 
 .. attribute:: Many2One.search_context
```

### Comparing `trytond-6.6.8/doc/ref/filestore.rst` & `trytond-6.8.0/doc/ref/filestore.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/i18n.rst` & `trytond-6.8.0/doc/ref/i18n.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/models.rst` & `trytond-6.8.0/doc/ref/models.rst`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,18 @@
 
 .. staticmethod:: ModelStorage.default_create_date()
 
     Return the default value for :attr:`create_date`.
 
 Class methods:
 
+.. classmethod:: ModelStorage.log(records, event[, target[, user[, \**extra]]])
+
+   Log event for records.
+
 .. classmethod:: ModelStorage.create(vlist)
 
    Create records.
 
    ``vlist`` is list of dictionaries with fields names as key and created
    values as value and return the list of new instances.
 
@@ -292,14 +296,18 @@
    The dictionary is composed of the fields as key and their values.
 
    ``fields_names`` can contain dereferenced fields from related models.
    Their values will be returned under the referencing field suffixed by a
    ``.``.
    The number of *dots* in the name is not limited.
 
+   ``fields_names`` can also contain ``<field>:string`` for
+   :class:`~fields.Selection` or :class:`~fields.MultiSelection` fields.
+   Their human-readable value are returned.
+
    The virtual fields ``_write`` and ``_delete`` can be used the read the
    writeable and deleteable state of the records.
    Regarding the ``_timestamp`` virtual fields it contains a timestamp that is
    used in the context to make a soft lock preventing update collisions.
 
    .. note::
       The order of the returned list is not guaranteed.
@@ -403,15 +411,15 @@
 
 .. classmethod:: ModelStorage.search_global(cls, text)
 
    Yield tuples (record, name, icon) for records matching text.
 
    It is used for the global search.
 
-.. classmethod:: ModelStorage.count()
+.. classmethod:: ModelStorage.estimated_count()
 
    Return an estimation of the number of records stored.
 
 .. classmethod:: ModelStorage.browse(ids)
 
    Return a list of record instance for the ``ids``.
 
@@ -438,17 +446,20 @@
    Create or update records for all values in ``data``.
 
    The field names of values must be defined in ``fields_names``.
    It returns the number of imported records.
 
 .. classmethod:: ModelStorage.check_xml_record(records, values)
 
-   Verify if the records are originating from XML data.
+   Raise an :exc:`~trytond.model.exceptions.AccessError` if the records can not
+   be modified because they originate from XML data.
+   ``values`` is a dictionary of written values or ``None`` for deletion.
 
-   It is used to prevent modification of data coming from XML files.
+   It is used by :meth:`~ModelStorage.write` and :meth:`~ModelStorage.delete`
+   to prevent modification of data coming from XML files.
 
    .. note::
       This method must be overiden to change this behavior.
 
 .. classmethod:: ModelStorage.validate(records)
 
    Validate the integrity of records after creation and modification.
@@ -465,14 +476,19 @@
 
 Dual methods:
 
 .. classmethod:: ModelStorage.save(records)
 
    Save the modification made on the records.
 
+   .. warning::
+
+      Fields that have a container as a value must be reassigned to the parent
+      record in order to be saved when the parent record is saved.
+
 Instance methods:
 
 .. method:: ModelStorage.resources()
 
    Return a dictionary with the number of attachments (``attachment_count``),
    notes (``note_count``) and unread note (``note_unread``).
 
@@ -567,24 +583,26 @@
 .. classmethod:: ModelSQL.restore_history(ids, datetime)
 
    Restore the record ids from history at the specified date time.
 
    Restoring a record still generates an entry in the history table.
 
    .. warning::
-      No access rights are verified and the records are not validated.
+      No access rights are verified, the restored records are not validated and
+      no triggers are called.
 
 .. classmethod:: ModelSQL.restore_history_before(ids, datetime)
 
    Restore the record ids from history before the specified date time.
 
    Restoring a record still generates an entry in the history table.
 
    .. warning::
-      No access rights are verified and the records are not validated.
+      No access rights are verified, the restored records are not validated and
+      not triggers are called.
 
 .. classmethod:: ModelSQL.search(domain[, offset[, limit[, order[, count[, query]]]]])
 
    Same as :meth:`ModelStorage.search` with the additional ``query`` argument.
 
    If ``query`` is set to ``True``, the the result is the SQL query.
 
@@ -723,14 +741,23 @@
 
 Represent a similar usage only for text.
 Additional options are available:
 
    * ``begin``: optimize for constant pattern and anchored to the beginning of
      the string
 
+
+convert_from
+------------
+
+.. method:: convert_from(table, tables[, type_])
+
+Return a SQL ``FromItem`` constructed by joining ``table`` and :ref:`tables
+<ref-tables>` using ``type_`` with default value ``LEFT``.
+
 Workflow
 ========
 
 .. class:: Workflow
 
 A mixin_ to handle transition check.
 
@@ -961,14 +988,22 @@
 
 ``field_name`` indicates the name of the field to be created and its default
 values is ``sequence``.
 ``field_label`` defines the label which will be used by the field and defaults
 to ``Sequence``.
 Order specifies the order direction and defaults to ``ASC NULLS FIRST``.
 
+sort
+====
+
+.. function:: sort(records, order)
+
+Return a new list of records ordered by the ``order`` list defined like in
+:meth:`~ModelStorage.search`.
+
 MultiValueMixin
 ===============
 
 .. class:: MultiValueMixin
 
 A mixin_ for :class:`Model` to help having :class:`~fields.MultiValue` fields
 with multi-values on a :class:`ValueMixin`.
```

### Comparing `trytond-6.6.8/doc/ref/pool.rst` & `trytond-6.8.0/doc/ref/pool.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/pyson.rst` & `trytond-6.8.0/doc/ref/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/rpc.rst` & `trytond-6.8.0/doc/ref/rpc.rst`

 * *Files 16% similar despite different names*

```diff
@@ -57,7 +57,18 @@
    A :py:class:`datetime.timedelta` instance.
 
 Instance methods are:
 
 .. method:: RCP.headers
 
    Return a dictionary of the headers.
+
+Exceptions
+==========
+
+.. exception:: RPCReturnException
+
+   The base class of exceptions to return the result of ``result`` method
+   instead of raising an exception.
+
+   The :class:`~trytond.transaction.Transaction` is rollbacked and tasks are
+   cleared.
```

### Comparing `trytond-6.6.8/doc/ref/sendmail.rst` & `trytond-6.8.0/doc/ref/sendmail.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/tests.rst` & `trytond-6.8.0/doc/ref/tests.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/tools/misc.rst` & `trytond-6.8.0/doc/ref/tools/misc.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
    Return the path of the named directory in subdir from root directory.
 
 .. function:: resolve(name)
 
    Resolve a dotted name to a global object.
 
+.. method:: safe_join(directory, \*pathnames)
+
+   Safely join zero or more untrusted path components to a base directory to
+   avoid escaping the base directory.
+
 .. function:: unescape_wildcard(string[, wildcards[, escape]])
 
    Return the string without the wild card escapes.
 
 .. function:: is_full_text(value[, escape])
 
    Determine if the value can be used as full text search.
```

### Comparing `trytond-6.6.8/doc/ref/tools/timezone.rst` & `trytond-6.8.0/doc/ref/tools/timezone.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/ref/transaction.rst` & `trytond-6.8.0/doc/ref/transaction.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 .. _ref-transaction:
 .. module:: trytond.transaction
 
 Transaction
 ===========
 
+.. exception:: TransactionError
+
+   The base class for transaction error that need to retry the transaction.
+
+.. method:: TransactionError.fix(extras)
+
+   Update the extras argument of :meth:`~Transaction.start` to restart the
+   transaction without the error.
+
 .. class:: Transaction
 
    Represents a Tryton transaction that contains thread-local parameters of a
    database connection.
    The Transaction instances are `context manager`_ that commits or
    rollbacks the database transaction.
    In the event of an exception the transaction is rolled back, otherwise it is
@@ -49,19 +58,27 @@
 
    The language code defines in the context.
 
 .. attribute:: Transaction.counter
 
    Count the number of modification made in this transaction.
 
+.. attribute:: Transaction.check_access
+
+   If the access must be enforced.
+
+.. attribute:: Transaction.active_records
+
+   If the active test is enabled.
+
 .. staticmethod:: Transaction.monotonic_time
 
-   Return a monotonic time used to populate :attr:~Transaction.started_at.
+   Return a monotonic time used to populate :attr:`~Transaction.started_at`.
 
-.. method:: Transaction.start(database_name, user[, readonly[, context[, close[, autocommit]]]])
+.. method:: Transaction.start(database_name, user[, readonly[, context[, close[, autocommit, \**extras]]]])
 
    Start a new transaction and return a `context manager`_.
    The non-readonly transaction will be committed when exiting the ``with``
    statement without exception.
    The other cases will be rollbacked.
 
 .. method:: Transaction.stop([commit])
@@ -85,21 +102,26 @@
 .. method:: Transaction.set_user(user[, set_context])
 
    Modify the user of the transaction and return a `context manager`_.
    ``set_context`` will put the previous user id in the context to simulate the
    record rules.
    The user will be restored when exiting the ``with`` statement.
 
+.. method:: Transaction.lock_table(table)
+
+   Raise a :exc:`TransactionError` to retry the transaction if the table has
+   not been locked at the start.
+
 .. method:: Transaction.set_current_transaction(transaction)
 
    Add a specific ``transaction`` on the top of the transaction stack.
    A transaction is commited or rollbacked only when its last reference is
    popped from the stack.
 
-.. method:: Transaction.new_transaction([autocommit[, readonly]])
+.. method:: Transaction.new_transaction([autocommit[, readonly, \**extras]])
 
    Create a new transaction with the same database, user and context as the
    original transaction and adds it to the stack of transactions.
 
 .. method:: Transaction.commit()
 
    Commit the transaction and all data managers associated.
@@ -119,10 +141,36 @@
 
 .. method:: Transaction.atexit(func, \*args, \*\*kwargs)
 
    Register a function to be executed upon normal transaction termination.
    The function can not use the current transaction because it will be already
    committed or rollbacked.
 
+.. function:: check_access([func])
+
+   When called with a function, it decorates the function to be executed with
+   check of access rights.
+   Otherwise it returns a `context manager`_ that check access rights until
+   exiting.
+
+.. function:: without_check_access([func])
+
+   When called with a function, it decorates the function to be executed
+   without check of access rights.
+   Otherwise it returns a `context manager`_ that disable check access rights
+   until exiting.
+
+.. function:: active_records([func])
+
+   When called with a function, it decorates the function to be executed with
+   active test enabled.
+   Otherwise it returns a `context manager`_ that enable active test.
+
+.. function:: with_inactive_records(func)
+
+   When called with a function, it decorates the function to be executed with
+   active test disabled.
+   Otherwise it returns a `context manager`_ that disables active test.
+
 .. _`context manager`: http://docs.python.org/reference/datamodel.html#context-managers
 .. _`PEP-0249`: https://www.python.org/dev/peps/pep-0249/
 .. _`Two-Phase Commit protocol`: https://en.wikipedia.org/wiki/Two-phase_commit_protocol
```

### Comparing `trytond-6.6.8/doc/ref/wizard.rst` & `trytond-6.8.0/doc/ref/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/access_rights.rst` & `trytond-6.8.0/doc/topics/access_rights.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/actions.rst` & `trytond-6.8.0/doc/topics/actions.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/backend_types.rst` & `trytond-6.8.0/doc/topics/backend_types.rst`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 
 The columns are in the following order:
 
 * The SQL type [#]_ representing the field
 * The python type expected on input
 * The python type received on output
 
-.. _`SQL 92`: http://www.contrib.andrew.cmu.edu/~shadow/sql/sql1992.txt
+.. _`SQL 92`: https://en.wikipedia.org/wiki/SQL-92
 .. _`PostgreSQL type`: https://www.postgresql.org/docs/current/static/datatype.html
 
 ``None`` will represent the ``NULL`` value and vice versa, it can be used as
 input or output for any SQL type.
 
 +----------------------+----------------------+----------------------+
 | SQL Type             | Python input type    | Python output type   |
 +======================+======================+======================+
 | ``BOOL``             | bool                 | bool                 |
 +----------------------+----------------------+----------------------+
+| ``SMALLINT``         | int                  | int                  |
++----------------------+----------------------+----------------------+
 | ``INTEGER``          | int                  | int                  |
 +----------------------+----------------------+----------------------+
 | ``BIGINT``           | int                  | int                  |
 +----------------------+----------------------+----------------------+
+| ``REAL``             | float / int          | float                |
++----------------------+----------------------+----------------------+
 | ``FLOAT``            | float / int          | float                |
 +----------------------+----------------------+----------------------+
 | ``NUMERIC``          | decimal.Decimal_     | decimal.Decimal_     |
 +----------------------+----------------------+----------------------+
 | ``VARCHAR`` /        | str                  | str                  |
 | ``VARCHAR(length)``  |                      |                      |
 +----------------------+----------------------+----------------------+
```

### Comparing `trytond-6.6.8/doc/topics/bus.rst` & `trytond-6.8.0/doc/topics/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/configuration.rst` & `trytond-6.8.0/doc/topics/configuration.rst`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,18 @@
 Please refer to `psycopg2 for the complete specification of the URI
 <https://www.psycopg.org/docs/module.html#psycopg2.connect>`_.
 
 A list of parameters supported by PostgreSQL can be found in the
 `documentation
 <https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-PARAMKEYWORDS>`__.
 
+.. note::
+   ``fallback_application_name`` parameter from aforementioned documentation can
+   be set directly thanks to the ``TRYTOND_APPNAME`` environment variable.
+
 SQLite
 ******
 
 The URI is defined as ``sqlite://``
 
 If the name of the database is ``:memory:``, the parameter ``mode`` will be set
 to ``memory`` thus using a pure in-memory database.
@@ -176,14 +180,21 @@
 retry
 ~~~~~
 
 The number of retries when a database operational error occurs during a request.
 
 Default: ``5``
 
+subquery_threshold
+~~~~~~~~~~~~~~~~~~
+
+The number of records in the target relation under which a sub-query is used.
+
+Default: ``1000``
+
 language
 ~~~~~~~~
 
 The main language of the database that will be used for storage in the main
 table for translations.
 
 Default: ``en``
@@ -293,14 +304,21 @@
 ~~~~~
 
 The number of field to load with an ``eager`` :attr:`Field.loading
 <trytond.model.fields.Field.loading>`.
 
 Default: ``100``
 
+default
+~~~~~~~
+
+The default :attr:`~trytond.cache.Cache.size_limit` of :class:`~trytond.cache.Cache`.
+
+Default: ``1024``
+
 clean_timeout
 ~~~~~~~~~~~~~
 
 The minimum number of seconds between two cleanings of the cache.
 If the value is 0, the notification between processes will be done using
 channels if the back-end supports them.
 
@@ -423,14 +441,16 @@
 Defines the default ``From`` address (using :rfc:`5322`) for emails sent by
 Tryton.
 
 For example::
 
     from: "Company Inc" <info@example.com>
 
+Default: The login name of the :abbr:`OS (Operating System)` user.
+
 retry
 ~~~~~
 
 The number of retries when the SMTP server returns a temporary error.
 
 Default: ``5``
 
@@ -628,15 +648,15 @@
 plugins
 ~~~~~~~
 
 The space separated list of TinyMCE plugins to load.
 It can be overridden for specific models and fields using the names:
 ``plugins-<model>-<field>`` or ``plugins-<model>``.
 
-Default: ``
+Default: ``''``
 
 css
 ~~~
 
 The JSON list of CSS files to load.
 It can be overridden for specific models and fields using the names:
 ``css-<model>-<field>`` or ``css-<model>``.
```

### Comparing `trytond-6.6.8/doc/topics/cron.rst` & `trytond-6.8.0/doc/topics/cron.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/domain.rst` & `trytond-6.8.0/doc/topics/domain.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/index.rst` & `trytond-6.8.0/doc/topics/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/install.rst` & `trytond-6.8.0/doc/topics/install.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/logs.rst` & `trytond-6.8.0/doc/topics/logs.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/models/fields_default_value.rst` & `trytond-6.8.0/doc/topics/models/fields_default_value.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 =======================
 
 When a record is created, each field, which doesn't have a value specified,
 is set with the default value if exists.
 
 The following class method:
 
+.. rstcheck: ignore-next-code-block
 .. code-block:: python
 
     Model.default_<field name>()
 
 Return the default value for ``field name``.
 
 This example defines an ``Item`` model which has a default ``since``:
```

### Comparing `trytond-6.6.8/doc/topics/models/fields_on_change.rst` & `trytond-6.8.0/doc/topics/models/fields_on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/models/index.rst` & `trytond-6.8.0/doc/topics/models/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/modules/index.rst` & `trytond-6.8.0/doc/topics/modules/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/pyson.rst` & `trytond-6.8.0/doc/topics/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/rpc.rst` & `trytond-6.8.0/doc/topics/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/setup_database.rst` & `trytond-6.8.0/doc/topics/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/start_server.rst` & `trytond-6.8.0/doc/topics/start_server.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/task_queue.rst` & `trytond-6.8.0/doc/topics/task_queue.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/testing.rst` & `trytond-6.8.0/doc/topics/testing.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/translation.rst` & `trytond-6.8.0/doc/topics/translation.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/triggers.rst` & `trytond-6.8.0/doc/topics/triggers.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/user_application.rst` & `trytond-6.8.0/doc/topics/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/user_errors_warnings.rst` & `trytond-6.8.0/doc/topics/user_errors_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/views/extension.rst` & `trytond-6.8.0/doc/topics/views/extension.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/topics/views/index.rst` & `trytond-6.8.0/doc/topics/views/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -347,14 +347,19 @@
    toolbar.
    The default value is ``True``.
 
 ``spell``
    Only for Text widgets, a :ref:`PYSON statement <topics-pyson>` that is
    evaluated to the language code for which spell checking must be done.
 
+``border``
+   The type of border for the image widget. Available values are ``square``,
+   ``rounded`` or ``circle``.
+   The default value is ``square``.
+
 :ref:`yexpand <common-attributes-yexpand>`,
 :ref:`yfill <common-attributes-yfill>`,
 :ref:`xexpand <common-attributes-xexpand>`,
 :ref:`xfill <common-attributes-xfill>`,
 :ref:`colspan <common-attributes-colspan>`,
 :ref:`help <common-attributes-help>`,
 :ref:`pre_validate <common-attributes-pre_validate>`,
@@ -382,14 +387,19 @@
 ``url_size``
    The name of the size parameter to add to the URL.
 
 ``size``
    The size of the image in pixels.
    The default value is ``48``.
 
+``border``
+   The type of border for the image. Available values are ``square``,
+   ``rounded`` or ``circle``.
+   The default value is ``square``.
+
 :ref:`yexpand <common-attributes-yexpand>`,
 :ref:`yfill <common-attributes-yfill>`,
 :ref:`colspan <common-attributes-colspan>`,
 :ref:`states <common-attributes-states>`,
 :ref:`help <common-attributes-help>`.
 
 .. _form-separator:
@@ -731,14 +741,19 @@
 ``icon_type``
    The type of icon source. Available values are ``icon`` or ``url``.
    The default value is ``icon``.
 
 ``url_size``
    The name of the size parameter to add to the URL.
 
+``border``
+   The type of border for the icon. Available values are ``square``,
+   ``rounded`` or ``circle``.
+   The default value is ``square``.
+
 button
 ------
 
 Same as form-button_.
 
 List-Form
 =========
@@ -949,14 +964,18 @@
       <field name="reference"/>
   </calendar>
 
 The RNG that describes the XML for a calendar view is stored in
 ``trytond/ir/ui/calendar.rng``.
 There is also a RNC in ``trytond/ir/ui/calendar.rnc``.
 
+The ``calendar_scroll_time`` context key determines the initial time to scroll
+to.
+The default value is ``datetime.time(6)``.
+
 calendar
 --------
 
 Each calendar view must start with this tag with those attributes:
 
 ``dtstart``
    The name of the field that contains the start date.
```

### Comparing `trytond-6.6.8/doc/topics/wizard.rst` & `trytond-6.8.0/doc/topics/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/anatomy.rst` & `trytond-6.8.0/doc/tutorial/module/anatomy.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/default_values.rst` & `trytond-6.8.0/doc/tutorial/module/default_values.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/domains.rst` & `trytond-6.8.0/doc/tutorial/module/domains.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/extend.rst` & `trytond-6.8.0/doc/tutorial/module/extend.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/function_fields.rst` & `trytond-6.8.0/doc/tutorial/module/function_fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/index.rst` & `trytond-6.8.0/doc/tutorial/module/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/model.rst` & `trytond-6.8.0/doc/tutorial/module/model.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/on_change.rst` & `trytond-6.8.0/doc/tutorial/module/on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/report.rst` & `trytond-6.8.0/doc/tutorial/module/report.rst`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 We use the `Genshi XML Template Language`_ implemented by relatorio_ using
 ``Placeholder Text``.
 The rendering context contains the variable ``records`` which is a list of
 selected record instances.
 
 Here is an example of the directives to insert in the document:
 
-.. code-block::
+.. code-block:: text
 
    <for each="opportunity in records">
    Opportunity: <opportunity.rec_name>
    Party: <opportunity.party.rec_name>
    Start Date: <format_date(opportunity.start_date) if opportunity.start_date else ''>
    End Date: <format_date(opportunity.end_date) if opportunity.end_date else ''>
```

### Comparing `trytond-6.6.8/doc/tutorial/module/setup.rst` & `trytond-6.8.0/doc/tutorial/module/setup.rst`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Setup module
 ------------
 
 The Tryton template can be rendered into a module with:
 
 .. code-block:: console
 
-   $ cookiecutter hg+https://hg.tryton.org/cookiecutter
+   $ cookiecutter hg+https://code.tryton.org/tryton --directory cookiecutter-module
    module_name [my_module]: opportunity
    prefix []: tuto
    package_name [tuto_opportunity]:
    version []: x.y.0
    description []:
    author [Tryton]: John Doe
    author_email [bugs@tryton.org]: john@example.com
```

### Comparing `trytond-6.6.8/doc/tutorial/module/setup_database.rst` & `trytond-6.8.0/doc/tutorial/module/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/states.rst` & `trytond-6.8.0/doc/tutorial/module/states.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/table_query.rst` & `trytond-6.8.0/doc/tutorial/module/table_query.rst`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 the :class:`~trytond.pool.Pool` as type ``model`` in :file:`__init__.py`:
 
 .. code-block:: python
 
     def register():
         ...
         Pool.register(
-            ...
+            ...,
             opportunity.OpportunityMonthly,
             module='opportunity', type_='model')
 
 And to display we create a list view and the menu entry in
 :file:`opportunity.xml`:
 
 .. code-block:: xml
```

### Comparing `trytond-6.6.8/doc/tutorial/module/view.rst` & `trytond-6.8.0/doc/tutorial/module/view.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/doc/tutorial/module/wizard.rst` & `trytond-6.8.0/doc/tutorial/module/wizard.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,22 +67,22 @@
 
 .. code-block:: python
 
     from trytond.wizard import Wizard, StateView, StateTransition, Button
     ...
     class Opportunity(...):
         ...
-       @classmethod
-       @Workflow.transition('converted')
-       def convert(cls, opportunities, end_date=None):
-           pool = Pool()
-           Date = pool.get('ir.date')
-           cls.write(opportunities, {
-               'end_date': end_date or Date.today(),
-               })
+        @classmethod
+        @Workflow.transition('converted')
+        def convert(cls, opportunities, end_date=None):
+            pool = Pool()
+            Date = pool.get('ir.date')
+            cls.write(opportunities, {
+                'end_date': end_date or Date.today(),
+                })
     ...
     class Convert(Wizard):
         "Convert Opportunities"
         __name__ = 'training.opportunity.convert'
 
         start = StateView(
             'training.opportunity.convert.start',
```

### Comparing `trytond-6.6.8/doc/tutorial/module/workflow.rst` & `trytond-6.8.0/doc/tutorial/module/workflow.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/setup.py` & `trytond-6.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,32 +43,35 @@
 
 version = get_version()
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 tests_require = ['pillow']
 
 setup(name=name,
     version=version,
     description='Tryton server',
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
-        "Source Code": 'https://hg.tryton.org/trytond',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='business application platform ERP',
     packages=find_packages(exclude=['*.modules.*', 'modules.*', 'modules',
             '*.proteus.*', 'proteus.*', 'proteus']),
     package_data={
         'trytond': ['ir/ui/icons/*.svg', '*.rnc', '*.rng', 'ir/fonts/*.ttf'],
         'trytond.backend.postgresql': ['init.sql'],
@@ -115,48 +118,49 @@
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
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         ],
     platforms='any',
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'defusedxml',
         'lxml >= 2.0',
         'relatorio[fodt] >= 0.7.0',
         'Genshi',
         'python-dateutil',
         'polib',
         'python-sql >= 1.3',
         'werkzeug >= 0.12',
-        'wrapt',
         'passlib >= 1.7.0',
         'pytz;python_version<"3.9"',
         ],
     extras_require={
         'test': tests_require,
         'PostgreSQL': ['psycopg2 >= 2.7.0'],
         'graphviz': ['pydot'],
         'Levenshtein': ['python-Levenshtein'],
         'BCrypt': ['passlib[bcrypt]'],
         'Argon2': ['passlib[argon2]'],
         'html2text': ['html2text'],
         'weasyprint': ['weasyprint'],
         'coroutine': ['gevent>=1.1'],
         'image': ['pillow'],
+        'barcode': ['python-barcode[images]'],
+        'qrcode': ['qrcode[pil]', 'webcolors'],
         'completion': ['argcomplete'],
         },
     zip_safe=False,
     cmdclass={
         'update_rng': rnc2rng,
         },
     )
```

### Comparing `trytond-6.6.8/trytond/__init__.py` & `trytond-6.8.0/trytond/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import os
 import time
 import warnings
 from email import charset
 
+import __main__
 from lxml import etree, objectify
 
-__version__ = "6.6.8"
+__version__ = "6.8.0"
 
+os.environ.setdefault(
+    'TRYTOND_APPNAME',
+    os.path.basename(getattr(__main__, '__file__', 'trytond')))
 os.environ.setdefault('TRYTOND_TZ', os.environ.get('TZ', 'UTC'))
 os.environ['TZ'] = 'UTC'
 if hasattr(time, 'tzset'):
     time.tzset()
 
 if time.tzname[0] != 'UTC':
     warnings.warn('Timezone must be set to UTC instead of %s' % time.tzname[0])
```

### Comparing `trytond-6.6.8/trytond/admin.py` & `trytond-6.8.0/trytond/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from sql import Literal, Table
 
 from trytond import backend
 from trytond.config import config
 from trytond.pool import Pool
 from trytond.sendmail import send_test_email
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, TransactionError, inactive_records
 
 __all__ = ['run']
 logger = logging.getLogger(__name__)
 
 
 def run(options):
     main_lang = config.get('database', 'language')
@@ -70,62 +70,78 @@
                         ('code', 'in', lang),
                         ])
                 Lang.write(languages, {
                         'translatable': True,
                         })
 
     for db_name in options.database_names:
-        with Transaction().start(db_name, 0) as transaction:
-            pool = Pool()
-            User = pool.get('res.user')
-            Configuration = pool.get('ir.configuration')
-            configuration = Configuration(1)
-            with transaction.set_context(active_test=False):
-                admin, = User.search([('login', '=', 'admin')])
-
-            if options.email is not None:
-                admin.email = options.email
-            elif init[db_name]:
-                admin.email = input(
-                    '"admin" email for "%s": ' % db_name)
-            if init[db_name] or options.password:
-                configuration.language = main_lang
-                # try to read password from environment variable
-                # TRYTONPASSFILE, empty TRYTONPASSFILE ignored
-                passpath = os.getenv('TRYTONPASSFILE')
-                password = ''
-                if passpath:
-                    try:
-                        with open(passpath) as passfile:
-                            password, = passfile.read().splitlines()
-                    except Exception as err:
-                        sys.stderr.write('Can not read password '
-                            'from "%s": "%s"\n' % (passpath, err))
-
-                if not password and not options.reset_password:
-                    while True:
-                        password = getpass(
-                            '"admin" password for "%s": ' % db_name)
-                        password2 = getpass('"admin" password confirmation: ')
-                        if password != password2:
-                            sys.stderr.write('"admin" password confirmation '
-                                'doesn\'t match "admin" password.\n')
-                            continue
-                        if not password:
-                            sys.stderr.write('"admin" password is required.\n')
-                            continue
-                        break
-                if not options.reset_password:
-                    admin.password = password
-            admin.save()
-            if options.reset_password:
-                User.reset_password([admin])
-            if options.hostname is not None:
-                configuration.hostname = options.hostname or None
-            configuration.save()
+        if options.email is not None:
+            email = options.email
+        elif init[db_name]:
+            email = input(
+                '"admin" email for "%s": ' % db_name)
+        else:
+            email = None
+
+        password = ''
+        if init[db_name] or options.password:
+            # try to read password from environment variable
+            # TRYTONPASSFILE, empty TRYTONPASSFILE ignored
+            passpath = os.getenv('TRYTONPASSFILE')
+            if passpath:
+                try:
+                    with open(passpath) as passfile:
+                        password, = passfile.read().splitlines()
+                except Exception as err:
+                    sys.stderr.write('Can not read password '
+                        'from "%s": "%s"\n' % (passpath, err))
+
+            if not password and not options.reset_password:
+                while True:
+                    password = getpass(
+                        '"admin" password for "%s": ' % db_name)
+                    password2 = getpass('"admin" password confirmation: ')
+                    if password != password2:
+                        sys.stderr.write('"admin" password confirmation '
+                            'doesn\'t match "admin" password.\n')
+                        continue
+                    if not password:
+                        sys.stderr.write('"admin" password is required.\n')
+                        continue
+                    break
+
+        transaction_extras = {}
+        while True:
+            with Transaction().start(
+                    db_name, 0, **transaction_extras) as transaction:
+                try:
+                    pool = Pool()
+                    User = pool.get('res.user')
+                    Configuration = pool.get('ir.configuration')
+                    configuration = Configuration(1)
+                    with inactive_records():
+                        admin, = User.search([('login', '=', 'admin')])
+
+                    if email is not None:
+                        admin.email = email
+                    if init[db_name] or options.password:
+                        configuration.language = main_lang
+                        if not options.reset_password:
+                            admin.password = password
+                    admin.save()
+                    if options.reset_password:
+                        User.reset_password([admin])
+                    if options.hostname is not None:
+                        configuration.hostname = options.hostname or None
+                    configuration.save()
+                except TransactionError as e:
+                    transaction.rollback()
+                    e.fix(transaction_extras)
+                    continue
+                break
         with Transaction().start(db_name, 0, readonly=True):
             if options.validate is not None:
                 validate(options.validate, options.validate_percentage)
 
 
 def validate(models, percentage=100):
     from trytond.model import ModelSingleton, ModelStorage
```

### Comparing `trytond-6.6.8/trytond/application.py` & `trytond-6.8.0/trytond/application.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/backend/__init__.py` & `trytond-6.8.0/trytond/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/backend/database.py` & `trytond-6.8.0/trytond/backend/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def test(self, hostname=None):
         '''
         Test if it is a Tryton database.
         '''
         raise NotImplementedError
 
-    def nextid(self, connection, table):
+    def nextid(self, connection, table, count=1):
         pass
 
     def setnextid(self, connection, table, value):
         pass
 
     def currid(self, connection, table):
         pass
```

### Comparing `trytond-6.6.8/trytond/backend/postgresql/database.py` & `trytond-6.8.0/trytond/backend/postgresql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,19 @@
     _has_select_for_skip_locked = None
     _has_proc = defaultdict(lambda: defaultdict(dict))
     _extensions = defaultdict(dict)
     _search_full_text_languages = defaultdict(dict)
     flavor = Flavor(ilike=True)
 
     TYPES_MAPPING = {
+        'SMALLINT': SQLType('INT2', 'INT2'),
         'BIGINT': SQLType('INT8', 'INT8'),
         'BLOB': SQLType('BYTEA', 'BYTEA'),
         'DATETIME': SQLType('TIMESTAMP', 'TIMESTAMP(0)'),
+        'REAL': SQLType('FLOAT4', 'FLOAT4'),
         'FLOAT': SQLType('FLOAT8', 'FLOAT8'),
         'FULLTEXT': SQLType('TSVECTOR', 'TSVECTOR'),
         'INTEGER': SQLType('INT4', 'INT4'),
         'JSON': SQLType('JSONB', 'JSONB'),
         'TIMESTAMP': SQLType('TIMESTAMP', 'TIMESTAMP(6)'),
         }
 
@@ -244,14 +246,16 @@
     @classmethod
     def _connection_params(cls, name):
         uri = parse_uri(config.get('database', 'uri'))
         if uri.path and uri.path != '/':
             warnings.warn("The path specified in the URI will be overridden")
         params = {
             'dsn': uri._replace(path=name).geturl(),
+            'fallback_application_name': os.environ.get(
+                'TRYTOND_APPNAME', 'trytond'),
             }
         return params
 
     def connect(self):
         return self
 
     def get_connection(self, autocommit=False, readonly=False):
@@ -406,30 +410,38 @@
                 hostnames = {h for h, in cursor if h}
                 if hostnames and hostname not in hostnames:
                     return False
             except ProgrammingError:
                 pass
         return True
 
-    def nextid(self, connection, table):
+    def nextid(self, connection, table, count=1):
         cursor = connection.cursor()
         cursor.execute(
-            "SELECT nextval(format(%s, %s))", ('%I', table + '_id_seq',))
-        return cursor.fetchone()[0]
+            "SELECT nextval(pg_get_serial_sequence(format(%s, %s), %s)) "
+            "FROM generate_series(1, %s)",
+            ('%I', table, 'id', count))
+        if count == 1:
+            return cursor.fetchone()[0]
+        else:
+            return [id for id, in cursor]
 
     def setnextid(self, connection, table, value):
         cursor = connection.cursor()
         cursor.execute(
-            "SELECT setval(format(%s, %s), %s)",
-            ('%I', table + '_id_seq', value))
+            "SELECT setval(pg_get_serial_sequence(format(%s, %s), %s), %s)",
+            ('%I', table, 'id', value))
 
     def currid(self, connection, table):
         cursor = connection.cursor()
-        cursor.execute(SQL("SELECT last_value FROM {}").format(
-                Identifier(table + '_id_seq')))
+        cursor.execute(
+            "SELECT pg_get_serial_sequence(format(%s, %s), %s)",
+            ('%I', table, 'id'))
+        sequence_name, = cursor.fetchone()
+        cursor.execute(f"SELECT last_value FROM {sequence_name}")
         return cursor.fetchone()[0]
 
     def lock(self, connection, table):
         cursor = connection.cursor()
         cursor.execute(SQL('LOCK {} IN EXCLUSIVE MODE NOWAIT').format(
                 Identifier(table)))
```

### Comparing `trytond-6.6.8/trytond/backend/postgresql/init.sql` & `trytond-6.8.0/trytond/backend/postgresql/init.sql`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,135 @@
-CREATE SEQUENCE ir_configuration_id_seq;
-
 CREATE TABLE ir_configuration (
-    id INTEGER DEFAULT NEXTVAL('ir_configuration_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     language VARCHAR,
     hostname VARCHAR,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE ir_model_id_seq;
-
 CREATE TABLE ir_model (
-    id INTEGER DEFAULT NEXTVAL('ir_model_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     model VARCHAR NOT NULL,
     name VARCHAR,
     info TEXT,
     module VARCHAR,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE ir_model_field_id_seq;
-
 CREATE TABLE ir_model_field (
-    id INTEGER DEFAULT NEXTVAL('ir_model_field_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     model INTEGER,
     name VARCHAR NOT NULL,
     relation VARCHAR,
     field_description VARCHAR,
     ttype VARCHAR,
     help TEXT,
     module VARCHAR,
     "access" BOOL,
     PRIMARY KEY(id),
     FOREIGN KEY (model) REFERENCES ir_model(id) ON DELETE CASCADE
 );
 
-CREATE SEQUENCE ir_ui_view_id_seq;
-
 CREATE TABLE ir_ui_view (
-    id INTEGER DEFAULT NEXTVAL('ir_ui_view_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     model VARCHAR NOT NULL,
     "type" VARCHAR,
     data TEXT NOT NULL,
     field_childs VARCHAR,
     priority INTEGER NOT NULL,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE ir_ui_menu_id_seq;
-
 CREATE TABLE ir_ui_menu (
-    id INTEGER DEFAULT NEXTVAL('ir_ui_menu_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     parent INTEGER,
     name VARCHAR NOT NULL,
     icon VARCHAR,
     PRIMARY KEY (id),
     FOREIGN KEY (parent) REFERENCES ir_ui_menu (id) ON DELETE SET NULL
 );
 
-CREATE SEQUENCE ir_translation_id_seq;
-
 CREATE TABLE ir_translation (
-    id INTEGER DEFAULT NEXTVAL('ir_translation_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     lang VARCHAR,
     src TEXT,
     name VARCHAR NOT NULL,
     res_id INTEGER,
     value TEXT,
     "type" VARCHAR,
     module VARCHAR,
     fuzzy BOOLEAN NOT NULL,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE ir_lang_id_seq;
-
 CREATE TABLE ir_lang (
-    id INTEGER DEFAULT NEXTVAL('ir_lang_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     name VARCHAR NOT NULL,
     code VARCHAR NOT NULL,
     translatable BOOLEAN NOT NULL,
     parent VARCHAR,
     active BOOLEAN NOT NULL,
     direction VARCHAR NOT NULL,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE res_user_id_seq;
-
 CREATE TABLE res_user (
-    id INTEGER DEFAULT NEXTVAL('res_user_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     name VARCHAR NOT NULL,
     active BOOLEAN NOT NULL,
     login VARCHAR NOT NULL,
     password VARCHAR,
     PRIMARY KEY(id)
 );
 
 ALTER TABLE res_user ADD CONSTRAINT res_user_login_key UNIQUE (login);
 
 INSERT INTO res_user (id, login, password, name, active) VALUES (0, 'root', NULL, 'Root', False);
 
-CREATE SEQUENCE res_group_id_seq;
-
 CREATE TABLE res_group (
-    id INTEGER DEFAULT NEXTVAL('res_group_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     name VARCHAR NOT NULL,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE "res_user-res_group_id_seq";
-
 CREATE TABLE "res_user-res_group" (
-    id INTEGER DEFAULT NEXTVAL('res_user-res_group_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     "user" INTEGER NOT NULL,
     "group" INTEGER NOT NULL,
     FOREIGN KEY ("user") REFERENCES res_user (id) ON DELETE CASCADE,
     FOREIGN KEY ("group") REFERENCES res_group (id) ON DELETE CASCADE,
     PRIMARY KEY(id)
 );
 
-CREATE SEQUENCE ir_module_id_seq;
-
 CREATE TABLE ir_module (
-    id INTEGER DEFAULT NEXTVAL('ir_module_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     create_uid INTEGER NOT NULL,
     create_date TIMESTAMP WITHOUT TIME ZONE NOT NULL,
     write_date TIMESTAMP WITHOUT TIME ZONE,
     write_uid INTEGER,
     name VARCHAR NOT NULL,
     state VARCHAR,
     PRIMARY KEY(id),
     FOREIGN KEY (create_uid) REFERENCES res_user ON DELETE SET NULL,
     FOREIGN KEY (write_uid) REFERENCES res_user ON DELETE SET NULL
 );
 
 ALTER TABLE ir_module ADD CONSTRAINT ir_module_name_uniq UNIQUE (name);
 
-CREATE SEQUENCE ir_module_dependency_id_seq;
-
 CREATE TABLE ir_module_dependency (
-    id INTEGER DEFAULT NEXTVAL('ir_module_dependency_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     create_uid INTEGER NOT NULL,
     create_date TIMESTAMP WITHOUT TIME ZONE NOT NULL,
     write_date TIMESTAMP WITHOUT TIME ZONE,
     write_uid INTEGER,
     name VARCHAR,
     module INTEGER,
     PRIMARY KEY(id),
     FOREIGN KEY (create_uid) REFERENCES res_user ON DELETE SET NULL,
     FOREIGN KEY (write_uid) REFERENCES res_user ON DELETE SET NULL,
     FOREIGN KEY (module) REFERENCES ir_module ON DELETE CASCADE
 );
 
-CREATE SEQUENCE ir_cache_id_seq;
-
 CREATE TABLE ir_cache (
-    id INTEGER DEFAULT NEXTVAL('ir_cache_id_seq') NOT NULL,
+    id INTEGER GENERATED BY DEFAULT AS IDENTITY,
     name VARCHAR NOT NULL,
     "timestamp" TIMESTAMP WITHOUT TIME ZONE
 );
```

### Comparing `trytond-6.6.8/trytond/backend/postgresql/table.py` & `trytond-6.8.0/trytond/backend/postgresql/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,19 +24,14 @@
         self.__columns = None
         self.__constraints = None
         self.__fk_deltypes = None
         self.__indexes = None
 
         transaction = Transaction()
         cursor = transaction.connection.cursor()
-        # Create sequence if necessary
-        if not transaction.database.sequence_exist(
-                transaction.connection, self.sequence_name):
-            transaction.database.sequence_create(
-                transaction.connection, self.sequence_name)
 
         # Create new table if necessary
         if not self.table_exist(self.table_name):
             cursor.execute(SQL('CREATE TABLE {} ()').format(
                     Identifier(self.table_name)))
         self.table_schema = transaction.database.get_table_schema(
             transaction.connection, self.table_name)
@@ -47,62 +42,84 @@
         self.is_owner, = cursor.fetchone()
 
         if model.__doc__ and self.is_owner:
             cursor.execute(SQL('COMMENT ON TABLE {} IS %s').format(
                         Identifier(self.table_name)),
                 (model.__doc__,))
 
+        def migrate_to_identity(table, column):
+            previous_seq_name = f"{table}_{column}_seq"
+            cursor.execute(
+                "SELECT nextval(format(%s, %s))", ('%I', previous_seq_name,))
+            next_val, = cursor.fetchone()
+            cursor.execute(
+                "SELECT seqincrement, seqmax, seqmin, seqcache "
+                "FROM pg_sequence WHERE seqrelid = %s::regclass",
+                (previous_seq_name,))
+            increment, s_max, s_min, cache = cursor.fetchone()
+            # Previously created sequences were setting bigint values for those
+            # identity column mimic the type of the underlying column
+            if (s_max > 2 ** 31 - 1
+                    and self._columns[column]['typname'] != 'int8'):
+                s_max = 2 ** 31 - 1
+            if (s_min < -(2 ** 31)
+                    and self._columns[column]['typname'] != 'int8'):
+                s_min = -(2 ** 31)
+            cursor.execute(
+                SQL("ALTER TABLE {} ALTER COLUMN {} DROP DEFAULT").format(
+                    Identifier(table), Identifier(column)))
+            cursor.execute(
+                SQL("DROP SEQUENCE {}").format(
+                    Identifier(previous_seq_name)))
+            cursor.execute(
+                SQL("ALTER TABLE {} ALTER COLUMN {} "
+                    "ADD GENERATED BY DEFAULT AS IDENTITY").format(
+                    Identifier(table), Identifier(column)))
+            cursor.execute(
+                "SELECT pg_get_serial_sequence(format(%s, %s), %s)",
+                ('%I', table, column))
+            serial_seq_name, = cursor.fetchone()
+            cursor.execute(
+                (f"ALTER SEQUENCE {serial_seq_name} INCREMENT BY %s "
+                    "MINVALUE %s MAXVALUE %s RESTART WITH %s CACHE %s"),
+                (increment, s_min, s_max, next_val, cache))
+
+        update_definitions = False
         if 'id' not in self._columns:
+            update_definitions = True
             if not self.history:
                 cursor.execute(
                     SQL(
                         "ALTER TABLE {} ADD COLUMN id INTEGER "
-                        "DEFAULT nextval(format(%s, %s)) NOT NULL").format(
-                        Identifier(self.table_name)),
-                    ('%I', self.sequence_name))
-                cursor.execute(
-                    SQL('ALTER TABLE {} ADD PRIMARY KEY(id)')
-                    .format(Identifier(self.table_name)))
+                        "GENERATED BY DEFAULT AS IDENTITY PRIMARY KEY").format(
+                        Identifier(self.table_name)))
             else:
                 cursor.execute(
                     SQL('ALTER TABLE {} ADD COLUMN id INTEGER')
                     .format(Identifier(self.table_name)))
-            self._update_definitions(columns=True)
+        else:
+            if not self.history and not self.__columns['id']['identity']:
+                update_definitions = True
+                migrate_to_identity(self.table_name, 'id')
         if self.history and '__id' not in self._columns:
+            update_definitions = True
             cursor.execute(
                 SQL(
                     "ALTER TABLE {} ADD COLUMN __id INTEGER "
-                    "DEFAULT nextval(format(%s, %s)) NOT NULL").format(
-                        Identifier(self.table_name)),
-                ('%I', self.sequence_name))
-            cursor.execute(
-                SQL('ALTER TABLE {} ADD PRIMARY KEY(__id)')
-                .format(Identifier(self.table_name)))
-            self._update_definitions(columns=True)
-        else:
-            default = (
-                "nextval((format('%%I'::text, '%s'))::regclass)"
-                % self.sequence_name)
-            if self.history:
-                if self._columns['__id']['default'] != default:
-                    cursor.execute(
-                        SQL("ALTER TABLE {} "
-                            "ALTER __id SET "
-                            "DEFAULT nextval(format(%s, %s))")
-                        .format(Identifier(self.table_name)),
-                        ('%I', self.sequence_name))
-                    self._update_definitions(columns=True)
-            if self._columns['id']['default'] != default:
+                    "GENERATED BY DEFAULT AS IDENTITY PRIMARY KEY").format(
+                        Identifier(self.table_name)))
+        elif self.history:
+            if not self.__columns['__id']['identity']:
+                update_definitions = True
                 cursor.execute(
-                    SQL("ALTER TABLE {} "
-                        "ALTER id SET "
-                        "DEFAULT nextval(format(%s, %s))")
-                    .format(Identifier(self.table_name)),
-                    ('%I', self.sequence_name,))
-                self._update_definitions(columns=True)
+                    SQL("ALTER TABLE {} ALTER COLUMN id DROP DEFAULT").format(
+                        Identifier(self.table_name)))
+                migrate_to_identity(self.table_name, '__id')
+        if update_definitions:
+            self._update_definitions(columns=True)
 
     @classmethod
     def table_exist(cls, table_name):
         transaction = Transaction()
         return bool(transaction.database.get_table_schema(
                 transaction.connection, table_name))
 
@@ -111,19 +128,14 @@
         transaction = Transaction()
         cursor = transaction.connection.cursor()
         # Rename table
         if (cls.table_exist(old_name)
                 and not cls.table_exist(new_name)):
             cursor.execute(SQL('ALTER TABLE {} RENAME TO {}').format(
                     Identifier(old_name), Identifier(new_name)))
-        # Rename sequence
-        old_sequence = old_name + '_id_seq'
-        new_sequence = new_name + '_id_seq'
-        transaction.database.sequence_rename(
-            transaction.connection, old_sequence, new_sequence)
         # Rename history table
         old_history = old_name + "__history"
         new_history = new_name + "__history"
         if (cls.table_exist(old_history)
                 and not cls.table_exist(new_history)):
             cursor.execute('ALTER TABLE "%s" RENAME TO "%s"'
                 % (old_history, new_history))
@@ -151,24 +163,25 @@
         if self.__columns is None:
             cursor = Transaction().connection.cursor()
             self.__columns = {}
             # Fetch columns definitions from the table
             cursor.execute('SELECT '
                 'column_name, udt_name, is_nullable, '
                 'character_maximum_length, '
-                'column_default '
+                'column_default, is_identity '
                 'FROM information_schema.columns '
                 'WHERE table_name = %s AND table_schema = %s',
                 (self.table_name, self.table_schema))
-            for column, typname, nullable, size, default in cursor:
+            for column, typname, nullable, size, default, identity in cursor:
                 self.__columns[column] = {
                     'typname': typname,
                     'notnull': True if nullable == 'NO' else False,
                     'size': size,
                     'default': default,
+                    'identity': False if identity == 'NO' else True,
                     }
         return self.__columns
 
     @property
     def _constraints(self):
         if self.__constraints is None:
             cursor = Transaction().connection.cursor()
@@ -300,36 +313,49 @@
                         'ALTER TABLE {} ALTER COLUMN {} TYPE timestamp')
                     .format(
                         Identifier(self.table_name),
                         Identifier(column_name)))
 
             add_comment()
             base_type = column_type[0].lower()
-            if base_type != self._columns[column_name]['typname']:
-                if (self._columns[column_name]['typname'], base_type) in [
+            typname = self._columns[column_name]['typname']
+            if base_type != typname:
+                if (typname, base_type) in [
                         ('varchar', 'text'),
                         ('text', 'varchar'),
                         ('date', 'timestamp'),
+                        ('int2', 'int4'),
+                        ('int2', 'float4'),
+                        ('int2', 'int8'),
+                        ('int2', 'float8'),
+                        ('int2', 'numeric'),
                         ('int4', 'int8'),
                         ('int4', 'float8'),
                         ('int4', 'numeric'),
                         ('int8', 'float8'),
                         ('int8', 'numeric'),
+                        ('float4', 'numeric'),
+                        ('float4', 'float8'),
                         ('float8', 'numeric'),
                         ]:
                     self.alter_type(column_name, base_type)
+                elif (typname, base_type) in [
+                        ('int8', 'int4'),
+                        ('int8', 'int2'),
+                        ('int4', 'int2'),
+                        ('float8', 'float4'),
+                        ]:
+                    pass
                 else:
                     logger.warning(
                         'Unable to migrate column %s on table %s '
                         'from %s to %s.',
-                        column_name, self.table_name,
-                        self._columns[column_name]['typname'], base_type)
+                        column_name, self.table_name, typname, base_type)
 
-            if (base_type == 'varchar'
-                    and self._columns[column_name]['typname'] == 'varchar'):
+            if base_type == typname == 'varchar':
                 # Migrate size
                 from_size = self._columns[column_name]['size']
                 if field_size is None:
                     if from_size:
                         self.alter_size(column_name, base_type)
                 elif from_size == field_size:
                     pass
```

### Comparing `trytond-6.6.8/trytond/backend/sqlite/database.py` & `trytond-6.8.0/trytond/backend/sqlite/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from weakref import WeakKeyDictionary
 
 from sql import Expression, Flavor, Literal, Null, Query, Table
 from sql.conditionals import NullIf
 from sql.functions import (
     CharLength, CurrentTimestamp, Extract, Function, Overlay, Position,
     Substring, Trim)
-from werkzeug.security import safe_join
 
 from trytond.backend.database import DatabaseInterface, SQLType
 from trytond.config import config, parse_uri
+from trytond.tools import safe_join
 from trytond.transaction import Transaction
 
 __all__ = [
     'Database',
     'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError']
 logger = logging.getLogger(__name__)
```

### Comparing `trytond-6.6.8/trytond/backend/sqlite/init.sql` & `trytond-6.8.0/trytond/backend/sqlite/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/backend/sqlite/table.py` & `trytond-6.8.0/trytond/backend/sqlite/table.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/backend/table.py` & `trytond-6.8.0/trytond/backend/table.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/bus.py` & `trytond-6.8.0/trytond/bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,21 @@
 import json
 import logging
 import os
 import selectors
 import threading
 import time
 import uuid
-
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
 from urllib.parse import urljoin
 
-from werkzeug.exceptions import BadRequest
-from werkzeug.exceptions import NotImplemented as NotImplementedException
-from werkzeug.utils import redirect
-from werkzeug.wrappers import Response
-
 from trytond import backend
 from trytond.config import config
 from trytond.protocols.jsonrpc import JSONDecoder, JSONEncoder
+from trytond.protocols.wrappers import (
+    HTTPStatus, Response, exceptions, redirect)
 from trytond.tools import resolve
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 logger = logging.getLogger(__name__)
 
 _db_timeout = config.getint('database', 'timeout')
@@ -143,15 +134,15 @@
         logger.debug('Bus: %s', response_data)
         return response_data
 
     @classmethod
     def _listen(cls, database):
         db = backend.Database(database)
         if not db.has_channel():
-            raise NotImplementedException
+            raise exceptions.NotImplemented
 
         logger.info("listening on channel '%s'", cls._channel)
         conn = db.get_connection(autocommit=True)
         pid = os.getpid()
         selector = selectors.DefaultSelector()
         try:
             cursor = conn.cursor()
@@ -223,26 +214,26 @@
     Bus = LongPollingBus
 
 
 @app.route('/<string:database_name>/bus', methods=['POST'])
 @app.auth_required
 def subscribe(request, database_name):
     if not _allow_subscribe:
-        raise NotImplementedException
+        raise exceptions.NotImplemented
     if _url_host and _url_host != request.host_url:
         response = redirect(
             urljoin(_url_host, request.path), HTTPStatus.PERMANENT_REDIRECT)
         # Allow to change the redirection after some time
         response.headers['Cache-Control'] = (
             'private, max-age=%s' % _web_cache_timeout)
         return response
     user = request.authorization.get('userid')
     channels = request.parsed_data.get('channels', [])
     if user is None:
-        raise BadRequest
+        raise exceptions.BadRequest
 
     channels = set(filter(lambda c: not c.startswith('user:'), channels))
     channels.add('user:%s' % user)
 
     last_message = request.parsed_data.get('last_message')
 
     logger.debug(
```

### Comparing `trytond-6.6.8/trytond/cache.py` & `trytond-6.8.0/trytond/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from trytond.config import config
 from trytond.pool import Pool
 from trytond.tools import grouped_slice, resolve
 from trytond.transaction import Transaction
 
 __all__ = ['BaseCache', 'Cache', 'LRUDict', 'LRUDictTransaction']
 _clear_timeout = config.getint('cache', 'clean_timeout', default=5 * 60)
+_default_size_limit = config.getint('cache', 'default')
 logger = logging.getLogger(__name__)
 
 
 def _cast(column):
     class SQLite_DateTime(Function):
         __slots__ = ()
         _function = 'DATETIME'
@@ -60,19 +61,32 @@
             where=ir_module.state.in_(
                 ['activated', 'to upgrade', 'to remove'])))
     return {m for m, in cursor}
 
 
 class BaseCache(object):
     _instances = {}
-
-    def __init__(self, name, size_limit=1024, duration=None, context=True):
+    context_ignored_keys = {
+        'client', '_request', '_check_access', '_skip_warnings',
+        }
+
+    def __init__(
+            self, name, duration=None, context=True,
+            context_ignored_keys=None):
+        assert ((context_ignored_keys is not None and context)
+            or (context_ignored_keys is None)), (
+                f"context_ignored_keys ({context_ignored_keys}) is not valid"
+                f" in regards to context ({context}).")
         self._name = name
-        self.size_limit = size_limit
+        self.size_limit = config.getint(
+            'cache', name, default=_default_size_limit)
         self.context = context
+        self.context_ignored_keys = set()
+        if context and context_ignored_keys:
+            self.context_ignored_keys.update(context_ignored_keys)
         self.hit = self.miss = 0
         if isinstance(duration, dt.timedelta):
             self.duration = duration
         elif isinstance(duration, (int, float)):
             self.duration = dt.timedelta(seconds=duration)
         elif duration:
             self.duration = dt.timedelta(**duration)
@@ -89,18 +103,17 @@
                 'hit': inst.hit,
                 'miss': inst.miss,
                 }
 
     def _key(self, key):
         if self.context:
             context = Transaction().context.copy()
-            context.pop('client', None)
-            context.pop('_request', None)
-            context.pop('_check_access', None)
-            context.pop('_skip_warnings', None)
+            for k in (self.__class__.context_ignored_keys
+                    | self.context_ignored_keys):
+                context.pop(k, None)
             return (key, Transaction().user, freeze(context))
         return key
 
     def get(self, key, default=None):
         raise NotImplementedError
 
     def set(self, key, value):
@@ -153,15 +166,15 @@
         self._transaction_lower = {}
         self._timestamp = {}
 
     def _get_cache(self):
         transaction = Transaction()
         dbname = transaction.database.name
         lower = self._transaction_lower.get(dbname, self._default_lower)
-        if (transaction in self._reset
+        if (self._name in self._reset.get(transaction, set())
                 or transaction.started_at < lower):
             try:
                 return self._transaction_cache[transaction]
             except KeyError:
                 cache = self._database_cache.default_factory()
                 self._transaction_cache[transaction] = cache
                 return cache
```

### Comparing `trytond-6.6.8/trytond/commandline.py` & `trytond-6.8.0/trytond/commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
     parser = get_base_parser()
     parser.add_argument("-d", "--database", dest="database_name",
         required=True, metavar='DATABASE', help="specify the database name")
     parser.add_argument("--histsize", dest="histsize", type=int, default=500,
         help="The number of commands to remember in the command history")
     parser.add_argument("--readonly", dest="readonly", action='store_true',
         help="Start a readonly transaction")
+    parser.add_argument(
+        "--lock-table", dest="lock_tables", nargs='+', default=[],
+        metavar='TABLE', help="Lock tables")
     parser.epilog = "To store changes, `transaction.commit()` must be called."
     return parser
 
 
 def get_parser_stat():
     parser = get_base_parser()
     parser.epilog = "To exit press 'q', to inverse sort order press 'r'."
```

### Comparing `trytond-6.6.8/trytond/config.py` & `trytond-6.8.0/trytond/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import configparser
 import logging
 import os
 import urllib.parse
+from getpass import getuser
 
 import __main__ as main
 
 from . import status
 
 __all__ = ['config', 'get_hostname', 'get_port', 'split_netloc',
     'parse_listen', 'parse_uri']
@@ -60,28 +61,33 @@
             os.environ.get('TRYTOND_DATABASE_URI', 'sqlite://'))
         self.set('database', 'path', os.path.join(
                 os.path.expanduser('~'), 'db'))
         self.set('database', 'list', 'True')
         self.set('database', 'retry', '5')
         self.set('database', 'language', 'en')
         self.set('database', 'timeout', str(30 * 60))
+        self.set('database', 'subquery_threshold', str(1_000))
         self.add_section('request')
         self.set('request', 'max_size', str(2 * 1024 * 1024))
         self.set('request', 'max_size_authenticated',
             str(2 * 1024 * 1024 * 1024))
         self.add_section('cache')
         self.set('cache', 'transaction', '10')
         self.set('cache', 'model', '200')
         self.set('cache', 'record', '2000')
         self.set('cache', 'field', '100')
+        self.set('cache', 'default', '1024')
+        self.set('cache', 'ir.message', '10240')
+        self.set('cache', 'ir.translation', '10240')
         self.add_section('queue')
         self.set('queue', 'worker', 'False')
         self.add_section('ssl')
         self.add_section('email')
         self.set('email', 'uri', 'smtp://localhost:25')
+        self.set('email', 'from', getuser())
         self.add_section('session')
         self.set('session', 'authentications', 'password')
         self.set('session', 'max_age', str(60 * 60 * 24 * 30))
         self.set('session', 'timeout', str(60 * 5))
         self.set('session', 'max_attempt', '5')
         self.set('session', 'max_attempt_ip_network', '300')
         self.set('session', 'ip_network_4', '32')
```

### Comparing `trytond-6.6.8/trytond/console.py` & `trytond-6.8.0/trytond/console.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 def run(options):
     db_name = options.database_name
     pool = Pool(db_name)
     with Transaction().start(db_name, 0, readonly=True):
         pool.init()
 
     with Transaction().start(
-            db_name, 0, readonly=options.readonly) as transaction:
+            db_name, 0, readonly=options.readonly,
+            _lock_tables=options.lock_tables) as transaction:
         local = {
             'pool': pool,
             'transaction': transaction,
             }
         if sys.stdin.isatty():
             console = Console(local, histsize=options.histsize)
             banner = "Tryton %s, Python %s on %s" % (
```

### Comparing `trytond-6.6.8/trytond/convert.py` & `trytond-6.8.0/trytond/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import defaultdict
 from decimal import Decimal
 from xml import sax
 
 from trytond import __version__
 from trytond.pyson import CONTEXT, PYSONEncoder
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 logger = logging.getLogger(__name__)
 
 CDATA_START = re.compile(r'^\s*\<\!\[cdata\[', re.IGNORECASE)
 CDATA_END = re.compile(r'\]\]\>\s*$', re.IGNORECASE)
 
 
@@ -246,15 +246,15 @@
             if pyson_attr:
                 context.update(CONTEXT)
 
             field = self.model._fields[field_name]
             if search_attr:
                 search_model = field.model_name
                 SearchModel = self.mh.pool.get(search_model)
-                with Transaction().set_context(active_test=False):
+                with inactive_records():
                     found, = SearchModel.search(eval(search_attr, context))
                     self.values[field_name] = found.id
 
             elif ref_attr:
                 model, id_ = self.mh.get_id(ref_attr)
                 if field._type == 'reference':
                     self.values[field_name] = '%s,%s' % (model, id_)
@@ -400,15 +400,15 @@
         for model_name in record_ids.keys():
             try:
                 Model = self.pool.get(model_name)
             except KeyError:
                 continue
             self.browserecord[module][model_name] = {}
             for sub_record_ids in grouped_slice(record_ids[model_name]):
-                with Transaction().set_context(active_test=False):
+                with inactive_records():
                     records = Model.search([
                         ('id', 'in', list(sub_record_ids)),
                         ], order=[('id', 'ASC')])
                 with Transaction().set_context(language='en'):
                     models = Model.browse(list(map(int, records)))
                 for model in models:
                     self.browserecord[module][model_name][model.id] = model
@@ -787,15 +787,15 @@
     """
     Remove the records that are given in to_delete.
     """
     transaction = Transaction()
     mdata_delete = []
     ModelData = pool.get("ir.model.data")
 
-    with Transaction().set_context(active_test=False):
+    with inactive_records():
         mdata = ModelData.search([
             ('fs_id', 'in', to_delete),
             ('module', '=', module),
             ], order=[('id', 'DESC')])
 
     for mrec in mdata:
         model, db_id, fs_id = mrec.model, mrec.db_id, mrec.fs_id
```

### Comparing `trytond-6.6.8/trytond/cron.py` & `trytond-6.8.0/trytond/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/exceptions.py` & `trytond-6.8.0/trytond/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/filestore.py` & `trytond-6.8.0/trytond/filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/i18n.py` & `trytond-6.8.0/trytond/i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/__init__.py` & `trytond-6.8.0/trytond/ir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         model.ModelAccess,
         model.ModelFieldAccess,
         model.ModelButton,
         model.ModelButtonRule,
         model.ModelButtonClick,
         model.ModelButtonReset,
         model.ModelData,
+        model.Log,
         model.PrintModelGraphStart,
         attachment.Attachment,
         note.Note,
         note.NoteRead,
         avatar.Avatar,
         avatar.AvatarCache,
         cron.Cron,
```

### Comparing `trytond-6.6.8/trytond/ir/action.py` & `trytond-6.8.0/trytond/ir/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DeactivableMixin, Index, ModelSingleton, ModelSQL, ModelStorage, ModelView,
     fields, sequence_ordered)
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
 from trytond.pyson import PYSON, Eval, PYSONDecoder, PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import file_open
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 if not config.get('html', 'plugins-ir.action.report-report_content_html'):
     config.set(
         'html', 'plugins-ir.action.report-report_content_html', 'fullpage')
 
 
 class WizardModelError(ValidationError):
@@ -49,15 +49,20 @@
 EMAIL_REFKEYS = set(('cc', 'to', 'subject'))
 
 
 class Action(DeactivableMixin, ModelSQL, ModelView):
     "Action"
     __name__ = 'ir.action'
     name = fields.Char('Name', required=True, translate=True)
-    type = fields.Char('Type', required=True, readonly=True)
+    type = fields.Selection([
+            ('ir.action.report', "Report"),
+            ('ir.action.act_window', "Window"),
+            ('ir.action.wizard', "Wizard"),
+            ('ir.action.url', "URL"),
+            ], "Type", required=True, readonly=True)
     records = fields.Selection([
             ('selected', "Selected"),
             ('listed', "Listed"),
             ], "Records",
         help="The records on which the action runs.")
     usage = fields.Char('Usage')
     keywords = fields.One2Many('ir.action.keyword', 'action',
@@ -82,34 +87,34 @@
     @classmethod
     def write(cls, actions, values, *args):
         pool = Pool()
         super(Action, cls).write(actions, values, *args)
         pool.get('ir.action.keyword')._get_keyword_cache.clear()
 
     @classmethod
+    @inactive_records
     def get_action_id(cls, action_id):
         pool = Pool()
-        with Transaction().set_context(active_test=False):
-            if cls.search([
-                        ('id', '=', action_id),
-                        ]):
-                return action_id
-            for action_type in (
-                    'ir.action.report',
-                    'ir.action.act_window',
-                    'ir.action.wizard',
-                    'ir.action.url',
-                    ):
-                Action = pool.get(action_type)
-                actions = Action.search([
+        if cls.search([
                     ('id', '=', action_id),
-                    ])
-                if actions:
-                    action, = actions
-                    return action.action.id
+                    ]):
+            return action_id
+        for action_type in (
+                'ir.action.report',
+                'ir.action.act_window',
+                'ir.action.wizard',
+                'ir.action.url',
+                ):
+            Action = pool.get(action_type)
+            actions = Action.search([
+                ('id', '=', action_id),
+                ])
+            if actions:
+                action, = actions
+                return action.action.id
 
     @classmethod
     def get_action_values(cls, type_, action_ids, columns=None):
         pool = Pool()
         Action = pool.get(type_)
         if columns is None:
             columns = []
@@ -154,14 +159,15 @@
     action = fields.Many2One('ir.action', 'Action',
         ondelete='CASCADE')
     _get_keyword_cache = Cache('ir_action_keyword.get_keyword')
 
     @classmethod
     def __setup__(cls):
         super(ActionKeyword, cls).__setup__()
+        cls.__access__.add('action')
         table = cls.__table__()
 
         cls.__rpc__.update({
                 'get_keyword': RPC(cache=dict(days=1)),
                 })
         cls._sql_indexes.add(
             Index(
@@ -299,18 +305,25 @@
         return keywords
 
 
 class ActionMixin(ModelSQL):
     _order_name = 'action'
     _action_name = 'name'
 
+    action = fields.Many2One(
+        'ir.action', "Action", required=True, ondelete='CASCADE')
+
     @classmethod
     def __setup__(cls):
         pool = Pool()
         super(ActionMixin, cls).__setup__()
+        cls.__access__.add('action')
+        cls.action.domain = [
+            ('type', '=', cls.__name__),
+            ]
         Action = pool.get('ir.action')
         for name in dir(Action):
             field = getattr(Action, name)
             if (isinstance(field, fields.Field)
                     and not getattr(cls, name, None)):
                 setattr(cls, name, fields.Function(field, 'get_action',
                         setter='set_action', searcher='search_action'))
@@ -469,16 +482,14 @@
             "Content HTML",
             states={
                 'invisible': ~Eval('template_extension').in_(
                     ['html', 'xhtml']),
                 },
             depends=['template_extension']),
         'get_report_content_html', setter='set_report_content_html')
-    action = fields.Many2One('ir.action', 'Action', required=True,
-            ondelete='CASCADE')
     direct_print = fields.Boolean('Direct Print')
     single = fields.Boolean("Single",
         help="Check if the template works only for one record.")
     translatable = fields.Boolean("Translatable",
         help="Uncheck to disable translations for this report.")
     template_extension = fields.Selection([
             ('odt', 'OpenDocument Text'),
@@ -743,16 +754,14 @@
     act_window_views = fields.One2Many('ir.action.act_window.view',
             'act_window', 'Views')
     views = fields.Function(fields.Binary('Views'), 'get_views')
     act_window_domains = fields.One2Many('ir.action.act_window.domain',
         'act_window', 'Domains')
     domains = fields.Function(fields.Binary('Domains'), 'get_domains')
     limit = fields.Integer('Limit', help='Default limit for the list view.')
-    action = fields.Many2One('ir.action', 'Action', required=True,
-            ondelete='CASCADE')
     search_value = fields.Char('Search Criteria',
             help='Default search criteria for the list view.')
     pyson_domain = fields.Function(fields.Char('PySON Domain'), 'get_pyson')
     pyson_context = fields.Function(fields.Char('PySON Context'),
             'get_pyson')
     pyson_order = fields.Function(fields.Char('PySON Order'), 'get_pyson')
     pyson_search_value = fields.Function(fields.Char(
@@ -952,28 +961,42 @@
         return Action(action_id).get_action_value()
 
 
 class ActionActWindowView(
         sequence_ordered(), DeactivableMixin, ModelSQL, ModelView):
     "Action act window view"
     __name__ = 'ir.action.act_window.view'
-    view = fields.Many2One('ir.ui.view', 'View', required=True,
-            ondelete='CASCADE')
+    view = fields.Many2One(
+        'ir.ui.view', "View", required=True, ondelete='CASCADE',
+        domain=[
+            ('model', '=', Eval('model')),
+            ])
     act_window = fields.Many2One('ir.action.act_window', 'Action',
             ondelete='CASCADE')
+    model = fields.Function(fields.Char("Model"), 'on_change_with_model')
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.add('act_window')
 
     @classmethod
     def __register__(cls, module_name):
         super().__register__(module_name)
 
         table = cls.__table_handler__(module_name)
 
         # Migration from 5.0: remove required on sequence
         table.not_null_action('sequence', 'remove')
 
+    @fields.depends('act_window', '_parent_act_window.res_model')
+    def on_change_with_model(self, name=None):
+        if self.act_window:
+            return self.act_window.res_model
+
     @classmethod
     def create(cls, vlist):
         pool = Pool()
         windows = super(ActionActWindowView, cls).create(vlist)
         pool.get('ir.action.keyword')._get_keyword_cache.clear()
         return windows
 
@@ -997,14 +1020,19 @@
     name = fields.Char('Name', translate=True)
     domain = fields.Char('Domain')
     count = fields.Boolean('Count')
     act_window = fields.Many2One('ir.action.act_window', 'Action',
         required=True, ondelete='CASCADE')
 
     @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.add('act_window')
+
+    @classmethod
     def __register__(cls, module_name):
         super().__register__(module_name)
 
         table = cls.__table_handler__(module_name)
 
         # Migration from 5.0: remove required on sequence
         table.not_null_action('sequence', 'remove')
@@ -1073,16 +1101,14 @@
 
 
 class ActionWizard(ActionMixin, ModelSQL, ModelView):
     "Action wizard"
     __name__ = 'ir.action.wizard'
     _action_name = 'wiz_name'
     wiz_name = fields.Char('Wizard name', required=True)
-    action = fields.Many2One('ir.action', 'Action', required=True,
-            ondelete='CASCADE')
     model = fields.Char('Model')
     window = fields.Boolean('Window', help='Run wizard in a new window.')
 
     @staticmethod
     def default_type():
         return 'ir.action.wizard'
 
@@ -1093,18 +1119,28 @@
             (cls._action_name, '=', name),
             ]
         if action_id:
             domain.append(('id', '=', action_id))
         actions = cls.search(domain)
         return {a.model for a in actions if a.model}
 
+    @classmethod
+    def get_name(cls, name, model):
+        # TODO add cache
+        actions = cls.search([
+                (cls._action_name, '=', name),
+                ('model', '=', model),
+                ], limit=1)
+        if actions:
+            action, = actions
+            return action.name
+        return name
+
 
 class ActionURL(ActionMixin, ModelSQL, ModelView):
     "Action URL"
     __name__ = 'ir.action.url'
     url = fields.Char('Action Url', required=True)
-    action = fields.Many2One('ir.action', 'Action', required=True,
-            ondelete='CASCADE')
 
     @staticmethod
     def default_type():
         return 'ir.action.url'
```

### Comparing `trytond-6.6.8/trytond/ir/action.xml` & `trytond-6.8.0/trytond/ir/action.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/attachment.py` & `trytond-6.8.0/trytond/ir/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/attachment.xml` & `trytond-6.8.0/trytond/ir/attachment.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/avatar.py` & `trytond-6.8.0/trytond/ir/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/calendar_.py` & `trytond-6.8.0/trytond/ir/calendar_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/calendar_.xml` & `trytond-6.8.0/trytond/ir/calendar_.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/configuration.py` & `trytond-6.8.0/trytond/ir/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/cron.py` & `trytond-6.8.0/trytond/ir/cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from trytond.exceptions import UserError, UserWarning
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, dualmethod, fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.status import processing
 from trytond.tools import timezone as tz
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, TransactionError
 from trytond.worker import run_task
 
 logger = logging.getLogger(__name__)
 
 
 class Cron(DeactivableMixin, ModelSQL, ModelView):
     "Cron"
@@ -105,17 +105,17 @@
     @classmethod
     def default_timezone(cls):
         return tz.SERVER.tzname(datetime.datetime.now())
 
     def get_timezone(self, name):
         return self.default_timezone()
 
-    @staticmethod
-    def check_xml_record(crons, values):
-        return True
+    @classmethod
+    def check_xml_record(cls, crons, values):
+        pass
 
     @classmethod
     def view_attributes(cls):
         return [(
                 '//label[@id="time_label"]', 'states', {
                     'invisible': Eval('interval_type') == 'minutes',
                 }),
@@ -171,26 +171,35 @@
                     ])
 
             for cron in crons:
                 def duration():
                     return (time.monotonic() - started) * 1000
                 started = time.monotonic()
                 name = '<Cron %s@%s %s>' % (cron.id, db_name, cron.method)
-                for count in range(retry, -1, -1):
-                    if count != retry:
+                transaction_extras = {}
+                count = 0
+                while True:
+                    if count:
                         time.sleep(0.02 * (retry - count))
                     try:
                         with processing(name), \
-                                transaction.new_transaction() as cron_trans:
+                                transaction.new_transaction(
+                                    **transaction_extras) as cron_trans:
                             cron.run_once()
                             cron_trans.commit()
                     except Exception as e:
+                        if isinstance(e, TransactionError):
+                            cron_trans.rollback()
+                            e.fix(transaction_extras)
+                            continue
                         if (isinstance(e, backend.DatabaseOperationalError)
-                                and count):
-                            logger.debug("Retry: %i", retry - count + 1)
+                                and count < retry):
+                            cron_trans.rollback()
+                            count += 1
+                            logger.debug("Retry: %i", count)
                             continue
                         if isinstance(e, (UserError, UserWarning)):
                             Error.log(cron, e)
                             logger.info(
                                 "%s failed after %i ms", name, duration())
                         else:
                             logger.exception(
```

### Comparing `trytond-6.6.8/trytond/ir/cron.xml` & `trytond-6.8.0/trytond/ir/cron.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/date.py` & `trytond-6.8.0/trytond/ir/date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/email.xml` & `trytond-6.8.0/trytond/ir/email.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/email_.py` & `trytond-6.8.0/trytond/ir/email_.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,20 +182,19 @@
             recipients_secondary=cc,
             recipients_hidden=bcc,
             addresses=[{'address': a} for a in to_addrs],
             subject=subject,
             body=body,
             resource=record)
         email.save()
-        with Transaction().set_context(_check_access=False):
-            attachments_ = []
-            for name, data in files:
-                attachments_.append(
-                    Attachment(resource=email, name=name, data=data))
-            Attachment.save(attachments_)
+        attachments_ = []
+        for name, data in files:
+            attachments_.append(
+                Attachment(resource=email, name=name, data=data))
+        Attachment.save(attachments_)
         return email
 
     @classmethod
     def complete(cls, text, limit):
         limit = int(limit)
         if not limit > 0:
             raise ValueError('limit must be > 0: %r' % (limit,))
@@ -551,23 +550,23 @@
 
     @classmethod
     def get_languages(cls, value):
         pool = Pool()
         Configuration = pool.get('ir.configuration')
         Lang = pool.get('ir.lang')
         if isinstance(value, (list, tuple)):
-            languagues = {cls._get_language(v) for v in value}
+            languages = {cls._get_language(v) for v in value}
         else:
-            languagues = {cls._get_language(value)}
-        languagues = list(filter(None, languagues))
-        if not languagues:
+            languages = {cls._get_language(value)}
+        languages = list(filter(None, languages))
+        if not languages:
             return Lang.search([
                     ('code', '=', Configuration.get_language()),
                     ], limit=1)
-        return languagues
+        return languages
 
     @classmethod
     def _get_language(cls, record):
         pool = Pool()
         User = pool.get('res.user')
         if isinstance(record, User) and record.language:
             return record.language
```

### Comparing `trytond-6.6.8/trytond/ir/error.py` & `trytond-6.8.0/trytond/ir/error.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/error.xml` & `trytond-6.8.0/trytond/ir/error.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/exceptions.py` & `trytond-6.8.0/trytond/ir/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/export.py` & `trytond-6.8.0/trytond/ir/export.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/export.xml` & `trytond-6.8.0/trytond/ir/export.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/fonts/LICENSE` & `trytond-6.8.0/trytond/ir/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/fonts/karla.ttf` & `trytond-6.8.0/trytond/ir/fonts/karla.ttf`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ir.xml` & `trytond-6.8.0/trytond/ir/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/lang.py` & `trytond-6.8.0/trytond/ir/lang.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.model import (
     Check, DeactivableMixin, ModelSQL, ModelView, Unique, fields)
 from trytond.modules import create_graph, load_translations
 from trytond.pool import Pool
 from trytond.pyson import Eval
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 Transaction.cache_keys.add('translate_name')
 
 
 class GroupingError(UserError):
     pass
@@ -34,14 +34,17 @@
     pass
 
 
 class DeleteDefaultError(UserError):
     pass
 
 
+NO_BREAKING_SPACE = '\u00A0'
+
+
 class Lang(DeactivableMixin, ModelSQL, ModelView):
     "Language"
     __name__ = "ir.lang"
     name = fields.Char('Name', required=True, translate=True)
     code = fields.Char('Code', required=True, help="RFC 4646 tag.")
     translatable = fields.Boolean('Translatable', readonly=True)
     parent = fields.Char("Parent Code", help="Code of the exceptional parent")
@@ -303,17 +306,17 @@
         for lang in langs:
             if (lang.code == Config.get_language()
                     and not lang.translatable):
                 raise TranslatableError(
                     gettext('ir.msg_language_default_translatable',
                         language=lang.rec_name))
 
-    @staticmethod
-    def check_xml_record(langs, values):
-        return True
+    @classmethod
+    def check_xml_record(cls, langs, values):
+        pass
 
     @classmethod
     def get_translatable_languages(cls):
         res = cls._lang_cache.get('translatable_languages')
         if res is None:
             langs = cls.search([
                     ('translatable', '=', True),
@@ -358,24 +361,24 @@
         cls._lang_cache.clear()
         cls._code_cache.clear()
         super(Lang, cls).delete(langs)
         Translation._get_language_cache.clear()
         _parents.clear()
 
     @classmethod
+    @inactive_records
     def get(cls, code=None):
         "Return language instance for the code or the transaction language"
         if code is None:
             code = Transaction().language
         lang_id = cls._code_cache.get(code)
         if not lang_id:
-            with Transaction().set_context(active_test=False):
-                lang, = cls.search([
-                        ('code', '=', code),
-                        ])
+            lang, = cls.search([
+                    ('code', '=', code),
+                    ])
             cls._code_cache.set(code, lang.id)
         else:
             lang = cls(lang_id)
         return lang
 
     def _group(self, s, monetary=False):
         # Code from _group in locale.py
@@ -469,15 +472,15 @@
                 formatted = _strip_padding(formatted, seps)
         elif percent[-1] in 'diu':
             seps = 0
             if grouping:
                 formatted, seps = self._group(formatted, monetary=monetary)
             if seps:
                 formatted = _strip_padding(formatted, seps)
-        return formatted
+        return formatted.replace(' ', NO_BREAKING_SPACE)
 
     def currency(
             self, val, currency, symbol=True, grouping=False, digits=None):
         """
         Formats val according to the currency settings in lang.
         """
         # Code from currency in locale.py
@@ -497,14 +500,17 @@
 
         if symbol:
             smb = currency.symbol
             precedes = (val < 0 and self.n_cs_precedes
                 or self.p_cs_precedes)
             separated = (val < 0 and self.n_sep_by_space
                 or self.p_sep_by_space)
+            if not smb and hasattr(currency, 'code'):
+                smb = currency.code
+                separated = True
 
             if precedes:
                 s = smb + (separated and ' ' or '') + s
             else:
                 s = s + (separated and ' ' or '') + smb
 
         sign_pos = val < 0 and self.n_sign_posn or self.p_sign_posn
@@ -521,15 +527,17 @@
         elif sign_pos == 4:
             s = s.replace('>', sign)
         else:
             # the default if nothing specified;
             # this should be the most fitting sign position
             s = sign + s
 
-        return s.replace('<', '').replace('>', '')
+        return (
+            s.replace('<', '').replace('>', '')
+            .replace(' ', NO_BREAKING_SPACE))
 
     def strftime(self, value, format=None):
         '''
         Convert value to a string as specified by the format argument.
         '''
         pool = Pool()
         Month = pool.get('ir.calendar.month')
@@ -554,35 +562,34 @@
                 time = None
         if time:
             if time < datetime.time(12):
                 p = self.am or 'AM'
             else:
                 p = self.pm or 'PM'
             format = format.replace('%p', p)
-        return value.strftime(format)
+        return value.strftime(format).replace(' ', NO_BREAKING_SPACE)
 
     def format_number(self, value, digits=None, grouping=True, monetary=None):
         if digits is None:
             d = value
             if not isinstance(d, Decimal):
                 d = Decimal(repr(value))
             digits = -int(d.as_tuple().exponent)
         return self.format(
             '%.*f', (digits, value), grouping=grouping, monetary=monetary)
 
     def format_number_symbol(self, value, symbol, digits=None, grouping=True):
         symbol, position = symbol.get_symbol(value)
-        separated = (
-            value < 0 and self.n_sep_by_space or self.p_sep_by_space)
+        separated = True
         s = self.format_number(value, digits, grouping)
         if position:
             s = s + (separated and ' ' or '') + symbol
         else:
             s = symbol + (separated and ' ' or '') + s
-        return s
+        return s.replace(' ', NO_BREAKING_SPACE)
 
 
 class LangConfigStart(ModelView):
     "Configure languages"
     __name__ = 'ir.lang.config.start'
 
     languages = fields.Many2Many('ir.lang', None, None, "Languages")
```

### Comparing `trytond-6.6.8/trytond/ir/lang.xml` & `trytond-6.8.0/trytond/ir/lang.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/locale/bg.po` & `trytond-6.8.0/trytond/ir/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,19 @@
 msgid "Name"
 msgstr "Име на прикачен файл"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Действие"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Модел"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Изглед"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Действие"
@@ -1032,14 +1037,37 @@
 msgid "Read Access"
 msgstr "Права за четене"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Права за писане"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Действие"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ресурс"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Потребител"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Филтър"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Ниво"
@@ -2000,14 +2028,18 @@
 msgstr "Fields"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Започване на изчакващите инталации/обновявания"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_config"
@@ -2518,14 +2550,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2643,15 +2679,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Бележка"
 
@@ -2900,19 +2936,18 @@
 msgstr "Не може да изтривате модул който инсталиран или ще бъде инсталиран"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Бележки"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -3017,14 +3052,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3100,30 +3139,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3227,14 +3269,19 @@
 msgid "Model field"
 msgstr "Поле на модел"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Модел на достъп до поле"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Печат на графика на модел"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Модул"
@@ -3487,14 +3534,18 @@
 msgstr "Fields Access"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
@@ -3641,23 +3692,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Избор"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Справка"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Прозорец"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Избор"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Справка"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Прозорец"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Форма за действие"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Свързана форма"
@@ -3679,32 +3770,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Избор"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Справка"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Прозорец"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Избор"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Справка"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Прозорец"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Избор"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Справка"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Прозорец"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Данни"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Препратка"
@@ -3768,14 +3919,37 @@
 msgid "Left-to-right"
 msgstr "Отляво надясно"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Отдясно наляво"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "При изтриване"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Превод"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3987,14 +4161,29 @@
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Форматиране на числа"
 
 #, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Дата"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Часове"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Път"
+
+#, fuzzy
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Модулите са обновени / инсталирани !"
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/ca.po` & `trytond-6.8.0/trytond/ir/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Acció"
 
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vista"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Acció"
@@ -954,14 +958,34 @@
 msgid "Read Access"
 msgstr "Permís per llegir"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Permís per modificar"
 
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Acció"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr "Esdeveniment"
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Recurs"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr "Desti"
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Usuari"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtre"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Nivell"
@@ -1859,14 +1883,18 @@
 msgid "Fields"
 msgstr "Camps"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr "Registres"
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realitza activacions/actualitzacions pendents"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configura els mòduls"
@@ -2336,14 +2364,18 @@
 msgid "Slovenian"
 msgstr "Eslovè"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turc"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr "Ucraïnès"
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Xinès simplificat"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Configurar els idiomes"
@@ -2457,16 +2489,18 @@
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu eliminar els registres \"%(ids)s\" de \"%(model)s\" per alguna de les següents regles:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "No podeu eliminar aquest registre."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"No teniu permisos per eliminar el registre %(record)s\" del model "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "No"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2706,20 +2740,18 @@
 msgstr "No podeu eliminar un mòdul que està activat o serà activat."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Esteu intentant llegir els registres \"%(ids)s\" del model \"%(model)s\" que"
-" ja no existeixen."
+" no existeixen."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu llegir els registres \"%(ids)s\" de \"%(model)s\" per almenys una d'aquestes regles:\n"
@@ -2829,14 +2861,18 @@
 msgid "Missing sequence."
 msgstr "No s'ha trobat la seqüència."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta funció d'escriptura del camp \"%(field)s\" a \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr "Només es pot crear un singleton."
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
 " es massa llarg (%(size)i > %(max_size)i)."
@@ -2922,30 +2958,34 @@
 msgstr ""
 "El domini o el criteri de cerca \"%(domain)s\" de l'acció \"%(action)s\" es "
 "invàlid."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Esteu intentant escriure als registres \"%(ids)s\" del model \"%(model)s\" "
-"que ja no existeixen."
+"que no existeixen."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu modificar els registres \"%(ids)s\" de \"%(model)s\" per almenys una d'aquestes regles:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "No podeu modificar aquest registre."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr ""
+"No podeu modificar el camp \"%(field)s\" del registre \"%(record)s\" de "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Error de sintaxis per l'ID de XML: %(value)r\" en \"%(field)s\" de "
@@ -3047,14 +3087,18 @@
 msgid "Model field"
 msgstr "Camp model"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Permís camp del model"
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Registre"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Imprimeix gràfica del model"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Mòdul"
@@ -3275,14 +3319,18 @@
 msgid "Fields Access"
 msgstr "Accés camps"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr "Registres"
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realitza activacions/actualitzacions pendents"
@@ -3403,22 +3451,54 @@
 msgid "Listed"
 msgstr "Llistats"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Seleccionats"
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Finestra"
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Llistats"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Seleccionats"
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Finestra"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Acció formulari"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Formulari relacionat"
@@ -3439,30 +3519,78 @@
 msgid "Listed"
 msgstr "Llistats"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Seleccionats"
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Finestra"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Llistats"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Seleccionats"
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Finestra"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Llistats"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Seleccionats"
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Finestra"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Dades"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Vincle"
@@ -3523,14 +3651,34 @@
 msgid "Left-to-right"
 msgstr "D'esquerra a dreta"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "De dreta a esquerra"
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clica a"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Eliminat"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr "Executat"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr "Modificat"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Transicionat a"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Activat"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Desactivat"
@@ -3735,14 +3883,26 @@
 msgid "Monetary Formatting"
 msgstr "Format de la moneda"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Format dels números"
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Hora"
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "a les"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Els mòduls han estat actualitzats/activats."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Tingueu en compte que aquesta operació pot trigar uns minuts."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/cs.po` & `trytond-6.8.0/trytond/ir/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,19 @@
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Views"
 
 #, fuzzy
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
@@ -1022,14 +1027,35 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Actions"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr ""
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr ""
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr ""
@@ -1950,14 +1976,18 @@
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configure Modules"
@@ -2433,14 +2463,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2553,15 +2587,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Notes"
 
@@ -2800,19 +2834,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2917,14 +2950,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3000,30 +3037,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3128,14 +3168,19 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3372,14 +3417,18 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
@@ -3507,23 +3556,61 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3545,33 +3632,90 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
 #, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
+#, fuzzy
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3633,14 +3777,36 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Translations"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3851,14 +4017,28 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Data"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/de.po` & `trytond-6.8.0/trytond/ir/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Aktion"
 
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modell"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Sicht"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Aktion"
@@ -954,14 +958,34 @@
 msgid "Read Access"
 msgstr "Lesen"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Schreiben"
 
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Aktion"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr "Ereignis"
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ressource"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr "Ziel"
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Benutzer"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filter"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Ebene"
@@ -1867,14 +1891,18 @@
 msgid "Fields"
 msgstr "Felder"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modelle"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr "Logs"
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Vorgemerkte Aktivierungen / Aktualisierungen durchführen"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Module konfigurieren"
@@ -2347,14 +2375,18 @@
 msgid "Slovenian"
 msgstr "Slowenisch"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Türkisch"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr "Ukrainisch"
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinesisch (Vereinfacht)"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Sprachen konfigurieren"
@@ -2468,16 +2500,18 @@
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Sie sind aufgrund mindestens einer der folgenden Regeln nicht berechtigt die Datensätze \"%(ids)s\" vom Typ \"%(model)s\" zu löschen:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Sie sind nicht berechtigt, diesen Datensatz zu löschen."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"Keine Berechtigung zum Löschen des Datensatzes \"%(record)s\" des Modells "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Nein"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2720,20 +2754,18 @@
 "nicht entfernt werden."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notizen"
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
-"Leseversuch von nicht mehr vorhandenen Datensätzen \"%(ids)s\". "
-"(Dokumententyp: \"%(model)s\")."
+"Leseversuch von nicht mehr vorhandenen Datensätzen \"%(ids)s\" des Modells "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Die sind aufgrund mindestens einer der folgenden Regeln nicht berechtigt, die Datensätze \"%(ids)s\" vom Typ \"%(model)s\" zu lesen:\n"
@@ -2843,14 +2875,18 @@
 msgid "Missing sequence."
 msgstr "Fehlender Nummernkreis."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Fehlende Setter-Funktion für das Feld \"%(field)s\" in \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr "Es kann nur ein einziger Datensatz erstellt werden."
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(model)s\" ist zu lang "
 "(%(size)i > %(max_size)i)."
@@ -2937,30 +2973,34 @@
 msgstr ""
 "Ungültiger Wertebereich (Domain) oder ungültige Suchkriterien \"%(domain)s\""
 " für Suche \"%(search)s\"."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
-"Schreibversuch auf nicht mehr vorhandene Datensätze \"%(ids)s\". "
-"(Dokumententyp: \"%(model)s\")."
+"Schreibversuch auf nicht mehr vorhandene Datensätze \"%(ids)s\" von "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Sie sind aufgrund mindestens einer der folgenden Regeln nicht dazu berechtigt, die Datensätze \"%(ids)s\" vom Typ \"%(model)s\" zu verändern:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Keine Berechtigung für die Änderung dieses Datensatzes."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr ""
+"Keine Berechtigung zur Änderung des Feldes \"%(field)s\" in \"%(record)s\" "
+"von \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Syntaxfehler für XML-ID: %(value)r in \"%(field)s\" von \"%(model)s\" "
@@ -3062,14 +3102,18 @@
 msgid "Model field"
 msgstr "Modell Feld"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Modell Feld Zugriffsberechtigung"
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Log"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Modelldiagramm drucken"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modul"
@@ -3291,14 +3335,18 @@
 msgid "Fields Access"
 msgstr "Zugriffsberechtigungen Felder"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modelle"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr "Logs"
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modelle"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Vorgemerkte Aktivierungen / Aktualisierungen durchführen"
@@ -3420,22 +3468,54 @@
 msgid "Listed"
 msgstr "Aufgelistete"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Ausgewählte"
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Bericht"
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Fenster"
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Aufgelistete"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Ausgewählte"
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Bericht"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Fenster"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Formularaktion"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Bezugsformular"
@@ -3456,30 +3536,78 @@
 msgid "Listed"
 msgstr "Aufgelistete"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Ausgewählte"
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Bericht"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Fenster"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Aufgelistete"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Ausgewählte"
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Bericht"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Fenster"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Aufgelistete"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Ausgewählte"
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Bericht"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Fenster"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Daten"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Verknüpfung"
@@ -3540,14 +3668,34 @@
 msgid "Left-to-right"
 msgstr "Links-nach-Rechts"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Rechts-nach-Links"
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Klick auf"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Gelöscht"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr "Gestartet"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr "Geändert"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Übergeleitet zu"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Aktiviert"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Nicht aktiviert"
@@ -3752,14 +3900,26 @@
 msgid "Monetary Formatting"
 msgstr "Währungsformat"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Zahlenformat"
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Datum"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Stunde"
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "um"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Die Module wurden installiert bzw. aktiviert."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Dieser Vorgang kann einige Zeit in Anspruch nehmen."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/es.po` & `trytond-6.8.0/trytond/ir/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Acción"
 
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vista"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Acción"
@@ -954,14 +958,34 @@
 msgid "Read Access"
 msgstr "Permiso para leer"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Permiso para modificar"
 
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Acción"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr "Evento"
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Recurso"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr "Destino"
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Usuario"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtro"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Nivel"
@@ -1863,14 +1887,18 @@
 msgid "Fields"
 msgstr "Campos"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modelos"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr "Registros"
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realizar activaciones/actualizaciones pendientes"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configurar los módulos"
@@ -2340,14 +2368,18 @@
 msgid "Slovenian"
 msgstr "Esloveno"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turco"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr "Ucraniano"
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chino simplificado"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Configurar idiomas"
@@ -2462,16 +2494,18 @@
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "No puede eliminar los registros \"%(ids)s\" de \"%(model)s\" debido a alguna de estas reglas:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "No está autorizado para eliminar este registro."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"No tiene permisos para eliminar el registro \"%(record)s\" del modelo "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "No"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2714,20 +2748,18 @@
 msgstr "No puede eliminar un módulo que está activado o será activado."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notas"
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Está intentando leer los registros \"%(ids)s\" del modelo \"%(model)s\" que "
-"ya no existen."
+"no existen."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No tiene permitido leer los registros \"%(ids)s\" para \"%(model)s\" debido a una de las reglas :\n"
@@ -2837,14 +2869,18 @@
 msgid "Missing sequence."
 msgstr "No se ha encontrado la secuencia."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta la función de escritura para el campo \"%(field)s\" en \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr "Solo se puede crear un singleton."
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del campo \"%(field)s\" del registro \"%(model)s\" en \"%(model)s\""
 " es demasiado largo (%(size)i > %(max_size)i)."
@@ -2932,30 +2968,34 @@
 msgstr ""
 "El dominio o el criterio de búsqueda \"%(domain)s\" de la acción "
 "\"%(action)s\" es invalido."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Está intentando escribir en los registros \"%(ids)s\" de \"%(model)s\" que "
-"ya no existen."
+"no existen."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No puede modificar los registros \"%(ids)s\" de \"%(model)s\" debido a alguna de estas reglas:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "No podéis modificar este registro."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr ""
+"No podéis modificar el campo \"%(field)s\" del registro \"%(record)s\" de "
+"\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Error de sintaxis para el id de XML: %(value)r\" en \"%(field)s\" de "
@@ -3057,14 +3097,18 @@
 msgid "Model field"
 msgstr "Campo modelo"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Acceso campo modelo"
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Registro"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Imprimir gráfico de modelos"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Módulo"
@@ -3285,14 +3329,18 @@
 msgid "Fields Access"
 msgstr "Acceso campos"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modelos"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr "Registros"
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modelos"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realizar activaciones/actualizaciones pendientes"
@@ -3413,22 +3461,54 @@
 msgid "Listed"
 msgstr "Listados"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Seleccionados"
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Ventana"
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Asistente"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Listados"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Seleccionados"
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Ventana"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Asistente"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Acción de formulario"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Formulario relacionado"
@@ -3449,30 +3529,78 @@
 msgid "Listed"
 msgstr "Listados"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Seleccionados"
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Ventana"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Asistente"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Listados"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Seleccionados"
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Ventana"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Asistente"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Listados"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Seleccionados"
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Informe"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Ventana"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Asistente"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Datos"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Enlace"
@@ -3533,14 +3661,34 @@
 msgid "Left-to-right"
 msgstr "De izquierda a derecha"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "De derecha a izquierda"
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Ha clicado en"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Eliminió"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr "Ejecutó"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr "Modificó"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Transicionó a"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Activado"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Desactivado"
@@ -3745,14 +3893,26 @@
 msgid "Monetary Formatting"
 msgstr "Formato de la moneda"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formato de los números"
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Fecha"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Hora"
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "a las"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Los módulos han sido actualizados/activados."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Tenga en cuenta que esta operación puede tardar unos minutos."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/es_419.po` & `trytond-6.8.0/trytond/ir/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 msgstr ""
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Acceso a modelos"
+
+#, fuzzy
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Views"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr ""
@@ -965,14 +970,36 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Acciones de ventana"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr ""
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Modificado por usuario"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr ""
@@ -1854,14 +1881,18 @@
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Installation/Upgrade"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
@@ -2335,14 +2366,18 @@
 msgid "Slovenian"
 msgstr ""
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr ""
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr ""
@@ -2450,15 +2485,15 @@
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
@@ -2681,17 +2716,15 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
@@ -2784,14 +2817,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_size_validation_record"
@@ -2863,25 +2900,27 @@
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
@@ -2984,14 +3023,18 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr ""
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr ""
@@ -3217,14 +3260,18 @@
 msgid "Fields Access"
 msgstr "Permisos de acceso a campos"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr ""
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
@@ -3352,22 +3399,54 @@
 msgid "Listed"
 msgstr ""
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr ""
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr ""
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr ""
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr ""
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr ""
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr ""
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr ""
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr ""
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr ""
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr ""
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3388,30 +3467,78 @@
 msgid "Listed"
 msgstr ""
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr ""
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr ""
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr ""
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr ""
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr ""
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr ""
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr ""
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr ""
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr ""
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr ""
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr ""
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr ""
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr ""
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr ""
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr ""
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr ""
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3473,14 +3600,34 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr ""
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3687,14 +3834,26 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr ""
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr ""
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr ""
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/et.po` & `trytond-6.8.0/trytond/ir/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 msgid "Keywords"
 msgstr "Märksõnad"
 
 msgctxt "field:ir.action,name:"
 msgid "Name"
 msgstr "Nimetus"
 
-#, fuzzy
 msgctxt "field:ir.action,records:"
 msgid "Records"
-msgstr "Kirje ID"
+msgstr "Kirjed"
 
 msgctxt "field:ir.action,type:"
 msgid "Type"
 msgstr "Tüüp"
 
 msgctxt "field:ir.action,usage:"
 msgid "Usage"
@@ -136,14 +135,19 @@
 msgid "Name"
 msgstr "Nimetus"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Toiming"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Mudel"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vaade"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Toiming"
@@ -985,14 +989,37 @@
 msgid "Read Access"
 msgstr "Lugemisõigus"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Kirjutamisõigus"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Toiming"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ressurss"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Kasutaja"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filter"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Tase"
@@ -1892,14 +1919,18 @@
 msgid "Fields"
 msgstr "Väljad"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Mudelid"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Teosta ootel aktiveerimine/uuendus"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Moodulite seadistus"
@@ -1939,15 +1970,15 @@
 
 msgctxt "model:ir.action,name:act_translation_export"
 msgid "Export Translations"
 msgstr "Ekspordi tõlked"
 
 msgctxt "model:ir.action,name:act_translation_form"
 msgid "Translations"
-msgstr "Tülked"
+msgstr "Tõlked"
 
 msgctxt "model:ir.action,name:act_translation_report"
 msgid "Translations"
 msgstr "Tõlked"
 
 msgctxt "model:ir.action,name:act_translation_set"
 msgid "Set Translations"
@@ -2375,14 +2406,18 @@
 msgid "Slovenian"
 msgstr "Sloveenia"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Lihtsustatud Hiina"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2496,17 +2531,18 @@
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Kirje kustutamine on keelatud"
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "Puudub ligipääs mudelile (mudelitele)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Nov"
 
 #, fuzzy
@@ -2758,18 +2794,17 @@
 "Ei saa eemaldada moodulit mis on aktiveeritud või aktiveeritakse peatselt"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Märkmed"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Ei saa lugeda kirjeid \"%(ids)s\" mudelist \"%(model)s\", mida enam ei "
 "eksisteeri."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
@@ -2873,14 +2908,18 @@
 msgid "Missing sequence."
 msgstr "Puudub jada"
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Välja \"%(field)s\" jaoks puudub setter funktsioon mudelis \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Väärtus on mudeli \"%(model)s\" välja \"%(field)s\" jaoks liiga pikk "
@@ -2962,31 +3001,35 @@
 msgstr "Vaate \"%(name)s\" jaoks sobimatu XML."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "Lubamatu eesliide \"%(affix)s\" järjestusele \"%(sequence)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Ei saa salvestada kirjeid \"%(ids)s\" mudelisse \"%(model)s\", mida enam ei "
 "eksisteeri."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Puudub õigus kirje muutmiseks"
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "Mudeli \"%(model)s\" välja \"%(field)s\" jaoks on väärtus nõutud."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "XML süntaksi viga: \"%(value)r\" in \"%(field)s\"."
@@ -3091,14 +3134,19 @@
 msgid "Model field"
 msgstr "Mudeli väli"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Mudeli välja ligipääs"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Prindi mudeli graafik"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Moodul"
@@ -3324,14 +3372,18 @@
 msgid "Fields Access"
 msgstr "Välja ligipääs"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Mudelid"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Mudelid"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Teosta ootel aktiveerimine/uuendus"
@@ -3455,23 +3507,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Valitud sõlmed"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Aruanne"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLid"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Aken"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Nõustajad"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Valitud sõlmed"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Aruanne"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLid"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Aken"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Nõustajad"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Tegevuse vorm"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Vormi seos"
@@ -3493,32 +3585,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Valitud sõlmed"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Aruanne"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLid"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Aken"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Nõustajad"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Valitud sõlmed"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Aruanne"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLid"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Aken"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Nõustajad"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Valitud sõlmed"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Aruanne"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLid"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Aken"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Nõustajad"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Andmed"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Link"
@@ -3582,14 +3734,37 @@
 msgid "Left-to-right"
 msgstr "Vasakult paremale"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Paremalt vasakule"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Klikid"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Kustutamisel"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Tõlge"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Aktiveeritud"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Aktiveerimata"
@@ -3796,14 +3971,29 @@
 msgid "Monetary Formatting"
 msgstr "Rahaväärtuse formaat"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Numbriväärtuse formaat"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Kuupäev"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Tund"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Laupäev"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Moodulid on uuendatud / aktiveeritud."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Selle toimingu teostamisele võib kuluda mitu minutit."
@@ -3863,15 +4053,14 @@
 msgstr "Kasutaja"
 
 msgctxt "view:ir.rule.group:"
 msgid ""
 "If there is no test defined, the rule is always satisfied if not global."
 msgstr ""
 
-#, fuzzy
 msgctxt "view:ir.rule.group:"
 msgid "The rule is satisfied if at least one test is True."
 msgstr "Reegel kehtib, kui vähemasti üks test õnnestub."
 
 msgctxt "view:ir.sequence:"
 msgid "${day}"
 msgstr "${day}"
@@ -3920,22 +4109,21 @@
 msgid "Synchronize Translations?"
 msgstr "Sünkroonida tõlked?"
 
 msgctxt "view:ir.translation.set.succeed:"
 msgid "Translations set successfully."
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:ir.lang.config,start,end:"
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "wizard_button:ir.lang.config,start,load:"
 msgid "Load"
-msgstr ""
+msgstr "Lae"
 
 msgctxt "wizard_button:ir.model.print_model_graph,start,end:"
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "wizard_button:ir.model.print_model_graph,start,print_:"
 msgid "Print"
@@ -3950,20 +4138,18 @@
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "wizard_button:ir.module.activate_upgrade,start,upgrade:"
 msgid "Start Upgrade"
 msgstr "Alusta uuendamist"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.config,start,activate:"
 msgid "Activate"
-msgstr "Aktiveeritud"
+msgstr "Aktiveeri"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.config,start,end:"
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "wizard_button:ir.module.config_wizard,done,end:"
 msgid "OK"
 msgstr "OK"
```

### Comparing `trytond-6.6.8/trytond/ir/locale/fa.po` & `trytond-6.8.0/trytond/ir/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "اقدام"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "مدل"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "مشاهده"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "اقدام"
@@ -989,14 +994,37 @@
 msgid "Read Access"
 msgstr "دسترسی خواندن"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "دسترسی نوشتن"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "اقدام"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "منبع"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "کاربر"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "فیلتر"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "سطح"
@@ -1922,14 +1950,18 @@
 msgid "Fields"
 msgstr "فیلدها"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "مدل ها"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "انجام در انتظار فعال سازی / ارتقاء"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "پیکربندی ماژول ها"
@@ -2408,14 +2440,18 @@
 msgid "Slovenian"
 msgstr "اسلوونیایی"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "چینی Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2531,17 +2567,18 @@
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "شما اجازه حذف این پرونده را ندارید."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "شما مجاز به دسترسی به \"%(model)s\" نیستید."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "توجه"
 
 #, fuzzy
@@ -2794,17 +2831,15 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "یادداشت ها"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr "شما تلاش می کنید پرونده ی :\"%(model)s\" را بخوانید، که دیگر وجود ندارد."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
@@ -2909,14 +2944,18 @@
 msgid "Missing sequence."
 msgstr "دنباله گمشده."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "مقدار فیلد :\"%(field)s\" در \"%(model)s\" خیلی طولانی است (%(size)i > "
@@ -3001,28 +3040,31 @@
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "نام دامنه یا معیارهای جستجوی: \"%s\" در اقدام: \"%s\" معتبر نیست."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "شما در حال تلاش برای نوشتن روی اسناد :\"%(model)s\" که دیگر وجود ندارد، می "
 "باشید."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "شما مجاز به تغییر این پرونده نیستید."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "یک مقدار برای فیلد :\"%(field)s\" در\"%(model)s\" مورد نیاز است."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "خطای نحوی برای شناسه xml :\"%(value)r\" در \"%(field)s\"."
@@ -3127,14 +3169,19 @@
 msgid "Model field"
 msgstr "مدل فیلد"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "مدل دسترسی فیلد"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "لائوای"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "چاپ مدل نمودار"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "ماژول"
@@ -3361,14 +3408,18 @@
 msgid "Fields Access"
 msgstr "دسترسی فیلدها"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "مدل ها"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "مدل ها"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "انجام در انتظار فعال سازی / ارتقاء"
@@ -3492,23 +3543,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "گره های انتخاب شده"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "گزارش"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "آدرس های اینترنتی"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "پنجره"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "دستیارها"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "گره های انتخاب شده"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "گزارش"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "آدرس های اینترنتی"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "پنجره"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "دستیارها"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "فرم اقدام"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "فرم ارتباط"
@@ -3530,32 +3621,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "گره های انتخاب شده"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "گزارش"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "آدرس های اینترنتی"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "پنجره"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "دستیارها"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "گره های انتخاب شده"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "گزارش"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "آدرس های اینترنتی"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "پنجره"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "دستیارها"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "گره های انتخاب شده"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "گزارش"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "آدرس های اینترنتی"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "پنجره"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "دستیارها"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "داده"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "پیوند"
@@ -3619,14 +3770,37 @@
 msgid "Left-to-right"
 msgstr "چپ به راست"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "راست به چپ"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "کلیک ها"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "درحذف"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "ترجمه"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "فعال شده"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "فعال نشده"
@@ -3833,14 +4007,29 @@
 msgid "Monetary Formatting"
 msgstr "قالب بندی الزامی"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "قالب بندی اعداد"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "تاریخ"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "ساعات"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "مسیر"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "ماژول ها فعال شده / ارتقاء یافته هستند."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "توجه داشته باشید که این عملیات ممکن است چند دقیقه طول بکشد."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/fi.po` & `trytond-6.8.0/trytond/ir/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,19 @@
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Views"
 
 #, fuzzy
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
@@ -1006,14 +1011,35 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Actions"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr ""
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr ""
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr ""
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr ""
@@ -1926,14 +1952,18 @@
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configure Modules"
@@ -2409,14 +2439,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2529,15 +2563,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Notes"
 
@@ -2775,19 +2809,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2892,14 +2925,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -2975,30 +3012,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3103,14 +3143,19 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3347,14 +3392,18 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
@@ -3482,23 +3531,61 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3520,33 +3607,90 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
 #, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
+#, fuzzy
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3608,14 +3752,36 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Translations"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3826,14 +3992,28 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Data"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/fr.po` & `trytond-6.8.0/trytond/ir/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Action"
 
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modèle"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vue"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Action"
@@ -954,14 +958,34 @@
 msgid "Read Access"
 msgstr "Accès en lecture"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Accès en écriture"
 
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Action"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr "Événement"
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ressource"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr "Cible"
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Utilisateur"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtre"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Niveau"
@@ -1865,14 +1889,18 @@
 msgid "Fields"
 msgstr "Champs"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modèles"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr "Journaux"
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Lancer l'activation/mise à jour en attente"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configurer les modules"
@@ -2342,14 +2370,18 @@
 msgid "Slovenian"
 msgstr "Slovène"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turc"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr "Ukrainien"
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinois Simplifié"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Configurer les langues"
@@ -2463,16 +2495,18 @@
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à supprimer les enregistrement « %(ids)s » de « %(model)s » à cause d'au moins une de ces règles :\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Vous n'êtes pas autorisé à supprimer cet enregistrement."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"Vous n'êtes pas autorisé à supprimer l'enregistrement « %(record)s » de "
+"« %(model)s »."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Non"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2717,20 +2751,18 @@
 "Vous ne pouvez pas supprimer un module qui est activé ou qui va être activé."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Vous essayez de lire les enregistrements « %(ids)s » de « %(model)s » qui "
-"n'existent plus."
+"n'existent pas."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à lire les enregistrements « %(ids)s » de « %(model)s » à cause d'au moins une de ces règles :\n"
@@ -2844,14 +2876,18 @@
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 "Fonction de définition manquante pour le champ « %(field)s » sur "
 "« %(model)s »."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr "Un seul singleton peut être créé."
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » sur « %(model)s » est "
 "trop longue (%(size)i > %(max_size)i)."
@@ -2938,30 +2974,34 @@
 msgstr ""
 "Domaine ou critère de recherche « %(domain)s » invalide pour la recherche "
 "« %(search)s »."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Vous essayez d'écrire sur les enregistrements « %(ids)s » de « %(model)s » "
-"qui n'existent plus."
+"qui n'existent pas."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à écrire sur les enregistrements « %(ids)s » de « %(model)s » à cause d'au moins une de ces règles :\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Vous n'êtes pas autorisé à modifier cet enregistrement."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr ""
+"Vous n'êtes pas autorisé à modifier le champ « %(field)s » sur "
+"« %(record)s » de « %(model)s »."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Erreur de syntaxe pour l'id XML : %(value)r sur « %(field)s » de "
@@ -3063,14 +3103,18 @@
 msgid "Model field"
 msgstr "Champ de modèle"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Droit d'accès au champ de modèle"
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Journal"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Imprimer le graphe de modèles"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Module"
@@ -3291,14 +3335,18 @@
 msgid "Fields Access"
 msgstr "Droits d'accès au champs"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modèles"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr "Journaux"
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modèles"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Lancer l'activation/mise à jour en attente"
@@ -3419,22 +3467,54 @@
 msgid "Listed"
 msgstr "Listés"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Sélectionnés"
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Onglet"
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Assistant"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Listés"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Sélectionnés"
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Onglet"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Assistant"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Formulaire"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Formulaire relié"
@@ -3455,30 +3535,78 @@
 msgid "Listed"
 msgstr "Listés"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Sélectionnés"
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Onglet"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Assistant"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Listés"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Sélectionnés"
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Onglet"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Assistant"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Listés"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Sélectionnés"
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Onglet"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Assistant"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Données"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Lien"
@@ -3539,14 +3667,34 @@
 msgid "Left-to-right"
 msgstr "Gauche-à-droite"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Droite-à-gauche"
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Cliqué sur"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Supprimé"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr "Lancé"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr "Modifié"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Transitionné vers"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Activé"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Inactif"
@@ -3753,14 +3901,26 @@
 msgid "Monetary Formatting"
 msgstr "Format monétaire"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formatage des nombres"
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Date"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Heure"
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "à"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Les modules ont été mis à niveau / activés."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Cette opération peut prendre quelques minutes."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/hu.po` & `trytond-6.8.0/trytond/ir/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Művelet"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Minta"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Nézet"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Művelet"
@@ -975,14 +980,37 @@
 msgid "Read Access"
 msgstr "Olvasási hozzáférés"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Írási hozzáférés:"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Művelet"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Elem"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Felhasználó"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Szűrő"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Szint"
@@ -1905,14 +1933,18 @@
 msgstr "Mezők"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Előjegyzett installációk/aktualizálás végrehajtása"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_config"
@@ -2410,14 +2442,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2541,15 +2577,15 @@
 "%(rules)s"
 msgstr ""
 "Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait törölni, mert a következő szabályok legalább egyike nem teljesül:\n"
 "%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "nov"
 
@@ -2793,19 +2829,20 @@
 "activated."
 msgstr "A már telepített vagy telepítésre előjegyzett modul nem törölhető."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Jegyzetek"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
+"Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait olvasni, mert a következő szabályok legalább egyike nem teljesül:\n"
+"%(rules)s"
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait olvasni, mert a következő szabályok legalább egyike nem teljesül:\n"
@@ -2918,14 +2955,18 @@
 msgid "Missing sequence."
 msgstr "Hiányzó számkör."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3011,32 +3052,37 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 "Érvénytelen értéktartomány (Domain) vagy keresési kritérium "
 "\"%(domain)s\"akcióban \"%(action)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
+"Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait módosítani, mert a következő szabályok legalább egyike nem teljesül:\n"
+"%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait módosítani, mert a következő szabályok legalább egyike nem teljesül:\n"
 "%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "A „%(model)s” elem „%(field)s” mezőjét ki kell tölteni."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3140,14 +3186,19 @@
 msgid "Model field"
 msgstr "Minta mező"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Minta mező hozzáférésének engedélyezése"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Grafikon nyomtatása"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modul"
@@ -3385,14 +3436,18 @@
 msgstr "Fields Access"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
@@ -3531,23 +3586,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Kiválasztott folyószámla"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Nyomtatvány"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Ablak"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Kiválasztott folyószámla"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Nyomtatvány"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Ablak"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Űrlap művelet"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Hivatkozási űrlap"
@@ -3569,32 +3664,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Kiválasztott folyószámla"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Nyomtatvány"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Ablak"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Kiválasztott folyószámla"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Nyomtatvány"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Ablak"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Kiválasztott folyószámla"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Nyomtatvány"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Ablak"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Adat"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Hivatkozás"
@@ -3657,14 +3812,37 @@
 msgid "Left-to-right"
 msgstr "Balról jobbra"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Jobbról balra"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Törléskor"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Fordítás"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3872,14 +4050,29 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Dátum"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Óra"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "szo"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/id.po` & `trytond-6.8.0/trytond/ir/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,19 @@
 msgid "Name"
 msgstr "Nama"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Tindakan"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr ""
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Tindakan"
@@ -969,14 +974,37 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Tindakan"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Sumber daya"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Pengguna"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Saring"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr ""
@@ -1856,14 +1884,18 @@
 msgid "Fields"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Lakukan Aktivasi/Upgrade Tertunda"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr ""
@@ -2337,14 +2369,18 @@
 msgid "Slovenian"
 msgstr ""
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turki"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2452,17 +2488,18 @@
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Anda tidak diizinkan untuk menghapus catatan ini."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Tidak"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2685,19 +2722,18 @@
 "activated."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Catatan-Catatan"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2791,14 +2827,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_size_validation_record"
@@ -2868,29 +2908,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Anda tidak diizinkan untuk mengubah catatan ini."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "Kesalahan sintaks untuk id XML: \"%(value)r\" di dalam \"%(field)s\"."
@@ -2993,14 +3037,18 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr ""
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modul"
@@ -3224,14 +3272,18 @@
 msgid "Fields Access"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr ""
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr ""
@@ -3353,23 +3405,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Pilihan"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Laporan"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL-URL"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Jendela"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wisaya-Wisaya"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Pilihan"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Laporan"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL-URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Jendela"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wisaya-Wisaya"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3391,32 +3483,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Pilihan"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Laporan"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL-URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Jendela"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wisaya-Wisaya"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Pilihan"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Laporan"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL-URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Jendela"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wisaya-Wisaya"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Pilihan"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Laporan"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL-URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Jendela"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wisaya-Wisaya"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Tautan"
@@ -3478,14 +3630,37 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Klik"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Saat Menghapus"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Terjemahan"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3690,14 +3865,29 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Tanggal"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Jam"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Sab"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Modul-Modul sudah ditingkatkan / diaktifkan."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Perhatikan bahwa operasi ini mungkin memakan waktu beberapa menit."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/it.po` & `trytond-6.8.0/trytond/ir/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Azione"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modello"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vista"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Azione"
@@ -991,14 +996,37 @@
 msgid "Read Access"
 msgstr "Accesso di lettura"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Accesso scrittura"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Azione"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Risorsa"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Utente"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtro"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Livello"
@@ -1939,14 +1967,18 @@
 msgstr "Fields"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_config"
@@ -2463,14 +2495,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2592,15 +2628,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Nota"
 
@@ -2861,19 +2897,18 @@
 msgstr "Non si può rimuovere un modulo attivato o da attivare."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2988,14 +3023,18 @@
 msgid "Missing sequence."
 msgstr "Sequenza mancante"
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3080,30 +3119,33 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 "Dominio o criterio di ricerca \"%(domain)s\" invalido nell'azione "
 "\"%(action)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3207,14 +3249,19 @@
 msgid "Model field"
 msgstr "Campo modello"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Accesso a campi modello"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Stampa modello grafico"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modulo"
@@ -3455,14 +3502,18 @@
 msgstr "Fields Access"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
@@ -3608,23 +3659,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Nodi selezionati"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Report"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Finestra"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Nodi selezionati"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Report"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Finestra"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Form Azione"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Relazione a Form"
@@ -3646,32 +3737,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Nodi selezionati"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Report"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Finestra"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Nodi selezionati"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Report"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Finestra"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Nodi selezionati"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Report"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Finestra"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Dati"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Link"
@@ -3735,14 +3886,37 @@
 msgid "Left-to-right"
 msgstr "Sinistra-destra"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Destra-Sinistra"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "click"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "All'eliminazione"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Traduzione"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Attivata"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "non attivato"
@@ -3949,14 +4123,29 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formattazione dei numeri"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Ora"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Percorso"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "I moduli sono stati elevati /attivati"
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Questa operazione potrebbe durare qualche minuto"
```

### Comparing `trytond-6.6.8/trytond/ir/locale/lo.po` & `trytond-6.8.0/trytond/ir/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,19 @@
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "ການປະຕິບັດ"
 
 #, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "ເບິ່ງ"
 
 #, fuzzy
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
@@ -1053,14 +1058,36 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "ການປະຕິບັດ"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr ""
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "ຜູ້ໃຊ້"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
@@ -2008,14 +2035,18 @@
 msgid "Fields"
 msgstr "ຟິນລ໌"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configure Modules"
@@ -2504,14 +2535,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2627,15 +2662,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "ໝາຍເຫດ"
 
@@ -2877,19 +2912,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "ໝາຍເຫດ"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2994,14 +3028,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3077,30 +3115,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3206,14 +3247,19 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3462,14 +3508,18 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
@@ -3607,23 +3657,61 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "ລາຍງານ"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "ລາຍງານ"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3645,33 +3733,90 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "ລາຍງານ"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "ລາຍງານ"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
 #, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "ລາຍງານ"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
+#, fuzzy
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "ວັນທີ:"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3734,14 +3879,36 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "ລ້າງການແປ"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3959,14 +4126,28 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "ວັນທີ:"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "ວັນທີ:"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/lt.po` & `trytond-6.8.0/trytond/ir/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Veiksmas"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modelis"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Peržiūra"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Veiksmas"
@@ -984,14 +989,37 @@
 msgid "Read Access"
 msgstr "Teisė skaityti"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Teisė įrašyti"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Veiksmas"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Resursas"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Naudotojas"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtras"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Lygis"
@@ -1880,14 +1908,18 @@
 msgid "Fields"
 msgstr "Laukai"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modeliai"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Aktyvuoti/Atnaujinti pažymėtus modulius"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Derinti modulius"
@@ -2363,14 +2395,18 @@
 msgid "Slovenian"
 msgstr "Slovėnų"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turkų"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Kiniečių supaprastinta"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2481,15 +2517,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Lap"
 
@@ -2731,19 +2767,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Pastabos"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2846,14 +2881,18 @@
 msgid "Missing sequence."
 msgstr "Trūksta numeruotės."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -2929,29 +2968,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Jums nėra leista taisyti šį įrašą."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3056,14 +3099,19 @@
 msgid "Model field"
 msgstr "Modelio laukas"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Spausdinti modelio grafiką"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modulis"
@@ -3290,14 +3338,18 @@
 msgid "Fields Access"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modeliai"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modeliai"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Aktyvuoti/Atnaujinti pažymėtus modulius"
@@ -3421,23 +3473,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Pasirinkti mazgai"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Ataskaitos"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Langas"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Vedikliai"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Pasirinkti mazgai"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Ataskaitos"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Langas"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Vedikliai"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Veiksmo forma"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3459,32 +3551,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Pasirinkti mazgai"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Ataskaitos"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Langas"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Vedikliai"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Pasirinkti mazgai"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Ataskaitos"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Langas"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Vedikliai"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Pasirinkti mazgai"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Ataskaitos"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Langas"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Vedikliai"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Duomenys"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Nuoroda"
@@ -3548,14 +3700,37 @@
 msgid "Left-to-right"
 msgstr "Iš kairės į dešinę"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Iš dešinės į kairę"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Spustelėjimai"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Ištrinant"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Vertimas"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Veiksnus"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Neveiksnus"
@@ -3762,14 +3937,29 @@
 msgid "Monetary Formatting"
 msgstr "Valiutos formatas"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Skaičių formatas"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Valanda"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Šeš"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/nl.po` & `trytond-6.8.0/trytond/ir/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actie"
 
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Weergave"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Actie"
@@ -954,14 +958,34 @@
 msgid "Read Access"
 msgstr "Toegang lezen"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Toegang schrijven"
 
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Actie"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr "Gebeurtenis"
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Bron"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr "Doel"
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Gebruiker"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filter"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Niveau"
@@ -1865,14 +1889,18 @@
 msgid "Fields"
 msgstr "Velden"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modellen"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr "Logboeken"
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Voer installatie / bijwerken uit"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Modules configureren"
@@ -2342,14 +2370,18 @@
 msgid "Slovenian"
 msgstr "Sloveens"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turks"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr "Oekraïens"
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinees Simplified"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Talen configureren"
@@ -2461,16 +2493,18 @@
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Het is niet toegestaan records \"%(ids)s\" van \"%(model)s\" te verwijderen vanwege ten minste één van deze regels:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "U mag dit record niet verwijderen."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"U hebt geen rechten om de record \"%(record)s\" van \"%(model)s\" te "
+"verwijderen."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Nee"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2715,20 +2749,16 @@
 "geactiveerd te worden."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notities"
 
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
-"U probeert records \"%(ids)s\"van \"%(model)s\" te lezen die niet meer "
-"bestaan."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "U probeert records \"%(ids)s\"van \"%(model)s\" te lezen die niet bestaan."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Het is niet toegestaan om deze velden \"%(ids)s\" van \"%(model)s\" te lezen vanwege ten minste één van deze regels:\n"
@@ -2838,14 +2868,18 @@
 msgid "Missing sequence."
 msgstr "Reeks ontbreekt."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Definitiefunctie voor het veld \"%(field)s\" in \"%(model)s\" ontbreekt."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr "Er kan slecht één singleton worden aangemaakt."
+
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "De waarde voor veld \"%(field)s\" in \"%(model)s\" is te lang (%(size)i > "
 "%(max_size)i)."
@@ -2929,30 +2963,34 @@
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "Ongeldig domein of zoekcriteria \"%(domain)s\" voor zoekactie \"%(action)s\"."
 
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
-"U probeert te schrijven in het record \"%(ids)s\" van\"%(model)s dat niet "
-"meer bestaat."
+"U probeert records \"%(ids)s\" van\"%(model)s weg te schrijven die niet "
+"bestaan."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Het is niet toegestaan om te schrijven in de records \"%(ids)s\" van \"%(model)s\"vanwege ten minste één van deze regels:\n"
 "%(rules)s"
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "U hebt niet de nodige bevoegdheid om dit record te wijzigen."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr ""
+"U hebt geen rechten om het veld \"%(field)s\" in \"%(record)s\" van "
+"\"%(model)s\" te wijzigen."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Syntaxfout voor XML-id: \"%(value)r\" in \"%(field)s\" van \"%(model)s\" "
@@ -3054,14 +3092,18 @@
 msgid "Model field"
 msgstr "Model veld"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Model veld toegang"
 
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Logboek"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Modelgrafiek afdrukken"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Module"
@@ -3282,14 +3324,18 @@
 msgid "Fields Access"
 msgstr "Toegang veld"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modellen"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr "Logboeken"
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modellen"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Voer installatie / bijwerken uit"
@@ -3410,22 +3456,54 @@
 msgid "Listed"
 msgstr "Vermeld"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Geselecteerd"
 
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Venster"
+
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Vermeld"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Geselecteerd"
 
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Venster"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Actieformulier"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Formulier relatie"
@@ -3446,30 +3524,78 @@
 msgid "Listed"
 msgstr "Vermeld"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Geselecteerd"
 
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Venster"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Vermeld"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Geselecteerd"
 
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Venster"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Vermeld"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Geselecteerd"
 
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Rapport"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Venster"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Assistent"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Gegevens"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Koppeling"
@@ -3530,14 +3656,34 @@
 msgid "Left-to-right"
 msgstr "Links naar rechts"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Rechts naar links"
 
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Aangeklikt"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Verwijderd"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr "Gelanceerd"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr "Gewijzigd"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Gewijzigd naar"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Geactiveerd"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Niet geactiveerd"
@@ -3742,14 +3888,26 @@
 msgid "Monetary Formatting"
 msgstr "Monetair formaat"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Getal weergave"
 
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Datum"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Uur"
+
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Om"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "De modules zijn bijgewerkt / geïnstalleerd."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Houd er rekening mee dat deze bewerking enkele minuten kan duren."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/pl.po` & `trytond-6.8.0/trytond/ir/locale/pl.po`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Nazwa"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Akcja"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Widok"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Akcja"
@@ -973,14 +978,37 @@
 msgid "Read Access"
 msgstr "Odczyt"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Zapis"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Akcja"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Zasób"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Użytkownik"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtr"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Poziom"
@@ -1892,14 +1920,18 @@
 msgid "Fields"
 msgstr "Pola"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modele"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Wykonaj aktywację/aktualizację"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Skonfiguruj moduły"
@@ -2375,14 +2407,18 @@
 msgid "Slovenian"
 msgstr "Słoweński"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turecki"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chiński uproszczony"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2500,17 +2536,20 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Nie masz uprawnień do usunięcia rekordów \"%(ids)s\" z modelu \"%(model)s\" z powodu niezgodności przynajmniej jednej z reguł:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Nie masz uprawnień do usunięcia tego rekordu."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr ""
+"Nie masz uprawnień do uruchomienia kreatora \"%(wizard)s\" w modelu "
+"\"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Lis"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
@@ -2755,18 +2794,17 @@
 "activated."
 msgstr "Nie możesz usunąć modułu, który jest aktywny lub będzie aktywny."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notatki"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Próbujesz odczytać rekordy \"%(ids)s\" modelu \"%(model)s\", które już nie "
 "istnieją."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
@@ -2880,14 +2918,18 @@
 msgid "Missing sequence."
 msgstr "Brakująca sekwencja."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Brakująca funkcja setter dla pola \"%(field)s\" w \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Wartość pola \"%(field)s\" w \"%(model)s\" jest zbyt długa (%(size)i > "
@@ -2974,33 +3016,37 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 "Nieprawidłowa domena lub kryteria wyszukiwania \"%(domain)s\" dla akcji "
 "\"%(action)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Próbujesz zapisać rekordy \"%(ids)s\" z modelu \"%(model)s\", które już nie "
 "istnieją."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Nie masz uprawnień do zapisu rekordów \"%(ids)s\" modelu \"%(model)s\" z powodu przynajmniej jednego z reguł:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Nie masz uprawnień do modyfikacji tego rekordu."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "Błąd składni w XML id: \"%(value)r\" w \"%(field)s\"."
@@ -3103,14 +3149,19 @@
 msgid "Model field"
 msgstr "Pole modelu"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Dostęp do pola modelu"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Laotański"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Wykres modelu druku"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Moduł"
@@ -3336,14 +3387,18 @@
 msgid "Fields Access"
 msgstr "Dostęp do pól"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modele"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modele"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Wykonaj aktywację/aktualizację"
@@ -3467,23 +3522,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Zaznaczone węzły"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "Adresy URL"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Kreatory"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Zaznaczone węzły"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "Adresy URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Kreatory"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Formularz akcji"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Relacja formularza"
@@ -3505,32 +3600,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Zaznaczone węzły"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "Adresy URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Kreatory"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Zaznaczone węzły"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "Adresy URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Kreatory"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Zaznaczone węzły"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "Adresy URL"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Kreatory"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Dane"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Odnośnik"
@@ -3593,14 +3748,37 @@
 msgid "Left-to-right"
 msgstr "Od lewej do prawej"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Od prawej do lewej"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Kliknięcia"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Przy usunięciu"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Tłumaczenie"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Aktywny"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Nieaktywny"
@@ -3808,14 +3986,29 @@
 msgid "Monetary Formatting"
 msgstr "Formatowanie pieniężne"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formatowanie liczb"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Godzina"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Sob"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Moduły zostały zaktualizowane / aktywowane."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Wykonanie operacji może zająć kilka minut."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/pt.po` & `trytond-6.8.0/trytond/ir/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Ação"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Modelo"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Sumário"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Ação"
@@ -987,14 +992,37 @@
 msgid "Read Access"
 msgstr "Acesso de leitura"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Acesso de edição"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Ação"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Recurso"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Usuário"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtro"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Nível"
@@ -1921,14 +1949,18 @@
 msgid "Fields"
 msgstr "Campos"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modelos"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realizar Ativações/Atualizações Pendentes"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configurar módulos"
@@ -2405,14 +2437,18 @@
 msgid "Slovenian"
 msgstr "Esloveno"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Turco"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinês Simplificado"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2528,17 +2564,18 @@
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Você não tem permissão para apagar este registro."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "Você não pode acessar \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Nov"
 
 #, fuzzy
@@ -2798,17 +2835,15 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notas"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr "Você está tentando ler registros de \"%(model)s\" que não existem mais."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
@@ -2916,14 +2951,18 @@
 msgstr "Faltando sequência."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "A função de busca no campo \"%(field)s\" está faltando."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "O valor para o campo \"%(field)s\" em \"%(model)s\" é longo demais (%(size)i"
@@ -3015,27 +3054,30 @@
 "Domínio ou critério de busca inválido \"%(domain)s\" para a ação "
 "\"%(action)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Você está tentando gravar registros de \"%(model)s\" que não existem mais."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Você não pode alterar este registro."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "É necessário um valor para o campo \"%(field)s\" em \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "Erro de sintaxe para XML id: \"%(value)r\" em \"%(field)s\"."
@@ -3140,14 +3182,19 @@
 msgid "Model field"
 msgstr "Campo do modelo"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Acesso ao campo do modelo"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Imprimir o grafo do modelo"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Módulo"
@@ -3373,14 +3420,18 @@
 msgid "Fields Access"
 msgstr "Acesso a Campos"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Modelos"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Modelos"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Realizar Ativações/Atualizações Pendentes"
@@ -3504,23 +3555,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Nodos selecionados"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Relatório"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Janela"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Assistentes"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Nodos selecionados"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Relatório"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Janela"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Assistentes"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Formulário de ação"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Relacionar formulário"
@@ -3542,32 +3633,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Nodos selecionados"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Relatório"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Janela"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Assistentes"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Nodos selecionados"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Relatório"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Janela"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Assistentes"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Nodos selecionados"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Relatório"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Janela"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Assistentes"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Dados"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Link"
@@ -3631,14 +3782,37 @@
 msgid "Left-to-right"
 msgstr "Esquerda para a direita"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Direta para a esquerda"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Cliques"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Ao apagar"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Tradução"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Ativo"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Inativo"
@@ -3845,14 +4019,29 @@
 msgid "Monetary Formatting"
 msgstr "Formatação Monetária"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Formato dos números"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Horas"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Sáb"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Os módulos foram atualizados / ativados."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Observação: Esta operação pode levar alguns minutos."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/ro.po` & `trytond-6.8.0/trytond/ir/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,19 @@
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Acțiune"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Vedere"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Acțiune"
@@ -379,54 +384,51 @@
 #, fuzzy
 msgctxt "field:ir.avatar,copy_to_resources_visible:"
 msgid "Copy to Resources Visible"
 msgstr "Resursă"
 
 msgctxt "field:ir.avatar,image:"
 msgid "Image"
-msgstr ""
+msgstr "Imagine"
 
 msgctxt "field:ir.avatar,image_id:"
 msgid "Image ID"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.avatar,last_modification:"
 msgid "Last Modification"
 msgstr "Ultima Modificare"
 
-#, fuzzy
 msgctxt "field:ir.avatar,last_user:"
 msgid "Last User"
 msgstr "Ultimul Utilizator"
 
-#, fuzzy
 msgctxt "field:ir.avatar,resource:"
 msgid "Resource"
 msgstr "Resursă"
 
 msgctxt "field:ir.avatar,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:ir.avatar.cache,avatar:"
 msgid "Avatar"
 msgstr ""
 
 msgctxt "field:ir.avatar.cache,image:"
 msgid "Image"
-msgstr ""
+msgstr "Imagine"
 
 msgctxt "field:ir.avatar.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:ir.avatar.cache,size:"
 msgid "Size"
-msgstr ""
+msgstr "Mărime"
 
 msgctxt "field:ir.cache,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.cache,timestamp:"
 msgid "Timestamp"
@@ -490,145 +492,136 @@
 
 msgctxt "field:ir.cron,next_call:"
 msgid "Next Call"
 msgstr "Următorul apel"
 
 msgctxt "field:ir.cron,timezone:"
 msgid "Timezone"
-msgstr ""
+msgstr "Fus orar"
 
 msgctxt "field:ir.cron,weekday:"
 msgid "Day of Week"
 msgstr "Ziua săptămânii"
 
 msgctxt "field:ir.email,addresses:"
 msgid "Addresses"
-msgstr ""
+msgstr "Adrese"
 
 msgctxt "field:ir.email,at:"
 msgid "At"
-msgstr ""
+msgstr "La"
 
 msgctxt "field:ir.email,body:"
 msgid "Body"
-msgstr ""
+msgstr "Corp"
 
 msgctxt "field:ir.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "Destinatari"
 
 msgctxt "field:ir.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Destinatari Ascunsi"
 
 msgctxt "field:ir.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Destinatari Secundari"
 
-#, fuzzy
 msgctxt "field:ir.email,resource:"
 msgid "Resource"
 msgstr "Resursă"
 
 msgctxt "field:ir.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Subiect"
 
-#, fuzzy
 msgctxt "field:ir.email,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.email.address,address:"
 msgid "Address"
-msgstr ""
+msgstr "Adresa"
 
-#, fuzzy
 msgctxt "field:ir.email.address,email:"
 msgid "E-mail"
-msgstr "Email"
+msgstr "E-mail"
 
 msgctxt "field:ir.email.template,body:"
 msgid "Body"
-msgstr ""
+msgstr "Corp"
 
-#, fuzzy
 msgctxt "field:ir.email.template,model:"
 msgid "Model"
 msgstr "Model"
 
-#, fuzzy
 msgctxt "field:ir.email.template,model_name:"
 msgid "Model Name"
-msgstr "Numele modelului"
+msgstr "Nume Model"
 
 #, fuzzy
 msgctxt "field:ir.email.template,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.email.template,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "Destinatari"
 
 msgctxt "field:ir.email.template,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Destinatari Ascunsi"
 
 msgctxt "field:ir.email.template,recipients_hidden_pyson:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Destinatari Ascunsi"
 
 msgctxt "field:ir.email.template,recipients_pyson:"
 msgid "Recipients"
-msgstr ""
+msgstr "Destinatari"
 
 msgctxt "field:ir.email.template,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Destinatari Secundari"
 
 msgctxt "field:ir.email.template,recipients_secondary_pyson:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Destinatari Secundari"
 
-#, fuzzy
 msgctxt "field:ir.email.template,reports:"
 msgid "Reports"
 msgstr "Rapoarte"
 
 msgctxt "field:ir.email.template,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Subiect"
 
-#, fuzzy
 msgctxt "field:ir.email.template-ir.action.report,report:"
 msgid "Report"
-msgstr "Rapoarte"
+msgstr "Raport"
 
 msgctxt "field:ir.email.template-ir.action.report,template:"
 msgid "Template"
 msgstr "Șablon"
 
-#, fuzzy
 msgctxt "field:ir.error,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:ir.error,message:"
 msgid "Message"
 msgstr "Mesaj"
 
 msgctxt "field:ir.error,origin:"
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:ir.error,processed_by:"
 msgid "Processed by"
-msgstr ""
+msgstr "Procesat de"
 
 msgctxt "field:ir.error,solved_by:"
 msgid "Solved by"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.error,state:"
@@ -642,15 +635,15 @@
 
 msgctxt "field:ir.export,export_fields:"
 msgid "Fields"
 msgstr "Câmpuri"
 
 msgctxt "field:ir.export,header:"
 msgid "Header"
-msgstr ""
+msgstr "Antet"
 
 msgctxt "field:ir.export,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.export,resource:"
 msgid "Resource"
@@ -912,15 +905,14 @@
 msgid "Out of Sync"
 msgstr "Nesincronizat"
 
 msgctxt "field:ir.model.data,values:"
 msgid "Values"
 msgstr "valori"
 
-#, fuzzy
 msgctxt "field:ir.model.field,access:"
 msgid "Access"
 msgstr "Acces"
 
 msgctxt "field:ir.model.field,field_description:"
 msgid "Field Description"
 msgstr "Descrierea câmpului"
@@ -973,14 +965,37 @@
 msgid "Read Access"
 msgstr "Acces citit"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Acces de scriere"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Acțiune"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Resursă"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Utilizator"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtru"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Nivel"
@@ -1009,15 +1024,14 @@
 msgid "Version"
 msgstr "Versiune"
 
 msgctxt "field:ir.module.activate_upgrade.start,module_info:"
 msgid "Modules to update"
 msgstr "Module de actualizat"
 
-#, fuzzy
 msgctxt "field:ir.module.config.start,modules:"
 msgid "Modules"
 msgstr "Module"
 
 msgctxt "field:ir.module.config_wizard.item,action:"
 msgid "Action"
 msgstr "Acțiune"
@@ -1310,20 +1324,18 @@
 msgstr "Fişier"
 
 #, fuzzy
 msgctxt "field:ir.translation.export.result,filename:"
 msgid "Filename"
 msgstr "Fişier"
 
-#, fuzzy
 msgctxt "field:ir.translation.export.result,language:"
 msgid "Language"
 msgstr "Limba"
 
-#, fuzzy
 msgctxt "field:ir.translation.export.result,module:"
 msgid "Module"
 msgstr "Modul"
 
 msgctxt "field:ir.translation.export.start,language:"
 msgid "Language"
 msgstr "Limba"
@@ -1332,15 +1344,14 @@
 msgid "Module"
 msgstr "Modul"
 
 msgctxt "field:ir.translation.update.start,language:"
 msgid "Language"
 msgstr "Limba"
 
-#, fuzzy
 msgctxt "field:ir.trigger,action:"
 msgid "Action"
 msgstr "Acțiune"
 
 msgctxt "field:ir.trigger,condition:"
 msgid "Condition"
 msgstr "Condiție"
@@ -1493,28 +1504,25 @@
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr "Utilizator"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,field:"
 msgid "Field"
 msgstr "Camp"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,user:"
 msgid "User"
 msgstr "Utilizator"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,value:"
 msgid "Value"
-msgstr "valori"
+msgstr "Valoare"
 
 #, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,view_id:"
 msgid "View ID"
 msgstr "Vederi"
 
 msgctxt "field:ir.ui.view_tree_state,child_name:"
@@ -1613,19 +1621,19 @@
 
 msgctxt "help:ir.action.wizard,window:"
 msgid "Run wizard in a new window."
 msgstr "Rulați asistentul într-o fereastră nouă."
 
 msgctxt "help:ir.email.template,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatar(i)."
 
 msgctxt "help:ir.email.template,recipients_hidden:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatar(i) secundar(i)."
 
 #, fuzzy
 msgctxt "help:ir.email.template,recipients_hidden_pyson:"
 msgid ""
 "A PYSON expression that generates a list of hidden recipients with the "
 "record represented by \"self\"."
 msgstr ""
@@ -1767,72 +1775,72 @@
 
 msgctxt "help:ir.trigger,minimum_time_delay:"
 msgid ""
 "Set a minimum time delay between call to \"Action Function\" for the same record.\n"
 "empty for no delay."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:ir.ui.view_search,domain:"
 msgid "The PYSON domain."
-msgstr ""
+msgstr "Domeniul PYSON."
 
 msgctxt "model:ir.action,name:"
 msgid "Action"
 msgstr "Acțiune"
 
 msgctxt "model:ir.action,name:act_action_act_window_form"
 msgid "Window Actions"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_action_form"
 msgid "Actions"
-msgstr ""
+msgstr "Acțiuni"
 
 msgctxt "model:ir.action,name:act_action_report_form"
 msgid "Reports"
-msgstr ""
+msgstr "Rapoarte"
 
 msgctxt "model:ir.action,name:act_action_url_form"
 msgid "URLs"
-msgstr ""
+msgstr "URL-uri"
 
 msgctxt "model:ir.action,name:act_action_wizard_form"
 msgid "Wizards"
 msgstr "Asistenți"
 
 msgctxt "model:ir.action,name:act_attachment_form"
 msgid "Attachments"
 msgstr "Fișiere atașate"
 
 msgctxt "model:ir.action,name:act_config_wizard_item_form"
 msgid "Config Wizard Items"
 msgstr "Configurarea articolelor de asistent"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_cron_form"
 msgid "Actions"
 msgstr "Acţiuni"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_email_form"
 msgid "E-mails"
-msgstr "Email"
+msgstr "E-mailuri"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_email_form_relate"
 msgid "E-mail Archives"
-msgstr "Email"
+msgstr "Arhive E-mailuri"
 
 msgctxt "model:ir.action,name:act_email_template_form"
 msgid "E-mail Templates"
-msgstr ""
+msgstr "Șabloane E-mail"
 
 msgctxt "model:ir.action,name:act_error_form"
 msgid "Errors"
-msgstr ""
+msgstr "Erori"
 
 msgctxt "model:ir.action,name:act_export_form"
 msgid "Exports"
 msgstr "Exporturi"
 
 msgctxt "model:ir.action,name:act_icon_form"
 msgid "Icons"
@@ -1891,14 +1899,18 @@
 msgid "Fields"
 msgstr "Câmpuri"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modele"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Efectuați activarea / modernizarea în așteptare"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configurarea modulelor"
@@ -1923,18 +1935,17 @@
 msgid "Sequences"
 msgstr "Secvenţe"
 
 msgctxt "model:ir.action,name:act_sequence_strict_form"
 msgid "Sequences Strict"
 msgstr "Secvențe Stricte"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_sequence_type_form"
 msgid "Types"
-msgstr "Tip"
+msgstr "Tipuri"
 
 msgctxt "model:ir.action,name:act_translation_clean"
 msgid "Clean Translations"
 msgstr "Curațare Traduceri"
 
 msgctxt "model:ir.action,name:act_translation_export"
 msgid "Export Translations"
@@ -2012,20 +2023,20 @@
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_error_form_domain_all"
 msgid "All"
 msgstr "Tot"
 
 msgctxt "model:ir.action.act_window.domain,name:act_error_form_domain_open"
 msgid "Open"
-msgstr ""
+msgstr "Deschis"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_error_form_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "În curs de procesare"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_model_data_form_domain_all"
 msgid "All"
 msgstr "Tot"
 
 msgctxt ""
@@ -2373,14 +2384,18 @@
 msgid "Slovenian"
 msgstr ""
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chineză simplificată"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2489,17 +2504,18 @@
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr ""
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "Nu aveț voie sa accessați \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Noi"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
@@ -2735,19 +2751,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notițe"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "Nu aveț voie sa accessați \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2850,14 +2865,18 @@
 msgid "Missing sequence."
 msgstr "Secvență lipsă."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
@@ -2937,29 +2956,35 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "Domeniu nevalid din schema \"% (schema) s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "Nu aveț voie sa accessați \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
+"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
+"\"%(model)s\" depășește limita de \"%(digits)i\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3062,14 +3087,19 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modul"
@@ -3295,14 +3325,18 @@
 msgid "Fields Access"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr ""
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr ""
@@ -3426,23 +3460,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL-uri"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Fereastră"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Asistenți"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL-uri"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Fereastră"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Asistenți"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3464,32 +3538,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL-uri"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Fereastră"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Asistenți"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL-uri"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Fereastră"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Asistenți"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Raport"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL-uri"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Fereastră"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Asistenți"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr ""
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3551,14 +3685,37 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicuri"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "La Ștergere"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Traducere"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3765,14 +3922,29 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Ora"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Sâm"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/ru.po` & `trytond-6.8.0/trytond/ir/locale/ru.po`

 * *Files 4% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 msgid "Name"
 msgstr "Наименование"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Действие"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Просмотр"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Действие"
@@ -1005,14 +1010,37 @@
 msgid "Read Access"
 msgstr "Чтение"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Запись"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Действие"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ресурс"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Пользователь"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Фильтр"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Уровень"
@@ -1965,14 +1993,18 @@
 msgstr "Fields"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Установить / Обновить"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_config"
@@ -2484,14 +2516,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2615,15 +2651,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Комментарий"
 
@@ -2883,19 +2919,18 @@
 msgstr "Вы не можете удалить модуль, который установлен или будет установлен"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Комментарии"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -3008,14 +3043,18 @@
 msgid "Missing sequence."
 msgstr "Отсутствует нумерация."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3098,30 +3137,33 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 "Некорректный домен или условия поиска \"%(domain)s\" у действия "
 "\"%(action)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3225,14 +3267,19 @@
 msgid "Model field"
 msgstr "Поле модели"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Доступ поля модели"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Распечатать граф модели"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Модуль"
@@ -3483,14 +3530,18 @@
 msgstr "Fields Access"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
@@ -3636,23 +3687,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Выбор"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Отчет"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Окно"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Выбор"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Отчет"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Окно"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Действие формы"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Форма связана"
@@ -3674,32 +3765,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Выбор"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Отчет"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Окно"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Выбор"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Отчет"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Окно"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Выбор"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Отчет"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Окно"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Данные"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Ссылка"
@@ -3763,14 +3914,37 @@
 msgid "Left-to-right"
 msgstr "Слева на право"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Справа на лево"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "При удалении"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Перевод"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3982,14 +4156,29 @@
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Формат числа"
 
 #, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Дата"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Часы"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Путь"
+
+#, fuzzy
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Модули были установлены (обновлены)!"
 
 #, fuzzy
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/sl.po` & `trytond-6.8.0/trytond/ir/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Ukrep"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Model"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Pogled"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Ukrep"
@@ -995,14 +1000,37 @@
 msgid "Read Access"
 msgstr "Branje"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Pisanje"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Ukrep"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Vir"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Uporabnik"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filter"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Nivo"
@@ -1951,14 +1979,18 @@
 msgstr "Fields"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_module_config"
@@ -2480,14 +2512,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
@@ -2613,15 +2649,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Zabeležka"
 
@@ -2883,19 +2919,18 @@
 msgstr "Modula, ki je ali bo aktiviran, ni mogoče odstraniti"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -3008,14 +3043,18 @@
 msgid "Missing sequence."
 msgstr "Manjka zaporedna številka."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -3101,30 +3140,33 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 "Neveljavna domena ali iskalni kriterij \"%(domain)s\" pri ukrepu "
 "\"%(action)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3228,14 +3270,19 @@
 msgid "Model field"
 msgstr "Polje modela"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Dostop do polj"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Izpis grafa modela"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Modul"
@@ -3481,14 +3528,18 @@
 msgstr "Fields Access"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
@@ -3634,23 +3685,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Izbrani vozli"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Poročilo"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Izbrani vozli"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Poročilo"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Ukrep za obrazec"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Relacija"
@@ -3672,32 +3763,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Izbrani vozli"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Poročilo"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Izbrani vozli"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Poročilo"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Izbrani vozli"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Poročilo"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Okno"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Podatki"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Povezava"
@@ -3761,14 +3912,37 @@
 msgid "Left-to-right"
 msgstr "Z leve proti desni"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Z desne proti levi"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Kliki"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "Ob brisanju"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Prevod"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Aktivirano"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Deaktivirano"
@@ -3975,14 +4149,29 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Številčni format"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Datum"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Ure"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Pot"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Moduli nadgrajeni oziroma aktivirani."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Ta operacija lahko traja nekaj minut."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/tr.po` & `trytond-6.8.0/trytond/ir/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,19 @@
 
 #, fuzzy
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Actions"
 
 #, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Models"
+
+#, fuzzy
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Views"
 
 #, fuzzy
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
@@ -1007,14 +1012,35 @@
 msgid "Read Access"
 msgstr ""
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Actions"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr ""
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr ""
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Filtre"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Seviye"
@@ -1928,14 +1954,18 @@
 msgid "Fields"
 msgstr "Fields"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Configure Modules"
@@ -2411,14 +2441,18 @@
 msgid "Slovenian"
 msgstr "Slovenian"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr ""
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chinese Simplified"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2532,15 +2566,15 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
 msgstr "You are not allowed to delete this record."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Notes"
 
@@ -2779,19 +2813,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notes"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
-msgstr ""
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
@@ -2896,14 +2929,18 @@
 msgid "Missing sequence."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
@@ -2979,30 +3016,33 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
-msgstr ""
+"exist."
+msgstr "You are not allowed to delete this record."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "You are not allowed to modify this record."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
@@ -3107,14 +3147,19 @@
 msgid "Model field"
 msgstr ""
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Lao"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3351,14 +3396,18 @@
 msgid "Fields Access"
 msgstr "Fields Access"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Models"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Models"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Perform Pending Activation/Upgrade"
@@ -3487,23 +3536,61 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
@@ -3525,33 +3612,90 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Scheduled Actions"
 
 #, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Reports"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URLs"
+
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Wizards"
+
+#, fuzzy
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Data"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr ""
@@ -3613,14 +3757,36 @@
 msgid "Left-to-right"
 msgstr ""
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Clicks"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Translations"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr ""
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr ""
@@ -3830,14 +3996,28 @@
 msgid "Monetary Formatting"
 msgstr ""
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Data"
+
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr ""
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Data"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr ""
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/ir/locale/uk.po` & `trytond-6.8.0/trytond/ir/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,19 @@
 msgid "Name"
 msgstr "Найменування"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "Дія"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "Модель"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "Перегляд"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "Дія"
@@ -955,14 +960,37 @@
 msgid "Read Access"
 msgstr "Читання"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Запис"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "Дія"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "Ресурс"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "Користувач"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "Фільтр"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "Рівень"
@@ -1860,14 +1888,18 @@
 msgid "Fields"
 msgstr "Поля"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Моделі"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Виконати активацію/оновлення"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "Налаштувати модулі"
@@ -2337,14 +2369,18 @@
 msgid "Slovenian"
 msgstr "Словенська"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "Турецька"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Китайська (спрощена)"
 
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
 msgstr "Налаштувати мови"
@@ -2453,17 +2489,18 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "Вам заборонено видаляти записи \"%(ids)s\" із \"%(model)s\" через принаймні одне з цих правил:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "Ви не можете видалити цей запис."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "Вам заборонено виконувати майстер \"%(wizard)s\" на \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "Ні"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
@@ -2706,18 +2743,17 @@
 "Ви не можете видалити модуль, який активований або який ви збираєтесь "
 "активувати."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Примітки"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr ""
 "Ви намагаєтеся прочитати записи \"%(ids)s\" із \"%(model)s\", які більше не "
 "існують."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
@@ -2831,14 +2867,18 @@
 msgid "Missing sequence."
 msgstr "Відсутня послідовність."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Відсутня функція setter для поля \"%(field)s\" в \"%(model)s\"."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Значення поля \"%(field)s\" в \"%(model)s\" задовге (%(size)i > "
@@ -2920,33 +2960,37 @@
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr "Недійсний XML для перегляду \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "Недійсний домен або критерії пошуку \"%(domain)s\" для пошуку \"%(search)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr ""
 "Ви намагаєтеся записати в записи \"%(ids)s\" із \"%(model)s\", які більше не"
 " існують."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Вам заборонено писати в записи \"%(ids)s\" з \"%(model)s\" через принаймні одне з цих правил:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "Вам заборонено змінювати цей запис."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "Потрібно значення для поля \"%(field)s\" в \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 "Синтаксична помилка для XML id: %(value)r в полі \"%(field)s\" моделі "
@@ -3048,14 +3092,19 @@
 msgid "Model field"
 msgstr "Поле моделі"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "Доступ до поля моделі"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "Лаоська"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "Друкувати графік моделі"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "Модуль"
@@ -3276,14 +3325,18 @@
 msgid "Fields Access"
 msgstr "Доступ до полів"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "Моделі"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "Моделі"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Виконати активацію/оновлення"
@@ -3404,22 +3457,62 @@
 msgid "Listed"
 msgstr "Перераховані"
 
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "Вибрані"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "Звіт"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "URL-адреси"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "Вікно"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "Майстри"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr "Перераховані"
 
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Вибрані"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "Звіт"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "URL-адреси"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "Вікно"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "Майстри"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "Форма дії"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "Пов'язана форма"
@@ -3440,30 +3533,90 @@
 msgid "Listed"
 msgstr "Перераховані"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "Вибрані"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "Звіт"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "URL-адреси"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "Вікно"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "Майстри"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr "Перераховані"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "Вибрані"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "Звіт"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "URL-адреси"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "Вікно"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "Майстри"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr "Перераховані"
 
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Вибрані"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "Звіт"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "URL-адреси"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "Вікно"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "Майстри"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "Дані"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "Посилання"
@@ -3524,14 +3677,37 @@
 msgid "Left-to-right"
 msgstr "Зліва-направо"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "Справа-наліво"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "Кліки"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "При видаленні"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "Переклад"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "Активовано"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "Не активовано"
@@ -3736,14 +3912,29 @@
 msgid "Monetary Formatting"
 msgstr "Форматування грошей"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "Форматування чисел"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "Дата"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "Година"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "Сб"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "Модулі оновлено/активовано."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "Зверніть увагу, що ця операція може тривати декілька хвилин."
```

### Comparing `trytond-6.6.8/trytond/ir/locale/zh_CN.po` & `trytond-6.8.0/trytond/ir/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,19 @@
 msgid "Name"
 msgstr "名称"
 
 msgctxt "field:ir.action.act_window.view,act_window:"
 msgid "Action"
 msgstr "动作"
 
+#, fuzzy
+msgctxt "field:ir.action.act_window.view,model:"
+msgid "Model"
+msgstr "模型"
+
 msgctxt "field:ir.action.act_window.view,view:"
 msgid "View"
 msgstr "视图"
 
 msgctxt "field:ir.action.keyword,action:"
 msgid "Action"
 msgstr "动作"
@@ -973,14 +978,37 @@
 msgid "Read Access"
 msgstr "读权限"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "写权限"
 
+#, fuzzy
+msgctxt "field:ir.model.log,action:"
+msgid "Action"
+msgstr "操作"
+
+msgctxt "field:ir.model.log,event:"
+msgid "Event"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,resource:"
+msgid "Resource"
+msgstr "资源"
+
+msgctxt "field:ir.model.log,target:"
+msgid "Target"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:ir.model.log,user:"
+msgid "User"
+msgstr "用户"
+
 msgctxt "field:ir.model.print_model_graph.start,filter:"
 msgid "Filter"
 msgstr "筛选"
 
 msgctxt "field:ir.model.print_model_graph.start,level:"
 msgid "Level"
 msgstr "层级"
@@ -1880,14 +1908,18 @@
 msgid "Fields"
 msgstr "字段"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "模型"
 
+msgctxt "model:ir.action,name:act_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "挂起激活 / 升级"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
 msgstr "配置模块"
@@ -2363,14 +2395,18 @@
 msgid "Slovenian"
 msgstr "斯洛文尼亚语"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
 msgstr "土耳其语"
 
+msgctxt "model:ir.lang,name:lang_uk"
+msgid "Ukrainian"
+msgstr ""
+
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "中文简体"
 
 #, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
@@ -2482,17 +2518,18 @@
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
 "不允许删除模型 \"%(model)s\" 的记录 \"%(ids)s\" ， 由于下面的规则（至少一条）:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
-msgid "You are not allowed to delete this record."
-msgstr "没有权限删除此记录."
+msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
+msgstr "没有权限在 \"%(model)s\" 上运行向导程序 \"%(wizard)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
 msgstr "十一月"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
@@ -2722,18 +2759,17 @@
 "activated."
 msgstr "无法移除未安装或者待安装状态的模块."
 
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "注释"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
-msgid ""
-"You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist"
-" anymore."
+msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
 msgstr "\"%(model)s\" 的记录 \"%(ids)s\" 已经不存在了，无法读取."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
@@ -2835,14 +2871,18 @@
 msgid "Missing sequence."
 msgstr "序列缺失."
 
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "模型 \"%(model)s\" 的字段\"%(field)s\" 没有 setter 函数."
 
+msgctxt "model:ir.message,text:msg_singleton"
+msgid "Only one singleton can be created."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "模型 \"%(model)s\" 的字段 \"%(field)s\" ，其取值位数太长(%(size)i > %(max_size)i)."
 
@@ -2917,31 +2957,35 @@
 msgstr "视图 \"%(name)s\" 对应的XML不合法."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
 msgstr "动作 \"%(action)s\" 的域或找条件 \"%(domain)s\" 无效."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
-"exist anymore."
+"exist."
 msgstr "\"%(model)s\" 的记录 \"%(ids)s\" 已经不存在了，无法写入."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "不允许写入模型 \"%(model)s\" 的记录 \"%(ids)s\" ， 由于下面的规则（至少一条）:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
-msgid "You are not allowed to modify this record."
-msgstr "你无权修改此记录."
+msgid ""
+"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "模型\"%(model)s\"的字段\"%(field)s\"需要有取值."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "XML id 语法错误：\"%(field)s\" 的取值 \"%(value)r\" ."
@@ -3044,14 +3088,19 @@
 msgid "Model field"
 msgstr "模型字段"
 
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr "模型字段权限"
 
+#, fuzzy
+msgctxt "model:ir.model.log,name:"
+msgid "Log"
+msgstr "老挝语"
+
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr "打印模型图"
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
 msgstr "模块"
@@ -3277,14 +3326,18 @@
 msgid "Fields Access"
 msgstr "字段访问权限"
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
 msgstr "模型"
 
+msgctxt "model:ir.ui.menu,name:menu_model_log_form"
+msgid "Logs"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
 msgstr "模型"
 
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "执行 \"未完成的安装\"/ \"升级\""
@@ -3408,23 +3461,63 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action,records:"
 msgid "Selected"
 msgstr "已选定的节点"
 
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Report"
+msgstr "报告"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "URL"
+msgstr "网址"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Window"
+msgstr "窗口"
+
+#, fuzzy
+msgctxt "selection:ir.action,type:"
+msgid "Wizard"
+msgstr "向导"
+
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "已选定的节点"
 
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Report"
+msgstr "报告"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "URL"
+msgstr "网址"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Window"
+msgstr "窗口"
+
+#, fuzzy
+msgctxt "selection:ir.action.act_window,type:"
+msgid "Wizard"
+msgstr "向导"
+
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr "动作表单"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr "关联表单"
@@ -3446,32 +3539,92 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
 msgstr "已选定的节点"
 
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Report"
+msgstr "报告"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "URL"
+msgstr "网址"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Window"
+msgstr "窗口"
+
+#, fuzzy
+msgctxt "selection:ir.action.report,type:"
+msgid "Wizard"
+msgstr "向导"
+
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
 msgstr "已选定的节点"
 
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Report"
+msgstr "报告"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "URL"
+msgstr "网址"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Window"
+msgstr "窗口"
+
+#, fuzzy
+msgctxt "selection:ir.action.url,type:"
+msgid "Wizard"
+msgstr "向导"
+
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "已选定的节点"
 
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Report"
+msgstr "报告"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "URL"
+msgstr "网址"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Window"
+msgstr "窗口"
+
+#, fuzzy
+msgctxt "selection:ir.action.wizard,type:"
+msgid "Wizard"
+msgstr "向导"
+
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
 msgstr "数据"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
 msgstr "链接"
@@ -3534,14 +3687,37 @@
 msgid "Left-to-right"
 msgstr "从左向右"
 
 msgctxt "selection:ir.lang,direction:"
 msgid "Right-to-left"
 msgstr "从右向左"
 
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Clicked on"
+msgstr "点击"
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Deleted"
+msgstr "删除时触发"
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Launched"
+msgstr ""
+
+msgctxt "selection:ir.model.log,event:"
+msgid "Modified"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:ir.model.log,event:"
+msgid "Transitioned to"
+msgstr "翻译"
+
 msgctxt "selection:ir.module,state:"
 msgid "Activated"
 msgstr "已启用"
 
 msgctxt "selection:ir.module,state:"
 msgid "Not Activated"
 msgstr "没有激活"
@@ -3749,14 +3925,29 @@
 msgid "Monetary Formatting"
 msgstr "货币格式"
 
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
 msgstr "数字格式"
 
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Date"
+msgstr "日期"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "Hour"
+msgstr "小时"
+
+#, fuzzy
+msgctxt "view:ir.model.log:"
+msgid "at"
+msgstr "星期六"
+
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
 msgstr "模块已升级/激活."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
 msgstr "注意：本操作可能需要几分钟时间."
```

### Comparing `trytond-6.6.8/trytond/ir/message.py` & `trytond-6.8.0/trytond/ir/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from trytond.transaction import Transaction
 
 
 class Message(ModelSQL, ModelView):
     "Message"
     __name__ = "ir.message"
 
-    _message_cache = Cache('ir.message', size_limit=10240, context=False)
+    _message_cache = Cache('ir.message', context=False)
     text = fields.Text("Text", required=True, translate=True)
 
     @classmethod
     def gettext(cls, *args, **variables):
         pool = Pool()
         ModelData = pool.get('ir.model.data')
         module, message_id, language = args
```

### Comparing `trytond-6.6.8/trytond/ir/message.xml` & `trytond-6.8.0/trytond/ir/message.xml`

 * *Files 0% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/ir/message.xml` & `trytond-6.8.0/trytond/ir/message.xml`

```diff
@@ -128,19 +128,22 @@
     </record>
     <record model="ir.message" id="msg_sequence">
       <field name="text">Sequence</field>
     </record>
     <record model="ir.message" id="msg_id_positive">
       <field name="text">ID must be positive.</field>
     </record>
+    <record model="ir.message" id="msg_singleton">
+      <field name="text">Only one singleton can be created.</field>
+    </record>
     <record model="ir.message" id="msg_write_xml_record">
-      <field name="text">You are not allowed to modify this record.</field>
+      <field name="text">You are not allowed to modify the field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_delete_xml_record">
-      <field name="text">You are not allowed to delete this record.</field>
+      <field name="text">You are not allowed to delete the record &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_base_config_record">
       <field name="text">This record is part of the base configuration.</field>
     </record>
     <record model="ir.message" id="msg_relation_not_found">
       <field name="text">Relation not found: %(value)r in &quot;%(model)s&quot; (%(column)s).</field>
     </record>
@@ -200,22 +203,22 @@
 %(rules)s</field>
     </record>
     <record model="ir.message" id="msg_read_rule_error">
       <field name="text">You are not allowed to read records &quot;%(ids)s&quot; of &quot;%(model)s&quot; because of at least one of these rules:
 %(rules)s</field>
     </record>
     <record model="ir.message" id="msg_read_error">
-      <field name="text">You are trying to read records &quot;%(ids)s&quot; of &quot;%(model)s&quot; that don't exist anymore.</field>
+      <field name="text">You are trying to read records &quot;%(ids)s&quot; of &quot;%(model)s&quot; that don't exist.</field>
     </record>
     <record model="ir.message" id="msg_write_rule_error">
       <field name="text">You are not allowed to write to records &quot;%(ids)s&quot; of &quot;%(model)s&quot; because of at least one of these rules:
 %(rules)s</field>
     </record>
     <record model="ir.message" id="msg_write_error">
-      <field name="text">You are trying to write to records &quot;%(ids)s&quot; of &quot;%(model)s&quot; that don't exist anymore.</field>
+      <field name="text">You are trying to write to records &quot;%(ids)s&quot; of &quot;%(model)s&quot; that don't exist.</field>
     </record>
     <record model="ir.message" id="msg_delete_rule_error">
       <field name="text">You are not allowed to delete records &quot;%(ids)s&quot; of &quot;%(model)s&quot; because of at lease one of those rules:
 %(rules)s</field>
     </record>
     <record model="ir.message" id="msg_dict_schema_invalid_domain">
       <field name="text">Invalid domain in schema &quot;%(schema)s&quot;.</field>
```

### Comparing `trytond-6.6.8/trytond/ir/model.py` & `trytond-6.8.0/trytond/ir/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 from trytond.pool import Pool
 from trytond.protocols.jsonrpc import JSONDecoder, JSONEncoder
 from trytond.pyson import Bool, Eval, PYSONDecoder
 from trytond.report import Report
 from trytond.rpc import RPC
 from trytond.tools import cursor_dict, grouped_slice, is_instance_method
 from trytond.tools.string_ import StringMatcher
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 from trytond.wizard import Button, StateAction, StateView, Wizard
 
+from .resource import ResourceAccessMixin
+
 logger = logging.getLogger(__name__)
 
 
 class ConditionError(ValidationError):
     pass
 
 
@@ -264,14 +266,15 @@
         "is also tested against the relation of the field.")
 
     _get_name_cache = Cache('ir.model.field.get_name')
 
     @classmethod
     def __setup__(cls):
         super(ModelField, cls).__setup__()
+        cls.__access__.add('model')
         table = cls.__table__()
         cls._sql_constraints += [
             ('name_model_uniq', Unique(table, table.name, table.model),
                 'The field name in model must be unique!'),
             ]
         cls._order.insert(0, ('name', 'ASC'))
 
@@ -484,21 +487,22 @@
     perm_delete = fields.Boolean('Delete Access')
     description = fields.Text('Description')
     _get_access_cache = Cache('ir_model_access.get_access', context=False)
 
     @classmethod
     def __setup__(cls):
         super(ModelAccess, cls).__setup__()
+        cls.__access__.add('model')
         cls.__rpc__.update({
                 'get_access': RPC(),
                 })
 
-    @staticmethod
-    def check_xml_record(accesses, values):
-        return True
+    @classmethod
+    def check_xml_record(cls, accesses, values):
+        pass
 
     @staticmethod
     def default_perm_read():
         return False
 
     @staticmethod
     def default_perm_write():
@@ -610,17 +614,17 @@
     @classmethod
     def check(cls, model_name, mode='read', raise_exception=True):
         'Check access for model_name and mode'
         pool = Pool()
         Model = pool.get(model_name)
         assert mode in ['read', 'write', 'create', 'delete'], \
             'Invalid access mode for security'
-        if ((Transaction().user == 0)
-                or (raise_exception
-                    and not Transaction().context.get('_check_access'))):
+        transaction = Transaction()
+        if (transaction.user == 0
+                or (raise_exception and not transaction.check_access)):
             return True
 
         access = cls.get_access([model_name])[model_name][mode]
         if not access and access is not None:
             if raise_exception:
                 raise AccessError(gettext(
                         'ir.msg_access_rule_error', **Model.__names__()))
@@ -697,17 +701,22 @@
     perm_read = fields.Boolean('Read Access')
     perm_write = fields.Boolean('Write Access')
     perm_create = fields.Boolean('Create Access')
     perm_delete = fields.Boolean('Delete Access')
     description = fields.Text('Description')
     _get_access_cache = Cache('ir_model_field_access.check', context=False)
 
-    @staticmethod
-    def check_xml_record(field_accesses, values):
-        return True
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.add('field')
+
+    @classmethod
+    def check_xml_record(cls, field_accesses, values):
+        pass
 
     @staticmethod
     def default_perm_read():
         return False
 
     @staticmethod
     def default_perm_write():
@@ -802,17 +811,17 @@
         '''
         Check access for fields on model_name.
         '''
         pool = Pool()
         Model = pool.get(model_name)
         assert mode in ('read', 'write', 'create', 'delete'), \
             'Invalid access mode'
-        if ((Transaction().user == 0)
-                or (raise_exception
-                    and not Transaction().context.get('_check_access'))):
+        transaction = Transaction()
+        if (transaction.user == 0
+                or (raise_exception and not transaction.check_access)):
             if access:
                 return dict((x, True) for x in fields)
             return True
 
         accesses = dict((f, a[mode])
             for f, a in cls.get_access([model_name])[model_name].items())
         if access:
@@ -890,14 +899,15 @@
 
         # Migration from 6.2: replace unique by exclude
         table_h.drop_constraint('name_model_uniq')
 
     @classmethod
     def __setup__(cls):
         super(ModelButton, cls).__setup__()
+        cls.__access__.add('model')
         t = cls.__table__()
         cls._sql_constraints += [
             ('name_model_exclude',
                 Exclude(t, (t.name, Equal), (t.model, Equal),
                     where=(t.active == Literal(True))),
                 'ir.msg_button_name_unique'),
             ]
@@ -932,14 +942,15 @@
             default = {}
         else:
             default = default.copy()
         default.setdefault('clicks')
         return super(ModelButton, cls).copy(buttons, default=default)
 
     @classmethod
+    @without_check_access
     def get_rules(cls, model, name):
         'Return a list of rules to apply on the named button of the model'
         pool = Pool()
         Rule = pool.get('ir.model.button.rule')
         key = (model, name)
         rule_ids = cls._rules_cache.get(key)
         if rule_ids is not None:
@@ -953,14 +964,15 @@
         else:
             button, = buttons
             rules = button.rules
         cls._rules_cache.set(key, [r.id for r in rules])
         return rules
 
     @classmethod
+    @without_check_access
     def get_reset(cls, model, name):
         "Return a list of button names to reset"
         key = (model, name)
         reset = cls._reset_cache.get(key)
         if reset is not None:
             return reset
         buttons = cls.search([
@@ -1008,14 +1020,19 @@
     number_user = fields.Integer('Number of User', required=True)
     condition = fields.Char(
         "Condition",
         help='A PYSON statement evaluated with the record represented by '
         '"self"\nIt activate the rule if true.')
 
     @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.add('button')
+
+    @classmethod
     def default_number_user(cls):
         return 1
 
     @classmethod
     def validate_fields(cls, rules, field_names):
         super().validate_fields(rules, field_names)
         cls.check_condition(rules, field_names)
@@ -1080,14 +1097,15 @@
     button = fields.Many2One(
         'ir.model.button', "Button", required=True, ondelete='CASCADE')
     record_id = fields.Integer("Record ID", required=True)
 
     @classmethod
     def __setup__(cls):
         super(ModelButtonClick, cls).__setup__()
+        cls.__access__.add('button')
         cls.__rpc__.update({
                 'get_click': RPC(),
                 })
 
     @classmethod
     def register(cls, model, name, records):
         pool = Pool()
@@ -1114,14 +1132,15 @@
                     ], order=[('record_id', 'ASC')])
             clicks.update(
                 (k, list(v)) for k, v in groupby(
                     records, key=lambda c: c.record_id))
         return clicks
 
     @classmethod
+    @without_check_access
     def reset(cls, model, names, records):
         assert all(r.__class__.__name__ == model for r in records)
 
         clicks = []
         for records in grouped_slice(records):
             clicks.extend(cls.search([
                         ('button.model.model', '=', model),
@@ -1267,14 +1286,63 @@
 
             cursor.execute(*table.select(table.model, group_by=[table.model]))
             models = [m for m, in cursor]
             cls._has_model_cache.set(None, models)
         return model in models
 
     @classmethod
+    @without_check_access
+    def can_modify(cls, records, values):
+        for Model, records in groupby(
+                records, key=lambda r: r.__class__):
+            for sub_records in grouped_slice(records):
+                id2record = {r.id: r for r in sub_records}
+                data = cls.search([
+                        ('model', '=', Model.__name__),
+                        ('db_id', 'in', list(id2record.keys())),
+                        ], order=[])
+                for data in data:
+                    record = id2record[data.db_id]
+                    if values is None:
+                        if not data.noupdate:
+                            raise AccessError(
+                                gettext(
+                                    'ir.msg_delete_xml_record',
+                                    **Model.__names__(record=record)),
+                                gettext('ir.msg_base_config_record'))
+                    else:
+                        if not data.values or data.noupdate:
+                            continue
+                        xml_values = cls.load_values(data.values)
+                        for key, val in values.items():
+                            if key in xml_values and val != xml_values[key]:
+                                raise AccessError(
+                                    gettext(
+                                        'ir.msg_write_xml_record',
+                                        **cls.__names__(
+                                            field=key, record=record)),
+                                    gettext('ir.msg_base_config_record'))
+
+    @classmethod
+    @without_check_access
+    def clean(cls, records):
+        data = []
+        for name, records in groupby(
+                records, key=lambda r: r.__class__.__name__):
+            for sub_records in grouped_slice(records):
+                ids = [r.id for r in sub_records]
+                data += cls.search([
+                        ('model', '=', name),
+                        ('db_id', 'in', ids),
+                        ('noupdate', '=', True),
+                        ], order=[])
+        cls.write(data, {'db_id': None})
+
+    @classmethod
+    @without_check_access
     def get_id(cls, module, fs_id=None):
         """
         Return for an fs_id the corresponding db_id.
         """
         if fs_id is None:
             module, fs_id = module.split('.', 1)
         key = (module, fs_id)
@@ -1349,14 +1417,92 @@
                             }])
             for Model, values_to_write in models_to_write.items():
                 Model.write(*values_to_write)
             if to_write:
                 cls.write(*to_write)
 
 
+class Log(ResourceAccessMixin, ModelSQL, ModelView):
+    "Log"
+    __name__ = 'ir.model.log'
+
+    user = fields.Many2One(
+        'res.user', "User",
+        states={
+            'required': Eval('event') != 'transition',
+            })
+    event = fields.Selection([
+            ('write', "Modified"),
+            ('delete', "Deleted"),
+            ('button', "Clicked on"),
+            ('wizard', "Launched"),
+            ('transition', "Transitioned to"),
+            ], "Event", required=True)
+    event_string = event.translated('event')
+    target = fields.Char(
+        "Target",
+        states={
+            'required': Eval('event').in_(
+                ['write', 'button', 'wizard', 'transition']),
+            'invisible': (
+                ~Eval('event').in_(
+                    ['write', 'button', 'wizard', 'transition'])),
+            })
+    action = fields.Function(
+        fields.Char("Action"), 'get_action', searcher='search_action')
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.resource.required = False  # store deleted record
+        cls._order = [
+            ('create_date', 'DESC'),
+            ('id', 'DESC'),
+            ]
+
+    @classmethod
+    def get_models(cls):
+        return super().get_models() + [(None, '')]  # store deleted record
+
+    def get_action(self, name):
+        pool = Pool()
+        Field = pool.get('ir.model.field')
+        Button = pool.get('ir.model.button')
+        Wizard = pool.get('ir.action.wizard')
+        if self.resource:
+            Model = self.resource.__class__
+            model = self.resource.__name__
+            if self.event == 'write':
+                fields = self.target.split(',')
+                get_name = Field.get_name
+                fields = [get_name(model, f) for f in fields]
+                return ', '.join(fields)
+            elif self.event == 'button':
+                return Button.get_view_attributes(model, self.target).get(
+                    'string', self.target)
+            elif self.event == 'wizard':
+                wiz_name, state_name = self.target.split(':')
+                wiz_name = Wizard.get_name(wiz_name, model)
+                return f'{state_name} @ {wiz_name}'
+            elif self.event == 'transition':
+                field_name, state = self.target.split(':')
+                field = getattr(Model, field_name, None)
+                field_name = Field.get_name(model, field_name)
+                if field:
+                    selection = field.get_selection(
+                        Model, field.name, self.resource)
+                    state = field.get_selection_string(selection, state)
+                return f'{field_name} : {state}'
+        return self.target
+
+    @classmethod
+    def search_action(cls, name, clause):
+        return [('target', *clause[1:])]
+
+
 class PrintModelGraphStart(ModelView):
     'Print Model Graph'
     __name__ = 'ir.model.print_model_graph.start'
     level = fields.Integer('Level', required=True)
     filter = fields.Text('Filter', help="Entering a Python "
             "Regular Expression will exclude matching models from the graph.")
```

### Comparing `trytond-6.6.8/trytond/ir/model.xml` & `trytond-6.8.0/trytond/ir/model.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/ir/model.xml` & `trytond-6.8.0/trytond/ir/model.xml`

```diff
@@ -248,9 +248,34 @@
     </record>
     <menuitem parent="menu_model_form" action="act_model_data_form" sequence="50" id="menu_model_data_form"/>
     <record model="ir.model.button" id="model_data_sync_button">
       <field name="name">sync</field>
       <field name="string">Sync</field>
       <field name="model" search="[('model', '=', 'ir.model.data')]"/>
     </record>
+    <record model="ir.ui.view" id="model_log_view_form">
+      <field name="model">ir.model.log</field>
+      <field name="type">form</field>
+      <field name="name">model_log_form</field>
+    </record>
+    <record model="ir.ui.view" id="model_log_view_list">
+      <field name="model">ir.model.log</field>
+      <field name="type">tree</field>
+      <field name="name">model_log_list</field>
+    </record>
+    <record model="ir.action.act_window" id="act_model_log_form">
+      <field name="name">Logs</field>
+      <field name="res_model">ir.model.log</field>
+    </record>
+    <record model="ir.action.act_window.view" id="act_model_log_form_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="model_log_view_list"/>
+      <field name="act_window" ref="act_model_log_form"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_model_log_form_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="model_log_view_form"/>
+      <field name="act_window" ref="act_model_log_form"/>
+    </record>
+    <menuitem parent="menu_model_form" action="act_model_log_form" sequence="50" id="menu_model_log_form"/>
   </data>
 </tryton>
```

### Comparing `trytond-6.6.8/trytond/ir/module.py` & `trytond-6.8.0/trytond/ir/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ModelView, Unique, fields, sequence_ordered
 from trytond.model.exceptions import AccessError
 from trytond.modules import get_module_info, get_module_list
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.rpc import RPC
+from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 
 class DeactivateDependencyError(UserError):
     pass
@@ -273,62 +274,42 @@
     @ModelView.button
     @filter_state('to upgrade')
     def upgrade_cancel(cls, modules):
         cls.write(modules, {'state': 'activated'})
 
     @classmethod
     def update_list(cls):
-        'Update the list of available packages'
-        count = 0
-        module_names = get_module_list()
-
-        modules = cls.search([])
-        name2id = dict((m.name, m.id) for m in modules)
-        cls.delete([m for m in modules
-                if m.state != 'activated' and m.name not in module_names])
-
-        # iterate through activated modules and mark them as being so
-        for name in module_names:
-            if name in name2id:
-                module = cls(name2id[name])
-                tryton = get_module_info(name)
-                cls._update_dependencies(module, tryton.get('depends', []))
-                continue
-
-            tryton = get_module_info(name)
-            if not tryton:
-                continue
-            module, = cls.create([{
-                        'name': name,
-                        'state': 'not activated',
-                        }])
-            count += 1
-            cls._update_dependencies(module, tryton.get('depends', []))
-        return count
-
-    @classmethod
-    def _update_dependencies(cls, module, depends=None):
+        "Update the list of available modules"
         pool = Pool()
         Dependency = pool.get('ir.module.dependency')
-        Dependency.delete([x for x in module.dependencies
-            if x.name not in depends])
-        if depends is None:
-            depends = []
-        # Restart Browse Cache for deleted dependencies
-        module = cls(module.id)
-        dependency_names = [x.name for x in module.dependencies]
-        to_create = []
-        for depend in depends:
-            if depend not in dependency_names:
-                to_create.append({
-                        'module': module.id,
-                        'name': depend,
-                        })
-        if to_create:
-            Dependency.create(to_create)
+        module_names = get_module_list(with_test=Pool.test)
+        for sub_module_names in grouped_slice(module_names):
+            cls.delete(cls.search([
+                        ('state', '!=', 'activated'),
+                        ('name', 'not in', list(sub_module_names)),
+                        ]))
+        modules = cls.search([])
+        name2module = {m.name: m for m in modules}
+
+        for name in set(module_names) - name2module.keys():
+            name2module[name] = cls(name=name, state=cls.default_state())
+        cls.save(name2module.values())
+
+        to_save, to_delete = [], []
+        for module in name2module.values():
+            depends = set(get_module_info(module.name).get('depends', []))
+            for dependency in module.dependencies:
+                if dependency.name not in depends:
+                    to_delete.append(dependency)
+            for name in depends - {d.name for d in module.dependencies}:
+                to_save.append(Dependency(name=name, module=module))
+        if to_delete:
+            Dependency.delete(to_delete)
+        if to_save:
+            Dependency.save(to_save)
 
 
 class ModuleDependency(ModelSQL, ModelView):
     "Module dependency"
     __name__ = "ir.module.dependency"
     name = fields.Char('Name')
     module = fields.Many2One('ir.module', 'Module',
@@ -341,14 +322,15 @@
                 ('to activate', 'To be activated'),
                 ('unknown', 'Unknown'),
                 ], 'State', readonly=True), 'get_state')
 
     @classmethod
     def __setup__(cls):
         super(ModuleDependency, cls).__setup__()
+        cls.__access__.add('module')
         table = cls.__table__()
         cls._sql_constraints += [
             ('name_module_uniq', Unique(table, table.name, table.module),
                 'Dependency must be unique by module!'),
         ]
 
     @classmethod
@@ -356,24 +338,26 @@
         # Migration from 3.6: remove double module
         old_table = 'ir_module_module_dependency'
         if backend.TableHandler.table_exist(old_table):
             backend.TableHandler.table_rename(old_table, cls._table)
 
         super(ModuleDependency, cls).__register__(module_name)
 
-    def get_state(self, name):
+    @classmethod
+    def get_state(cls, dependencies, name):
         pool = Pool()
         Module = pool.get('ir.module')
-        dependencies = Module.search([
-                ('name', '=', self.name),
-                ])
-        if dependencies:
-            return dependencies[0].state
-        else:
-            return 'unknown'
+        modules = []
+        names = [d.name for d in dependencies]
+        for sub_names in grouped_slice(names):
+            modules.extend(Module.search([
+                        ('name', 'in', list(sub_names)),
+                        ]))
+        name2state = {m.name: m.state for m in modules}
+        return {d.id: name2state.get(d.name, 'unknown') for d in dependencies}
 
 
 class ModuleConfigWizardItem(sequence_ordered(), ModelSQL, ModelView):
     "Config wizard to run after activating a module"
     __name__ = 'ir.module.config_wizard.item'
     action = fields.Many2One('ir.action', 'Action', required=True,
         readonly=True)
@@ -420,25 +404,25 @@
     __name__ = 'ir.module.config_wizard.first'
 
 
 class ModuleConfigWizardOther(ModelView):
     'Module Config Wizard Other'
     __name__ = 'ir.module.config_wizard.other'
 
-    percentage = fields.Float('Percentage', readonly=True)
+    percentage = fields.Float('Percentage', digits=(1, 2), readonly=True)
 
     @staticmethod
     def default_percentage():
         pool = Pool()
         Item = pool.get('ir.module.config_wizard.item')
         done = Item.search([
             ('state', '=', 'done'),
             ], count=True)
         all = Item.search([], count=True)
-        return done / all
+        return round(done / all, 2)
 
 
 class ModuleConfigWizardDone(ModelView):
     'Module Config Wizard Done'
     __name__ = 'ir.module.config_wizard.done'
 
 
@@ -624,9 +608,10 @@
 class ModuleConfigStart(ModelView):
     "Configure Modules"
     __name__ = 'ir.module.config.start'
 
     modules = fields.Many2Many(
         'ir.module', None, None, "Modules",
         domain=[
+            ('name', '!=', 'tests'),
             ('state', '=', 'not activated'),
             ])
```

### Comparing `trytond-6.6.8/trytond/ir/module.xml` & `trytond-6.8.0/trytond/ir/module.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/note.py` & `trytond-6.8.0/trytond/ir/note.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/note.xml` & `trytond-6.8.0/trytond/ir/note.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/queue_.py` & `trytond-6.8.0/trytond/ir/queue_.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sql.aggregate import Min
 from sql.functions import CurrentTimestamp, Extract
 
 from trytond.config import config
 from trytond.model import Index, ModelSQL, fields
 from trytond.pool import Pool
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 has_worker = config.getboolean('queue', 'worker', default=False)
 clean_days = config.getint('queue', 'clean_days', default=30)
 batch_size = config.getint('queue', 'batch_size', default=20)
 
 
 class Queue(ModelSQL):
@@ -153,22 +153,22 @@
         Model = Pool().get(self.data['model'])
         with transaction.set_user(self.data['user']), \
                 transaction.set_context(
                     self.data['context'], _skip_warnings=True):
             instances = self.data['instances']
             # Ensure record ids still exist
             if isinstance(instances, int):
-                with transaction.set_context(active_test=False):
+                with inactive_records():
                     if Model.search([('id', '=', instances)]):
                         instances = Model(instances)
                     else:
                         instances = None
             else:
                 ids = set()
-                with transaction.set_context(active_test=False):
+                with inactive_records():
                     for sub_ids in grouped_slice(instances):
                         records = Model.search([('id', 'in', list(sub_ids))])
                         ids.update(map(int, records))
                 if ids:
                     instances = Model.browse(
                         [i for i in instances if i in ids])
                 else:
```

### Comparing `trytond-6.6.8/trytond/ir/resource.py` & `trytond-6.8.0/trytond/ir/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # this repository contains the full copyright notices and license terms.
 from sql.conditionals import Coalesce
 
 from trytond.i18n import lazy_gettext
 from trytond.model import Index, ModelSQL, ModelStorage, ModelView, fields
 from trytond.pool import Pool
 from trytond.pyson import Eval
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 __all__ = ['ResourceAccessMixin', 'ResourceMixin', 'resource_copy']
 
 
 class ResourceAccessMixin(ModelStorage):
 
     resource = fields.Reference(
@@ -30,28 +30,28 @@
 
     @staticmethod
     def get_models():
         pool = Pool()
         Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
         models = Model.get_name_items()
-        if Transaction().context.get('_check_access'):
+        if Transaction().check_access:
             access = ModelAccess.get_access([m for m, _ in models])
             models = [(m, n) for m, n in models if access[m]['read']]
         return models
 
     @classmethod
     def check_access(cls, ids, mode='read'):
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
-        if ((Transaction().user == 0)
-                or not Transaction().context.get('_check_access')):
+        transaction = Transaction()
+        if transaction.user == 0 or not transaction.check_access:
             return
         model_names = set()
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             for record in cls.browse(ids):
                 if record.resource:
                     model_names.add(str(record.resource).split(',')[0])
         for model_name in model_names:
             checks = cls._convert_check_access(model_name, mode)
             for model, check_mode in checks:
                 ModelAccess.check(model, mode=check_mode)
```

### Comparing `trytond-6.6.8/trytond/ir/routes.py` & `trytond-6.8.0/trytond/ir/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,19 @@
 # this repository contains the full copyright notices and license terms.
 import csv
 import datetime as dt
 import io
 import json
 from numbers import Number
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
-from werkzeug.exceptions import abort
-from werkzeug.utils import redirect
-from werkzeug.wrappers import Response
-
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.protocols.jsonrpc import JSONDecoder
-from trytond.protocols.wrappers import with_pool, with_transaction
+from trytond.protocols.wrappers import (
+    HTTPStatus, Response, abort, redirect, with_pool, with_transaction)
 from trytond.tools import slugify
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 SOURCE = config.get(
     'html', 'src', default='https://cloud.tinymce.com/stable/tinymce.min.js')
 AVATAR_TIMEOUT = config.getint(
```

### Comparing `trytond-6.6.8/trytond/ir/rule.py` & `trytond-6.8.0/trytond/ir/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from trytond.cache import Cache
 from trytond.i18n import gettext
 from trytond.model import (
     Check, EvalEnvironment, Index, ModelSQL, ModelView, fields)
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
 from trytond.pyson import PYSONDecoder
-from trytond.transaction import Transaction
+from trytond.transaction import (
+    Transaction, inactive_records, without_check_access)
 
 
 class DomainError(ValidationError):
     pass
 
 
 class RuleGroup(ModelSQL, ModelView):
@@ -112,14 +113,15 @@
     _domain_get_cache = Cache('ir_rule.domain_get', context=False)
 
     modes = {'read', 'write', 'create', 'delete'}
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
+        cls.__access__.add('rule_group')
         table = cls.__table__()
 
         cls._sql_indexes.add(
             Index(table, (table.rule_group, Index.Equality())))
 
     @classmethod
     def validate_fields(cls, rules, field_names):
@@ -148,15 +150,16 @@
                             'ir.msg_rule_invalid_domain', name=rule.rec_name))
 
     @staticmethod
     def _get_context():
         User = Pool().get('res.user')
         transaction = Transaction()
         user_id = transaction.user
-        with transaction.set_context(_check_access=False, _datetime=None), \
+        with transaction.set_context(_datetime=None), \
+                without_check_access(), \
                 transaction.set_user(0):
             user = EvalEnvironment(User(user_id), User)
         return {
             'user': user,
             'groups': User.get_groups()
             }
 
@@ -264,16 +267,15 @@
 
         return clause, clause_global
 
     @classmethod
     def domain_get(cls, model_name, mode='read'):
         transaction = Transaction()
         # root user above constraint
-        if ((transaction.user == 0)
-                or not transaction.context.get('_check_access')):
+        if transaction.user == 0 or not transaction.check_access:
             return []
 
         assert mode in cls.modes
 
         key = (model_name, mode) + cls._get_cache_key()
         domain = cls._domain_get_cache.get(key, False)
         if domain is not False:
@@ -302,16 +304,15 @@
     def query_get(cls, model_name, mode='read'):
         pool = Pool()
         Model = pool.get(model_name)
 
         domain = cls.domain_get(model_name, mode=mode)
 
         # Use root to prevent infinite recursion
-        with Transaction().set_user(0), \
-                Transaction().set_context(active_test=False, user=0):
+        with Transaction().set_user(0, set_context=True), inactive_records():
             return Model.search(domain, order=[], query=True)
 
     @classmethod
     def delete(cls, rules):
         super(Rule, cls).delete(rules)
         # Restart the cache on the domain_get method of ir.rule
         cls._domain_get_cache.clear()
```

### Comparing `trytond-6.6.8/trytond/ir/rule.xml` & `trytond-6.8.0/trytond/ir/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/sequence.py` & `trytond-6.8.0/trytond/ir/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from trytond import backend
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.model import Check, DeactivableMixin, ModelSQL, ModelView, fields
 from trytond.model.exceptions import AccessError, ValidationError
 from trytond.pool import Pool
 from trytond.pyson import And, Eval
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 sql_sequence = backend.Database.has_sequence()
 
 
 class AffixError(ValidationError):
     pass
 
@@ -199,16 +199,15 @@
                 sequence.update_sql_sequence(values.get('number_next',
                         cls.default_number_next()))
         return sequences
 
     @classmethod
     def write(cls, *args):
         transaction = Transaction()
-        if (transaction.user != 0
-                and transaction.context.get('_check_access')):
+        if transaction.user != 0 and transaction.check_access:
             for values in args[1::2]:
                 if 'sequence_type' in values:
                     raise AccessError(gettext(
                             'ir.msg_sequence_change_sequence_type'))
         super().write(*args)
         if sql_sequence and not cls._strict:
             actions = iter(args)
@@ -370,34 +369,32 @@
                 })
             if sequence.type == 'decimal timestamp':
                 return '%d' % timestamp
             else:
                 return hex(timestamp)[2:].upper()
         return ''
 
+    @without_check_access
     def get(self, _lock=False):
         '''
         Return the next sequence value
         '''
         cls = self.__class__
-        # bypass rules on sequences
-        with Transaction().set_context(user=False, _check_access=False):
-            with Transaction().set_user(0):
-                try:
-                    sequence = cls(self.id)
-                except TypeError:
-                    raise MissingError(gettext('ir.msg_sequence_missing'))
-                if _lock:
-                    self.lock()
-                date = Transaction().context.get('date')
-                return '%s%s%s' % (
-                    cls._process(sequence.prefix, date=date),
-                    cls._get_sequence(sequence),
-                    cls._process(sequence.suffix, date=date),
-                    )
+        try:
+            sequence = cls(self.id)
+        except TypeError:
+            raise MissingError(gettext('ir.msg_sequence_missing'))
+        if _lock:
+            self.lock()
+        date = Transaction().context.get('date')
+        return '%s%s%s' % (
+            cls._process(sequence.prefix, date=date),
+            cls._get_sequence(sequence),
+            cls._process(sequence.suffix, date=date),
+            )
 
 
 class SequenceStrict(Sequence):
     "Sequence Strict"
     __name__ = 'ir.sequence.strict'
     _table = None  # Needed to reset Sequence._table
     _strict = True
```

### Comparing `trytond-6.6.8/trytond/ir/sequence.xml` & `trytond-6.8.0/trytond/ir/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/session.py` & `trytond-6.8.0/trytond/ir/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     _session_reset_cache = Cache('ir_session.session_reset', context=False)
 
     @classmethod
     def __setup__(cls):
         super(Session, cls).__setup__()
         table = cls.__table__()
         cls.__rpc__ = {}
-        cls.__rpc__ = {}
         cls._sql_indexes.update({
                 Index(table,
                     (table.key, Index.Equality()),
                     (table.create_uid, Index.Equality())),
                 Index(table,
                     (table.key, Index.Equality()),
                     (table.create_date, Index.Equality())),
```

### Comparing `trytond-6.6.8/trytond/ir/translation.py` & `trytond-6.8.0/trytond/ir/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, fields
 from trytond.pool import Pool
 from trytond.pyson import Eval, PYSONEncoder
 from trytond.tools import cursor_dict, file_open, grouped_slice
 from trytond.tools.string_ import LazyString, StringPartitioned
-from trytond.transaction import Transaction
+from trytond.transaction import (
+    Transaction, inactive_records, without_check_access)
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .lang import get_parent_language as get_parent
 
 TRANSLATION_TYPE = [
     ('field', 'Field'),
     ('model', 'Model'),
     ('report', 'Report'),
     ('selection', 'Selection'),
     ('view', 'View'),
     ('wizard_button', 'Wizard Button'),
     ('help', 'Help'),
 ]
+INTERNAL_LANG = 'en'
 
 
 class OverriddenError(UserError):
     pass
 
 
 class TrytonPOFile(polib.POFile):
@@ -65,16 +67,15 @@
     src = fields.Text('Source')
     value = fields.Text('Translation Value')
     module = fields.Char('Module', readonly=True)
     fuzzy = fields.Boolean('Fuzzy')
     model = fields.Function(fields.Char('Model'), 'get_model',
             searcher='search_model')
     overriding_module = fields.Char('Overriding Module', readonly=True)
-    _translation_cache = Cache('ir.translation', size_limit=10240,
-        context=False)
+    _translation_cache = Cache('ir.translation', context=False)
     _translation_report_cache = Cache(
         'ir.translation.get_report', context=False)
     _get_language_cache = Cache('ir.translation.get_language', context=False)
 
     @classmethod
     def __setup__(cls):
         cls.name.search_unaccented = False
@@ -135,15 +136,15 @@
             return
 
         name = model.__name__ + ',name'
         src = model._get_name()
         if not src:
             return
         cursor.execute(*ir_translation.select(ir_translation.id,
-                where=(ir_translation.lang == 'en')
+                where=(ir_translation.lang == INTERNAL_LANG)
                 & (ir_translation.type == 'model')
                 & (ir_translation.name == name)
                 # Keep searching on all values for migration
                 & ((ir_translation.res_id == -1)
                     | (ir_translation.res_id == Null)
                     | (ir_translation.res_id == 0))))
         trans_id = None
@@ -154,15 +155,16 @@
         elif cursor.rowcount != 0:
             trans_id, = cursor.fetchone()
         if trans_id is None:
             cursor.execute(*ir_translation.insert(
                     [Column(ir_translation, c)
                         for c in ('name', 'lang', 'type', 'src',
                             'value', 'module', 'fuzzy', 'res_id')],
-                    [[name, 'en', 'model', src,
+                    [[
+                            name, INTERNAL_LANG, 'model', src,
                             '', module_name, False, -1]]))
         else:
             cursor.execute(*ir_translation.update(
                     [ir_translation.src],
                     [src],
                     where=ir_translation.id == trans_id))
 
@@ -177,15 +179,15 @@
             help=defaultdict(dict),
             selection=defaultdict(dict))
         if model._fields:
             names = ['%s,%s' % (model.__name__, f) for f in model._fields]
             cursor.execute(*ir_translation.select(ir_translation.id,
                     ir_translation.name, ir_translation.src,
                     ir_translation.type,
-                    where=((ir_translation.lang == 'en')
+                    where=((ir_translation.lang == INTERNAL_LANG)
                         & ir_translation.type.in_(
                             ('field', 'help', 'selection'))
                         & ir_translation.name.in_(names))))
             for trans in cursor_dict(cursor):
                 sources = translations[trans['type']][trans['name']]
                 sources[trans['src']] = trans
 
@@ -201,15 +203,17 @@
                 if isinstance(val, LazyString):
                     continue
                 assert type not in {'field', 'help'} or not inserted, (
                     "More than one resource "
                     f"for {type} of {name} in {module_name}")
                 cursor.execute(
                     *ir_translation.insert(columns,
-                        [[name, 'en', type, val, '', module_name, False, -1]]))
+                        [[
+                                name, INTERNAL_LANG, type, val,
+                                '', module_name, False, -1]]))
                 inserted = True
 
         for field_name, field in model._fields.items():
             name = model.__name__ + ',' + field_name
             insert(field, 'field', name, field.string)
             insert(field, 'help', name, field.help)
             if (hasattr(field, 'selection')
@@ -222,15 +226,15 @@
     def register_wizard(cls, wizard, module_name):
         cursor = Transaction().connection.cursor()
         ir_translation = cls.__table__()
 
         # Prefetch button translations
         cursor.execute(*ir_translation.select(
                 ir_translation.id, ir_translation.name, ir_translation.src,
-                where=((ir_translation.lang == 'en')
+                where=((ir_translation.lang == INTERNAL_LANG)
                     & (ir_translation.type == 'wizard_button')
                     & (ir_translation.name.like(wizard.__name__ + ',%')))))
         trans_buttons = {t['name']: t for t in cursor_dict(cursor)}
 
         def update_insert_button(state_name, button):
             if not button.string:
                 return
@@ -239,15 +243,15 @@
             if trans_name not in trans_buttons:
                 cursor.execute(*ir_translation.insert(
                         [ir_translation.name, ir_translation.lang,
                             ir_translation.type, ir_translation.src,
                             ir_translation.value, ir_translation.module,
                             ir_translation.fuzzy, ir_translation.res_id],
                         [[
-                                trans_name, 'en',
+                                trans_name, INTERNAL_LANG,
                                 'wizard_button', button.string,
                                 '', module_name,
                                 False, -1]]))
             elif trans_buttons[trans_name] != button.string:
                 cursor.execute(*ir_translation.update(
                         [ir_translation.src],
                         [button.string],
@@ -310,38 +314,38 @@
         return result
 
     @classmethod
     def view_attributes(cls):
         return [('/form//field[@name="value"]', 'spell', Eval('lang'))]
 
     @classmethod
+    @without_check_access
     def get_ids(cls, name, ttype, lang, ids, cached_after=None):
         "Return translation for each id"
         pool = Pool()
         ModelFields = pool.get('ir.model.field')
         Model = pool.get('ir.model')
         context = Transaction().context
         fuzzy_translation = context.get('fuzzy_translation', False)
 
         translations, to_fetch = {}, []
         name = str(name)
         ttype = str(ttype)
         lang = str(lang)
         if name.split(',')[0] in ('ir.model.field', 'ir.model'):
             field_name = name.split(',')[1]
-            with Transaction().set_context(_check_access=False):
-                if name.split(',')[0] == 'ir.model.field':
-                    if field_name == 'field_description':
-                        ttype = 'field'
-                    else:
-                        ttype = 'help'
-                    records = ModelFields.browse(ids)
+            if name.split(',')[0] == 'ir.model.field':
+                if field_name == 'field_description':
+                    ttype = 'field'
                 else:
-                    ttype = 'model'
-                    records = Model.browse(ids)
+                    ttype = 'help'
+                records = ModelFields.browse(ids)
+            else:
+                ttype = 'model'
+                records = Model.browse(ids)
 
             trans_args = []
             for record in records:
                 if ttype in ('field', 'help'):
                     name = record.model.model + ',' + record.name
                 else:
                     name = record.model + ',' + field_name
@@ -422,14 +426,15 @@
                 for res_id in to_fetch:
                     value = translations.setdefault(res_id)
                     cls._translation_cache.set(
                         (name, ttype, lang, res_id), value)
         return translations
 
     @classmethod
+    @without_check_access
     def set_ids(cls, name, ttype, lang, ids, values):
         "Set translation for each id"
         pool = Pool()
         ModelFields = pool.get('ir.model.field')
         Model = pool.get('ir.model')
         Config = pool.get('ir.configuration')
         transaction = Transaction()
@@ -445,126 +450,124 @@
         model_name, field_name = name.split(',')
         if model_name in ('ir.model.field', 'ir.model'):
             if model_name == 'ir.model.field':
                 if field_name == 'field_description':
                     ttype = 'field'
                 else:
                     ttype = 'help'
-                with Transaction().set_context(language='en'):
+                with Transaction().set_context(language=INTERNAL_LANG):
                     records = ModelFields.browse(ids)
             else:
                 ttype = 'model'
-                with Transaction().set_context(language='en'):
+                with Transaction().set_context(language=INTERNAL_LANG):
                     records = Model.browse(ids)
 
             def get_name(record):
                 if ttype in ('field', 'help'):
                     return record.model.model + ',' + record.name
                 else:
                     return record.model + ',' + field_name
 
-            with Transaction().set_context(_check_access=False):
-                name2translations = defaultdict(list)
-                for translation in cls.search([
-                            ('lang', '=', lang),
-                            ('type', '=', ttype),
-                            ('name', 'in', [get_name(r) for r in records]),
-                            ]):
-                    name2translations[translation.name].append(translation)
-
-                to_save = []
-                for record, value in zip(records, values):
-                    translations = name2translations.get(get_name(record))
-                    if lang == 'en':
-                        src = value
-                    else:
-                        src = getattr(record, field_name)
-                    if not translations:
-                        if not src and not value:
-                            continue
-                        translation = cls()
-                        translation.name = name
-                        translation.lang = lang
-                        translation.type = ttype
-                        translations.append(translation)
-                    for translation in translations:
-                        translation.src = src
-                        translation.value = value
-                        translation.fuzzy = False
-                        to_save.append(translation)
-                cls.save(to_save)
-            return
-
-        Model = pool.get(model_name)
-        with Transaction().set_context(language=Config.get_language()):
-            records = Model.browse(ids)
-
-        id2translations = defaultdict(list)
-        other_translations = defaultdict(list)
-        with Transaction().set_context(_check_access=False):
+            name2translations = defaultdict(list)
             for translation in cls.search([
                         ('lang', '=', lang),
                         ('type', '=', ttype),
-                        ('name', '=', name),
-                        ('res_id', 'in', ids),
+                        ('name', 'in', [get_name(r) for r in records]),
                         ]):
-                id2translations[translation.res_id].append(translation)
-
-            if (lang == Config.get_language()
-                    and Transaction().context.get('fuzzy_translation', True)):
-                for translation in cls.search([
-                            ('lang', '!=', lang),
-                            ('type', '=', ttype),
-                            ('name', '=', name),
-                            ('res_id', 'in', ids),
-                            ]):
-                    other_translations[translation.res_id].append(translation)
+                name2translations[translation.name].append(translation)
 
             to_save = []
             for record, value in zip(records, values):
-                translations = id2translations[record.id]
-                if lang == Config.get_language():
+                translations = name2translations.get(get_name(record))
+                if lang == INTERNAL_LANG:
                     src = value
                 else:
                     src = getattr(record, field_name)
                 if not translations:
                     if not src and not value:
                         continue
                     translation = cls()
                     translation.name = name
                     translation.lang = lang
                     translation.type = ttype
-                    translation.res_id = record.id
                     translations.append(translation)
-                else:
-                    other_langs = other_translations[record.id]
-                    if other_langs:
-                        for other_lang in other_langs:
-                            other_lang.src = src
-                            other_lang.fuzzy = True
-                            to_save.append(other_lang)
                 for translation in translations:
-                    translation.value = value
                     translation.src = src
+                    translation.value = value
                     translation.fuzzy = False
                     to_save.append(translation)
             cls.save(to_save)
+            return
+
+        Model = pool.get(model_name)
+        with Transaction().set_context(language=Config.get_language()):
+            records = Model.browse(ids)
+
+        id2translations = defaultdict(list)
+        other_translations = defaultdict(list)
+        for translation in cls.search([
+                    ('lang', '=', lang),
+                    ('type', '=', ttype),
+                    ('name', '=', name),
+                    ('res_id', 'in', ids),
+                    ]):
+            id2translations[translation.res_id].append(translation)
+
+        if (lang == Config.get_language()
+                and Transaction().context.get('fuzzy_translation', True)):
+            for translation in cls.search([
+                        ('lang', '!=', lang),
+                        ('type', '=', ttype),
+                        ('name', '=', name),
+                        ('res_id', 'in', ids),
+                        ]):
+                other_translations[translation.res_id].append(translation)
+
+        to_save = []
+        for record, value in zip(records, values):
+            translations = id2translations[record.id]
+            if lang == Config.get_language():
+                src = value
+            else:
+                src = getattr(record, field_name)
+            if not translations:
+                if not src and not value:
+                    continue
+                translation = cls()
+                translation.name = name
+                translation.lang = lang
+                translation.type = ttype
+                translation.res_id = record.id
+                translations.append(translation)
+            else:
+                other_langs = other_translations[record.id]
+                if other_langs:
+                    for other_lang in other_langs:
+                        other_lang.src = src
+                        other_lang.fuzzy = True
+                        to_save.append(other_lang)
+            for translation in translations:
+                translation.value = value
+                translation.src = src
+                translation.fuzzy = False
+                to_save.append(translation)
+        cls.save(to_save)
 
     @classmethod
+    @without_check_access
     def delete_ids(cls, model, ttype, ids):
         "Delete translation for each id"
         translations = []
-        with Transaction().set_context(_check_access=False):
-            for sub_ids in grouped_slice(ids):
-                translations += cls.search([
-                        ('type', '=', ttype),
-                        ('name', 'like', model + ',%'),
-                        ('res_id', 'in', list(sub_ids)),
-                        ])
-            cls.delete(translations)
+        for sub_ids in grouped_slice(ids):
+            translations += cls.search([
+                    ('type', '=', ttype),
+                    ('name', 'like', model + ',%'),
+                    ('res_id', 'in', list(sub_ids)),
+                    ])
+        cls.delete(translations)
 
     @classmethod
     def get_source(cls, name, ttype, lang, source=None):
         "Return translation for source"
         args = (name, ttype, lang, source)
         result = cls.get_sources([args])
         return result[args]
@@ -1031,24 +1034,24 @@
         factories.get('markup', factories.get('xml')))
     extract_report_html = extract_report_genshi(
         factories.get('markup', factories.get('xml')))
     extract_report_xhtml = extract_report_genshi(
         factories.get('markup', factories.get('xml')))
     del factories
 
+    @inactive_records
     def set_report(self):
         pool = Pool()
         Report = pool.get('ir.action.report')
         Translation = pool.get('ir.translation')
 
         if self.model == Report:
             reports = self.records
         elif not self.model or self.model.__name__ == 'ir.ui.menu':
-            with Transaction().set_context(active_test=False):
-                reports = Report.search([('translatable', '=', True)])
+            reports = Report.search([('translatable', '=', True)])
         else:
             return
 
         cursor = Transaction().connection.cursor()
         translation = Translation.__table__()
         report_strings = defaultdict(set)
         for report in reports:
@@ -1061,15 +1064,15 @@
                     (report.report_content_custom, None),
                     (content, report.module)]:
                 if not content:
                     continue
 
                 cursor.execute(*translation.select(
                         translation.id, translation.name, translation.src,
-                        where=(translation.lang == 'en')
+                        where=(translation.lang == INTERNAL_LANG)
                         & (translation.type == 'report')
                         & (translation.name == report.report_name)
                         & (translation.module == module)))
                 trans_reports = {t['src']: t for t in cursor_dict(cursor)}
 
                 strings = report_strings[report.report_name, report.module]
                 func_name = 'extract_report_%s' % report.template_extension
@@ -1104,15 +1107,15 @@
                     if not done:
                         cursor.execute(*translation.insert(
                                 [translation.name, translation.lang,
                                     translation.type, translation.src,
                                     translation.value, translation.module,
                                     translation.fuzzy, translation.res_id],
                                 [[
-                                        report.report_name, 'en',
+                                        report.report_name, INTERNAL_LANG,
                                         'report', string,
                                         '', module,
                                         False, -1]]))
         for (report_name, module), strings in report_strings.items():
             query = translation.delete(
                 where=(translation.name == report_name)
                 & (translation.type == 'report')
@@ -1128,50 +1131,49 @@
                 string = element.get(attr)
                 if string:
                     strings.append(string)
         for child in element:
             strings.extend(self._translate_view(child))
         return strings
 
+    @inactive_records
     def set_view(self):
         pool = Pool()
         View = pool.get('ir.ui.view')
         Translation = pool.get('ir.translation')
 
         if self.model == View:
             views = self.records
         elif not self.model or self.model.__name__ == 'ir.ui.menu':
-            with Transaction().set_context(active_test=False):
-                views = View.search([])
+            views = View.search([])
         else:
             return
 
         cursor = Transaction().connection.cursor()
         translation = Translation.__table__()
         for view in views:
             cursor.execute(*translation.select(
                     translation.id, translation.name, translation.src,
-                    where=(translation.lang == 'en')
+                    where=(translation.lang == INTERNAL_LANG)
                     & (translation.type == 'view')
                     & (translation.name == view.model)
                     & (translation.module == view.module)))
             trans_views = {t['src']: t for t in cursor_dict(cursor)}
 
             xml = (view.arch or '').strip()
             if not xml:
                 continue
             tree = etree.fromstring(xml)
             root_element = tree.getroottree().getroot()
             strings = self._translate_view(root_element)
-            with Transaction().set_context(active_test=False):
-                views2 = View.search([
-                    ('model', '=', view.model),
-                    ('id', '!=', view.id),
-                    ('module', '=', view.module),
-                    ])
+            views2 = View.search([
+                ('model', '=', view.model),
+                ('id', '!=', view.id),
+                ('module', '=', view.module),
+                ])
             for view2 in views2:
                 xml2 = view2.arch
                 if not xml2:
                     continue
                 tree2 = etree.fromstring(xml2)
                 root2_element = tree2.getroottree().getroot()
                 strings += self._translate_view(root2_element)
@@ -1204,15 +1206,15 @@
                 if not done:
                     cursor.execute(*translation.insert(
                             [translation.name, translation.lang,
                                 translation.type, translation.src,
                                 translation.value, translation.module,
                                 translation.fuzzy, translation.res_id],
                             [[
-                                    view.model, 'en',
+                                    view.model, INTERNAL_LANG,
                                     'view', string,
                                     '', view.module,
                                     False, -1]]))
             if strings:
                 cursor.execute(*translation.delete(
                         where=(translation.name == view.model)
                         & (translation.type == 'view')
@@ -1285,23 +1287,23 @@
             if (not hasattr(field, 'translate')
                     or not field.translate):
                 return True
         elif field_name not in ('name'):
             return True
 
     @staticmethod
+    @inactive_records
     def _clean_report(translation):
         pool = Pool()
         Report = pool.get('ir.action.report')
-        with Transaction().set_context(active_test=False):
-            if not Report.search([
-                        ('report_name', '=', translation.name),
-                        ('translatable', '=', True),
-                        ]):
-                return True
+        if not Report.search([
+                    ('report_name', '=', translation.name),
+                    ('translatable', '=', True),
+                    ]):
+            return True
 
     @staticmethod
     def _clean_selection(translation):
         pool = Pool()
         try:
             model_name, field_name = translation.name.split(',', 1)
         except ValueError:
@@ -1372,27 +1374,41 @@
 
     def transition_clean(self):
         pool = Pool()
         Translation = pool.get('ir.translation')
         ModelData = pool.get('ir.model.data')
 
         to_delete = []
+        records = defaultdict(lambda: defaultdict(set))
         keys = set()
         translations = Translation.search([])
         for translation in translations:
             if getattr(self, '_clean_%s' % translation.type)(translation):
                 to_delete.append(translation.id)
             elif translation.type in ('field', 'model', 'wizard_button',
                     'help'):
                 key = (translation.module, translation.lang, translation.type,
                     translation.name, translation.res_id)
                 if key in keys:
                     to_delete.append(translation.id)
                 else:
                     keys.add(key)
+                if translation.type == 'model' and translation.res_id >= 0:
+                    model_name, _ = translation.name.split(',', 1)
+                    records[model_name][translation.res_id].add(translation.id)
+
+        with inactive_records():
+            for model_name, translations in records.items():
+                Model = pool.get(model_name)
+                for sub_ids in grouped_slice(translations.keys()):
+                    sub_ids = list(sub_ids)
+                    records = Model.search([('id', 'in', sub_ids)])
+                    for record_id in set(sub_ids) - set(map(int, records)):
+                        to_delete.extend(translations[record_id])
+
         # skip translation handled in ir.model.data
         models_data = ModelData.search([
             ('db_id', 'in', to_delete),
             ('model', '=', 'ir.translation'),
             ])
         for mdata in models_data:
             if mdata.db_id in to_delete:
@@ -1440,14 +1456,15 @@
 
     @staticmethod
     def transition_update():
         return 'end'
 
     def do_update(self, action):
         pool = Pool()
+        Config = pool.get('ir.configuration')
         Translation = pool.get('ir.translation')
         Report = pool.get('ir.action.report')
         View = pool.get('ir.ui.view')
         cursor = Transaction().connection.cursor()
         cursor_update = Transaction().connection.cursor()
         translation = Translation.__table__()
         lang = self.start.language.code
@@ -1459,20 +1476,21 @@
                 & translation.name.in_([r.report_name for r in reports]))
         elif self.model == View:
             views = self.records
             source_clause = ((translation.type == 'view')
                 & translation.name.in_([v.model for v in views]))
         else:
             source_clause = Literal(True)
+        default_lang = Config.get_language()
 
         columns = [translation.name.as_('name'),
             translation.res_id.as_('res_id'), translation.type.as_('type'),
             translation.src.as_('src'), translation.module.as_('module')]
         cursor.execute(*(translation.select(*columns,
-                    where=(translation.lang == 'en')
+                    where=(translation.lang == default_lang)
                     & source_clause
                     & translation.type.in_(self._source_types))
                 - translation.select(*columns,
                     where=(translation.lang == lang)
                     & source_clause
                     & translation.type.in_(self._source_types))))
         to_create = []
@@ -1512,15 +1530,15 @@
         if self.model in {Report, View}:
             return
 
         columns = [translation.name.as_('name'),
             translation.res_id.as_('res_id'), translation.type.as_('type'),
             translation.module.as_('module')]
         cursor.execute(*(translation.select(*columns,
-                    where=(translation.lang == 'en')
+                    where=(translation.lang == default_lang)
                     & translation.type.in_(self._ressource_types))
                 - translation.select(*columns,
                     where=(translation.lang == lang)
                     & translation.type.in_(self._ressource_types))))
         to_create = []
         for row in cursor_dict(cursor):
             to_create.append({
@@ -1551,15 +1569,15 @@
                         & (translation.module == row['module'])
                         & (translation.lang == lang)))
 
         columns = [translation.name.as_('name'),
             translation.res_id.as_('res_id'), translation.type.as_('type'),
             translation.src.as_('src'), translation.module.as_('module')]
         cursor.execute(*(translation.select(*columns,
-                    where=(translation.lang == 'en')
+                    where=(translation.lang == default_lang)
                     & translation.type.in_(self._updatable_types))
                 - translation.select(*columns,
                     where=(translation.lang == lang)
                     & translation.type.in_(self._updatable_types))))
         for row in cursor_dict(cursor):
             cursor_update.execute(*translation.update(
                     [translation.fuzzy, translation.src],
@@ -1574,15 +1592,17 @@
                 translation.src.as_('src'),
                 Max(translation.value).as_('value'),
                 where=(translation.lang == lang)
                 & translation.src.in_(
                     translation.select(translation.src,
                         where=((translation.value == '')
                             | (translation.value == Null))
-                        & (translation.lang == lang)))
+                        & (translation.lang == lang)
+                        & (translation.src != '')
+                        & (translation.src != Null)))
                 & (translation.value != '')
                 & (translation.value != Null),
                 group_by=translation.src))
 
         for row in cursor_dict(cursor):
             cursor_update.execute(*translation.update(
                     [translation.fuzzy, translation.value],
@@ -1607,15 +1627,15 @@
 class TranslationExportStart(ModelView):
     "Export translation"
     __name__ = 'ir.translation.export.start'
 
     language = fields.Many2One('ir.lang', 'Language', required=True,
         domain=[
             ('translatable', '=', True),
-            ('code', '!=', 'en'),
+            ('code', '!=', INTERNAL_LANG),
             ])
     module = fields.Many2One('ir.module', 'Module', required=True,
         domain=[
             ('state', 'in', ['activated', 'to upgrade', 'to remove']),
             ])
 
     @classmethod
```

### Comparing `trytond-6.6.8/trytond/ir/translation.xml` & `trytond-6.8.0/trytond/ir/translation.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/trigger.py` & `trytond-6.8.0/trytond/ir/trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from trytond.cache import Cache
 from trytond.i18n import gettext
 from trytond.model import (
     Check, DeactivableMixin, EvalEnvironment, Index, ModelSQL, ModelView,
     fields)
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
-from trytond.pyson import Eval, PYSONDecoder
+from trytond.pyson import Eval, PYSONDecoder, TimeDelta
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.transaction import Transaction
 
 
 class ConditionError(ValidationError):
     pass
 
@@ -45,15 +45,20 @@
         }, depends=['on_time'])
     condition = fields.Char('Condition', required=True,
         help='A PYSON statement evaluated with record represented by '
         '"self"\nIt triggers the action if true.')
     limit_number = fields.Integer('Limit Number', required=True,
         help='Limit the number of call to "Action Function" by records.\n'
         '0 for no limit.')
-    minimum_time_delay = fields.TimeDelta('Minimum Delay',
+    minimum_time_delay = fields.TimeDelta(
+        "Minimum Delay",
+        domain=['OR',
+            ('minimum_time_delay', '=', None),
+            ('minimum_time_delay', '>=', TimeDelta()),
+            ],
         help='Set a minimum time delay between call to "Action Function" '
         'for the same record.\n'
         'empty for no delay.')
     action = fields.Selection([], "Action", required=True)
     _get_triggers_cache = Cache('ir_trigger.get_triggers')
 
     @classmethod
@@ -313,14 +318,15 @@
     trigger = fields.Many2One(
         'ir.trigger', 'Trigger', required=True, ondelete='CASCADE')
     record_id = fields.Integer('Record ID', required=True)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
+        cls.__access__.add('trigger')
 
         table = cls.__table__()
         cls._sql_indexes.add(
             Index(
                 table,
                 (table.trigger, Index.Equality()),
                 (table.record_id, Index.Range())))
```

### Comparing `trytond-6.6.8/trytond/ir/trigger.xml` & `trytond-6.8.0/trytond/ir/trigger.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/board.rnc` & `trytond-6.8.0/trytond/ir/ui/board.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/board.rng` & `trytond-6.8.0/trytond/ir/ui/board.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/calendar.rnc` & `trytond-6.8.0/trytond/ir/ui/calendar.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/calendar.rng` & `trytond-6.8.0/trytond/ir/ui/calendar.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/form.rnc` & `trytond-6.8.0/trytond/ir/ui/form.rnc`

 * *Files 1% similar despite different names*

```diff
@@ -113,18 +113,20 @@
 attlist.field &= [a:defaultValue = "1"] attribute factor { text }?
 attlist.field &= attribute filename { text }?
 attlist.field &= attribute help_field { text }?
 attlist.field &=
   [a:defaultValue = "0"] attribute toolbar { "0" | "1" }?
 attlist.field &= attribute symbol { text }?
 attlist.field &= [a:defaultValue = "1"] attribute grouping { "0" | "1" }?
+attlist.field &= [a:defaultValue = "square"] attribute border { "square" | "circle" | "rounded" }?
 image = element image { attlist.image, empty }
 attlist.image &= attribute name { text }
 attlist.image &= [a:defaultValue = "icon"] attribute type { "icon" | "url" }?
 attlist.image &= attribute url_size { text }?
+attlist.image &= [a:defaultValue = "square"] attribute border { "square" | "circle" | "rounded" }?
 attlist.image &= [ a:defaultValue = "1" ] attribute colspan { text }?
 attlist.image &=
   [ a:defaultValue = "0" ] attribute yexpand { "0" | "1" }?
 attlist.image &= [ a:defaultValue = "0" ] attribute yfill { "0" | "1" }?
 attlist.image &=
   [ a:defaultValue = "1" ] attribute xexpand { "0" | "1" }?
 attlist.image &=
```

### Comparing `trytond-6.6.8/trytond/ir/ui/form.rng` & `trytond-6.8.0/trytond/ir/ui/form.rng`

 * *Files 1% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/ir/ui/form.rng` & `trytond-6.8.0/trytond/ir/ui/form.rng`

```diff
@@ -532,14 +532,26 @@
         <choice>
           <value>0</value>
           <value>1</value>
         </choice>
       </attribute>
     </optional>
   </define>
+  <define name="attlist.field" combine="interleave">
+    <optional>
+      <attribute a:defaultValue="square">
+        <name ns="">border</name>
+        <choice>
+          <value>square</value>
+          <value>circle</value>
+          <value>rounded</value>
+        </choice>
+      </attribute>
+    </optional>
+  </define>
   <define name="image">
     <element>
       <name ns="">image</name>
       <ref name="attlist.image"/>
       <empty/>
     </element>
   </define>
@@ -566,14 +578,26 @@
         <name ns="">url_size</name>
         <text/>
       </attribute>
     </optional>
   </define>
   <define name="attlist.image" combine="interleave">
     <optional>
+      <attribute a:defaultValue="square">
+        <name ns="">border</name>
+        <choice>
+          <value>square</value>
+          <value>circle</value>
+          <value>rounded</value>
+        </choice>
+      </attribute>
+    </optional>
+  </define>
+  <define name="attlist.image" combine="interleave">
+    <optional>
       <attribute a:defaultValue="1">
         <name ns="">colspan</name>
         <text/>
       </attribute>
     </optional>
   </define>
   <define name="attlist.image" combine="interleave">
```

### Comparing `trytond-6.6.8/trytond/ir/ui/graph.rnc` & `trytond-6.8.0/trytond/ir/ui/graph.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/graph.rng` & `trytond-6.8.0/trytond/ir/ui/graph.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/icon.py` & `trytond-6.8.0/trytond/ir/ui/icon.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/icon.xml` & `trytond-6.8.0/trytond/ir/ui/icon.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/icons/LICENSE` & `trytond-6.8.0/trytond/ir/ui/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/icons/tryton-settings.svg` & `trytond-6.8.0/trytond/ir/ui/icons/tryton-settings.svg`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/menu.py` & `trytond-6.8.0/trytond/ir/ui/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from itertools import groupby
 
 from trytond.model import (
     DeactivableMixin, ModelSQL, ModelView, fields, sequence_ordered, tree)
 from trytond.pool import Pool
 from trytond.rpc import RPC
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 
 def one_in(i, j):
     """Check the presence of an element of setA in setB
     """
     for k in i:
         if k in j:
@@ -149,19 +149,19 @@
                     if (x.parent and x.parent in parents) or not x.parent])
 
         if count:
             return len(menus)
         return menus
 
     @classmethod
+    @inactive_records
     def get_action(cls, menus, name):
         pool = Pool()
         actions = dict((m.id, None) for m in menus)
-        with Transaction().set_context(active_test=False):
-            menus = cls.browse(menus)
+        menus = cls.browse(menus)
         action_keywords = sum((list(m.action_keywords) for m in menus), [])
 
         def action_type(keyword):
             return keyword.action.type
         action_keywords.sort(key=action_type)
         for type, action_keywords in groupby(action_keywords, key=action_type):
             action_keywords = list(action_keywords)
@@ -169,18 +169,17 @@
             for action_keyword in action_keywords:
                 model = action_keyword.model
                 actions[model.id] = '%s,-1' % type
                 action2keywords[action_keyword.action.id].append(
                     action_keyword)
 
             Action = pool.get(type)
-            with Transaction().set_context(active_test=False):
-                factions = Action.search([
-                        ('action', 'in', list(action2keywords.keys())),
-                        ])
+            factions = Action.search([
+                    ('action', 'in', list(action2keywords.keys())),
+                    ])
             for action in factions:
                 for action_keyword in action2keywords[action.id]:
                     actions[action_keyword.model.id] = str(action)
         return actions
 
     @classmethod
     def set_action(cls, menus, name, value):
```

### Comparing `trytond-6.6.8/trytond/ir/ui/menu.xml` & `trytond-6.8.0/trytond/ir/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/tree.rnc` & `trytond-6.8.0/trytond/ir/ui/tree.rnc`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 prefix = element prefix { attlist.affix, empty }
 suffix = element suffix { attlist.affix, empty }
 attlist.affix &= attribute string { text }?
 attlist.affix &= ( attribute name { text } | attribute id { text } )
 attlist.affix &= attribute icon { text }?
 attlist.affix &= [a:defaultValue = "icon"] attribute icon_type { "icon" | "url" }?
 attlist.affix &= attribute url_size { text }?
+attlist.affix &= [a:defaultValue = "square"] attribute border { "square" | "circle" | "rounded" }?
 button = element button { attlist.button, empty }
 attlist.button &= attribute help { text }?
 attlist.button &= attribute string { text }?
 attlist.button &= attribute confirm { text }?
 attlist.button &= attribute name { text }
 attlist.button &= attribute states { text }?
 attlist.button &=
```

### Comparing `trytond-6.6.8/trytond/ir/ui/tree.rng` & `trytond-6.8.0/trytond/ir/ui/tree.rng`

 * *Files 1% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/ir/ui/tree.rng` & `trytond-6.8.0/trytond/ir/ui/tree.rng`

```diff
@@ -382,14 +382,26 @@
     <optional>
       <attribute>
         <name ns="">url_size</name>
         <text/>
       </attribute>
     </optional>
   </define>
+  <define name="attlist.affix" combine="interleave">
+    <optional>
+      <attribute a:defaultValue="square">
+        <name ns="">border</name>
+        <choice>
+          <value>square</value>
+          <value>circle</value>
+          <value>rounded</value>
+        </choice>
+      </attribute>
+    </optional>
+  </define>
   <define name="button">
     <element>
       <name ns="">button</name>
       <ref name="attlist.button"/>
       <empty/>
     </element>
   </define>
```

### Comparing `trytond-6.6.8/trytond/ir/ui/ui.xml` & `trytond-6.8.0/trytond/ir/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/ui/view.py` & `trytond-6.8.0/trytond/ir/ui/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         cls._view_get_cache.clear()
         ModelView._fields_view_get_cache.clear()
 
     @property
     def _module_index(self):
         from trytond.modules import create_graph, get_module_list
         if self.__class__.__module_index is None:
-            graph = create_graph(get_module_list())
+            graph = create_graph(get_module_list(with_test=Pool.test))
             modules = [m.name for m in graph]
             self.__class__.__module_index = {
                 m: i for i, m in enumerate(reversed(modules))}
         return self.__class__.__module_index
 
     def view_get(self, model=None):
         key = (self.id, model)
```

### Comparing `trytond-6.6.8/trytond/ir/ui/view.xml` & `trytond-6.8.0/trytond/ir/ui/view.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/action_act_window_domain_form.xml` & `trytond-6.8.0/trytond/ir/view/action_act_window_domain_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/action_act_window_form.xml` & `trytond-6.8.0/trytond/ir/view/action_act_window_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/action_form.xml` & `trytond-6.8.0/trytond/ir/view/action_form.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/ir/view/action_form.xml` & `trytond-6.8.0/trytond/ir/view/action_form.xml`

```diff
@@ -4,14 +4,16 @@
 <form>
   <label name="name"/>
   <field name="name"/>
   <label name="active"/>
   <field name="active" xexpand="0" width="100"/>
   <notebook colspan="4">
     <page string="General" id="general">
+      <label name="type"/>
+      <field name="type"/>
       <label name="records"/>
       <field name="records"/>
       <label name="usage"/>
       <field name="usage"/>
       <label name="icon"/>
       <field name="icon"/>
     </page>
```

### Comparing `trytond-6.6.8/trytond/ir/view/action_report_form.xml` & `trytond-6.8.0/trytond/ir/view/action_report_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/action_url_form.xml` & `trytond-6.8.0/trytond/ir/view/action_url_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/action_wizard_form.xml` & `trytond-6.8.0/trytond/ir/view/action_wizard_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/attachment_form.xml` & `trytond-6.8.0/trytond/ir/view/attachment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/attachment_list.xml` & `trytond-6.8.0/trytond/ir/view/attachment_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/cron_form.xml` & `trytond-6.8.0/trytond/ir/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/cron_list.xml` & `trytond-6.8.0/trytond/ir/view/cron_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/email_form.xml` & `trytond-6.8.0/trytond/ir/view/email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/email_template_form.xml` & `trytond-6.8.0/trytond/ir/view/email_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/error_form.xml` & `trytond-6.8.0/trytond/ir/view/error_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/lang_form.xml` & `trytond-6.8.0/trytond/ir/view/lang_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_access_form.xml` & `trytond-6.8.0/trytond/ir/view/model_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_button_form.xml` & `trytond-6.8.0/trytond/ir/view/model_button_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_button_rule_form.xml` & `trytond-6.8.0/trytond/ir/view/model_button_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_data_form.xml` & `trytond-6.8.0/trytond/ir/view/model_data_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_field_access_form.xml` & `trytond-6.8.0/trytond/ir/view/model_field_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_field_form.xml` & `trytond-6.8.0/trytond/ir/view/model_field_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/model_form.xml` & `trytond-6.8.0/trytond/ir/view/model_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/module_activate_upgrade_start_form.xml` & `trytond-6.8.0/trytond/ir/view/module_activate_upgrade_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/module_form.xml` & `trytond-6.8.0/trytond/ir/view/module_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/module_list.xml` & `trytond-6.8.0/trytond/ir/view/module_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/note_form.xml` & `trytond-6.8.0/trytond/ir/view/note_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/note_list.xml` & `trytond-6.8.0/trytond/ir/view/note_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/rule_group_form.xml` & `trytond-6.8.0/trytond/ir/view/rule_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/sequence_form.xml` & `trytond-6.8.0/trytond/ir/view/sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/translation_form.xml` & `trytond-6.8.0/trytond/ir/view/translation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/translation_list.xml` & `trytond-6.8.0/trytond/ir/view/translation_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/trigger_form.xml` & `trytond-6.8.0/trytond/ir/view/trigger_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/ui_menu_form.xml` & `trytond-6.8.0/trytond/ir/view/ui_menu_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/ui_view_form.xml` & `trytond-6.8.0/trytond/ir/view/ui_view_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/ir/view/ui_view_tree_state_form.xml` & `trytond-6.8.0/trytond/ir/view/ui_view_tree_state_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/__init__.py` & `trytond-6.8.0/trytond/model/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from .avatar import avatar_mixin
 from .descriptors import dualmethod
 from .dictschema import DictSchemaMixin
 from .digits import DigitsMixin
 from .match import MatchMixin
 from .model import Model
 from .modelsingleton import ModelSingleton
-from .modelsql import Check, Exclude, Index, ModelSQL, Unique
+from .modelsql import Check, Exclude, Index, ModelSQL, Unique, convert_from
 from .modelstorage import EvalEnvironment, ModelStorage
 from .modelview import ModelView
 from .multivalue import MultiValueMixin, ValueMixin
-from .order import sequence_ordered
+from .order import sequence_ordered, sort
 from .symbol import SymbolMixin
 from .tree import tree
 from .union import UnionMixin
 from .workflow import Workflow
 
 __all__ = ['Model', 'ModelView', 'ModelStorage', 'ModelSingleton', 'ModelSQL',
-    'Check', 'Unique', 'Exclude', 'Index',
+    'Check', 'Unique', 'Exclude', 'Index', 'convert_from',
     'Workflow', 'DictSchemaMixin', 'MatchMixin', 'UnionMixin', 'dualmethod',
     'MultiValueMixin', 'ValueMixin', 'SymbolMixin', 'DigitsMixin',
-    'EvalEnvironment', 'sequence_ordered', 'DeactivableMixin', 'tree',
+    'EvalEnvironment', 'sequence_ordered', 'sort', 'DeactivableMixin', 'tree',
     'avatar_mixin']
```

### Comparing `trytond-6.6.8/trytond/model/active.py` & `trytond-6.8.0/trytond/model/active.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/avatar.py` & `trytond-6.8.0/trytond/model/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/descriptors.py` & `trytond-6.8.0/trytond/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/dictschema.py` & `trytond-6.8.0/trytond/model/dictschema.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/digits.py` & `trytond-6.8.0/trytond/model/digits.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/exceptions.py` & `trytond-6.8.0/trytond/model/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 from .modelsql import ForeignKeyError, SQLConstraintError
 from .modelstorage import (
     AccessError, DigitsValidationError, DomainValidationError,
     ForbiddenCharValidationError, ImportDataError, RequiredValidationError,
     SelectionValidationError, SizeValidationError, TimeFormatValidationError,
     ValidationError)
-from .modelview import AccessButtonError
+from .modelview import AccessButtonError, ButtonActionException
 from .tree import RecursionError
 
 __all__ = [
     AccessButtonError,
     AccessError,
+    ButtonActionException,
     DigitsValidationError,
     DomainValidationError,
     ForeignKeyError,
     ImportDataError,
     RecursionError,
     RequiredValidationError,
     SQLConstraintError,
```

### Comparing `trytond-6.6.8/trytond/model/fields/__init__.py` & `trytond-6.8.0/trytond/model/fields/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from .binary import Binary
 from .boolean import Boolean
 from .char import Char
 from .date import Date, DateTime, Time, TimeDelta, Timestamp
 from .dict import Dict
 from .field import (
     SQL_OPERATORS, Field, context_validate, depends, domain_validate,
-    get_eval_fields, on_change_result, states_validate, with_inactive_records)
+    get_eval_fields, on_change_result, states_validate)
 from .float import Float
 from .function import Function, MultiValue
-from .integer import BigInteger, Integer
+from .integer import Integer
 from .many2many import Many2Many
 from .many2one import Many2One
 from .multiselection import MultiSelection
 from .numeric import Numeric
 from .one2many import One2Many
 from .one2one import One2One
 from .reference import Reference
 from .selection import Selection
 from .text import FullText, Text
 
 __all__ = [
-    depends, with_inactive_records, SQL_OPERATORS, on_change_result,
+    depends, SQL_OPERATORS, on_change_result,
     get_eval_fields, states_validate, domain_validate, context_validate, Field,
-    Boolean, Integer, BigInteger, Char, Text, FullText, Float, Numeric, Date,
+    Boolean, Integer, Char, Text, FullText, Float, Numeric, Date,
     Timestamp, DateTime, Time, TimeDelta, Binary, Selection, Reference,
     Many2One, One2Many, Many2Many, Function, MultiValue, One2One, Dict,
     MultiSelection]
```

### Comparing `trytond-6.6.8/trytond/model/fields/binary.py` & `trytond-6.8.0/trytond/model/fields/binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/boolean.py` & `trytond-6.8.0/trytond/model/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/char.py` & `trytond-6.8.0/trytond/model/fields/char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/date.py` & `trytond-6.8.0/trytond/model/fields/date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/dict.py` & `trytond-6.8.0/trytond/model/fields/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from trytond import backend
 from trytond.pool import Pool
 from trytond.protocols.jsonrpc import JSONDecoder, JSONEncoder
 from trytond.tools import grouped_slice
 from trytond.tools.immutabledict import ImmutableDict
 from trytond.transaction import Transaction
 
-from .field import SQL_OPERATORS, Field
+from .field import SQL_OPERATORS, Field, domain_method
 
 # Use canonical form
 dumps = partial(
     json.dumps, cls=JSONEncoder, separators=(',', ':'), sort_keys=True,
     ensure_ascii=False)
 
 
@@ -108,14 +108,15 @@
         if value is None and operator.endswith('='):
             if operator == '=':
                 expression |= (column == Null)
             else:
                 expression &= (column != Null)
         return expression
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         name, operator, value = domain[:3]
         if '.' not in name:
             return super().convert_domain(domain, tables, Model)
         database = Transaction().database
         table, _ = tables[None]
         name, key = name.split('.', 1)
```

### Comparing `trytond-6.6.8/trytond/model/fields/field.py` & `trytond-6.8.0/trytond/model/fields/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import warnings
-from functools import wraps
+from functools import partial, wraps
 
 import sql
 from sql import (
     Cast, Column, CombiningQuery, Expression, Literal, Null, Query, Select,
     operators)
 from sql.aggregate import Min
 from sql.conditionals import Coalesce, NullIf
@@ -138,15 +138,17 @@
     elif isinstance(value, dict):
         for val in value.values():
             yield from _iter_eval_fields(val)
 
 
 def get_eval_fields(value):
     "Return fields evaluated"
-    return set(_iter_eval_fields(value))
+    fields = set(_iter_eval_fields(value))
+    fields.discard('context')  # TODO: remove when context is renamed
+    return fields
 
 
 def instanciate_values(Target, value, **extra):
     from ..modelstorage import ModelStorage, local_cache
     kwargs = {}
     ids = []
     if issubclass(Target, ModelStorage):
@@ -189,19 +191,37 @@
     return ctx
 
 
 def on_change_result(record):
     return record._changed_values
 
 
-def with_inactive_records(func):
+def on_change_with_result(field, value):
+    from ..modelstorage import ModelStorage
+    if field._type in {'many2one', 'one2one', 'reference'}:
+        if isinstance(value, ModelStorage):
+            if field._type == 'reference':
+                value = str(value)
+            else:
+                value = value.id
+    elif field._type in {'one2many', 'many2many'}:
+        if isinstance(value, (list, tuple)):
+            value = [int(r) for r in value]
+    return value
+
+
+def domain_method(func):
     @wraps(func)
-    def wrapper(*args, **kwargs):
-        with Transaction().set_context(active_test=False):
-            return func(*args, **kwargs)
+    def wrapper(self, domain, tables, Model):
+        name = domain[0].split('.', 1)[0]
+        assert name == self.name
+        method = getattr(Model, f'domain_{name}', None)
+        if method:
+            return method(domain, tables)
+        return func(self, domain, tables, Model)
     return wrapper
 
 
 SQL_OPERATORS = {
     '=': operators.Equal,
     '!=': operators.NotEqual,
     'like': operators.Like,
@@ -419,22 +439,19 @@
                     and any(v is None for v in value)):
                 if operator == 'in':
                     expression |= (column == Null)
                 else:
                     expression &= (column != Null)
         return expression
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         "Return a SQL expression for the domain using tables"
         table, _ = tables[None]
         name, operator, value = domain
-        assert name == self.name
-        method = getattr(Model, 'domain_%s' % name, None)
-        if method:
-            return method(domain, tables)
         Operator = SQL_OPERATORS[operator]
         column = self.sql_column(table)
         column = self._domain_column(operator, column)
         expression = Operator(column, self._domain_value(operator, value))
         expression = sanitize_sql_expression(expression)
         expression = self._domain_add_null(column, operator, value, expression)
         return expression
@@ -448,15 +465,15 @@
             return method(tables)
         else:
             return [self.sql_column(table)]
 
     def set_rpc(self, model):
         for attribute, result in (
                 ('on_change', on_change_result),
-                ('on_change_with', None),
+                ('on_change_with', partial(on_change_with_result, self)),
                 ):
             if not getattr(self, attribute):
                 continue
             func_name = '%s_%s' % (attribute, self.name)
             assert hasattr(model, func_name), \
                 'Missing %s on model %s' % (func_name, model.__name__)
             model.__rpc__.setdefault(
@@ -473,16 +490,16 @@
             'on_change': list(self.on_change),
             'on_change_with': list(self.on_change_with),
             'readonly': self.readonly,
             'required': self.required,
             'states': encoder.encode(self.states),
             'type': self._type,
             'domain': encoder.encode(self.domain),
-            'searchable': hasattr(model, 'search'),
-            'sortable': hasattr(model, 'search'),
+            'searchable': self.searchable(model),
+            'sortable': self.sortable(model),
             }
 
         # Add id to on_change's if they are not cached
         # Not having the id increase the efficiency of the cache
         for method in ['on_change', 'on_change_with']:
             changes = definition[method]
             if changes:
@@ -527,14 +544,20 @@
         translations = []
         for attr, ttype in [('string', 'field'), ('help', 'help')]:
             for source in getattr(self, attr):
                 if not isinstance(source, LazyString):
                     translations.append((name, ttype, language, source))
         return translations
 
+    def searchable(self, model):
+        return hasattr(model, 'search')
+
+    def sortable(self, model):
+        return hasattr(model, 'search')
+
 
 class FieldTranslate(Field):
 
     def _get_translation_join(
             self, Model, name, translation, model, table, from_, language,
             domain=None):
         if Model.__name__ == 'ir.model.field':
@@ -648,14 +671,15 @@
             translation, join = self._get_translation_join(
                 Model, name, translation, model, table, join, language,
                 domain=domain)
             column = Coalesce(NullIf(column, ''), translation.value)
             language = get_parent_language(language)
         return table, join, column
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         if not self.translate:
             return super(FieldTranslate, self).convert_domain(
                 domain, tables, Model)
         table, _ = tables[None]
         name, operator, value = domain
         model, join, column = self._get_translation_column(
```

### Comparing `trytond-6.6.8/trytond/model/fields/float.py` & `trytond-6.8.0/trytond/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/function.py` & `trytond-6.8.0/trytond/model/fields/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # this repository contains the full copyright notices and license terms.
 
 import copy
 import inspect
 from functools import wraps
 
 from trytond.i18n import gettext
-from trytond.model.fields.field import Field
 from trytond.tools import is_instance_method
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
+
+from .field import Field, domain_method, on_change_with_result
 
 
 def getter_context(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if not self.getter_with_context:
             transaction = Transaction()
@@ -87,78 +88,76 @@
 
     def sql_format(self, value):
         return self._field.sql_format(value)
 
     def sql_type(self):
         return None
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
-        name, operator, value = domain[:3]
-        assert name.startswith(self.name)
-        method = getattr(Model, 'domain_%s' % self.name, None)
-        if method:
-            return method(domain, tables)
         if self.searcher:
             return getattr(Model, self.searcher)(self.name, domain)
         raise NotImplementedError(gettext(
                 'ir.msg_search_function_missing',
                 **Model.__names__(self.name)))
 
     @getter_context
+    @without_check_access
     def get(self, ids, Model, name, values=None):
         '''
         Call the getter.
         If the function has ``names`` in the function definition then
         it will call it with a list of name.
         '''
-        with Transaction().set_context(_check_access=False):
-            method = getattr(Model, self.getter)
-            instance_method = is_instance_method(Model, self.getter)
-            multiple = self.getter_multiple(method)
-
-            records = Model.browse(ids)
-            for record, value in zip(records, values):
-                assert record.id == value['id']
-                for fname, val in value.items():
-                    field = Model._fields.get(fname)
-                    if field and field._type not in {
-                            'many2one', 'reference',
-                            'one2many', 'many2many', 'one2one'}:
-                        record._local_cache[record.id][fname] = val
-
-            def call(name):
-                if not instance_method:
-                    return method(records, name)
-                else:
-                    return dict((r.id, method(r, name)) for r in records)
-            if isinstance(name, list):
-                names = name
-                if multiple:
-                    return call(names)
-                return dict((name, call(name)) for name in names)
+        method = getattr(Model, self.getter)
+        instance_method = is_instance_method(Model, self.getter)
+        multiple = self.getter_multiple(method)
+
+        records = Model.browse(ids)
+        for record, value in zip(records, values):
+            assert record.id == value['id']
+            for fname, val in value.items():
+                field = Model._fields.get(fname)
+                if field and field._type not in {
+                        'many2one', 'reference',
+                        'one2many', 'many2many', 'one2one'}:
+                    record._local_cache[record.id][fname] = val
+
+        def call(name):
+            if not instance_method:
+                return on_change_with_result(self, method(records, name))
             else:
-                if multiple:
-                    name = [name]
-                return call(name)
+                return {
+                    r.id: on_change_with_result(self, method(r, name))
+                    for r in records}
+        if isinstance(name, list):
+            names = name
+            if multiple:
+                return call(names)
+            return dict((name, call(name)) for name in names)
+        else:
+            if multiple:
+                name = [name]
+            return call(name)
 
+    @without_check_access
     def set(self, Model, name, ids, value, *args):
         '''
         Call the setter.
         '''
-        with Transaction().set_context(_check_access=False):
-            if self.setter:
-                # TODO change setter API to use sequence of records, value
-                setter = getattr(Model, self.setter)
-                args = iter((ids, value) + args)
-                for ids, value in zip(args, args):
-                    setter(Model.browse(ids), name, value)
-            else:
-                raise NotImplementedError(gettext(
-                        'ir.msg_setter_function_missing',
-                        **Model.__names__(self.name)))
+        if self.setter:
+            # TODO change setter API to use sequence of records, value
+            setter = getattr(Model, self.setter)
+            args = iter((ids, value) + args)
+            for ids, value in zip(args, args):
+                setter(Model.browse(ids), name, value)
+        else:
+            raise NotImplementedError(gettext(
+                    'ir.msg_setter_function_missing',
+                    **Model.__names__(self.name)))
 
     def __get__(self, inst, cls):
         try:
             return super().__get__(inst, cls)
         except AttributeError:
             if not self.getter.startswith('on_change_with'):
                 raise
@@ -170,19 +169,25 @@
             return super().__get__(temp_inst, cls)
 
     def __set__(self, inst, value):
         self._field.__set__(inst, value)
 
     def definition(self, model, language):
         definition = self._field.definition(model, language)
-        definition['searchable'] &= (
-            bool(self.searcher) or hasattr(model, 'domain_' + self.name))
-        definition['sortable'] &= hasattr(model, 'order_' + self.name)
+        definition['searchable'] = self.searchable(model)
+        definition['sortable'] = self.sortable(model)
         return definition
 
+    def searchable(self, model):
+        return super().searchable(model) and (
+            bool(self.searcher) or hasattr(model, f'domain_{self.name}'))
+
+    def sortable(self, model):
+        return super().sortable(model) and hasattr(model, f'order_{self.name}')
+
     def getter_multiple(self, method):
         "Returns True if getter function accepts multiple fields"
         signature = inspect.signature(method)
         return 'names' in signature.parameters
 
 
 for name in [
```

### Comparing `trytond-6.6.8/trytond/model/fields/many2many.py` & `trytond-6.8.0/trytond/model/fields/many2many.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from trytond.pool import Pool
 from trytond.pyson import PYSONEncoder
 from trytond.tools import cached_property, grouped_slice
 from trytond.transaction import Transaction
 
 from .field import (
-    Field, context_validate, domain_validate, get_eval_fields,
+    Field, context_validate, domain_method, domain_validate, get_eval_fields,
     instanciate_values, instantiate_context, search_order_validate,
     size_validate)
 from .function import Function
 
 
 class Many2Many(Field):
     '''
@@ -350,14 +350,15 @@
             expression = Literal(False)
         else:
             expression = table.id.in_(ids)
         if operator.startswith('not'):
             return ~expression
         return expression
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         from ..modelsql import convert_from
         pool = Pool()
         Rule = pool.get('ir.rule')
         Target = self.get_target()
         Relation = self.get_relation()
         transaction = Transaction()
@@ -488,14 +489,16 @@
         definition['datetime_field'] = self.datetime_field
         if self.filter:
             definition['domain'] = encoder.encode(
                 ['AND', self.domain, self.filter])
         definition['relation'] = self.get_target().__name__
         definition['search_context'] = encoder.encode(self.search_context)
         definition['search_order'] = encoder.encode(self.search_order)
-        definition['sortable'] &= hasattr(model, 'order_' + self.name)
         definition['order'] = (
             getattr(self.get_target(), '_order', None)
             if self.order is None else self.order)
         if self.size is not None:
             definition['size'] = encoder.encode(self.size)
         return definition
+
+    def sortable(self, model):
+        return super().sortable(model) and hasattr(model, f'order_{self.name}')
```

### Comparing `trytond-6.6.8/trytond/model/fields/many2one.py` & `trytond-6.8.0/trytond/model/fields/many2one.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from sql import As, Column, Expression, Literal, Query, With
 from sql.aggregate import Max
 from sql.conditionals import Coalesce
 from sql.operators import Or
 
+from trytond.config import config
 from trytond.pool import Pool
 from trytond.pyson import PYSONEncoder
 from trytond.tools import cached_property, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 from .field import (
-    Field, context_validate, instantiate_context, search_order_validate,
-    with_inactive_records)
+    Field, context_validate, domain_method, instantiate_context,
+    search_order_validate)
+
+_subquery_threshold = config.getint('database', 'subquery_threshold')
 
 
 class Many2One(Field):
     '''
     Define many2one field (``int``).
     '''
     _type = 'many2one'
     _sql_type = 'INTEGER'
 
     def __init__(self, model_name, string='', left=None, right=None, path=None,
-            ondelete='SET NULL', datetime_field=None, target_search='join',
+            ondelete='SET NULL', datetime_field=None,
             search_order=None, search_context=None, help='', required=False,
             readonly=False, domain=None, states=None,
             on_change=None, on_change_with=None, depends=None, context=None,
             loading='eager'):
         '''
         :param model_name: The name of the target model.
         :param left: The name of the field to store the left value for
@@ -53,16 +56,14 @@
             on_change=on_change, on_change_with=on_change_with,
             depends=depends, context=context, loading=loading)
         self.model_name = model_name
         self.left = left
         self.right = right
         self.path = path
         self.datetime_field = datetime_field
-        assert target_search in ['subquery', 'join']
-        self.target_search = target_search
         self.__search_order = None
         self.search_order = search_order
         self.__search_context = None
         self.search_context = search_context or {}
     __init__.__doc__ += Field.__init__.__doc__
 
     def __get_required(self):
@@ -113,15 +114,18 @@
                     value = Target(**value)
                 elif isinstance(value, int):
                     value = Target(value)
         assert isinstance(value, (Target, type(None)))
         super(Many2One, self).__set__(inst, value)
 
     def sql_format(self, value):
+        from ..model import Model
         assert value is not False
+        assert (
+            not isinstance(value, Model) or value.__name__ == self.model_name)
         if value and not isinstance(value, (Query, Expression)):
             value = int(value)
         return super().sql_format(value)
 
     def convert_domain_path(self, domain, tables):
         cursor = Transaction().connection.cursor()
         table, _ = tables[None]
@@ -187,15 +191,16 @@
 
         expression = table.id.in_(tree.select(tree.id, with_=[tree]))
 
         if operator.startswith('not'):
             return ~expression
         return expression
 
-    @with_inactive_records
+    @inactive_records
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         pool = Pool()
         Rule = pool.get('ir.rule')
         Target = self.get_target()
 
         table, _ = tables[None]
         name, operator, value = domain[:3]
@@ -254,25 +259,27 @@
                 return super(Many2One, self).convert_domain(domain, tables,
                     Model)
             else:
                 target_name = 'rec_name'
         else:
             _, target_name = name.split('.', 1)
         target_domain = [(target_name,) + tuple(domain[1:])]
-        if 'active' in Target._fields:
-            target_domain.append(('active', 'in', [True, False]))
-        if self.target_search == 'subquery':
+        if Target.estimated_count() < _subquery_threshold:
             query = Target.search(target_domain, order=[], query=True)
             return column.in_(query)
         else:
-            target_tables = self._get_target_tables(tables)
-            target_table, _ = target_tables[None]
             rule_domain = Rule.domain_get(Target.__name__, mode='read')
             if rule_domain:
                 target_domain = [target_domain, rule_domain]
+            elif target_name == 'id':
+                # No need to join with the target table
+                return super().convert_domain(
+                    (self.name, operator, value), tables, Model)
+            target_tables = self._get_target_tables(tables)
+            target_table, _ = target_tables[None]
             _, expression = Target.search_domain(
                 target_domain, tables=target_tables)
             return expression
 
     def convert_order(self, name, tables, Model):
         fname, _, oexpr = name.partition('.')
         if not oexpr and getattr(Model, 'order_%s' % fname, None):
@@ -281,17 +288,19 @@
 
         Target = self.get_target()
 
         if oexpr:
             oname, _, _ = oexpr.partition('.')
         else:
             oname = 'id'
-            if Target._rec_name in Target._fields:
+            if (Target._rec_name in Target._fields
+                    and Target._fields[Target._rec_name].sortable(Target)):
                 oname = Target._rec_name
-            if Target._order_name in Target._fields:
+            if (Target._order_name in Target._fields
+                    and Target._fields[Target._order_name].sortable(Target)):
                 oname = Target._order_name
             oexpr = oname
 
         table, _ = tables[None]
         if oname == 'id':
             return [self.sql_column(table)]
```

### Comparing `trytond-6.6.8/trytond/model/fields/multiselection.py` & `trytond-6.8.0/trytond/model/fields/multiselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 
 from sql import Literal, operators
 
 from trytond.rpc import RPC
 from trytond.transaction import Transaction
 
-from .field import Field
+from .field import Field, domain_method
 from .selection import SelectionMixin
 
 # Use canonical form
 dumps = partial(json.dumps, separators=(',', ':'), sort_keys=True)
 
 
 class MultiSelection(SelectionMixin, Field):
@@ -47,16 +47,17 @@
 
     def set_rpc(self, model):
         super().set_rpc(model)
         if not isinstance(self.selection, (list, tuple)):
             assert hasattr(model, self.selection), \
                 'Missing %s on model %s' % (self.selection, model.__name__)
             instantiate = 0 if self.selection_change_with else None
+            cache = dict(days=1) if instantiate is None else None
             model.__rpc__.setdefault(
-                self.selection, RPC(instantiate=instantiate))
+                self.selection, RPC(instantiate=instantiate, cache=cache))
 
     def get(self, ids, model, name, values=None):
         lists = {id: () for id in ids}
         for value in values or []:
             data = value[name]
             if data:
                 # If stored as JSON conversion is done on backend
@@ -78,14 +79,15 @@
     def _domain_value(self, operator, value):
         database = Transaction().database
         domain_value = super()._domain_value(operator, value)
         if value is not None:
             domain_value = database.json_get(domain_value)
         return domain_value
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         name, operator, value = domain[:3]
         if operator not in {'in', 'not in'}:
             return super().convert_domain(domain, tables, Model)
         database = Transaction().database
         table, _ = tables[None]
         raw_column = self.sql_column(table)
```

### Comparing `trytond-6.6.8/trytond/model/fields/numeric.py` & `trytond-6.8.0/trytond/model/fields/numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/one2many.py` & `trytond-6.8.0/trytond/model/fields/one2many.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import defaultdict
 from itertools import chain
 
+from sql import Literal
 from sql.conditionals import Coalesce
+from sql.operators import Exists
 
+from trytond.config import config
 from trytond.pool import Pool
 from trytond.pyson import PYSONEncoder
 from trytond.tools import cached_property, grouped_slice
 from trytond.transaction import Transaction
 
 from .field import (
-    Field, context_validate, domain_validate, get_eval_fields,
+    Field, context_validate, domain_method, domain_validate, get_eval_fields,
     instanciate_values, instantiate_context, search_order_validate,
     size_validate)
 from .function import Function
 
+_subquery_threshold = config.getint('database', 'subquery_threshold')
+
 
 class One2Many(Field):
     '''
     Define one2many field (``list``).
     '''
     _type = 'one2many'
 
@@ -303,14 +308,15 @@
         if inst._removed is None:
             inst._removed = defaultdict(set)
         inst._removed[self.name].update(map(int, records))
         setattr(
             inst, self.name,
             [r for r in getattr(inst, self.name) if r not in records])
 
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         from ..modelsql import convert_from
         pool = Pool()
         Rule = pool.get('ir.rule')
         Target = self.get_target()
         transaction = Transaction()
         table, _ = tables[None]
@@ -328,28 +334,50 @@
         origin_field = Target._fields[self.field]
         origin = getattr(Target, self.field).sql_column(target)
         origin_where = None
         if origin_field._type == 'reference':
             origin_where = origin.like(Model.__name__ + ',%')
             origin = origin_field.sql_id(origin, Target)
 
+        use_in = Target.estimated_count() < _subquery_threshold
         if '.' not in name:
             if value is None:
-                where = origin != value
-                if history_where:
-                    where &= history_where
-                if origin_where:
-                    where &= origin_where
-                if self.filter:
-                    query = Target.search(self.filter, order=[], query=True)
-                    where &= origin.in_(query)
-                query = target.select(origin, where=where)
-                expression = ~table.id.in_(query)
+                if use_in:
+                    where = origin != value
+                    if history_where:
+                        where &= history_where
+                    if origin_where:
+                        where &= origin_where
+                    if self.filter:
+                        query = Target.search(
+                            self.filter, order=[], query=True)
+                        where &= origin.in_(query)
+                    query = target.select(origin, where=where)
+                    expression = ~table.id.in_(query)
+                else:
+                    where = origin == table.id
+                    if history_where:
+                        where &= history_where
+                    if origin_where:
+                        where &= origin_where
+                    if self.filter:
+                        target_tables = {
+                            None: (target, None),
+                            }
+                        target_tables, clause = Target.search_domain(
+                            self.filter, tables=target_tables)
+                        where &= clause
+                        query_table = convert_from(None, target_tables)
+                        query = query_table.select(Literal(1), where=where)
+                    else:
+                        query = target.select(Literal(1), where=where)
+                    expression = ~Exists(query)
+
                 if operator == '!=':
-                    return ~expression
+                    expression = ~expression
                 return expression
             else:
                 if isinstance(value, str):
                     target_name = 'rec_name'
                 else:
                     target_name = 'id'
         else:
@@ -368,21 +396,30 @@
             target_domain = [target_domain, self.filter]
         target_tables = {
             None: (target, None),
             }
         tables, expression = Target.search_domain(
             target_domain, tables=target_tables)
         query_table = convert_from(None, target_tables)
-        query = query_table.select(origin, where=expression)
-        expression = table.id.in_(query)
+        if use_in:
+            query = query_table.select(origin, where=expression)
+            expression = table.id.in_(query)
+        else:
+            query = query_table.select(
+                Literal(1), where=expression & (origin == table.id))
+            expression = Exists(query)
 
         if operator == 'not where':
             expression = ~expression
         elif operator.startswith('!') or operator.startswith('not '):
-            expression |= ~table.id.in_(target.select(origin))
+            if use_in:
+                expression |= ~table.id.in_(target.select(origin))
+            else:
+                expression |= ~Exists(target.select(
+                        Literal(1), where=origin == table.id))
         return expression
 
     def definition(self, model, language):
         encoder = PYSONEncoder()
         definition = super().definition(model, language)
         if self.add_remove is not None:
             definition['add_remove'] = encoder.encode(self.add_remove)
@@ -393,12 +430,14 @@
         definition['relation'] = self.model_name
         if self.field:
             definition['relation_field'] = self.field
         definition['search_context'] = encoder.encode(self.search_context)
         definition['search_order'] = encoder.encode(self.search_order)
         if self.size is not None:
             definition['size'] = encoder.encode(self.size)
-        definition['sortable'] &= hasattr(model, 'order_' + self.name)
         definition['order'] = (
             getattr(self.get_target(), '_order', None)
             if self.order is None else self.order)
         return definition
+
+    def sortable(self, model):
+        return super().sortable(model) and hasattr(model, f'order_{self.name}')
```

### Comparing `trytond-6.6.8/trytond/model/fields/one2one.py` & `trytond-6.8.0/trytond/model/fields/one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/fields/reference.py` & `trytond-6.8.0/trytond/model/fields/reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from sql import Cast, Expression, Literal, Query
 from sql.functions import Position, Substring
 
 from trytond.pool import Pool
 from trytond.pyson import PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import cached_property
-from trytond.transaction import Transaction
+from trytond.transaction import (
+    Transaction, inactive_records, without_check_access)
 
 from .field import (
-    Field, context_validate, domain_validate, instantiate_context,
-    search_order_validate, with_inactive_records)
+    Field, context_validate, domain_method, domain_validate,
+    instantiate_context, search_order_validate)
 from .selection import SelectionMixin
 
 
 class Reference(SelectionMixin, Field):
     '''
     Define a reference field (``str``).
     '''
@@ -106,16 +107,17 @@
 
     def set_rpc(self, model):
         super(Reference, self).set_rpc(model)
         if not isinstance(self.selection, (list, tuple)):
             assert hasattr(model, self.selection), \
                 'Missing %s on model %s' % (self.selection, model.__name__)
             instantiate = 0 if self.selection_change_with else None
+            cache = dict(days=1) if instantiate is None else None
             model.__rpc__.setdefault(
-                self.selection, RPC(instantiate=instantiate))
+                self.selection, RPC(instantiate=instantiate, cache=cache))
 
     def get(self, ids, model, name, values=None):
         '''
         Replace removed reference id by None.
         '''
         pool = Pool()
         if values is None:
@@ -141,16 +143,15 @@
                 continue
             res[i] = ref_model + ',' + str(ref_id)
             ref_to_check.setdefault(ref_model, (set(), []))
             ref_to_check[ref_model][0].add(ref_id)
             ref_to_check[ref_model][1].append(i)
 
         # Check if reference ids still exist
-        with Transaction().set_context(active_test=False), \
-                Transaction().set_context(_check_access=False):
+        with inactive_records(), without_check_access():
             for ref_model, (ref_ids, ids) in ref_to_check.items():
                 try:
                     pool.get(ref_model)
                 except KeyError:
                     res.update(dict((i, None) for i in ids))
                     continue
                 Ref = pool.get(ref_model)
@@ -189,15 +190,16 @@
 
     def sql_id(self, column, Model):
         "Return SQL expression for the id part of the field"
         return Cast(Substring(
                 column, Position(',', column) + Literal(1)),
             Model.id.sql_type().base)
 
-    @with_inactive_records
+    @inactive_records
+    @domain_method
     def convert_domain(self, domain, tables, Model):
         if '.' not in domain[0]:
             return super(Reference, self).convert_domain(domain, tables, Model)
         pool = Pool()
         name, operator, value, target = domain[:4]
         Target = pool.get(target)
         table, _ = tables[None]
```

### Comparing `trytond-6.6.8/trytond/model/fields/selection.py` & `trytond-6.8.0/trytond/model/fields/selection.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,35 @@
             sources.append(self.help_selection.items())
         for key, source in chain(*sources):
             if not isinstance(source, LazyString):
                 selection.append(
                     (name, 'selection', language, source))
         return super().definition_translations(model, language) + selection
 
+    @classmethod
+    def get_selection(cls, model, name, inst):
+        selection = model.fields_get([name])[name]['selection']
+        if isinstance(selection, str):
+            sel_func = getattr(model, selection)
+            if not is_instance_method(model, selection):
+                selection = sel_func()
+            else:
+                selection = sel_func(inst)
+        return dict(selection)
+
+    @classmethod
+    def get_selection_string(cls, selection, value):
+        # None and '' are equivalent
+        if value is None or value == '':
+            if value not in selection:
+                switch_value = {None: '', '': None}[value]
+                if switch_value in selection:
+                    value = switch_value
+        return selection[value]
+
 
 class Selection(SelectionMixin, Field):
     '''
     Define a selection field (``str``).
     '''
     _type = 'selection'
     _sql_type = 'VARCHAR'
@@ -112,16 +133,17 @@
 
     def set_rpc(self, model):
         super(Selection, self).set_rpc(model)
         if not isinstance(self.selection, (list, tuple)):
             assert hasattr(model, self.selection), \
                 'Missing %s on model %s' % (self.selection, model.__name__)
             instantiate = 0 if self.selection_change_with else None
+            cache = dict(days=1) if instantiate is None else None
             model.__rpc__.setdefault(
-                self.selection, RPC(instantiate=instantiate))
+                self.selection, RPC(instantiate=instantiate, cache=cache))
 
     def convert_order(self, name, tables, Model):
         if getattr(Model, 'order_%s' % name, None):
             return super(Selection, self).convert_order(name, tables, Model)
 
         assert name == self.name
         table, _ = tables[None]
@@ -152,33 +174,21 @@
     def __init__(self, name):
         self.name = name
 
     def __get__(self, inst, cls):
         from ..model import Model
         if inst is None:
             return self
+        field = cls._fields[self.name]
         with Transaction().set_context(getattr(inst, '_context', {})):
-            selection = cls.fields_get([self.name])[self.name]['selection']
-            if not isinstance(selection, (tuple, list)):
-                sel_func = getattr(cls, selection)
-                if not is_instance_method(cls, selection):
-                    selection = sel_func()
-                else:
-                    selection = sel_func(inst)
-            selection = dict(selection)
+            selection = field.get_selection(cls, self.name, inst)
         value = getattr(inst, self.name)
-        # None and '' are equivalent
-        if value is None or value == '':
-            if value not in selection:
-                switch_value = {None: '', '': None}[value]
-                if switch_value in selection:
-                    value = switch_value
         # Use Model __name__ for Reference field
-        elif isinstance(value, Model):
+        if isinstance(value, Model):
             value = value.__name__
         if isinstance(value, (list, tuple)):
             values = []
             for item in value:
-                values.append(selection.get(item, item))
+                values.append(field.get_selection_string(selection, item))
             return values
         else:
-            return selection.get(value, value)
+            return field.get_selection_string(selection, value)
```

### Comparing `trytond-6.6.8/trytond/model/fields/text.py` & `trytond-6.8.0/trytond/model/fields/text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/match.py` & `trytond-6.8.0/trytond/model/match.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/model.py` & `trytond-6.8.0/trytond/model/model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/modelsingleton.py` & `trytond-6.8.0/trytond/model/modelsingleton.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from trytond.transaction import Transaction
 
+from sql.operators import Equal
+
+from trytond.transaction import Transaction, without_check_access
+
+from .modelsql import Exclude, ModelSQL
 from .modelstorage import ModelStorage
 
 
 class ModelSingleton(ModelStorage):
     """
     Define a singleton model in Tryton.
     """
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         # Cache disable because it is used as a read by the client
         cls.__rpc__['default_get'].cache = None
 
+        if issubclass(cls, ModelSQL):
+            table = cls.__table__()
+            cls._sql_constraints.append(
+                ('singleton', Exclude(table, (table.id * 0, Equal)),
+                    'ir.msg_singleton'))
+
     @classmethod
     def get_singleton(cls):
         '''
         Return the instance of the unique record if there is one.
         '''
         singletons = super(ModelSingleton, cls).search([], limit=1)
         if singletons:
             return singletons[0]
 
     @classmethod
     def create(cls, vlist):
         assert len(vlist) == 1
         singleton = cls.get_singleton()
         if not singleton:
+            if issubclass(cls, ModelSQL):
+                cls.lock()
             return super(ModelSingleton, cls).create(vlist)
         cls.write([singleton], vlist[0])
         return [singleton]
 
     @classmethod
     def read(cls, ids, fields_names):
         singleton = cls.get_singleton()
@@ -54,15 +66,15 @@
         res[0]['id'] = ids[0]
         return res
 
     @classmethod
     def write(cls, records, values, *args):
         singleton = cls.get_singleton()
         if not singleton:
-            with Transaction().set_context(_check_access=False):
+            with without_check_access():
                 singleton, = cls.create([values])
             actions = (records, {}) + args
         else:
             actions = (records, values) + args
         args = []
         for values in actions[1:None:2]:
             args.extend(([singleton], values))
```

### Comparing `trytond-6.6.8/trytond/model/modelsql.py` & `trytond-6.8.0/trytond/model/modelsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from trytond.config import config
 from trytond.exceptions import ConcurrencyException
 from trytond.i18n import gettext
 from trytond.pool import Pool
 from trytond.pyson import PYSONDecoder, PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import cursor_dict, grouped_slice, reduce_ids
-from trytond.transaction import Transaction, record_cache_size
+from trytond.transaction import (
+    Transaction, inactive_records, record_cache_size, without_check_access)
 
 from . import fields
 from .descriptors import dualmethod
 from .modelstorage import (
     AccessError, ModelStorage, RequiredValidationError, SizeValidationError,
     ValidationError, is_leaf)
 from .modelview import ModelView
@@ -487,14 +488,15 @@
             history_table = cls.__table_handler__(history=True)
             for field_name, field in cls._fields.items():
                 if not field.sql_type():
                     continue
                 history_table.add_column(field_name, field._sql_type)
 
     @classmethod
+    @without_check_access
     def __raise_integrity_error(
             cls, exception, values, field_names=None, transaction=None):
         pool = Pool()
         if field_names is None:
             field_names = list(cls._fields.keys())
         if transaction is None:
             transaction = Transaction()
@@ -533,14 +535,15 @@
                     error_args = cls.__names__(field_name)
                     error_args['value'] = values[field_name]
                     raise ForeignKeyError(
                             gettext('ir.msg_foreign_model_missing',
                                 **error_args))
 
     @classmethod
+    @without_check_access
     def __raise_data_error(
             cls, exception, values, field_names=None, transaction=None):
         if field_names is None:
             field_names = list(cls._fields.keys())
         if transaction is None:
             transaction = Transaction()
         for field_name in field_names:
@@ -636,14 +639,22 @@
     def _restore_history(cls, ids, datetime, _before=False):
         if not cls._history:
             return
         transaction = Transaction()
         cursor = transaction.connection.cursor()
         table = cls.__table__()
         history = cls.__table_history__()
+
+        transaction.counter += 1
+        for cache in transaction.cache.values():
+            if cls.__name__ in cache:
+                cache_cls = cache[cls.__name__]
+                for id_ in ids:
+                    cache_cls.pop(id_, None)
+
         columns = []
         hcolumns = []
         fnames = sorted(n for n, f in cls._fields.items()
             if f.sql_type())
         for fname in fnames:
             columns.append(Column(table, fname))
             if fname == 'write_uid':
@@ -732,25 +743,88 @@
                         'Records were modified in the meanwhile')
 
     @classmethod
     @no_table_query
     def create(cls, vlist):
         transaction = Transaction()
         cursor = transaction.connection.cursor()
+        in_max = transaction.database.IN_MAX
         pool = Pool()
         Translation = pool.get('ir.translation')
 
         super(ModelSQL, cls).create(vlist)
 
         table = cls.__table__()
         modified_fields = set()
         defaults_cache = {}  # Store already computed default values
         missing_defaults = {}  # Store missing default values by schema
         new_ids = []
         vlist = [v.copy() for v in vlist]
+
+        def db_insert(columns, vlist, fields):
+            if transaction.database.has_multirow_insert():
+                vlist = (
+                    s for s in grouped_slice(
+                        vlist, in_max // (len(fields) or 1)))
+            else:
+                vlist = ([v] for v in vlist)
+
+            for values in vlist:
+                values = list(values)
+                cols = list(columns)
+                try:
+                    if len(values) > 1:
+                        ids = transaction.database.nextid(
+                            transaction.connection, cls._table,
+                            count=len(values))
+                        if ids is not None:
+                            assert len(ids) == len(values)
+                            cols.append(table.id)
+                            for val, id in zip(values, ids):
+                                val.append(id)
+                            cursor.execute(*table.insert(cols, values))
+                            yield from ids
+                            continue
+                    for i, val in enumerate(values):
+                        if transaction.database.has_returning():
+                            cursor.execute(*table.insert(
+                                    cols, [val], [table.id]))
+                            yield from (r[0] for r in cursor)
+                        else:
+                            id_new = transaction.database.nextid(
+                                transaction.connection, cls._table)
+                            if id_new:
+                                if i == 0:
+                                    cols.append(table.id)
+                                val.append(id_new)
+                                cursor.execute(*table.insert(cols, [val]))
+                            else:
+                                cursor.execute(*table.insert(cols, [val]))
+                                id_new = transaction.database.lastid(cursor)
+                            yield id_new
+                except (
+                        backend.DatabaseIntegrityError,
+                        backend.DatabaseDataError
+                        ) as exception:
+                    if isinstance(exception, backend.DatabaseIntegrityError):
+                        raise_func = cls.__raise_integrity_error
+                    elif isinstance(exception, backend.DatabaseDataError):
+                        raise_func = cls.__raise_data_error
+                    with transaction.new_transaction():
+                        for value in values:
+                            skip = len(['create_uid', 'create_date'])
+                            recomposed = dict(zip(fields, value[skip:]))
+                            raise_func(
+                                exception, recomposed, transaction=transaction)
+                    raise
+
+        to_insert = []
+        previous_columns = [table.create_uid, table.create_date]
+        previous_column_names = set()
+
         for values in vlist:
             # Clean values
             for key in ('create_uid', 'create_date',
                     'write_uid', 'write_date', 'id'):
                 if key in values:
                     del values[key]
             modified_fields |= values.keys()
@@ -776,55 +850,39 @@
 
                 if default:
                     defaults = cls.default_get(default, with_rec_name=False)
                     default_values.update(cls._clean_defaults(defaults))
                     defaults_cache.update(default_values)
             values.update(missing_defaults[values_schema])
 
-            insert_columns = [table.create_uid, table.create_date]
-            insert_values = [transaction.user, CurrentTimestamp()]
+            current_column_names = set()
+            current_columns = [table.create_uid, table.create_date]
+            current_values = [transaction.user, CurrentTimestamp()]
 
             # Insert record
-            for fname, value in values.items():
+            for fname, value in sorted(values.items()):
                 field = cls._fields[fname]
                 if not hasattr(field, 'set'):
-                    insert_columns.append(Column(table, fname))
-                    insert_values.append(field.sql_format(value))
-
-            try:
-                if transaction.database.has_returning():
-                    cursor.execute(*table.insert(insert_columns,
-                            [insert_values], [table.id]))
-                    id_new, = cursor.fetchone()
-                else:
-                    id_new = transaction.database.nextid(
-                        transaction.connection, cls._table)
-                    if id_new:
-                        insert_columns.append(table.id)
-                        insert_values.append(id_new)
-                        cursor.execute(*table.insert(insert_columns,
-                                [insert_values]))
-                    else:
-                        cursor.execute(*table.insert(insert_columns,
-                                [insert_values]))
-                        id_new = transaction.database.lastid(cursor)
-                new_ids.append(id_new)
-            except (
-                    backend.DatabaseIntegrityError,
-                    backend.DatabaseDataError) as exception:
-                transaction = Transaction()
-                with Transaction().new_transaction(), \
-                        Transaction().set_context(_check_access=False):
-                    if isinstance(exception, backend.DatabaseIntegrityError):
-                        cls.__raise_integrity_error(
-                            exception, values, transaction=transaction)
-                    elif isinstance(exception, backend.DatabaseDataError):
-                        cls.__raise_data_error(
-                            exception, values, transaction=transaction)
-                raise
+                    current_columns.append(Column(table, fname))
+                    current_values.append(field.sql_format(value))
+                    current_column_names.add(fname)
+
+            if current_column_names != previous_column_names:
+                if to_insert:
+                    new_ids.extend(db_insert(
+                            previous_columns, to_insert,
+                            previous_column_names))
+                    to_insert.clear()
+                previous_columns = current_columns
+                previous_column_names = current_column_names
+            to_insert.append(current_values)
+        else:
+            if to_insert:
+                new_ids.extend(db_insert(
+                        current_columns, to_insert, current_column_names))
 
         transaction.create_records[cls.__name__].update(new_ids)
 
         # Update path before fields_to_set which could create children
         if cls._path_fields:
             field_names = list(sorted(cls._path_fields))
             cls._set_path(field_names, repeat(new_ids, len(field_names)))
@@ -895,14 +953,17 @@
             extra_fields.add('write_date')
         for field_name in fields_names:
             if field_name in {'_timestamp', '_write', '_delete'}:
                 continue
             if '.' in field_name:
                 field_name, field_related = field_name.split('.', 1)
                 fields_related[field_name].add(field_related)
+            if field_name.endswith(':string'):
+                field_name = field_name[:-len(':string')]
+                fields_related[field_name]
             field = cls._fields[field_name]
             if hasattr(field, 'datetime_field') and field.datetime_field:
                 extra_fields.add(field.datetime_field)
             if field.context:
                 extra_fields.update(fields.get_eval_fields(field.context))
         extra_fields.discard('id')
         all_fields = (
@@ -1112,14 +1173,25 @@
             key = name + '.'
             if field._type.endswith('2many'):
                 for row in rows:
                     row[key] = values = list()
                     for target in row[name]:
                         if target is not None:
                             values.append(targets[target])
+            elif field._type in {'selection', 'multiselection'}:
+                key = name + ':string'
+                for row, target in zip(rows, targets):
+                    selection = field.get_selection(cls, name, target)
+                    if field._type == 'selection':
+                        row[key] = field.get_selection_string(
+                            selection, row[name])
+                    else:
+                        row[key] = [
+                            field.get_selection_string(selection, v)
+                            for v in row[name]]
             else:
                 for row in rows:
                     value = row[name]
                     if isinstance(value, str):
                         try:
                             value = int(value.split(',', 1)[1])
                         except ValueError:
@@ -1143,15 +1215,17 @@
             def groupfunc(row):
                 ctx = {}
                 if field.context:
                     pyson_context = PYSONEncoder().encode(field.context)
                     ctx.update(PYSONDecoder(row).decode(pyson_context))
                 if datetime_field:
                     ctx['_datetime'] = row.get(datetime_field)
-                if field._type == 'reference':
+                if field._type in {'selection', 'multiselection'}:
+                    Target = None
+                elif field._type == 'reference':
                     value = row[fname]
                     if not value:
                         Target = None
                     else:
                         model, _ = value.split(',', 1)
                         Target = pool.get(model)
                 else:
@@ -1167,15 +1241,15 @@
                 rows = list(rows)
                 with Transaction().set_context(ctx):
                     if Target:
                         targets = read_related(
                             field, Target, rows, list(fields_related[fname]))
                         targets = {t['id']: t for t in targets}
                     else:
-                        targets = {}
+                        targets = cls.browse([r['id'] for r in rows])
                     add_related(field, rows, targets)
 
         for row, field in product(result, to_del):
             del row[field]
 
         return result
 
@@ -1234,16 +1308,15 @@
                 try:
                     cursor.execute(*table.update(columns, update_values,
                             where=red_sql))
                 except (
                         backend.DatabaseIntegrityError,
                         backend.DatabaseDataError) as exception:
                     transaction = Transaction()
-                    with Transaction().new_transaction(), \
-                            Transaction().set_context(_check_access=False):
+                    with Transaction().new_transaction():
                         if isinstance(
                                 exception, backend.DatabaseIntegrityError):
                             cls.__raise_integrity_error(
                                 exception, values, list(values.keys()),
                                 transaction=transaction)
                         elif isinstance(exception, backend.DatabaseDataError):
                             cls.__raise_data_error(
@@ -1354,46 +1427,50 @@
         def get_related_records(Model, field_name, sub_ids):
             if issubclass(Model, ModelSQL):
                 foreign_table = Model.__table__()
                 foreign_red_sql = reduce_ids(
                     Column(foreign_table, field_name), sub_ids)
                 cursor.execute(*foreign_table.select(foreign_table.id,
                         where=foreign_red_sql))
-                records = Model.browse([x[0] for x in cursor])
+                related_records = Model.browse([x[0] for x in cursor])
             else:
-                with transaction.set_context(active_test=False):
-                    records = Model.search([(field_name, 'in', sub_ids)])
-            return records
+                with inactive_records():
+                    related_records = Model.search(
+                        [(field_name, 'in', sub_ids)])
+            if Model == cls:
+                related_records = list(set(related_records) - set(records))
+            return related_records
 
         for sub_ids, sub_records in zip(
                 grouped_slice(ids), grouped_slice(records)):
             sub_ids = list(sub_ids)
             red_sql = reduce_ids(table.id, sub_ids)
 
             for Model, field_name in foreign_keys_toupdate:
                 if (not hasattr(Model, 'search')
                         or not hasattr(Model, 'write')):
                     continue
-                records = get_related_records(Model, field_name, sub_ids)
-                if records:
-                    Model.write(records, {
+                related_records = get_related_records(
+                    Model, field_name, sub_ids)
+                if related_records:
+                    Model.write(related_records, {
                             field_name: None,
                             })
 
             for Model, field_name in foreign_keys_todelete:
                 if (not hasattr(Model, 'search')
                         or not hasattr(Model, 'delete')):
                     continue
-                records = get_related_records(Model, field_name, sub_ids)
-                if records:
-                    Model.delete(records)
+                related_records = get_related_records(
+                    Model, field_name, sub_ids)
+                if related_records:
+                    Model.delete(related_records)
 
             for Model, field_name in foreign_keys_tocheck:
-                with Transaction().set_context(
-                        _check_access=False, active_test=False):
+                with without_check_access(), inactive_records():
                     if Model.search([
                                 (field_name, 'in', sub_ids),
                                 ], order=[]):
                         error_args = Model.__names__(field_name)
                         raise ForeignKeyError(
                             gettext('ir.msg_foreign_model_exist',
                                 **error_args))
@@ -1643,17 +1720,15 @@
         if order is None or order is False:
             order = cls._order
         tables, expression = cls.__search_query(domain, count, query, order)
 
         main_table, _ = tables[None]
         if count:
             table = convert_from(None, tables)
-            if (limit is not None
-                    and callable(cls.count)
-                    and limit < cls.count()) or offset:
+            if (limit is not None and limit < cls.estimated_count()) or offset:
                 select = table.select(
                     Literal(1), where=expression, limit=limit, offset=offset
                     ).select(Count(Literal('*')))
             else:
                 select = table.select(Count(Literal('*')), where=expression)
             if query:
                 return select
@@ -1776,15 +1851,15 @@
                 return Literal(True)
             elif domain[0] == 'OR':
                 return Or((convert(d) for d in domain[1:]))
             else:
                 return And((convert(d) for d in (
                             domain[1:] if domain[0] == 'AND' else domain)))
 
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             expression = convert(domain)
 
         if cls._history and transaction.context.get('_datetime'):
             table, _ = tables[None]
             expression &= (Coalesce(table.write_date, table.create_date)
                 <= transaction.context['_datetime'])
         return tables, expression
@@ -1876,15 +1951,15 @@
             field = cls._fields[field_name]
             if (values is not None
                     and (field.left in values or field.right in values)):
                 raise Exception('ValidateError',
                     'You can not update fields: "%s", "%s"' %
                     (field.left, field.right))
 
-            if callable(cls.count) and len(ids) < max(cls.count() / 4, 4):
+            if len(ids) < max(cls.estimated_count() / 4, 4):
                 for id_ in ids:
                     cls._update_tree(id_, field_name,
                         field.left, field.right)
             else:
                 cls._rebuild_tree(field_name, None, 0)
 
     @classmethod
@@ -2032,28 +2107,28 @@
             for sub_records in grouped_slice(records):
                 where = reduce_ids(table.id, sub_records)
                 query = table.select(
                     Literal(1), where=where, for_=For('UPDATE', nowait=True))
                 with connection.cursor() as cursor:
                     cursor.execute(*query)
         else:
-            database.lock(connection, cls._table)
+            transaction.lock_table(cls._table)
 
 
-def convert_from(table, tables):
+def convert_from(table, tables, type_='LEFT'):
     # Don't nested joins as SQLite doesn't support
     right, condition = tables[None]
     if table:
-        table = table.join(right, 'LEFT', condition)
+        table = table.join(right, type_, condition)
     else:
         table = right
     for k, sub_tables in tables.items():
         if k is None:
             continue
-        table = convert_from(table, sub_tables)
+        table = convert_from(table, sub_tables, type_=type_)
     return table
 
 
 def split_subquery_domain(domain):
     """
     Split a domain in two parts:
         - the first one contains all the sub-domains with only local fields
```

### Comparing `trytond-6.6.8/trytond/model/modelstorage.py` & `trytond-6.8.0/trytond/model/modelstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 import base64
 import csv
 import datetime
 import decimal
 import random
 import time
+import warnings
 from collections import defaultdict
 from decimal import Decimal
-from functools import lru_cache, wraps
+from functools import lru_cache
 from itertools import chain, groupby, islice
 from operator import itemgetter
 
 from trytond.cache import Cache, LRUDictTransaction, freeze, unfreeze
 from trytond.config import config
 from trytond.const import OPERATORS
 from trytond.exceptions import UserError
 from trytond.i18n import gettext, lazy_gettext
 from trytond.pool import Pool
 from trytond.pyson import PYSON, PYSONDecoder, PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import grouped_slice, is_instance_method, reduce_domain
 from trytond.tools.domain_inversion import domain_inversion, eval_domain
 from trytond.tools.domain_inversion import parse as domain_parse
-from trytond.transaction import Transaction, record_cache_size
+from trytond.transaction import (
+    Transaction, inactive_records, record_cache_size, without_check_access)
 
 from . import fields
 from .descriptors import dualmethod
 from .model import Model
 
 __all__ = ['ModelStorage', 'EvalEnvironment']
 _cache_field = config.getint('cache', 'field')
@@ -80,20 +82,18 @@
     pass
 
 
 class TimeFormatValidationError(ValidationError):
     pass
 
 
-def without_check_access(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        with Transaction().set_context(_check_access=False):
-            return func(*args, **kwargs)
-    return wrapper
+class _UnsavedRecordError(ValueError):
+
+    def __init__(self, record):
+        self.record = record
 
 
 def is_leaf(expression):
     return (isinstance(expression, (list, tuple))
         and len(expression) > 2
         and isinstance(expression[1], str)
         and expression[1] in OPERATORS)  # TODO remove OPERATORS test
@@ -115,14 +115,15 @@
     write_date = fields.Timestamp(
         lazy_gettext('ir.msg_edited_at'), readonly=True)
     rec_name = fields.Function(
         fields.Char(lazy_gettext('ir.msg_record_name')), 'get_rec_name',
         searcher='search_rec_name')
     _count_cache = Cache(
         'modelstorage.count', duration=_cache_count_timeout, context=False)
+    _log = None
 
     @classmethod
     def __setup__(cls):
         from .modelview import ModelView
         super(ModelStorage, cls).__setup__()
         if issubclass(cls, ModelView):
             cls.__rpc__.update({
@@ -138,14 +139,16 @@
                     'search_count': RPC(),
                     'search_read': RPC(),
                     'resources': RPC(instantiate=0, unique=False),
                     'export_data_domain': RPC(),
                     'export_data': RPC(instantiate=0, unique=False),
                     'import_data': RPC(readonly=False),
                     })
+        if cls._log is None:
+            cls._log = not cls.__name__.startswith('ir.')
 
     @classmethod
     def __post_setup__(cls):
         super().__post_setup__()
 
         cls._mptt_fields = set()
         cls._path_fields = set()
@@ -163,14 +166,29 @@
         return int(Transaction().user)
 
     @staticmethod
     def default_create_date():
         "Default value for create_date field."
         return datetime.datetime.today()
 
+    @dualmethod
+    def log(cls, records, event, target=None, user=None, **extra):
+        if not cls._log:
+            return
+        pool = Pool()
+        Log = pool.get('ir.model.log')
+        transaction = Transaction()
+        if user is None:
+            user = transaction.user
+        for record in records:
+            assert record.id >= 0
+            transaction.log_records.append(Log(
+                    resource=record, event=event, target=target, user=user,
+                    **extra))
+
     @classmethod
     def create(cls, vlist):
         '''
         Returns the list of created records.
         '''
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
@@ -226,26 +244,26 @@
     def write(cls, records, values, *args):
         '''
         Write values on records.
         '''
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         ModelFieldAccess = pool.get('ir.model.field.access')
+        transaction = Transaction()
 
         assert not len(args) % 2
         actions = iter((records, values) + args)
         all_records = []
         all_fields = set()
         for records, values in zip(actions, actions):
-            if not cls.check_xml_record(records, values):
-                raise AccessError(
-                    gettext('ir.msg_write_xml_record'),
-                    gettext('ir.msg_base_config_record'))
+            cls.check_xml_record(records, values)
             all_records += records
             all_fields.update(values.keys())
+            if transaction.check_access and values:
+                cls.log(records, 'write', ','.join(sorted(values.keys())))
 
         ModelAccess.check(cls.__name__, 'write')
         ModelFieldAccess.check(cls.__name__, all_fields, 'write')
 
         # Increase transaction counter
         Transaction().counter += 1
 
@@ -297,34 +315,26 @@
     def delete(cls, records):
         '''
         Delete records.
         '''
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         ModelData = pool.get('ir.model.data')
+        transaction = Transaction()
 
         ModelAccess.check(cls.__name__, 'delete')
-        if not cls.check_xml_record(records, None):
-            raise AccessError(
-                gettext('ir.msg_delete_xml_record'),
-                gettext('ir.msg_base_config_record'))
+        cls.check_xml_record(records, None)
         if ModelData.has_model(cls.__name__):
-            with Transaction().set_context(_check_access=False):
-                data = []
-                for sub_records in grouped_slice(records):
-                    ids = [r.id for r in sub_records]
-                    data += ModelData.search([
-                            ('model', '=', cls.__name__),
-                            ('db_id', 'in', ids),
-                            ('noupdate', '=', True),
-                            ])
-                ModelData.write(data, {'db_id': None})
+            ModelData.clean(records)
+
+        if transaction.check_access:
+            cls.log(records, 'delete')
 
         # Increase transaction counter
-        Transaction().counter += 1
+        transaction.counter += 1
 
         # Clean local cache
         for record in records:
             record._local_cache.pop(record.id, None)
 
         # Clean transaction cache
         for cache in Transaction().cache.values():
@@ -435,16 +445,24 @@
                     and field.left and field.right):
                 mptt.add(field.left)
                 mptt.add(field.right)
         fields_names = [n for n, f in cls._fields.items()
             if (not isinstance(f, fields.Function)
                 or isinstance(f, fields.MultiValue))
             and n not in mptt]
+
+        def _default_fields():
+            return {k.split('.', 1)[0] for k in default.keys()}
+        assert _default_fields() <= set(fields_names), (
+            f"Invalid default fields {_default_fields() - set(fields_names)} "
+            f"for {cls.__name__}")
         ids = list(map(int, records))
-        values = {d['id']: d for d in cls.read(ids, fields_names=fields_names)}
+        with without_check_access():
+            values = {
+                d['id']: d for d in cls.read(ids, fields_names=fields_names)}
         field_defs = cls.fields_get(fields_names=fields_names)
         default_values = cls.default_get(fields_names, with_rec_name=False)
         to_create = []
         for id_ in ids:
             data = convert_data(field_defs, values[id_], default_values)
             to_create.append(data)
         new_records = cls.create(to_create)
@@ -528,15 +546,15 @@
                 to_check[cls.__name__].add(local)
                 field = cls._fields[local]
                 if relate and hasattr(field, 'get_target'):
                     target = field.get_target()
                     target_order = [(relate, otype)]
                     check_order(target_order, target, to_check)
 
-        if transaction.user and transaction.context.get('_check_access'):
+        if transaction.user and transaction.check_access:
             to_check = defaultdict(set)
             check_domain(domain, cls, to_check)
             check_order(order, cls, to_check)
             for name, fields_names in to_check.items():
                 ModelAccess.check(name, 'read')
                 ModelFieldAccess.check(name, fields_names, 'read')
         if count:
@@ -576,15 +594,15 @@
     def _search_domain_active(cls, domain, active_test=True):
         # reduce_domain return a new instance so we can safety modify domain
         domain = reduce_domain(domain)
         # if the object has a field named 'active', filter out all inactive
         # records unless they were explicitely asked for
         if not ('active' in cls._fields
                 and active_test
-                and Transaction().context.get('active_test', True)):
+                and Transaction().active_records):
             return domain
 
         def process(domain):
             i = 0
             active_found = False
             while i < len(domain):
                 arg = domain[i]
@@ -602,15 +620,15 @@
                     domain.append(('active', '=', True))
                 else:
                     domain = ['AND', domain, ('active', '=', True)]
             return domain
         return process(domain)
 
     @classmethod
-    def count(cls):
+    def estimated_count(cls):
         "Returns the estimation of the number of records."
         count = cls._count_cache.get(cls.__name__)
         if count is None:
             count = cls.search([], count=True)
             cls._count_cache.set(cls.__name__, count)
         return count
 
@@ -1118,48 +1136,20 @@
             records = sum(to_write[0:None:2], [])
             translate(records, to_write_translations)
             count += len(records)
         return count
 
     @classmethod
     def check_xml_record(cls, records, values):
-        """
-        Check if a list of records and their corresponding fields are
-        originating from xml data. This is used by write and delete
-        functions: if the return value is True the records can be
-        written/deleted, False otherwise. The default behaviour is to
-        forbid any modification on records/fields originating from
-        xml. Values is the dictionary of written values. If values is
-        equal to None, no field by field check is performed, False is
-        returned as soon as one of the record comes from the xml.
-        """
         ModelData = Pool().get('ir.model.data')
         # Allow root user to update/delete
         if (Transaction().user == 0
                 or not ModelData.has_model(cls.__name__)):
-            return True
-        with Transaction().set_context(_check_access=False):
-            models_data = ModelData.search([
-                ('model', '=', cls.__name__),
-                ('db_id', 'in', list(map(int, records))),
-                ])
-            if not models_data:
-                return True
-            for model_data in models_data:
-                if values is None:
-                    if not model_data.noupdate:
-                        return False
-                else:
-                    if not model_data.values or model_data.noupdate:
-                        continue
-                    xml_values = ModelData.load_values(model_data.values)
-                    for key, val in values.items():
-                        if key in xml_values and val != xml_values[key]:
-                            return False
-        return True
+            return
+        ModelData.can_modify(records, values)
 
     @classmethod
     def validate(cls, records):
         pass
 
     @classmethod
     def validate_fields(cls, records, field_names):
@@ -1286,15 +1276,17 @@
             relations = set()
             if field._type in {'many2one', 'one2one', 'reference'}:
                 relations.update(getattr(r, field.name) for r in records)
             elif field._type in {'one2many', 'many2many'}:
                 relations.update(*(getattr(r, field.name) for r in records))
             else:
                 # Cache alignment is not a problem
-                relations = set(records)
+                relations = {
+                    r for r in records
+                    if getattr(r, field.name) is not None}
             relations.discard(None)
             return relations
 
         def validate_relation_domain(field, records, Relation, domain):
             relations = relation_domain(field, records)
             if relations:
                 for sub_relations in grouped_slice(relations):
@@ -1363,15 +1355,15 @@
 
         if field_names is None:
             field_names = cls._fields.keys()
         elif not isinstance(field_names, set):
             field_names = set(field_names)
         function_fields = {name for name, field in cls._fields.items()
             if isinstance(field, fields.Function)}
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             for field_name, field in cls._fields.items():
                 if (field_name not in field_names
                         and not (field.validation_depends & field_names)
                         and not (field.validation_depends & function_fields)):
                     continue
                 if isinstance(field, fields.Function):
                     continue
@@ -1788,16 +1780,16 @@
 
         model2ids = {}
         model2cache = {}
         # Read the data
         with Transaction().set_current_transaction(self._transaction), \
                 self._transaction.set_user(self._user), \
                 self._transaction.reset_context(), \
-                self._transaction.set_context(
-                    self._context, _check_access=False) as transaction:
+                self._transaction.set_context(self._context), \
+                without_check_access() as transaction:
             if (self.id in self._cache and name in self._cache[self.id]
                     and ffields.keys() <= set(self._cache[self.id]._keys())):
                 # Use values from cache
                 read_data = []
                 for id_ in islice(chain(islice(self._ids, index, None),
                             islice(self._ids, 0, max(index - 1, 0))),
                         read_size):
@@ -1854,15 +1846,15 @@
             field = self._fields[fname]
             if isinstance(field, fields.Function) and not field.setter:
                 continue
             if field._type in ('many2one', 'one2one', 'reference'):
                 if value:
                     if ((value.id is None or value.id < 0)
                             and field._type != 'reference'):
-                        value.save()
+                        raise _UnsavedRecordError(value)
                     if field._type == 'reference':
                         value = str(value)
                     else:
                         value = value.id
             if field._type in ('one2many', 'many2many'):
                 targets = value
                 if self.id is not None and self.id >= 0:
@@ -1945,26 +1937,34 @@
             for record in records:
                 assert isinstance(record, cls), (record, cls)
                 if (record._transaction != transaction
                         or user != record._user
                         or context != record._context):
                     latter.append(record)
                     continue
-                save_values[record] = record._save_values
+                while True:
+                    try:
+                        save_values[record] = record._save_values
+                        break
+                    except _UnsavedRecordError as e:
+                        warnings.warn(
+                            f"Using an unsaved relation record: {e.record}")
+                        e.record.save()
                 values[record] = record._values
                 record._values = None
                 if record.id is None or record.id < 0:
                     to_create.append(record)
                 elif save_values[record]:
                     to_write.append(record)
             try:
                 with Transaction().set_current_transaction(transaction), \
                         transaction.set_user(user), \
                         transaction.reset_context(), \
-                        transaction.set_context(context, _check_access=False):
+                        transaction.set_context(context), \
+                        without_check_access():
                     if to_create:
                         news = cls.create([save_values[r] for r in to_create])
                         for record, new in zip(to_create, news):
                             record._ids.remove(record.id)
                             record._id = new.id
                             record._ids.append(record.id)
                     if to_write:
```

### Comparing `trytond-6.6.8/trytond/model/modelview.py` & `trytond-6.8.0/trytond/model/modelview.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,49 @@
 from lxml import etree
 
 from trytond.cache import Cache
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.pool import Pool
 from trytond.pyson import PYSONEncoder
-from trytond.rpc import RPC
+from trytond.rpc import RPC, RPCReturnException
 from trytond.tools import is_instance_method
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access, without_check_access
 
 from . import fields
 from .fields import on_change_result
 from .model import Model
 
 __all__ = ['ModelView']
 
 
 class AccessButtonError(UserError):
     pass
 
 
+class ButtonActionException(RPCReturnException):
+    "Exception to launch action instead of executing button."
+
+    def __init__(self, action, value=None):
+        super().__init__()
+        pool = Pool()
+        ModelData = pool.get('ir.model.data')
+        Action = pool.get('ir.action')
+
+        module, fs_id = action.split('.')
+        action_id = Action.get_action_id(
+            ModelData.get_id(module, fs_id))
+        self.value = Action(action_id).get_action_value()
+        if value:
+            self.value.update(value)
+
+    def result(self):
+        return self.value
+
+
 def on_change(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         result = func(self, *args, **kwargs)
         assert result is None, func
         return self
     wrapper.on_change = True
@@ -607,15 +627,15 @@
             for depend in states.get('depends', []):
                 fields_attrs.setdefault(depend, {})
 
         if element.tag == 'link':
             link_name = element.attrib['name']
             action_id = ModelData.get_id(*link_name.split('.'))
             try:
-                with Transaction().set_context(_check_access=True):
+                with check_access():
                     action, = ActionWindow.search([('id', '=', action_id)])
             except ValueError:
                 action = None
             if (not action
                     or not action.res_model
                     or not ModelAccess.check(
                         action.res_model, 'read', raise_exception=False)):
@@ -653,15 +673,15 @@
             pool = Pool()
             ModelAccess = pool.get('ir.model.access')
             Button = pool.get('ir.model.button')
             ButtonClick = pool.get('ir.model.button.click')
             User = pool.get('res.user')
 
             transaction = Transaction()
-            check_access = transaction.context.get('_check_access')
+            check_access = transaction.check_access
 
             assert len(records) == len(set(records)), "Duplicate records"
 
             if (transaction.user != 0) and check_access:
                 ModelAccess.check(cls.__name__, 'read')
                 if issubclass(cls, ModelStorage):
                     # Check record rule access
@@ -676,28 +696,31 @@
                         raise AccessButtonError(
                             gettext('ir.msg_access_button_error',
                                 button=func.__name__,
                                 model=cls.__name__))
                 else:
                     ModelAccess.check(cls.__name__, 'write')
 
-            with Transaction().set_context(_check_access=False):
-                if (transaction.user != 0) and check_access:
-                    button_rules = Button.get_rules(
-                        cls.__name__, func.__name__)
-                    if button_rules:
-                        clicks = ButtonClick.register(
-                            cls.__name__, func.__name__, records)
-                        records = [r for r in records
-                            if all(br.test(r, clicks.get(r.id, []))
-                                for br in button_rules)]
-                # Reset click after filtering in case the button also has rules
-                names = Button.get_reset(cls.__name__, func.__name__)
-                if names:
-                    ButtonClick.reset(cls.__name__, names, records)
+            if (transaction.user != 0) and check_access:
+                button_rules = Button.get_rules(
+                    cls.__name__, func.__name__)
+                if button_rules:
+                    clicks = ButtonClick.register(
+                        cls.__name__, func.__name__, records)
+                    records = [r for r in records
+                        if all(br.test(r, clicks.get(r.id, []))
+                            for br in button_rules)]
+            # Reset click after filtering in case the button also has rules
+            names = Button.get_reset(cls.__name__, func.__name__)
+            if names:
+                ButtonClick.reset(cls.__name__, names, records)
+
+            if check_access and issubclass(cls, ModelStorage):
+                cls.log(records, 'button', func.__name__)
+            with without_check_access():
                 return func(cls, records, *args, **kwargs)
         return wrapper
 
     @staticmethod
     def button_action(action):
         def decorator(func):
             func = ModelView.button(func)
@@ -740,18 +763,34 @@
             method = getattr(self, 'on_change_%s' % fieldname, None)
             if method:
                 method()
         # XXX remove backward compatibility
         return [self._changed_values]
 
     def on_change_with(self, fieldnames):
+        from .modelstorage import ModelStorage
         changes = {}
         for fieldname in fieldnames:
+            field = self._fields[fieldname]
             method_name = 'on_change_with_%s' % fieldname
-            changes[fieldname] = getattr(self, method_name)()
+            value = getattr(self, method_name)()
+            if field._type in {'many2one', 'one2one', 'reference'}:
+                if isinstance(value, ModelStorage):
+                    if value.id and value.id >= 0:
+                        changes[f'%{fieldname}.'] = {
+                            'rec_name': value.rec_name,
+                            }
+                    if field._type == 'reference':
+                        value = str(value)
+                    else:
+                        value = value.id
+            elif field._type in {'one2many', 'many2many'}:
+                if isinstance(value, (list, tuple)):
+                    value = [int(r) for r in value]
+            changes[fieldname] = value
         return changes
 
     def on_change_notify(self):
         """Return a list of type and message couples.
         Available types are info, warning and error.
         """
         return []
```

### Comparing `trytond-6.6.8/trytond/model/multivalue.py` & `trytond-6.8.0/trytond/model/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/symbol.py` & `trytond-6.8.0/trytond/model/symbol.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/tree.py` & `trytond-6.8.0/trytond/model/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/union.py` & `trytond-6.8.0/trytond/model/union.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/model/workflow.py` & `trytond-6.8.0/trytond/model/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,21 @@
 
                 result = func(cls, filtered, *args, **kwargs)
                 if to_update:
                     for record in list(to_update.keys()):
                         current_state = getattr(record, cls._transition_state)
                         if current_state != to_update[record]:
                             del to_update[record]
-                    cls.write(list(to_update), {
+                    to_update = list(to_update)
+                    cls.write(to_update, {
                             cls._transition_state: state,
                             })
+                    cls.log(
+                        to_update, 'transition',
+                        f'{cls._transition_state}:{state}')
                 return result
             return wrapper
         return check_transition
 
     @classmethod
     def copy(cls, records, default=None):
         if default is None:
```

### Comparing `trytond-6.6.8/trytond/modules/__init__.py` & `trytond-6.8.0/trytond/modules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,44 +314,46 @@
         if update:
             # Ensure cache is clear for other instances
             Cache.clear_all()
             Cache.refresh_pool(transaction)
     logger.info('all modules loaded')
 
 
-def get_module_list():
+def get_module_list(with_test=False):
     module_list = set()
     if os.path.exists(MODULES_PATH) and os.path.isdir(MODULES_PATH):
         for file in os.listdir(MODULES_PATH):
             if file.startswith('.'):
                 continue
             if file == '__pycache__':
                 continue
             if os.path.isdir(OPJ(MODULES_PATH, file)):
                 module_list.add(file)
     update_egg_modules()
     module_list.update(EGG_MODULES.keys())
     module_list.add('ir')
     module_list.add('res')
-    module_list.add('tests')
+    if with_test:
+        module_list.add('tests')
     return list(module_list)
 
 
-def register_classes():
+def register_classes(with_test=False):
     '''
     Import modules to register the classes in the Pool
     '''
     import trytond.ir
     trytond.ir.register()
     import trytond.res
     trytond.res.register()
-    import trytond.tests
-    trytond.tests.register()
+    if with_test:
+        import trytond.tests
+        trytond.tests.register()
 
-    for node in create_graph(get_module_list()):
+    for node in create_graph(get_module_list(with_test=with_test)):
         module = node.name
         logger.info('%s:registering classes', module)
 
         if module in ('ir', 'res', 'tests'):
             MODULES.append(module)
             continue
```

### Comparing `trytond-6.6.8/trytond/pool.py` & `trytond-6.8.0/trytond/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,34 +80,36 @@
     def register(*classes, **kwargs):
         '''
         Register a list of classes
         '''
         module = kwargs['module']
         type_ = kwargs['type_']
         depends = set(kwargs.get('depends', []))
-        assert type_ in ('model', 'report', 'wizard')
+        assert type_ in {'model', 'report', 'wizard'}, (
+            f"{type_} is not a valid type_")
         for cls in classes:
             mpool = Pool.classes[type_][module]
-            assert cls not in mpool, cls
-            assert issubclass(cls.__class__, PoolMeta), cls
+            assert cls not in mpool, f"{cls} is already registered"
+            assert issubclass(cls.__class__, PoolMeta), (
+                f"{cls} is missing metaclass {PoolMeta}")
             mpool[cls] = depends
 
     @staticmethod
     def register_mixin(mixin, classinfo, module):
         Pool.classes_mixin[module].append((classinfo, mixin))
 
     @classmethod
     def start(cls):
         '''
         Start/restart the Pool
         '''
         with cls._lock:
             for classes in Pool.classes.values():
                 classes.clear()
-            register_classes()
+            register_classes(with_test=cls.test)
             cls._started = True
 
     @classmethod
     def stop(cls, database_name):
         '''
         Stop the Pool
         '''
@@ -229,15 +231,16 @@
                     continue
                 try:
                     previous_cls = self.get(cls.__name__, type=type_)
                     cls = type(
                         cls.__name__, (cls, previous_cls), {'__slots__': ()})
                 except KeyError:
                     pass
-                assert issubclass(cls, PoolBase), cls
+                assert issubclass(cls, PoolBase), (
+                    f"{cls} is not a subclass of {PoolBase}")
                 self.add(cls, type=type_)
                 classes[type_].append(cls)
         self._modules.append(module)
         return classes
 
     def setup(self, classes=None):
         logger.info('setup pool for "%s"', self.database_name)
```

### Comparing `trytond-6.6.8/trytond/protocols/dispatcher.py` & `trytond-6.8.0/trytond/protocols/dispatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 # -*- coding: utf-8 -*-
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import logging
 import pydoc
 import time
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
 from sql import Table
-from werkzeug.exceptions import abort
-from werkzeug.wrappers import Response
 
 from trytond import __version__, backend, security
 from trytond.config import config, get_hostname
 from trytond.exceptions import (
     ConcurrencyException, LoginException, RateLimitException, UserError,
     UserWarning)
+from trytond.rpc import RPCReturnException
 from trytond.tools import is_instance_method
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, TransactionError
 from trytond.worker import run_task
 from trytond.wsgi import app
 
-from .wrappers import with_pool
+from .wrappers import HTTPStatus, Response, abort, with_pool
 
 __all__ = ['register_authentication_service']
 
 logger = logging.getLogger(__name__)
 
 ir_configuration = Table('ir_configuration')
 ir_lang = Table('ir_lang')
@@ -188,19 +182,22 @@
         username, request.remote_addr, request.path)
 
     def duration():
         return (time.monotonic() - started) * 1000
     started = time.monotonic()
 
     retry = config.getint('database', 'retry')
-    for count in range(retry, -1, -1):
-        if count != retry:
+    count = 0
+    transaction_extras = {}
+    while True:
+        if count:
             time.sleep(0.02 * (retry - count))
-        with Transaction().start(pool.database_name, user,
-                readonly=rpc.readonly) as transaction:
+        with Transaction().start(
+                pool.database_name, user, readonly=rpc.readonly,
+                **transaction_extras) as transaction:
             try:
                 c_args, c_kwargs, transaction.context, transaction.timestamp \
                     = rpc.convert(obj, *args, **kwargs)
                 transaction.context['_request'] = request.context
                 meth = getattr(obj, method)
                 if (rpc.instantiate is None
                         or not is_instance_method(obj, method)):
@@ -209,21 +206,32 @@
                     assert rpc.instantiate == 0
                     inst = c_args.pop(0)
                     if hasattr(inst, method):
                         result = rpc.result(meth(inst, *c_args, **c_kwargs))
                     else:
                         result = [rpc.result(meth(i, *c_args, **c_kwargs))
                             for i in inst]
+            except TransactionError as e:
+                transaction.rollback()
+                transaction.tasks.clear()
+                e.fix(transaction_extras)
+                continue
             except backend.DatabaseOperationalError:
-                if count and not rpc.readonly:
+                if count < retry and not rpc.readonly:
                     transaction.rollback()
                     transaction.tasks.clear()
+                    count += 1
+                    logger.debug("Retry: %i", count)
                     continue
                 logger.exception(log_message, *log_args, duration())
                 raise
+            except RPCReturnException as e:
+                transaction.rollback()
+                transaction.tasks.clear()
+                result = e.result()
             except (ConcurrencyException, UserError, UserWarning,
                     LoginException):
                 logger.info(
                     log_message, *log_args, duration(),
                     exc_info=logger.isEnabledFor(logging.DEBUG))
                 raise
             except Exception:
```

### Comparing `trytond-6.6.8/trytond/protocols/jsonrpc.py` & `trytond-6.8.0/trytond/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/protocols/wrappers.py` & `trytond-6.8.0/trytond/protocols/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,41 @@
 from io import BytesIO
 
 try:
     from http import HTTPStatus
 except ImportError:
     from http import client as HTTPStatus
 
+from werkzeug import exceptions
 from werkzeug.datastructures import Authorization
-from werkzeug.exceptions import HTTPException, abort
+from werkzeug.exceptions import abort
+from werkzeug.utils import redirect
 from werkzeug.wrappers import Request as _Request
 from werkzeug.wrappers import Response
 
 from trytond import backend, security
 from trytond.config import config
 from trytond.exceptions import RateLimitException, UserError, UserWarning
 from trytond.pool import Pool
 from trytond.tools import cached_property
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
+
+__all__ = [
+    'HTTPStatus',
+    'Request',
+    'Response',
+    'abort',
+    'allow_null_origin',
+    'exceptions',
+    'redirect',
+    'set_max_request_size',
+    'user_application',
+    'with_pool',
+    'with_transaction',
+    ]
 
 logger = logging.getLogger(__name__)
 
 
 class Request(_Request):
 
     view_args = None
@@ -72,16 +88,18 @@
     def rpc_params(self):
         return
 
     @cached_property
     def authorization(self):
         authorization = super(Request, self).authorization
         if authorization is None:
-            header = self.environ.get('HTTP_AUTHORIZATION')
+            header = self.headers.get('Authorization')
             return parse_authorization_header(header)
+        elif authorization.type == 'session':
+            return parse_session(authorization.token)
         return authorization
 
     @cached_property
     def user_id(self):
         if not self.view_args:
             return None
         database_name = self.view_args.get('database_name')
@@ -92,17 +110,18 @@
             return None
         context = {'_request': self.context}
         if auth.type == 'session':
             user_id = security.check(
                 database_name, auth.get('userid'), auth.get('session'),
                 context=context)
         else:
+            parameters = getattr(auth, 'parameters', auth)
             try:
                 user_id = security.login(
-                    database_name, auth.username, auth, cache=False,
+                    database_name, auth.username, parameters, cache=False,
                     context=context)
             except RateLimitException:
                 abort(HTTPStatus.TOO_MANY_REQUESTS)
         return user_id
 
     @cached_property
     def context(self):
@@ -113,33 +132,41 @@
             'is_secure': self.is_secure,
             }
 
 
 def parse_authorization_header(value):
     if not value:
         return
-    if not isinstance(value, bytes):
-        value = value.encode('latin1')
+    if isinstance(value, bytes):
+        value = value.decode('latin1')
     try:
         auth_type, auth_info = value.split(None, 1)
         auth_type = auth_type.lower()
     except ValueError:
         return
-    if auth_type == b'session':
-        try:
-            username, userid, session = base64.b64decode(auth_info).split(
-                b':', 3)
-            userid = int(userid)
-        except Exception:
-            return
-        return Authorization('session', {
-                'username': username.decode("latin1"),
-                'userid': userid,
-                'session': session.decode("latin1"),
-                })
+    if auth_type == 'session':
+        return parse_session(auth_info)
+    else:
+        authorization = Authorization(auth_type)
+        authorization.token = auth_info
+        return authorization
+
+
+def parse_session(token):
+    try:
+        username, userid, session = (
+            base64.b64decode(token).decode().split(':', 3))
+        userid = int(userid)
+    except Exception:
+        return
+    return Authorization('session', {
+            'username': username,
+            'userid': userid,
+            'session': session,
+            })
 
 
 def set_max_request_size(size):
     def decorator(func):
         func.max_request_size = size
         return func
     return decorator
@@ -156,15 +183,15 @@
         database_list = Pool.database_list()
         pool = Pool(database_name)
         if database_name not in database_list:
             with Transaction().start(database_name, 0, readonly=True):
                 pool.init()
         try:
             return func(request, pool, *args, **kwargs)
-        except HTTPException:
+        except exceptions.HTTPException:
             logger.debug('%s', request, exc_info=True)
             raise
         except (UserError, UserWarning) as e:
             logger.debug('%s', request, exc_info=True)
             if request.rpc_method:
                 raise
             else:
@@ -229,30 +256,31 @@
 
     def decorator(func):
         @wraps(func)
         def wrapper(request, *args, **kwargs):
             pool = Pool()
             UserApplication = pool.get('res.user.application')
 
-            authorization = request.headers['Authorization']
-            try:
-                auth_type, auth_info = authorization.split(None, 1)
-                auth_type = auth_type.lower()
-            except ValueError:
+            authorization = request.authorization
+            if authorization is None:
+                header = request.headers.get('Authorization')
+                authorization = parse_authorization_header(header)
+            if authorization is None:
                 abort(HTTPStatus.UNAUTHORIZED)
-            if auth_type != 'bearer':
+            if authorization.type != 'bearer':
                 abort(HTTPStatus.FORBIDDEN)
 
-            application = UserApplication.check(auth_info, name)
+            token = getattr(authorization, 'token', '')
+            application = UserApplication.check(token, name)
             if not application:
                 abort(HTTPStatus.FORBIDDEN)
             transaction = Transaction()
             # TODO language
             with transaction.set_user(application.user.id), \
-                    transaction.set_context(_check_access=True):
+                    check_access():
                 response = func(request, *args, **kwargs)
             if not isinstance(response, Response) and json:
                 response = Response(json_.dumps(response, cls=JSONEncoder),
                     content_type='application/json')
             return response
         return wrapper
     return decorator
```

### Comparing `trytond-6.6.8/trytond/protocols/xmlrpc.py` & `trytond-6.8.0/trytond/protocols/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/pyson.py` & `trytond-6.8.0/trytond/pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/report/report.py` & `trytond-6.8.0/trytond/report/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 from trytond.i18n import gettext
 from trytond.pool import Pool, PoolBase
 from trytond.rpc import RPC
 from trytond.tools import slugify
 from trytond.transaction import Transaction
 from trytond.url import URLMixin
 
+try:
+    from trytond.tools import barcode
+except ImportError:
+    barcode = None
+try:
+    from trytond.tools import qrcode
+except ImportError:
+    qrcode = None
+
 warnings.simplefilter("ignore")
 import relatorio.reporting  # noqa: E402
 
 warnings.resetwarnings()
 try:
     from relatorio.templates.opendocument import MANIFEST, Manifest
 except ImportError:
@@ -88,14 +97,16 @@
 TIMEDELTA_DEFAULT_CONVERTER['m'] = TIMEDELTA_DEFAULT_CONVERTER['s'] * 60
 TIMEDELTA_DEFAULT_CONVERTER['h'] = TIMEDELTA_DEFAULT_CONVERTER['m'] * 60
 TIMEDELTA_DEFAULT_CONVERTER['d'] = TIMEDELTA_DEFAULT_CONVERTER['h'] * 24
 TIMEDELTA_DEFAULT_CONVERTER['w'] = TIMEDELTA_DEFAULT_CONVERTER['d'] * 7
 TIMEDELTA_DEFAULT_CONVERTER['M'] = TIMEDELTA_DEFAULT_CONVERTER['d'] * 30
 TIMEDELTA_DEFAULT_CONVERTER['Y'] = TIMEDELTA_DEFAULT_CONVERTER['d'] * 365
 
+NO_BREAKING_SPACE = '\u00A0'
+
 # For most OS maximum filename is 255 but Excel has a limitation which include
 # the path of 218.
 # As on Windows report is most likely to be open from
 # C:\Users\<username>\AppData\Local\Temp\tryton_<random>\ which has a length of
 # 56 with 12 for username and 8 for random. So 162 should be the maximum but we
 # round it to 100.
 REPORT_NAME_MAX_LENGTH = 100
@@ -259,14 +270,15 @@
         Model = pool.get(model)
         Config = pool.get('ir.configuration')
         Lang = pool.get('ir.lang')
         context = Transaction().context
 
         class TranslateModel(object):
             _languages = {}
+            __class__ = Model
 
             def __init__(self, id):
                 self.id = id
                 self._language = Transaction().language
 
             def set_lang(self, language=None):
                 if isinstance(language, Lang):
@@ -311,14 +323,18 @@
         report_context['format_date'] = cls.format_date
         report_context['format_datetime'] = cls.format_datetime
         report_context['format_timedelta'] = cls.format_timedelta
         report_context['format_currency'] = cls.format_currency
         report_context['format_number'] = cls.format_number
         report_context['format_number_symbol'] = cls.format_number_symbol
         report_context['datetime'] = datetime
+        if barcode:
+            report_context['barcode'] = cls.barcode
+        if qrcode:
+            report_context['qrcode'] = cls.qrcode
 
         def set_lang(language=None):
             if isinstance(language, Lang):
                 language = language.code
             Transaction().set_context(language=language)
         report_context['set_lang'] = set_lang
 
@@ -465,15 +481,15 @@
             text.append(time)
         text = sign + ' '.join(text)
         if value:
             if not any(values[-3:]):
                 # Add space if no time
                 text += ' '
             text += ('%.6f' % value)[1:]
-        return text
+        return text.replace(' ', NO_BREAKING_SPACE)
 
     @classmethod
     def format_currency(
             cls, value, lang, currency, symbol=True, grouping=True,
             digits=None):
         pool = Pool()
         Lang = pool.get('ir.lang')
@@ -498,14 +514,26 @@
         pool = Pool()
         Lang = pool.get('ir.lang')
         if lang is None:
             lang = Lang.get()
         return lang.format_number_symbol(
             value, symbol, digits=digits, grouping=grouping)
 
+    if barcode:
+        @classmethod
+        def barcode(cls, name, code, size=(), **kwargs):
+            image = barcode.generate_svg(name, code, **kwargs)
+            return (image, 'image/svg+xml', *size)
+
+    if qrcode:
+        @classmethod
+        def qrcode(cls, code, size=(), **kwargs):
+            image = qrcode.generate_svg(code, **kwargs)
+            return (image, 'image/svg+xml', *size)
+
 
 def get_email(report, record, languages):
     "Return email.mime and title from the report execution"
     pool = Pool()
     ActionReport = pool.get('ir.action.report')
     report_id = None
     if inspect.isclass(report) and issubclass(report, Report):
```

### Comparing `trytond-6.6.8/trytond/res/__init__.py` & `trytond-6.8.0/trytond/res/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/email_reset_password.html` & `trytond-6.8.0/trytond/res/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/group.py` & `trytond-6.8.0/trytond/res/group.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/group.xml` & `trytond-6.8.0/trytond/res/group.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/ir.py` & `trytond-6.8.0/trytond/res/ir.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/ir.xml` & `trytond-6.8.0/trytond/res/ir.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/res/ir.xml` & `trytond-6.8.0/trytond/res/ir.xml`

```diff
@@ -74,119 +74,14 @@
       <field name="model" search="[('model', '=', 'ir.action')]"/>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.access" id="access_ir_action_keyword">
-      <field name="model" search="[('model', '=', 'ir.action.keyword')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_keyword_admin">
-      <field name="model" search="[('model', '=', 'ir.action.keyword')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_report">
-      <field name="model" search="[('model', '=', 'ir.action.report')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_report_admin">
-      <field name="model" search="[('model', '=', 'ir.action.report')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window">
-      <field name="model" search="[('model', '=', 'ir.action.act_window')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window_admin">
-      <field name="model" search="[('model', '=', 'ir.action.act_window')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window_view">
-      <field name="model" search="[('model', '=', 'ir.action.act_window.view')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window_view_admin">
-      <field name="model" search="[('model', '=', 'ir.action.act_window.view')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window_domain">
-      <field name="model" search="[('model', '=', 'ir.action.act_window.domain')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_act_window_domain_admin">
-      <field name="model" search="[('model', '=', 'ir.action.act_window.domain')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_wizard">
-      <field name="model" search="[('model', '=', 'ir.action.wizard')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_wizard_admin">
-      <field name="model" search="[('model', '=', 'ir.action.wizard')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_url">
-      <field name="model" search="[('model', '=', 'ir.action.url')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_action_url_admin">
-      <field name="model" search="[('model', '=', 'ir.action.url')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
     <record model="ir.model.access" id="access_ir_model">
       <field name="model" search="[('model', '=', 'ir.model')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
@@ -194,91 +89,23 @@
       <field name="model" search="[('model', '=', 'ir.model')]"/>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.access" id="access_ir_model_field">
-      <field name="model" search="[('model', '=', 'ir.model.field')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_field_admin">
-      <field name="model" search="[('model', '=', 'ir.model.field')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_access">
-      <field name="model" search="[('model', '=', 'ir.model.access')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_access_ir_admin">
-      <field name="model" search="[('model', '=', 'ir.model.access')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_button">
-      <field name="model" search="[('model', '=', 'ir.model.button')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_button_admin">
-      <field name="model" search="[('model', '=', 'ir.model.button')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_button_rule">
-      <field name="model" search="[('model', '=', 'ir.model.button.rule')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_button_rule_admin">
-      <field name="model" search="[('model', '=', 'ir.model.button.rule')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_button_click">
-      <field name="model" search="[('model', '=', 'ir.model.button.click')]"/>
+    <record model="ir.model.access" id="access_ir_model_data">
+      <field name="model" search="[('model', '=', 'ir.model.data')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
-    <record model="ir.model.access" id="access_ir_model_button_click_admin">
-      <field name="model" search="[('model', '=', 'ir.model.button.click')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_model_data">
-      <field name="model" search="[('model', '=', 'ir.model.data')]"/>
+    <record model="ir.model.access" id="access_ir_model_log">
+      <field name="model" search="[('model', '=', 'ir.model.log')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_cron">
       <field name="model" search="[('model', '=', 'ir.cron')]"/>
@@ -351,29 +178,14 @@
       <field name="model" search="[('model', '=', 'ir.rule.group')]"/>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.access" id="access_ir_rule">
-      <field name="model" search="[('model', '=', 'ir.rule')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_rule_admin">
-      <field name="model" search="[('model', '=', 'ir.rule')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
     <record model="ir.model.access" id="access_ir_module">
       <field name="model" search="[('model', '=', 'ir.module')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
@@ -381,29 +193,14 @@
       <field name="model" search="[('model', '=', 'ir.module')]"/>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.access" id="access_ir_module_dependency">
-      <field name="model" search="[('model', '=', 'ir.module.dependency')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_module_dependency_admin">
-      <field name="model" search="[('model', '=', 'ir.module.dependency')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
     <record model="ir.model.access" id="access_ir_trigger">
       <field name="model" search="[('model', '=', 'ir.trigger')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
@@ -411,29 +208,14 @@
       <field name="model" search="[('model', '=', 'ir.trigger')]"/>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
-    <record model="ir.model.access" id="access_ir_trigger_log">
-      <field name="model" search="[('model', '=', 'ir.trigger.log')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_ir_trigger_log_admin">
-      <field name="model" search="[('model', '=', 'ir.trigger.log')]"/>
-      <field name="group" ref="group_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
     <record model="ir.rule.group" id="rule_group_menu">
       <field name="name">User in groups</field>
       <field name="model" search="[('model', '=', 'ir.ui.menu')]"/>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_menu1">
       <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
@@ -452,79 +234,14 @@
       <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_action"/>
     </record>
     <record model="ir.rule" id="rule_action2">
       <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_action"/>
     </record>
-    <record model="ir.rule.group" id="rule_group_action_keyword">
-      <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action.keyword')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_action_keyword1">
-      <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_keyword"/>
-    </record>
-    <record model="ir.rule" id="rule_action_keyword2">
-      <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_keyword"/>
-    </record>
-    <record model="ir.rule.group" id="rule_group_action_report">
-      <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action.report')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_action_report1">
-      <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_report"/>
-    </record>
-    <record model="ir.rule" id="rule_action_report2">
-      <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_report"/>
-    </record>
-    <record model="ir.rule.group" id="rule_group_action_act_window">
-      <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action.act_window')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_action_act_window1">
-      <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_act_window"/>
-    </record>
-    <record model="ir.rule" id="rule_action_act_window2">
-      <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_act_window"/>
-    </record>
-    <record model="ir.rule.group" id="rule_group_action_wizard">
-      <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action.wizard')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_action_wizard1">
-      <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_wizard"/>
-    </record>
-    <record model="ir.rule" id="rule_action_wizard2">
-      <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_wizard"/>
-    </record>
-    <record model="ir.rule.group" id="rule_group_action_url">
-      <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action.url')]"/>
-      <field name="global_p" eval="True"/>
-    </record>
-    <record model="ir.rule" id="rule_action_url1">
-      <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_url"/>
-    </record>
-    <record model="ir.rule" id="rule_action_url2">
-      <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
-      <field name="rule_group" ref="rule_group_action_url"/>
-    </record>
     <record model="ir.action-res.group" id="act_module_activate_upgrade_group_admin">
       <field name="action" ref="ir.act_module_activate_upgrade"/>
       <field name="group" ref="group_admin"/>
     </record>
     <record model="ir.action-res.group" id="act_translation_update_group_admin">
       <field name="action" ref="ir.act_translation_update"/>
       <field name="group" ref="group_admin"/>
```

### Comparing `trytond-6.6.8/trytond/res/locale/bg.po` & `trytond-6.8.0/trytond/res/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -414,34 +414,14 @@
 msgid "Model Button - Group"
 msgstr "Бутон модел - група"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/ca.po` & `trytond-6.8.0/trytond/res/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -391,34 +391,14 @@
 msgid "Model Button - Group"
 msgstr "Model Botó - Grup"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Usuari als grups"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Usuari als grups"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Usuari als grups"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Usuari als grups"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Usuari als grups"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Usuari als grups"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Qualsevol exportació"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Qualsevol exportació"
```

### Comparing `trytond-6.6.8/trytond/res/locale/cs.po` & `trytond-6.8.0/trytond/res/locale/fi.po`

 * *Files 5% similar despite different names*

```diff
@@ -144,18 +144,17 @@
 msgid "Access Menu"
 msgstr ""
 
 msgctxt "field:res.group,model_access:"
 msgid "Access Model"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.group,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:res.group,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:res.group,rule_groups:"
 msgid "Rules"
@@ -199,18 +198,17 @@
 msgid "Login"
 msgstr ""
 
 msgctxt "field:res.user,menu:"
 msgid "Menu Action"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:res.user,password:"
 msgid "Password"
 msgstr ""
 
 msgctxt "field:res.user,password_hash:"
 msgid "Password Hash"
@@ -305,18 +303,17 @@
 msgid "Login"
 msgstr ""
 
 msgctxt "field:res.user.warning,always:"
 msgid "Always"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user.warning,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:res.user.warning,user:"
 msgid "User"
 msgstr "Users"
 
 msgctxt "help:ir.export,groups:"
@@ -417,34 +414,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/de.po` & `trytond-6.8.0/trytond/res/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -392,34 +392,14 @@
 msgid "Model Button - Group"
 msgstr "Modell Button - Gruppe"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Benutzer in den Gruppen"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Benutzer in den Gruppen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Benutzer in den Gruppen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Benutzer in den Gruppen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Benutzer in den Gruppen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Benutzer in den Gruppen"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Alle Exporte"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Alle Exporte"
```

### Comparing `trytond-6.6.8/trytond/res/locale/es.po` & `trytond-6.8.0/trytond/res/locale/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -392,34 +392,14 @@
 msgid "Model Button - Group"
 msgstr "Modelo Botón - Grupo"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Usuario en grupos"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Usuario en grupos"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Usuario en grupos"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Usuario en grupos"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Usuario en grupos"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Usuario en grupos"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Cualquier exportación"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Cualquier exportación"
```

### Comparing `trytond-6.6.8/trytond/res/locale/es_419.po` & `trytond-6.8.0/trytond/res/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -396,34 +396,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/et.po` & `trytond-6.8.0/trytond/res/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -405,34 +405,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Kasutaja gruppides"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Kasutaja gruppides"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Kasutaja gruppides"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Kasutaja gruppides"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Kasutaja gruppides"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Kasutaja gruppides"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/fa.po` & `trytond-6.8.0/trytond/res/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -407,34 +407,14 @@
 msgid "Model Button - Group"
 msgstr "مدل دکمه - گروه"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/fi.po` & `trytond-6.8.0/trytond/res/locale/tr.po`

 * *Files 5% similar despite different names*

```diff
@@ -414,34 +414,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/fr.po` & `trytond-6.8.0/trytond/res/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -393,34 +393,14 @@
 msgid "Model Button - Group"
 msgstr "Bouton de modèle - Groupe"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Utilisateur dans les groupes"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Utilisateur dans les groupes"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Utilisateur dans les groupes"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Utilisateur dans les groupes"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Utilisateur dans les groupes"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Utilisateur dans les groupes"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "N'importe quel export"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "N'importe quel export"
```

### Comparing `trytond-6.6.8/trytond/res/locale/hu.po` & `trytond-6.8.0/trytond/res/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -396,34 +396,14 @@
 msgid "Model Button - Group"
 msgstr "Minta gomb- csoport"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/id.po` & `trytond-6.8.0/trytond/res/locale/id.po`

 * *Files 3% similar despite different names*

```diff
@@ -398,34 +398,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Pengguna dalam kelompok"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Pengguna dalam kelompok"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Pengguna dalam kelompok"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Pengguna dalam kelompok"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Pengguna dalam kelompok"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Pengguna dalam kelompok"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/it.po` & `trytond-6.8.0/trytond/res/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -404,34 +404,14 @@
 msgid "Model Button - Group"
 msgstr "Modello Biottone - Gruppo"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Qualsiasi esportazione"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Qualsiasi esportazione"
```

### Comparing `trytond-6.6.8/trytond/res/locale/lo.po` & `trytond-6.8.0/trytond/res/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -413,34 +413,14 @@
 msgid "Model Button - Group"
 msgstr "ແບບປຸ່ມ - ກຸ່ມ"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/lt.po` & `trytond-6.8.0/trytond/res/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -404,34 +404,14 @@
 msgid "Model Button - Group"
 msgstr "Modelio mygtukas - Grupė"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Naudotojo grupės"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Naudotojo grupės"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Naudotojo grupės"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Naudotojo grupės"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Naudotojo grupės"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Naudotojo grupės"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Bet koks eksportavimas"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Bet koks eksportavimas"
```

### Comparing `trytond-6.6.8/trytond/res/locale/nl.po` & `trytond-6.8.0/trytond/res/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -393,34 +393,14 @@
 msgid "Model Button - Group"
 msgstr "Modelknop - groep"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Gebruiker in groepen"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Gebruiker in groepen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Gebruiker in groepen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Gebruiker in groepen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Gebruiker in groepen"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Gebruiker in groepen"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Elke export"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Elke export"
```

### Comparing `trytond-6.6.8/trytond/res/locale/pl.po` & `trytond-6.8.0/trytond/res/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -394,34 +394,14 @@
 msgid "Model Button - Group"
 msgstr "Przycisk modelu - Grupa"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Użytkownik w grupach"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Użytkownik w grupach"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Użytkownik w grupach"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Użytkownik w grupach"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Użytkownik w grupach"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Użytkownik w grupach"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Dowolny eksport"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Dowolny eksport"
```

### Comparing `trytond-6.6.8/trytond/res/locale/pt.po` & `trytond-6.8.0/trytond/res/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -407,34 +407,14 @@
 msgid "Model Button - Group"
 msgstr "Modelo Botão - Grupo"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/ro.po` & `trytond-6.8.0/trytond/res/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 msgid "Export"
 msgstr "Export"
 
 msgctxt "field:ir.export-write-res.group,group:"
 msgid "Group"
 msgstr "Grup"
 
-#, fuzzy
 msgctxt "field:ir.model.button,groups:"
 msgid "Groups"
 msgstr "Grupuri"
 
 msgctxt "field:ir.model.button-res.group,button:"
 msgid "Button"
 msgstr "Buton"
@@ -75,15 +74,14 @@
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.model.button.rule,group:"
 msgid "Group"
 msgstr "Grup"
 
-#, fuzzy
 msgctxt "field:ir.rule.group,groups:"
 msgid "Groups"
 msgstr "Grupuri"
 
 msgctxt "field:ir.rule.group-res.group,group:"
 msgid "Group"
 msgstr "Grup"
@@ -100,15 +98,14 @@
 msgid "User Groups"
 msgstr "Grupuri de utilizatori"
 
 msgctxt "field:ir.sequence.type-res.group,sequence_type:"
 msgid "Sequence Type"
 msgstr "Tip de secvență"
 
-#, fuzzy
 msgctxt "field:ir.ui.menu,groups:"
 msgid "Groups"
 msgstr "Grupuri"
 
 msgctxt "field:ir.ui.menu-res.group,group:"
 msgid "Group"
 msgstr "Grup"
@@ -393,34 +390,14 @@
 msgid "Model Button - Group"
 msgstr "Buton Model - Grup"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Utilizator în grupuri"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Utilizator în grupuri"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Utilizator în grupuri"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Utilizator în grupuri"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Utilizator în grupuri"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Utilizator în grupuri"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Orice export"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Orice export"
```

### Comparing `trytond-6.6.8/trytond/res/locale/ru.po` & `trytond-6.8.0/trytond/res/locale/ru.po`

 * *Files 3% similar despite different names*

```diff
@@ -414,34 +414,14 @@
 msgid "Model Button - Group"
 msgstr "Кнопка модели - Группа"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/sl.po` & `trytond-6.8.0/trytond/res/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -413,34 +413,14 @@
 msgid "Model Button - Group"
 msgstr "Model Gumb - Skupina"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/tr.po` & `trytond-6.8.0/trytond/res/locale/cs.po`

 * *Files 8% similar despite different names*

```diff
@@ -144,17 +144,18 @@
 msgid "Access Menu"
 msgstr ""
 
 msgctxt "field:res.group,model_access:"
 msgid "Access Model"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:res.group,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:res.group,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:res.group,rule_groups:"
 msgid "Rules"
@@ -198,17 +199,18 @@
 msgid "Login"
 msgstr ""
 
 msgctxt "field:res.user,menu:"
 msgid "Menu Action"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:res.user,password:"
 msgid "Password"
 msgstr ""
 
 msgctxt "field:res.user,password_hash:"
 msgid "Password Hash"
@@ -303,17 +305,18 @@
 msgid "Login"
 msgstr ""
 
 msgctxt "field:res.user.warning,always:"
 msgid "Always"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user.warning,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:res.user.warning,user:"
 msgid "User"
 msgstr "Users"
 
 msgctxt "help:ir.export,groups:"
@@ -414,34 +417,14 @@
 msgid "Model Button - Group"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr ""
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr ""
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr ""
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr ""
```

### Comparing `trytond-6.6.8/trytond/res/locale/uk.po` & `trytond-6.8.0/trytond/res/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -393,34 +393,14 @@
 msgid "Model Button - Group"
 msgstr "Кнопка моделі - Група"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "Групи користувача"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "Групи користувача"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "Групи користувача"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "Групи користувача"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "Групи користувача"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "Групи користувача"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "Будь-який експорт"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "Будь-який експорт"
```

### Comparing `trytond-6.6.8/trytond/res/locale/zh_CN.po` & `trytond-6.8.0/trytond/res/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -392,34 +392,14 @@
 msgid "Model Button - Group"
 msgstr "模型按钮 - 组"
 
 msgctxt "model:ir.rule.group,name:rule_group_action"
 msgid "User in groups"
 msgstr "组中的用户"
 
-msgctxt "model:ir.rule.group,name:rule_group_action_act_window"
-msgid "User in groups"
-msgstr "组中的用户"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_keyword"
-msgid "User in groups"
-msgstr "组中的用户"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_report"
-msgid "User in groups"
-msgstr "组中的用户"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_url"
-msgid "User in groups"
-msgstr "组中的用户"
-
-msgctxt "model:ir.rule.group,name:rule_group_action_wizard"
-msgid "User in groups"
-msgstr "组中的用户"
-
 msgctxt "model:ir.rule.group,name:rule_group_export_any"
 msgid "Any export"
 msgstr "任意导出"
 
 msgctxt "model:ir.rule.group,name:rule_group_export_line_any"
 msgid "Any export"
 msgstr "任意导出"
```

### Comparing `trytond-6.6.8/trytond/res/message.xml` & `trytond-6.8.0/trytond/res/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/routes.py` & `trytond-6.8.0/trytond/res/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import logging
 import random
 import time
 
-from werkzeug.exceptions import abort
-
 from trytond.config import config
 from trytond.protocols.wrappers import (
-    allow_null_origin, with_pool, with_transaction)
+    abort, allow_null_origin, with_pool, with_transaction)
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 logger = logging.getLogger(__name__)
 
 
 @app.route('/<database_name>/user/application/', methods=['POST', 'DELETE'])
```

### Comparing `trytond-6.6.8/trytond/res/user.py` & `trytond-6.8.0/trytond/res/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,14 +302,15 @@
                     ]:
                 if test and password.lower() == test.lower():
                     raise PasswordError(gettext(message))
 
     @classmethod
     @ModelView.button
     def reset_password(cls, users, length=8, from_=None):
+        length = max(length, config.getint('password', 'length', default=0))
         for user in users:
             user.password_reset = gen_password(length=length)
             user.password_reset_expire = (
                 datetime.datetime.now() + datetime.timedelta(
                     seconds=config.getint('password', 'reset_timeout')))
             user.password = None
         cls.save(users)
```

### Comparing `trytond-6.6.8/trytond/res/user.xml` & `trytond-6.8.0/trytond/res/user.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/view/group_form.xml` & `trytond-6.8.0/trytond/res/view/group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/view/user_application_form.xml` & `trytond-6.8.0/trytond/res/view/user_application_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/view/user_config_start_form.xml` & `trytond-6.8.0/trytond/res/view/user_config_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/res/view/user_form.xml` & `trytond-6.8.0/trytond/res/view/user_form.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/res/view/user_form.xml` & `trytond-6.8.0/trytond/res/view/user_form.xml`

```diff
@@ -11,15 +11,15 @@
     <field name="login"/>
     <label name="email"/>
     <field name="email" widget="email"/>
     <label name="password"/>
     <field name="password" widget="password"/>
     <button name="reset_password" colspan="2"/>
   </group>
-  <field name="avatar" widget="image" height="100" width="100" xexpand="0"/>
+  <field name="avatar" widget="image" height="100" width="100" xexpand="0" border="circle"/>
   <notebook colspan="4">
     <page string="User" id="user">
       <separator name="signature" colspan="4"/>
       <field name="signature" colspan="4" widget="richtext"/>
     </page>
     <page string="Actions" id="actions">
       <label name="menu"/>
```

### Comparing `trytond-6.6.8/trytond/res/view/user_form_preferences.xml` & `trytond-6.8.0/trytond/res/view/user_form_preferences.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond-6.6.8/trytond/res/view/user_form_preferences.xml` & `trytond-6.8.0/trytond/res/view/user_form_preferences.xml`

```diff
@@ -7,15 +7,15 @@
     <field name="name"/>
     <newline/>
     <label name="email"/>
     <field name="email" widget="email"/>
     <label name="password"/>
     <field name="password" widget="password"/>
   </group>
-  <field name="avatar" widget="image" height="100" width="100" xexpand="0"/>
+  <field name="avatar" widget="image" height="100" width="100" xexpand="0" border="circle"/>
   <notebook colspan="4">
     <page string="User" id="user">
       <separator name="signature" colspan="4"/>
       <field name="signature" colspan="4" widget="richtext"/>
     </page>
     <page string="Actions" id="actions">
       <label name="menu"/>
```

### Comparing `trytond-6.6.8/trytond/rpc.py` & `trytond-6.8.0/trytond/rpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import copy
 import datetime as dt
 
+from trytond.exceptions import TrytonException
 from trytond.transaction import Transaction
 
-__all__ = ['RPC']
-
 
 class RPC(object):
     '''Define RPC behavior
 
     readonly: The transaction mode
     instantiate: The position or the slice of the arguments to be instanciated
     result: The function to transform the result
@@ -91,7 +90,14 @@
     def __init__(self, days=0, seconds=0):
         self.duration = dt.timedelta(days=days, seconds=seconds)
 
     def headers(self):
         return {
             'X-Tryton-Cache': int(self.duration.total_seconds()),
             }
+
+
+class RPCReturnException(TrytonException):
+    "Exception to return response instead of being raised"
+
+    def result(self):
+        pass
```

### Comparing `trytond-6.6.8/trytond/security.py` & `trytond-6.8.0/trytond/security.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/sendmail.py` & `trytond-6.8.0/trytond/sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/status.py` & `trytond-6.8.0/trytond/status.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/__init__.py` & `trytond-6.8.0/trytond/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 def register():
     from . import (
         access, copy_, export_data, field_binary, field_boolean, field_char,
         field_context, field_date, field_datetime, field_dict, field_float,
         field_function, field_integer, field_many2many, field_many2one,
         field_multiselection, field_numeric, field_one2many, field_one2one,
         field_reference, field_selection, field_text, field_time,
-        field_timedelta, history, import_data, mixin, model, modelsql,
-        modelstorage, modelview, mptt, multivalue, path, resource, rule, tree,
-        trigger, wizard, workflow)
+        field_timedelta, history, import_data, mixin, model, model_log,
+        modelsql, modelstorage, modelview, mptt, multivalue, path, resource,
+        rule, tree, trigger, wizard, workflow)
 
     access.register('tests')
     copy_.register('tests')
     export_data.register('tests')
     field_binary.register('tests')
     field_boolean.register('tests')
     field_char.register('tests')
@@ -45,14 +45,15 @@
     history.register('tests')
     import_data.register('tests')
     mixin.register('tests')
     model.register('tests')
     modelsql.register('tests')
     modelstorage.register('tests')
     modelview.register('tests')
+    model_log.register('tests')
     mptt.register('tests')
     multivalue.register('tests')
     path.register('tests')
     resource.register('tests')
     rule.register('tests')
     tree.register('tests')
     trigger.register('tests')
```

### Comparing `trytond-6.6.8/trytond/tests/access.py` & `trytond-6.8.0/trytond/tests/access.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/copy_.py` & `trytond-6.8.0/trytond/tests/copy_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/export_data.py` & `trytond-6.8.0/trytond/tests/export_data.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_binary.py` & `trytond-6.8.0/trytond/tests/field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_boolean.py` & `trytond-6.8.0/trytond/tests/field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_char.py` & `trytond-6.8.0/trytond/tests/field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_context.py` & `trytond-6.8.0/trytond/tests/field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_date.py` & `trytond-6.8.0/trytond/tests/field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_datetime.py` & `trytond-6.8.0/trytond/tests/field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_dict.py` & `trytond-6.8.0/trytond/tests/field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_float.py` & `trytond-6.8.0/trytond/tests/field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_function.py` & `trytond-6.8.0/trytond/tests/field_function.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-from trytond.model import ModelSQL, fields
+from trytond.model import ModelSQL, ModelStorage, fields
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 
 
+class FunctionDefinition(ModelStorage):
+    "Function Definition"
+    __name__ = 'test.function.definition'
+    function = fields.Function(
+        fields.Integer("Integer"),
+        'on_change_with_function', searcher='search_function')
+
+    def on_change_with_function(self, name=None):
+        return self.id
+
+    @classmethod
+    def search_function(cls, name, clause):
+        return [('id',) + tuple(clause[1:])]
+
+
 class FunctionAccessor(ModelSQL):
     "Function Accessor"
     __name__ = 'test.function.accessor'
 
     target = fields.Many2One('test.function.accessor.target', "Target")
     function = fields.Function(
         fields.Many2One('test.function.accessor.target', "Function"),
@@ -64,12 +79,13 @@
         if name == 'function2':
             index = cls.index_get_field('function1') + 1
         return index
 
 
 def register(module):
     Pool.register(
+        FunctionDefinition,
         FunctionAccessor,
         FunctionAccessorTarget,
         FunctionGetterContext,
         FunctionGetterLocalCache,
         module=module, type_='model')
```

### Comparing `trytond-6.6.8/trytond/tests/field_integer.py` & `trytond-6.8.0/trytond/tests/field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_many2many.py` & `trytond-6.8.0/trytond/tests/field_many2many.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,14 +86,37 @@
 class Many2ManySizeRelation(ModelSQL):
     'Many2Many Size Relation'
     __name__ = 'test.many2many_size.relation'
     origin = fields.Many2One('test.many2many_size', 'Origin')
     target = fields.Many2One('test.many2many_size.target', 'Target')
 
 
+class Many2ManyDomain(ModelSQL):
+    "Many2Many Domain"
+    __name__ = 'test.many2many_domain'
+    targets = fields.Many2Many(
+        'test.many2many_domain.relation', 'origin', 'target', "Targets",
+        domain=[
+            ('value', '=', 42),
+            ])
+
+
+class Many2ManyDomainTarget(ModelSQL):
+    "Many2Many Domain Target"
+    __name__ = 'test.many2many_domain.target'
+    value = fields.Integer("Value")
+
+
+class Many2ManyDomainRelation(ModelSQL):
+    "Many2Many Domain Relation"
+    __name__ = 'test.many2many_domain.relation'
+    origin = fields.Many2One('test.many2many_domain', "Origin")
+    target = fields.Many2One('test.many2many_domain.target', "Target")
+
+
 class Many2ManyFilter(ModelSQL):
     'Many2Many Filter Relation'
     __name__ = 'test.many2many_filter'
     targets = fields.Many2Many('test.many2many_filter.relation', 'origin',
         'target', 'Targets')
     filtered_targets = fields.Many2Many('test.many2many_filter.relation',
         'origin', 'target', 'Targets',
@@ -190,14 +213,17 @@
         Many2ManyRequiredRelation,
         Many2ManyReference,
         Many2ManyReferenceTarget,
         Many2ManyReferenceRelation,
         Many2ManySize,
         Many2ManySizeTarget,
         Many2ManySizeRelation,
+        Many2ManyDomain,
+        Many2ManyDomainTarget,
+        Many2ManyDomainRelation,
         Many2ManyFilter,
         Many2ManyFilterTarget,
         Many2ManyFilterRelation,
         Many2ManyFilterDomain,
         Many2ManyFilterDomainTarget,
         Many2ManyFilterDomainRelation,
         Many2ManyTree,
```

### Comparing `trytond-6.6.8/trytond/tests/field_many2one.py` & `trytond-6.8.0/trytond/tests/field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_multiselection.py` & `trytond-6.8.0/trytond/tests/field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_numeric.py` & `trytond-6.8.0/trytond/tests/field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_one2many.py` & `trytond-6.8.0/trytond/tests/field_one2many.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,31 @@
 
 class One2ManySizePYSONTarget(ModelSQL):
     'One2Many Size PYSON Target'
     __name__ = 'test.one2many_size_pyson.target'
     origin = fields.Many2One('test.one2many_size_pyson', 'Origin')
 
 
+class One2ManyDomain(ModelSQL):
+    "One2Many Domain"
+    __name__ = 'test.one2many_domain'
+    targets = fields.One2Many(
+        'test.one2many_domain.target', 'origin', "Targets",
+        domain=[
+            ('value', '=', 42),
+            ])
+
+
+class One2ManyDomainTarget(ModelSQL):
+    "One2Many Domain Target"
+    __name__ = 'test.one2many_domain.target'
+    origin = fields.Many2One('test.one2many_domain', "Origin")
+    value = fields.Integer("Value")
+
+
 class One2ManyFilter(ModelSQL):
     'One2Many Filter Relation'
     __name__ = 'test.one2many_filter'
     targets = fields.One2Many('test.one2many_filter.target', 'origin',
         'Targets')
     filtered_targets = fields.One2Many('test.one2many_filter.target', 'origin',
         'Filtered Targets', filter=[('value', '>', 2)])
@@ -138,14 +155,16 @@
         One2ManyRequiredTarget,
         One2ManyReference,
         One2ManyReferenceTarget,
         One2ManySize,
         One2ManySizeTarget,
         One2ManySizePYSON,
         One2ManySizePYSONTarget,
+        One2ManyDomain,
+        One2ManyDomainTarget,
         One2ManyFilter,
         One2ManyFilterTarget,
         One2ManyFilterDomain,
         One2ManyFilterDomainTarget,
         One2ManyContext,
         One2ManyContextTarget,
         module=module, type_='model')
```

### Comparing `trytond-6.6.8/trytond/tests/field_one2one.py` & `trytond-6.8.0/trytond/tests/field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_reference.py` & `trytond-6.8.0/trytond/tests/field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_selection.py` & `trytond-6.8.0/trytond/tests/field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_text.py` & `trytond-6.8.0/trytond/tests/field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_time.py` & `trytond-6.8.0/trytond/tests/field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/field_timedelta.py` & `trytond-6.8.0/trytond/tests/field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/history.py` & `trytond-6.8.0/trytond/tests/history.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/import_data.py` & `trytond-6.8.0/trytond/tests/import_data.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/import_data.xml` & `trytond-6.8.0/trytond/tests/import_data.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/mixin.py` & `trytond-6.8.0/trytond/tests/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/model.py` & `trytond-6.8.0/trytond/tests/model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/modelsql.py` & `trytond-6.8.0/trytond/tests/modelsql.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,14 +44,22 @@
 
 
 class ModelSQLTimestamp(ModelSQL):
     'Model to test timestamp'
     __name__ = 'test.modelsql.timestamp'
 
 
+class ModelSQLCreate(ModelSQL):
+    "Model to test creation"
+    __name__ = 'test.modelsql.create'
+
+    char = fields.Char("Char")
+    integer = fields.Integer("Integer")
+
+
 class ModelSQLFieldSet(ModelSQL):
     'Model to test field set'
     __name__ = 'test.modelsql.field_set'
 
     field = fields.Function(fields.Integer('Field'),
         'get_field', setter='set_field')
 
@@ -224,14 +232,15 @@
 def register(module):
     Pool.register(
         ModelSQLRead,
         ModelSQLReadTarget,
         ModelSQLReadContextID,
         ModelSQLRequiredField,
         ModelSQLTimestamp,
+        ModelSQLCreate,
         ModelSQLFieldSet,
         ModelSQLOne2Many,
         ModelSQLOne2ManyTarget,
         ModelSQLSearch,
         ModelSQLSearchOR2Union,
         ModelSQLSearchOR2UnionTarget,
         ModelSQLSearchOR2UnionOrder,
```

### Comparing `trytond-6.6.8/trytond/tests/modelstorage.py` & `trytond-6.8.0/trytond/tests/modelstorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,36 @@
 
 class ModelStorageRequired(ModelSQL):
     'Model stored'
     __name__ = 'test.modelstorage.required'
     name = fields.Char('Name', required=True)
 
 
+class ModelStorageSaveMany2One(ModelSQL):
+    "ModelStorage to test save with Many2One"
+    __name__ = 'test.modelstorage.save_m2o'
+    target = fields.Many2One('test.modelstorage.save_m2o.target', "Target")
+    targets = fields.One2Many(
+        'test.modelstorage.save_m2o.target', 'parent', "Targets")
+
+
+class ModelStorageSaveMany2OneTarget(ModelSQL):
+    "ModelStorage to test save with Many2One - Target"
+    __name__ = 'test.modelstorage.save_m2o.target'
+
+    parent = fields.Many2One('test.modelstorage.save_m2o', "Parent")
+    target = fields.Many2One(
+        'test.modelstorage.save_m2o.o2m_target.target', "Target")
+
+
+class ModelStorageSaveMany2OneTargetTarget(ModelSQL):
+    "ModelStorage to test save with Many2One - Target of Target"
+    __name__ = 'test.modelstorage.save_m2o.o2m_target.target'
+
+
 class ModelStorageSave2Many(ModelSQL):
     "Model Storage to test save with xxx2many"
     __name__ = 'test.modelstorage.save2many'
     targets = fields.One2Many(
         'test.modelstorage.save2many.target', 'parent', "Targets")
     m2m_targets = fields.Many2Many(
         'test.modelstorage.save2many.relation', 'parent', 'target', "Targets")
@@ -168,24 +190,36 @@
             ], "MultiSelection")
     many2one = fields.Many2One(
         'test.modelstorage.eval_environment', "Many2One")
     one2many = fields.One2Many(
         'test.modelstorage.eval_environment', 'many2one', "One2Many")
 
 
+class ModelStorageDomainNotRequired(ModelSQL):
+    "Model for domain on not required field"
+    __name__ = 'test.modelstorage.domain_not_required'
+
+    domain_not_required = fields.Integer(
+        "Domain Not Required", domain=[('domain_not_required', '>', 0)])
+
+
 def register(module):
     Pool.register(
         ModelStorage,
         ModelStorageRequired,
+        ModelStorageSaveMany2One,
+        ModelStorageSaveMany2OneTarget,
+        ModelStorageSaveMany2OneTargetTarget,
         ModelStorageSave2Many,
         ModelStorageSave2ManyTarget,
         ModelStorageSave2ManyRelation,
         ModelStorageContext,
         ModelStoragePYSONDomain,
         ModelStorageRelationDomain,
         ModelStorageRelationDomainTarget,
         ModelStorageRelationMultiDomain,
         ModelStorageRelationMultiDomainTarget,
         ModelStorageRelationDomain2,
         ModelStorageRelationDomain2Target,
         ModelStorageEvalEnvironment,
+        ModelStorageDomainNotRequired,
         module=module, type_='model')
```

### Comparing `trytond-6.6.8/trytond/tests/modelview.py` & `trytond-6.8.0/trytond/tests/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/modelview.xml` & `trytond-6.8.0/trytond/tests/modelview.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/mptt.py` & `trytond-6.8.0/trytond/tests/mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/multivalue.py` & `trytond-6.8.0/trytond/tests/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/path.py` & `trytond-6.8.0/trytond/tests/path.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/resource.py` & `trytond-6.8.0/trytond/tests/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/rule.py` & `trytond-6.8.0/trytond/tests/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/sequence.xml` & `trytond-6.8.0/trytond/tests/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_access.py` & `trytond-6.8.0/trytond/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_backend.py` & `trytond-6.8.0/trytond/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_bus.py` & `trytond-6.8.0/trytond/tests/test_bus.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_cache.py` & `trytond-6.8.0/trytond/tests/test_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     LRUDict, LRUDictTransaction, MemoryCache, freeze, unfreeze)
 from trytond.tests.test_tryton import (
     DB_NAME, USER, activate_module, with_transaction)
 from trytond.transaction import Transaction
 
 cache = MemoryCache('test.cache')
 cache_expire = MemoryCache('test.cache_expire', duration=1)
+cache_ignored_local_context = MemoryCache(
+    'test.cache.ignored.local', context_ignored_keys={'ignored'})
+cache_ignored_global_context = MemoryCache('test.cache.ignored.global')
 
 
 class CacheTestCase(unittest.TestCase):
     "Test Cache"
 
     def testFreeze(self):
         "Test freeze"
@@ -60,14 +63,36 @@
                                 },
                             },
                         }),
                 ]:
             with self.subTest(value=value):
                 self.assertEqual(unfreeze(value), result)
 
+    @with_transaction()
+    def test_ignored_context_key_global(self):
+        "Test global keys are ignored from context"
+        with Transaction().set_context(client='foo'):
+            cache_ignored_global_context.set('key', 0)
+
+        with Transaction().set_context(client='bar'):
+            value = cache_ignored_global_context.get('key')
+
+        self.assertEqual(value, 0)
+
+    @with_transaction()
+    def test_ignored_context_key_local(self):
+        "Test local keys are ignored from context"
+        with Transaction().set_context(ignored='foo'):
+            cache_ignored_local_context.set('key', 1)
+
+        with Transaction().set_context(ignored='bar'):
+            value = cache_ignored_local_context.get('key')
+
+        self.assertEqual(value, 1)
+
 
 class MemoryCacheTestCase(unittest.TestCase):
     "Test Cache"
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
```

### Comparing `trytond-6.6.8/trytond/tests/test_copy.py` & `trytond-6.8.0/trytond/tests/test_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,38 @@
                     'perm_write': False,
                     }])
 
         with self.assertRaises(AccessError):
             new_record, = TestAccess.copy(
                 [record], default={'name': 'nondefault'})
 
+    @with_transaction(context={'_check_access': True})
+    def test_copy_with_no_read_access(self):
+        "Test copying field with no read access"
+        pool = Pool()
+        Field = pool.get('ir.model.field')
+        FieldAccess = pool.get('ir.model.field.access')
+        TestAccess = pool.get('test.copy.access')
+
+        record, = TestAccess.create([{}])
+
+        field, = Field.search([
+                ('model.model', '=', 'test.copy.access'),
+                ('name', '=', 'name'),
+                ])
+        FieldAccess.create([{
+                    'field': field.id,
+                    'group': None,
+                    'perm_read': False,
+                    'perm_write': False,
+                    }])
+
+        new_record, = TestAccess.copy([record])
+        self.assertNotEqual(new_record.id, record.id)
+
 
 class CopyTranslationTestCase(TranslationTestCase):
     "Test copy translation"
 
     @with_transaction()
     def test_copy(self):
         "Test copy"
```

### Comparing `trytond-6.6.8/trytond/tests/test_exportdata.py` & `trytond-6.8.0/trytond/tests/test_exportdata.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_binary.py` & `trytond-6.8.0/trytond/tests/test_field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_boolean.py` & `trytond-6.8.0/trytond/tests/test_field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_char.py` & `trytond-6.8.0/trytond/tests/test_field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_context.py` & `trytond-6.8.0/trytond/tests/test_field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_date.py` & `trytond-6.8.0/trytond/tests/test_field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_datetime.py` & `trytond-6.8.0/trytond/tests/test_field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_depends.py` & `trytond-6.8.0/trytond/tests/test_field_depends.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_dict.py` & `trytond-6.8.0/trytond/tests/test_field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_float.py` & `trytond-6.8.0/trytond/tests/test_field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_function.py` & `trytond-6.8.0/trytond/tests/test_field_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,37 @@
     "Test Field Function"
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
     @with_transaction()
+    def test_definition(self):
+        pool = Pool()
+        Model = pool.get('test.function.definition')
+
+        definition = Model.function.definition(Model, 'en')
+        self.assertEqual(definition, {
+                'context': '{}',
+                'loading': 'lazy',
+                'name': 'function',
+                'on_change': [],
+                'on_change_with': [],
+                'readonly': True,
+                'required': False,
+                'states': '{}',
+                'type': 'integer',
+                'domain': '[]',
+                'searchable': True,
+                'sortable': False,
+                'help': '',
+                'string': 'Integer',
+                })
+
+    @with_transaction()
     def test_accessor(self):
         "Test accessing field on unsaved instance"
         pool = Pool()
         Model = pool.get('test.function.accessor')
         Target = pool.get('test.function.accessor.target')
 
         target = Target()
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_integer.py` & `trytond-6.8.0/trytond/tests/test_field_integer.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,18 @@
         self.assertEqual(integer.integer, 100)
 
     @with_transaction()
     def test_create_with_domain_invalid(self):
         "Test create integer with domain invalid"
         Integer = Pool().get('test.integer_domain')
 
-        with self.assertRaises(DomainValidationError):
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value "10" for field "Integer" '
+                'in ".*" of "Integer Domain"'):
             Integer.create([{
                         'integer': 10,
                         }])
 
     @with_transaction()
     def test_search_equals(self):
         "Test search integer equals"
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_many2many.py` & `trytond-6.8.0/trytond/tests/test_field_many2many.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
 
 from trytond.model.exceptions import (
-    RequiredValidationError, SizeValidationError)
+    DomainValidationError, RequiredValidationError, SizeValidationError)
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 
 
 class CommonTestCaseMixin:
 
     @with_transaction()
@@ -432,14 +432,44 @@
             Many2Many.create([{
                         'targets': [
                             ('create', [{}] * 4),
                             ],
                         }])
 
     @with_transaction()
+    def test_create_with_domain_valid(self):
+        "Test create many2many with valid domain"
+        pool = Pool()
+        Many2Many = pool.get('test.many2many_domain')
+
+        many2many, = Many2Many.create([{
+                    'targets': [
+                        ('create', [{'value': 42}]),
+                        ],
+                    }])
+
+        self.assertEqual(len(many2many.targets), 1)
+
+    @with_transaction()
+    def test_create_with_domain_invalid(self):
+        "Test create many2many with invalid domain"
+        pool = Pool()
+        Many2Many = pool.get('test.many2many_domain')
+
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value ".*,.*" for field "Targets" '
+                'in ".*" of "Many2Many Domain"'):
+            Many2Many.create([{
+                        'targets': [
+                            ('create', [{'value': 10}, {'value': None}]),
+                            ],
+                        }])
+
+    @with_transaction()
     def test_create_filter(self):
         "Test create many2many with filter"
         Many2Many = Pool().get('test.many2many_filter')
 
         filtered, = Many2Many.create([{
                     'targets': [
                         ('create', [{'value': x} for x in range(4)])],
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_many2one.py` & `trytond-6.8.0/trytond/tests/test_field_many2one.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
 
+from sql import Join
+
 from trytond.model.exceptions import DomainValidationError
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 
 
 class FieldMany2OneTestCase(unittest.TestCase):
     "Test Field Many2One"
@@ -72,15 +74,18 @@
     def test_create_with_domain_invalid(self):
         "Test create many2one with invalid domain"
         pool = Pool()
         Target = pool.get('test.many2one_target')
         Many2One = pool.get('test.many2one_domainvalidation')
         target, = Target.create([{'value': 1}])
 
-        with self.assertRaises(DomainValidationError):
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value "%s" for field "many2one" '
+                'in ".*" of "Many2One Domain Validation"' % target.rec_name):
             Many2One.create([{
                         'many2one': target.id,
                         }])
 
     @with_transaction()
     def test_create_with_domain_inactive(self):
         "Test create many2one with domain and inactive target"
@@ -140,45 +145,64 @@
 
         records = Many2One.search([], order=[('many2one.value', 'ASC')])
         values = [r.many2one.value for r in records]
 
         self.assertListEqual(values, [2, 3, 5])
 
     @with_transaction()
-    def _test_search_join(self, target_search):
+    def test_search_id(self):
+        "Test search on many2one id"
+        pool = Pool()
+        Target = pool.get('test.many2one_target')
+        Many2One = pool.get('test.many2one')
+
+        target, = Target.create([{}])
+        record, = Many2One.create([{'many2one': target.id}])
+
+        result = Many2One.search([('many2one', '=', target.id)])
+        self.assertListEqual(result, [record])
+
+    @with_transaction()
+    def _test_search_join(self, subquery_threshold=1_000):
+        from trytond.model.fields import many2one
+
         pool = Pool()
         Target = pool.get('test.many2one_target')
         Many2One = pool.get('test.many2one')
         target1, target2 = Target.create([
                 {'value': 1},
                 {'value': 2},
                 ])
         many2one1, many2one2 = Many2One.create([
                 {'many2one': target1},
                 {'many2one': target2},
                 ])
 
-        def set_target_search(target_search):
-            Many2One.many2one.target_search = target_search
-        self.addCleanup(set_target_search, Many2One.many2one.target_search)
-        set_target_search(target_search)
+        previous = many2one._subquery_threshold
+        many2one._subquery_threshold = subquery_threshold
+        self.addCleanup(setattr, many2one, '_subquery_threshold', previous)
 
         many2ones = Many2One.search([
                 ('many2one.value', '=', 1),
                 ])
-
         self.assertListEqual(many2ones, [many2one1])
 
+        return Many2One.search([
+                ('many2one.value', '=', 1),
+                ], query=True)
+
     def test_search_join(self):
         "Test search by many2one join"
-        self._test_search_join('join')
+        query = self._test_search_join(0)
+        self.assertIsInstance(query.from_[0], Join)
 
     def test_search_subquery(self):
         "Test search by many2one subquery"
-        self._test_search_join('subquery')
+        query = self._test_search_join()
+        self.assertNotIsInstance(query.from_[0], Join)
 
     @with_transaction()
     def test_context_attribute(self):
         "Test context on many2one attribute"
         pool = Pool()
         Many2One = pool.get('test.many2one_context')
         Target = pool.get('test.many2one_context.target')
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_multiselection.py` & `trytond-6.8.0/trytond/tests/test_field_multiselection.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,14 +315,53 @@
                 ])
 
         self.assertEqual(foo, [])
         self.assertEqual(baz, [selection])
         self.assertEqual(foo_baz, [])
         self.assertEqual(empty, [selection])
 
+    @with_transaction()
+    def test_read_string(self):
+        "Test reading value and string"
+        Selection = Pool().get('test.multi_selection')
+        foo, foo_bar, null = Selection.create([{
+                    'selects': ['foo'],
+                    }, {
+                    'selects': ['foo', 'bar'],
+                    }, {
+                    'selects': [],
+                    }])
+
+        foo_read, foo_bar_read, null_read = Selection.read(
+            [foo.id, foo_bar.id, null.id], ['selects:string'])
+
+        self.assertEqual(foo_read['selects:string'], ["Foo"])
+        self.assertEqual(foo_bar_read['selects:string'], ["Bar", "Foo"])
+        self.assertEqual(null_read['selects:string'], [])
+
+    @with_transaction()
+    def test_read_string_dynamic_selection(self):
+        "Test reading value and string of a dynamic selection"
+        Selection = Pool().get('test.multi_selection')
+        foo, bar, null = Selection.create([{
+                    'selects': ['foo'],
+                    'dyn_selects': ['foo', 'foobar'],
+                    }, {
+                    'dyn_selects': ['bar', 'baz'],
+                    }, {
+                    'dyn_selects': [],
+                    }])
+
+        foo_read, bar_read, null_read = Selection.read(
+            [foo.id, bar.id, null.id], ['dyn_selects:string'])
+
+        self.assertEqual(foo_read['dyn_selects:string'], ["Foo", "FooBar"])
+        self.assertEqual(bar_read['dyn_selects:string'], ["Bar", "Baz"])
+        self.assertEqual(null_read['dyn_selects:string'], [])
+
 
 @unittest.skipIf(
     backend.name != 'postgresql', 'jsonb only supported by postgresql')
 class FieldMultiSelectionJSONBTestCase(FieldMultiSelectionTestCase):
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_numeric.py` & `trytond-6.8.0/trytond/tests/test_field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_one2many.py` & `trytond-6.8.0/trytond/tests/test_field_one2many.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,19 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
 
+from trytond.config import config
 from trytond.model.exceptions import (
-    RequiredValidationError, SizeValidationError)
+    DomainValidationError, RequiredValidationError, SizeValidationError)
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 
 
-class CommonTestCaseMixin:
-
-    @with_transaction()
-    def test_set_reverse_field_instance(self):
-        "Test reverse field is set on instance"
-        One2Many = self.One2Many()
-        Target = self.One2ManyTarget()
-
-        record = One2Many()
-        target = Target()
-        record.targets = [target]
-
-        self.assertEqual(target.origin, record)
-
-    @with_transaction()
-    def test_save_reverse_field(self):
-        "Test save with reverse field set"
-        One2Many = self.One2Many()
-        Target = self.One2ManyTarget()
-
-        record = One2Many()
-        target = Target()
-        record.targets = [target]
-
-        record.save()
-
-    @with_transaction()
-    def test_save_reverse_field_saved(self):
-        "Test save with reverse field set on saved"
-        One2Many = self.One2Many()
-        Target = self.One2ManyTarget()
-
-        record = One2Many()
-        target = Target()
-        target.save()
-        record.targets = [target]
-
-        record.save()
-
-    @with_transaction()
-    def test_set_reverse_field_dict(self):
-        "Test reverse field is set on dict"
-        One2Many = self.One2Many()
-
-        record = One2Many()
-        record.targets = [{}]
-        target, = record.targets
-
-        self.assertEqual(target.origin, record)
-
-    @with_transaction()
-    def test_set_reverse_field_id(self):
-        "Test reverse field is set on id"
-        One2Many = self.One2Many()
-        Target = self.One2ManyTarget()
-
-        record = One2Many()
-        target = Target()
-        target.save()
-        record.targets = [target.id]
-        target, = record.targets
-
-        self.assertEqual(target.origin, record)
-
-    @with_transaction()
-    def test_create(self):
-        "Test create one2many"
-        One2Many = self.One2Many()
-
-        one2many, = One2Many.create([{
-                    'targets': [
-                        ('create', [{
-                                    'name': "Target",
-                                    }]),
-                        ],
-                    }])
-
-        self.assertEqual(len(one2many.targets), 1)
+class SearchTestCaseMixin:
 
     @with_transaction()
     def test_search_equals(self):
         "Test search one2many equals"
         One2Many = self.One2Many()
         one2many, = One2Many.create([{
                     'targets': [('create', [{'name': "Target"}])],
@@ -317,14 +241,106 @@
         one2manys = One2Many.search([
                 ('targets', 'not where', [('name', '=', "Target")]),
                 ])
 
         self.assertListEqual(one2manys, [])
 
     @with_transaction()
+    def test_search_strategy(self):
+        "Test search one2many with the right strategy"
+        One2Many = self.One2Many()
+        one2many, = One2Many.create([{
+                    'targets': [('create', [{'name': "Target"}])],
+                    }])
+
+        One2Many.search([('targets.name', '=', "Target")])
+        query = One2Many.search([('targets.name', '=', "Target")], query=True)
+        self.assertIn(self._strategy, str(query))
+
+
+class CommonTestCaseMixin:
+
+    @with_transaction()
+    def test_set_reverse_field_instance(self):
+        "Test reverse field is set on instance"
+        One2Many = self.One2Many()
+        Target = self.One2ManyTarget()
+
+        record = One2Many()
+        target = Target()
+        record.targets = [target]
+
+        self.assertEqual(target.origin, record)
+
+    @with_transaction()
+    def test_save_reverse_field(self):
+        "Test save with reverse field set"
+        One2Many = self.One2Many()
+        Target = self.One2ManyTarget()
+
+        record = One2Many()
+        target = Target()
+        record.targets = [target]
+
+        record.save()
+
+    @with_transaction()
+    def test_save_reverse_field_saved(self):
+        "Test save with reverse field set on saved"
+        One2Many = self.One2Many()
+        Target = self.One2ManyTarget()
+
+        record = One2Many()
+        target = Target()
+        target.save()
+        record.targets = [target]
+
+        record.save()
+
+    @with_transaction()
+    def test_set_reverse_field_dict(self):
+        "Test reverse field is set on dict"
+        One2Many = self.One2Many()
+
+        record = One2Many()
+        record.targets = [{}]
+        target, = record.targets
+
+        self.assertEqual(target.origin, record)
+
+    @with_transaction()
+    def test_set_reverse_field_id(self):
+        "Test reverse field is set on id"
+        One2Many = self.One2Many()
+        Target = self.One2ManyTarget()
+
+        record = One2Many()
+        target = Target()
+        target.save()
+        record.targets = [target.id]
+        target, = record.targets
+
+        self.assertEqual(target.origin, record)
+
+    @with_transaction()
+    def test_create(self):
+        "Test create one2many"
+        One2Many = self.One2Many()
+
+        one2many, = One2Many.create([{
+                    'targets': [
+                        ('create', [{
+                                    'name': "Target",
+                                    }]),
+                        ],
+                    }])
+
+        self.assertEqual(len(one2many.targets), 1)
+
+    @with_transaction()
     def test_write_write(self):
         "Test write one2many write"
         One2Many = self.One2Many()
         one2many, = One2Many.create([{
                     'targets': [('create', [{'name': "Foo"}])],
                     }])
         target, = one2many.targets
@@ -429,16 +445,18 @@
                     'targets': [('add', {target.id})],
                     })
 
         target, = one2many.targets
         self.assertIsNone(target.write_date)
 
 
-class FieldOne2ManyTestCase(unittest.TestCase, CommonTestCaseMixin):
+class FieldOne2ManyTestCase(
+        unittest.TestCase, CommonTestCaseMixin, SearchTestCaseMixin):
     "Test Field One2Many"
+    _strategy = 'IN'
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
     def One2Many(self):
         return Pool().get('test.one2many')
@@ -531,14 +549,44 @@
                     'limit': None,
                     'targets': [
                         ('create', [{}]),
                         ],
                     }])
 
     @with_transaction()
+    def test_create_with_domain_valid(self):
+        "Test create one2many with valid domain"
+        pool = Pool()
+        One2Many = pool.get('test.one2many_domain')
+
+        one2many, = One2Many.create([{
+                    'targets': [
+                        ('create', [{'value': 42}]),
+                        ],
+                    }])
+
+        self.assertEqual(len(one2many.targets), 1)
+
+    @with_transaction()
+    def test_create_with_domain_invalid(self):
+        "Test create one2many with invalid domain"
+        pool = Pool()
+        One2Many = pool.get('test.one2many_domain')
+
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value ".*,.*" for field "Targets" '
+                'in ".*" of "One2Many Domain"'):
+            One2Many.create([{
+                        'targets': [
+                            ('create', [{'value': 10}, {'value': None}]),
+                            ],
+                        }])
+
+    @with_transaction()
     def test_create_filter(self):
         "Test create one2many with filter"
         One2Many = Pool().get('test.one2many_filter')
 
         filtered, = One2Many.create([{
                     'targets': [
                         ('create', [{'value': x} for x in range(4)])],
@@ -642,19 +690,71 @@
 
         target, = Target.create([{}])
         record = Many2One(targets=[target.id])
 
         self.assertEqual(record.targets[0].context, record.id)
 
 
-class FieldOne2ManyReferenceTestCase(unittest.TestCase, CommonTestCaseMixin):
+class FieldOne2ManyReferenceTestCase(
+        unittest.TestCase, CommonTestCaseMixin, SearchTestCaseMixin):
     "Test Field One2Many Reference"
+    _strategy = 'IN'
+
+    @classmethod
+    def setUpClass(cls):
+        activate_module('tests')
+
+    def One2Many(self):
+        return Pool().get('test.one2many_reference')
+
+    def One2ManyTarget(self):
+        return Pool().get('test.one2many_reference.target')
+
+
+class FieldOne2ManyExistsTestCase(unittest.TestCase, SearchTestCaseMixin):
+    "Test Field One2Many when using EXISTS"
+    _strategy = 'EXISTS'
+
+    @classmethod
+    def setUpClass(cls):
+        activate_module('tests')
+
+    def setUp(self):
+        from trytond.model.fields import one2many
+        super().setUp()
+        previous = int(
+            config.get('database', 'subquery_threshold', default='1_000'))
+        one2many._subquery_threshold = 0
+        self.addCleanup(setattr, one2many, '_subquery_threshold', previous)
+
+    def One2Many(self):
+        return Pool().get('test.one2many')
+
+    def One2ManyTarget(self):
+        return Pool().get('test.one2many.target')
+
+
+class FieldOne2ManyReferenceExistsTestCase(
+        unittest.TestCase, SearchTestCaseMixin):
+    "Test Field One2Many Reference when using EXISTS"
+    _strategy = 'EXISTS'
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
+    def setUp(self):
+        from trytond.model.fields import one2many
+        super().setUp()
+        previous = int(
+            config.get('database', 'subquery_threshold', default='1_000'))
+        one2many._subquery_threshold = 0
+        self.addCleanup(setattr, one2many, '_subquery_threshold', previous)
+
     def One2Many(self):
         return Pool().get('test.one2many_reference')
 
     def One2ManyTarget(self):
         return Pool().get('test.one2many_reference.target')
+
+    def assert_strategy(self, query):
+        self.assertIn('EXISTS', query)
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_one2one.py` & `trytond-6.8.0/trytond/tests/test_field_one2one.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,18 @@
         pool = Pool()
         Target = pool.get('test.one2one.target')
         One2One = pool.get('test.one2one_domain')
         target, = Target.create([{
                     'name': "invalid domain",
                     }])
 
-        with self.assertRaises(DomainValidationError):
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value "%s" for field "One2One" '
+                'in ".*" of "One2One"' % target.rec_name):
             One2One.create([{
                         'one2one': target.id,
                         }])
 
     @with_transaction()
     def test_search_equals(self):
         "Test search one2one equals"
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_reference.py` & `trytond-6.8.0/trytond/tests/test_field_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,18 @@
         pool = Pool()
         Reference = pool.get('test.reference_domainvalidation')
         Target = pool.get('test.reference_domainvalidation.target')
         target = Target(value=1)
         target.save()
 
         reference = Reference(reference=target)
-        with self.assertRaises(DomainValidationError):
+        with self.assertRaisesRegexp(
+                DomainValidationError,
+                'The value "%s" for field "Reference" '
+                'in ".*" of "Reference Domain Validation"' % target.rec_name):
             reference.save()
 
     @with_transaction()
     def test_no_domain(self):
         "Test reference with no domain"
         pool = Pool()
         Reference = pool.get('test.reference_domainvalidation')
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_selection.py` & `trytond-6.8.0/trytond/tests/test_field_selection.py`

 * *Files 10% similar despite different names*

```diff
@@ -238,7 +238,46 @@
         Selection = Pool().get('test.selection')
 
         selection, = Selection.create([{
                     'dyn_select_static': '1',
                     }])
 
         self.assertEqual(selection.dyn_select_static_string, '1')
+
+    @with_transaction()
+    def test_read_string(self):
+        "Test reading value and string"
+        Selection = Pool().get('test.selection')
+
+        arabic, null = Selection.create([
+                {
+                    'select': 'arabic',
+                    },
+                {
+                    'select': None,
+                    },
+                ])
+        arabic_read, null_read = Selection.read(
+            [arabic.id, null.id], ['select:string'])
+
+        self.assertEqual(arabic_read['select:string'], 'Arabic')
+        self.assertEqual(null_read['select:string'], '')
+
+    @with_transaction()
+    def test_read_string_dynamic_selection(self):
+        "Test reading value and string of dynamic selection"
+        Selection = Pool().get('test.selection')
+
+        one, null = Selection.create([
+                {
+                    'select': 'arabic',
+                    'dyn_select': '1'
+                    },
+                {
+                    'select': None,
+                    },
+                ])
+        one_read, null_read = Selection.read(
+            [one.id, null.id], ['dyn_select:string'])
+
+        self.assertEqual(one_read['dyn_select:string'], '1')
+        self.assertEqual(null_read['dyn_select:string'], '')
```

### Comparing `trytond-6.6.8/trytond/tests/test_field_text.py` & `trytond-6.8.0/trytond/tests/test_field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_time.py` & `trytond-6.8.0/trytond/tests/test_field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_field_timedelta.py` & `trytond-6.8.0/trytond/tests/test_field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_filestore.py` & `trytond-6.8.0/trytond/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_history.py` & `trytond-6.8.0/trytond/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_i18n.py` & `trytond-6.8.0/trytond/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_importdata.py` & `trytond-6.8.0/trytond/tests/test_importdata.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_ir.py` & `trytond-6.8.0/trytond/tests/test_ir.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,33 @@
             ]
         for value, symbol, grouping, digits, result in test_data:
             self.assertEqual(
                 lang.currency(value, currency, symbol, grouping, digits),
                 result)
 
     @with_transaction()
+    def test_lang_currency_without_symbol(self):
+        "Test Lang.currency without symbol"
+        pool = Pool()
+        Lang = pool.get('ir.lang')
+        lang = Lang.get('en')
+        currency = Mock()
+        currency.digits = 2
+        currency.symbol = None
+        currency.code = 'USD'
+        test_data = [
+            (Decimal('10.50'), True, False, None, 'USD 10.50'),
+            (Decimal('10.50'), True, False, 4, 'USD 10.5000'),
+            ]
+        for value, symbol, grouping, digits, result in test_data:
+            self.assertEqual(
+                lang.currency(value, currency, symbol, grouping, digits),
+                result)
+
+    @with_transaction()
     def test_lang_format(self):
         "Test Lang.format"
         pool = Pool()
         Lang = pool.get('ir.lang')
         lang = Lang.get('en')
         test_data = [
             ('%i', 42, False, False, [], "42"),
@@ -158,25 +177,25 @@
     @with_transaction()
     def test_lang_strftime(self):
         "Test Lang.strftime"
         pool = Pool()
         Lang = pool.get('ir.lang')
         lang = Lang.get('en')
         test_data = [
-            (datetime.date(2016, 8, 3), '%d %B %Y', "03 August 2016"),
-            (datetime.time(8, 20), '%I:%M %p', "08:20 AM"),
+            (datetime.date(2016, 8, 3), '%d %B %Y', "03 August 2016"),
+            (datetime.time(8, 20), '%I:%M %p', "08:20 AM"),
             (datetime.datetime(2018, 11, 1, 14, 30), '%a %d %b %Y %I:%M %p',
-                "Thu 01 Nov 2018 02:30 PM"),
+                "Thu 01 Nov 2018 02:30 PM"),
             (datetime.date(2018, 11, 1), '%x', "11/01/2018"),
             (datetime.datetime(2018, 11, 1, 14, 30, 12),
-                '%x %X', "11/01/2018 14:30:12"),
+                '%x %X', "11/01/2018 14:30:12"),
             (datetime.datetime(2018, 11, 1, 14, 30, 12),
                 '%H:%M:%S', "14:30:12"),
             (datetime.datetime(2018, 11, 1, 14, 30, 12), None,
-                "11/01/2018 14:30:12"),
+                "11/01/2018 14:30:12"),
             ]
         for date, format_, result in test_data:
             self.assertEqual(lang.strftime(date, format_), result)
 
     @with_transaction()
     def test_lang_format_number(self):
         "Test Lang.format_number"
@@ -199,16 +218,16 @@
         Lang = pool.get('ir.lang')
         lang = Lang.get('en')
         unit = Mock()
         unit.symbol = 'Kg'
         unit.get_symbol = Mock()
         unit.get_symbol.return_value = 'Kg', 1
         test_data = [
-            (Decimal('10.50'), False, None, '10.50Kg'),
-            (Decimal('1000.50'), True, 4, '1,000.5000Kg'),
+            (Decimal('10.50'), False, None, '10.50 Kg'),
+            (Decimal('1000.50'), True, 4, '1,000.5000 Kg'),
             ]
         for value, grouping, digits, result in test_data:
             self.assertEqual(
                 lang.format_number_symbol(value, unit, digits, grouping),
                 result)
 
     @with_transaction()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond-6.6.8/trytond/tests/test_mixins.py` & `trytond-6.8.0/trytond/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_model.py` & `trytond-6.8.0/trytond/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_model_index.py` & `trytond-6.8.0/trytond/tests/test_model_index.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_modelsingleton.py` & `trytond-6.8.0/trytond/tests/test_modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_modelsql.py` & `trytond-6.8.0/trytond/tests/test_modelsql.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 from trytond import backend
 from trytond.exceptions import ConcurrencyException
 from trytond.model.exceptions import (
     ForeignKeyError, RequiredValidationError, SQLConstraintError)
 from trytond.model.modelsql import split_subquery_domain
 from trytond.pool import Pool
-from trytond.tests.test_tryton import activate_module, with_transaction
-from trytond.transaction import Transaction
+from trytond.tests.test_tryton import (
+    CONTEXT, DB_NAME, USER, activate_module, with_transaction)
+from trytond.transaction import Transaction, TransactionError
 
 
 class ModelSQLTestCase(unittest.TestCase):
     'Test ModelSQL'
 
     @classmethod
     def setUpClass(cls):
@@ -362,14 +363,109 @@
         transaction.timestamp.pop(str(record), None)
         ModelsqlTimestamp.write([record], {})
         transaction.commit()
         ModelsqlTimestamp.delete([record])
         transaction.commit()
 
     @with_transaction()
+    def test_create(self):
+        "Test create record"
+        pool = Pool()
+        Model = pool.get('test.modelsql.create')
+
+        m1, = Model.create([{
+                    'char': "Value 1",
+                    }])
+
+        self.assertTrue(m1.id)
+        self.assertEqual(m1.char, "Value 1")
+
+    def test_create_without_returning(self):
+        "Test create record without returning"
+        with patch.object(backend.Database, 'has_returning') as returning:
+            returning.return_value = False
+            with Transaction().start(DB_NAME, USER, context=CONTEXT):
+                pool = Pool()
+                Model = pool.get('test.modelsql.create')
+
+                m1, = Model.create([{
+                            'char': "Value 1",
+                            }])
+
+                self.assertTrue(m1.id)
+                self.assertEqual(m1.char, "Value 1")
+
+    @with_transaction()
+    def test_create_many_records(self):
+        "Test create many records"
+        pool = Pool()
+        Model = pool.get('test.modelsql.create')
+
+        # The order of the keys shouldn't matter
+        foo, bar, baz = Model.create([{
+                    'char': "Foo",
+                    'integer': 2
+                    }, {
+                    'integer': 4,
+                    'char': "Bar"
+                    }, {
+                    'char': "Baz"
+                    }])
+
+        self.assertEqual(foo.char, "Foo")
+        self.assertEqual(foo.integer, 2)
+        self.assertEqual(bar.char, "Bar")
+        self.assertEqual(bar.integer, 4)
+        self.assertEqual(baz.char, "Baz")
+        self.assertEqual(baz.integer, None)
+
+    def test_create_many_records_without_multirow_insert(self):
+        "Test create many records without multirow insert"
+        with patch.object(backend.Database, 'has_multirow_insert') as multirow:
+            multirow.return_value = False
+            with Transaction().start(DB_NAME, USER, context=CONTEXT):
+                pool = Pool()
+                Model = pool.get('test.modelsql.create')
+
+                m1, m2 = Model.create([{
+                            'char': "Value 1",
+                            }, {
+                            'char': "Value 2",
+                            }])
+
+                self.assertTrue(m1.id)
+                self.assertEqual(m1.char, "Value 1")
+                self.assertTrue(m2.id)
+                self.assertEqual(m2.char, "Value 2")
+                self.assertLess(m1.id, m2.id)
+
+    def test_create_many_without_returning_and_multirow_insert(self):
+        "Test create record without returning an multirow insert"
+        with patch.object(backend.Database, 'has_returning') as returning, \
+                patch.object(
+                    backend.Database, 'has_multirow_insert') as multirow:
+            returning.return_value = False
+            multirow.return_value = False
+            with Transaction().start(DB_NAME, USER, context=CONTEXT):
+                pool = Pool()
+                Model = pool.get('test.modelsql.create')
+
+                m1, m2 = Model.create([{
+                            'char': "Value 1",
+                            }, {
+                            'char': "Value 2",
+                            }])
+
+                self.assertTrue(m1.id)
+                self.assertEqual(m1.char, "Value 1")
+                self.assertTrue(m2.id)
+                self.assertEqual(m2.char, "Value 2")
+                self.assertLess(m1.id, m2.id)
+
+    @with_transaction()
     def test_create_field_set(self):
         'Test field.set in create'
         pool = Pool()
         Model = pool.get('test.modelsql.field_set')
 
         with patch.object(Model, 'set_field') as setter:
             records = Model.create([{'field': 1}])
@@ -667,19 +763,34 @@
     @with_transaction()
     def test_table_lock(self):
         "Test table lock"
         pool = Pool()
         Model = pool.get('test.modelsql.lock')
         transaction = Transaction()
 
-        with transaction.new_transaction():
-            Model.lock()
-            with transaction.new_transaction():
-                with self.assertRaises(backend.DatabaseOperationalError):
+        args1 = {}
+        while True:
+            with transaction.new_transaction(**args1):
+                try:
                     Model.lock()
+                except TransactionError as e:
+                    e.fix(args1)
+                    continue
+                with self.assertRaises(
+                        backend.DatabaseOperationalError):
+                    args2 = {}
+                    while True:
+                        with transaction.new_transaction(**args2):
+                            try:
+                                Model.lock()
+                            except TransactionError as e:
+                                e.fix(args2)
+                                continue
+                            break
+                break
 
     @with_transaction()
     def test_search_or_to_union(self):
         """
         Test searching for 'OR'-ed domain
         """
         pool = Pool()
```

### Comparing `trytond-6.6.8/trytond/tests/test_modelstorage.py` & `trytond-6.8.0/trytond/tests/test_modelstorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # repository contains the full copyright notices and license terms.
 
 import unittest
 
 from trytond.model import EvalEnvironment
 from trytond.model.exceptions import (
     AccessError, DomainValidationError, RequiredValidationError)
+from trytond.model.modelstorage import _UnsavedRecordError
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 
 
 class ModelStorageTestCase(unittest.TestCase):
     'Test ModelStorage'
 
     @classmethod
     def setUpClass(cls):
@@ -148,14 +149,86 @@
 
         bar.name = None
         foo.name = 'foo'
         with self.assertRaises(RequiredValidationError):
             ModelStorage.save([foo, bar])
 
     @with_transaction()
+    def test_many2one_save_raise_exception(self):
+        "Test _save_values raises _UnsavedRecordError on unsaved record"
+        pool = Pool()
+        ModelStorage = pool.get('test.modelstorage.save_m2o')
+        Target = pool.get('test.modelstorage.save_m2o.target')
+
+        record = ModelStorage()
+        record.target = target = Target()
+
+        with self.assertRaises(_UnsavedRecordError) as cm:
+            record._save_values
+
+        self.assertEqual(cm.exception.record, target)
+
+    @with_transaction()
+    def test_save_many2one_create(self):
+        "Test saving a record while creating a Many2One"
+        pool = Pool()
+        ModelStorage = pool.get('test.modelstorage.save_m2o')
+        Target = pool.get('test.modelstorage.save_m2o.target')
+
+        record = ModelStorage()
+        record.target = target = Target()
+        with self.assertWarnsRegex(
+                UserWarning, r"Using an unsaved relation record:"):
+            record.save()
+
+        self.assertIsNotNone(record.id)
+        self.assertIsNotNone(target.id)
+
+    @with_transaction()
+    def test_save_many2one_create_multi(self):
+        "Test saving multiple records while creating a M2O"
+        pool = Pool()
+        ModelStorage = pool.get('test.modelstorage.save_m2o')
+        Target = pool.get('test.modelstorage.save_m2o.target')
+
+        record1 = ModelStorage()
+        record1.target = target = Target()
+        record1.save()
+
+        record2 = ModelStorage()
+        record2.target = target
+        record2.save()
+
+        ModelStorage.save([record1, record2])
+
+        self.assertIsNotNone(record1.id)
+        self.assertIsNotNone(record2.id)
+        self.assertEqual(record1.target.id, record2.target.id)
+        self.assertNotEqual(record2.id, record1.id)
+
+    @with_transaction()
+    def test_save_many2one_in_one2many_create(self):
+        "Test saving a record while creating a M2O contained in a O2M"
+        pool = Pool()
+        ModelStorage = pool.get('test.modelstorage.save_m2o')
+        Target = pool.get('test.modelstorage.save_m2o.target')
+        M2OTarget = pool.get('test.modelstorage.save_m2o.o2m_target.target')
+
+        target = Target()
+        target.target = m2o_target = M2OTarget()
+        record = ModelStorage()
+        record.targets = [target]
+        record.save()
+
+        self.assertIsNotNone(record.id)
+        self.assertIsNotNone(m2o_target.id)
+        self.assertEqual(len(record.targets), 1)
+        self.assertEqual(record.targets[0].target, m2o_target)
+
+    @with_transaction()
     def test_save_one2many_create(self):
         "Test save one2many create"
         pool = Pool()
         ModelStorage = pool.get('test.modelstorage.save2many')
         Target = pool.get('test.modelstorage.save2many.target')
 
         record = ModelStorage()
@@ -505,23 +578,37 @@
         self.assertEqual(
             cm.exception.domain[0], [('relation2.value', '=', 'valid')])
         self.assertTrue(cm.exception.domain[1]['relation2'])
         self.assertTrue(
             cm.exception.domain[1]['relation2']['relation_fields']['value'])
 
     @with_transaction()
+    def test_domain_not_required_validation(self):
+        "Test domain validation on not required"
+        pool = Pool()
+        Model = pool.get('test.modelstorage.domain_not_required')
+        Model.create([{'domain_not_required': None}])
+
+    @with_transaction()
+    def test_domain_not_required_invalid(self):
+        "Test invalid domain on not required"
+        pool = Pool()
+        Model = pool.get('test.modelstorage.domain_not_required')
+
+        with self.assertRaises(DomainValidationError):
+            Model.create([{'domain_not_required': 0}])
+
+    @with_transaction()
     def test_check_xml_record_without_record(self):
         "Test check_xml_record without record"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         record, = Model.create([{}])
 
-        result = Model.check_xml_record([record], {'name': "Test"})
-
-        self.assertTrue(result)
+        Model.check_xml_record([record], {'name': "Test"})
 
     @with_transaction()
     def test_check_xml_record_with_record_no_matching_values(self):
         "Test check_xml_record with record and no matching values"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -531,17 +618,15 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': ModelData.dump_values({}),
                     'noupdate': False,
                     }])
 
-        result = Model.check_xml_record([record], {'name': "Test"})
-
-        self.assertTrue(result)
+        Model.check_xml_record([record], {'name': "Test"})
 
     @with_transaction()
     def test_check_xml_record_with_record_matching_values(self):
         "Test check_xml_record with record and matching values"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -551,17 +636,16 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': ModelData.dump_values({'name': "Foo"}),
                     'noupdate': False,
                     }])
 
-        result = Model.check_xml_record([record], {'name': "Bar"})
-
-        self.assertFalse(result)
+        with self.assertRaises(AccessError):
+            Model.check_xml_record([record], {'name': "Bar"})
 
     @with_transaction()
     def test_check_xml_record_with_record_matching_values_noupdate(self):
         "Test check_xml_record with record and matching values but noupdate"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -571,17 +655,15 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': ModelData.dump_values({'name': "Foo"}),
                     'noupdate': True,
                     }])
 
-        result = Model.check_xml_record([record], {'name': "Bar"})
-
-        self.assertTrue(result)
+        Model.check_xml_record([record], {'name': "Bar"})
 
     @with_transaction(user=0)
     def test_check_xml_record_with_record_matching_values_root(self):
         "Test check_xml_record with record with matching values as root"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -591,17 +673,15 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': ModelData.dump_values({'name': "Foo"}),
                     'noupdate': False,
                     }])
 
-        result = Model.check_xml_record([record], {'name': "Bar"})
-
-        self.assertTrue(result)
+        Model.check_xml_record([record], {'name': "Bar"})
 
     @with_transaction()
     def test_check_xml_record_with_record_no_values(self):
         "Test check_xml_record with record and no values"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -611,17 +691,16 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': None,
                     'noupdate': False,
                     }])
 
-        result = Model.check_xml_record([record], None)
-
-        self.assertFalse(result)
+        with self.assertRaises(AccessError):
+            Model.check_xml_record([record], None)
 
     @with_transaction()
     def test_check_xml_record_with_record_no_values_noupdate(self):
         "Test check_xml_record with record and no values but noupdate"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -631,17 +710,15 @@
                     'model': 'test.modelstorage',
                     'module': 'tests',
                     'db_id': record.id,
                     'values': None,
                     'noupdate': True,
                     }])
 
-        result = Model.check_xml_record([record], None)
-
-        self.assertTrue(result)
+        Model.check_xml_record([record], None)
 
     @with_transaction()
     def test_delete_clear_db_id_model_data_noupdate(self):
         "Test delete record clear DB id from model data"
         pool = Pool()
         Model = pool.get('test.modelstorage')
         ModelData = pool.get('ir.model.data')
@@ -764,15 +841,15 @@
         IrModelAccess.create([{
                     'model': model.id,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     }])
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             record = Model(name="Test")
             record.save()
 
     @with_transaction()
     def test_model_getattr_skip_check_access(self):
         "Test model getattr skips check access"
         pool = Pool()
@@ -786,11 +863,11 @@
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     }])
         record, = Model.create([{'name': "Test"}])
 
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             record = Model(record.id)
 
             self.assertEqual(record.name, "Test")
```

### Comparing `trytond-6.6.8/trytond/tests/test_modelview.py` & `trytond-6.8.0/trytond/tests/test_modelview.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # this repository contains the full copyright notices and license terms.
 
 import unittest
 from unittest.mock import patch
 
 from lxml import etree
 
-from trytond.model.exceptions import AccessButtonError, AccessError
+from trytond.model.exceptions import (
+    AccessButtonError, AccessError, ButtonActionException)
 from trytond.pool import Pool
 from trytond.pyson import Eval, PYSONDecoder, PYSONEncoder
 from trytond.tests.test_tryton import activate_module, with_transaction
 
 
 class ModelView(unittest.TestCase):
     "Test ModelView"
@@ -685,7 +686,31 @@
         pool = Pool()
         Depends = pool.get('test.modelview.states_depends')
 
         writeable_fields = Depends.fields_view_get(view_type='form')['fields']
         self.assertIn('bar', writeable_fields)
         self.assertIn('baz', writeable_fields)
         self.assertIn('quux', writeable_fields)
+
+    @with_transaction()
+    def test_button_action_exception(self):
+        "Test value of ButtonActionException"
+        exception = ButtonActionException('tests.test_modelview_button_action')
+        self.assertEqual(exception.value, {
+                **exception.value,
+                'name': "Test Button Action",
+                'url': 'http://www.example.com/',
+                })
+
+    @with_transaction()
+    def test_button_action_exception_value(self):
+        "Test value of ButtonActionException"
+        exception = ButtonActionException(
+            'tests.test_modelview_button_action',
+            value={
+                'url': 'https://www.example.net',
+                })
+        self.assertEqual(exception.value, {
+                **exception.value,
+                'name': "Test Button Action",
+                'url': 'https://www.example.net',
+                })
```

### Comparing `trytond-6.6.8/trytond/tests/test_mptt.py` & `trytond-6.8.0/trytond/tests/test_mptt.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # this repository contains the full copyright notices and license terms.
 import sys
 import unittest
 from unittest.mock import patch
 
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
-from trytond.transaction import Transaction
+from trytond.transaction import inactive_records
 
 from .test_tree import TreeTestCaseMixin
 
 
 class MPTTTestCase(TreeTestCaseMixin, unittest.TestCase):
     'Test Modified Preorder Tree Traversal'
     model_name = 'test.mptt'
@@ -20,15 +20,15 @@
     def setUpClass(cls):
         activate_module('tests')
 
     def check_tree(self, parent_id=None, left=-1, right=sys.maxsize):
         pool = Pool()
         Mptt = pool.get(self.model_name)
 
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             childs = Mptt.search([
                     ('parent', '=', parent_id),
                     ], order=[('left', 'ASC')])
         for child in childs:
             self.assertGreater(child.left, left,
                 msg='%s: left %d <= parent left %d' % (
                     child, child.left, left))
```

### Comparing `trytond-6.6.8/trytond/tests/test_multivalue.py` & `trytond-6.8.0/trytond/tests/test_multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_path.py` & `trytond-6.8.0/trytond/tests/test_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
 
 from trytond.pool import Pool
-from trytond.transaction import Transaction
+from trytond.transaction import inactive_records
 
 from .test_tree import TreeTestCaseMixin
 
 
 class PathTestCase(TreeTestCaseMixin, unittest.TestCase):
     "Test Path"
     model_name = 'test.path'
 
     def check_tree(self, parent_id=None):
         pool = Pool()
         Path = pool.get(self.model_name)
 
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             children = Path.search([
                     ('parent', '=', parent_id),
                     ])
         for child in children:
             if child.parent:
                 self.assertEqual(
                     child.path, '%s%s/' % (child.parent.path, child.id))
```

### Comparing `trytond-6.6.8/trytond/tests/test_protocols.py` & `trytond-6.8.0/trytond/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_pyson.py` & `trytond-6.8.0/trytond/tests/test_pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_report.py` & `trytond-6.8.0/trytond/tests/test_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,47 +15,47 @@
         activate_module('tests')
 
     @with_transaction()
     def test_format_datetime(self):
         "Test format datetime"
         self.assertEqual(Report.format_datetime(
                 datetime.datetime(2020, 7, 8, 13, 30, 00)),
-            '07/08/2020 13:30:00')
+            '07/08/2020 13:30:00')
 
     @with_transaction()
     def test_format_datetime_custom_format(self):
         "Test format datetime custom format"
         self.assertEqual(Report.format_datetime(
                 datetime.datetime(2020, 7, 8, 13, 30, 00),
                 format='%d %b %Y %I:%M %p'),
-            "08 Jul 2020 01:30 PM"),
+            "08 Jul 2020 01:30 PM"),
 
 
 def create_test_format_timedelta(i, in_, out):
     @with_transaction()
     def test(self):
         self.assertEqual(Report.format_timedelta(in_), out)
     test.__name__ = 'test_format_timedelta_%d' % i
     test.__doc__ = "test format_timedelta of %s" % in_
     return test
 
 
 for i, (in_, out) in enumerate([
             (None, ''),
             (datetime.timedelta(), '00:00'),
-            (datetime.timedelta(days=3, hours=5, minutes=30), '3d 05:30'),
-            (datetime.timedelta(weeks=48), '11M 6d'),
-            (datetime.timedelta(weeks=50), '11M 2w 6d'),
-            (datetime.timedelta(weeks=52), '12M 4d'),
+            (datetime.timedelta(days=3, hours=5, minutes=30), '3d 05:30'),
+            (datetime.timedelta(weeks=48), '11M 6d'),
+            (datetime.timedelta(weeks=50), '11M 2w 6d'),
+            (datetime.timedelta(weeks=52), '12M 4d'),
             (datetime.timedelta(days=360), '12M'),
-            (datetime.timedelta(days=364), '12M 4d'),
+            (datetime.timedelta(days=364), '12M 4d'),
             (datetime.timedelta(days=365), '1Y'),
-            (datetime.timedelta(days=366), '1Y 1d'),
+            (datetime.timedelta(days=366), '1Y 1d'),
             (datetime.timedelta(hours=2, minutes=5, seconds=10), '02:05:10'),
             (datetime.timedelta(minutes=15, microseconds=42),
                 '00:15:00.000042'),
-            (datetime.timedelta(days=1, microseconds=42), '1d .000042'),
+            (datetime.timedelta(days=1, microseconds=42), '1d .000042'),
             (datetime.timedelta(seconds=-1), '-00:00:01'),
-            (datetime.timedelta(days=-1, hours=-5, minutes=-30), '-1d 05:30'),
+            (datetime.timedelta(days=-1, hours=-5, minutes=-30), '-1d 05:30'),
             ]):
     test_method = create_test_format_timedelta(i, in_, out)
     setattr(ReportTestCase, test_method.__name__, test_method)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond-6.6.8/trytond/tests/test_res.py` & `trytond-6.8.0/trytond/tests/test_res.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_resource.py` & `trytond-6.8.0/trytond/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_routes.py` & `trytond-6.8.0/trytond/tests/test_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of this
 # repository contains the full copyright notices and license terms.
 
 import base64
 import json
 import unittest
 
-from werkzeug.test import Client
-from werkzeug.wrappers import Response
-
 from trytond.pool import Pool
-from trytond.tests.test_tryton import DB_NAME, activate_module, drop_db
+from trytond.protocols.wrappers import Response
+from trytond.tests.test_tryton import DB_NAME, Client, activate_module, drop_db
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 
 class RoutesTestCase(unittest.TestCase):
 
     @classmethod
@@ -31,15 +29,16 @@
     def tearDownClass(cls):
         super().tearDownClass()
         drop_db()
 
     @property
     def auth_headers(self):
         return {
-            'Authorization': b'Basic ' + base64.b64encode(b'admin:password'),
+            'Authorization': (
+                'Basic ' + base64.b64encode(b'admin:password').decode()),
             }
 
     def data_url(self, model):
         return '/%(database)s/data/%(model)s' % {
             'database': DB_NAME,
             'model': model,
             }
```

### Comparing `trytond-6.6.8/trytond/tests/test_rpc.py` & `trytond-6.8.0/trytond/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_rule.py` & `trytond-6.8.0/trytond/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_sendmail.py` & `trytond-6.8.0/trytond/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_sequence.py` & `trytond-6.8.0/trytond/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_tools.py` & `trytond-6.8.0/trytond/tests/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import datetime as dt
 import doctest
 import sys
 import unittest
+from io import BytesIO
 
 import sql
 import sql.operators
 
 from trytond.tools import (
     decimal_, escape_wildcard, file_open, firstline, grouped_slice,
     is_full_text, is_instance_method, lstrip_wildcard, reduce_domain,
@@ -18,14 +19,23 @@
 from trytond.tools.domain_inversion import (
     concat, domain_inversion, eval_domain, extract_reference_models,
     localize_domain, merge, parse, prepare_reference_domain, simplify,
     unique_value)
 from trytond.tools.immutabledict import ImmutableDict
 from trytond.tools.string_ import LazyString, StringPartitioned
 
+try:
+    from trytond.tools import barcode
+except ImportError:
+    barcode = None
+try:
+    from trytond.tools import qrcode
+except ImportError:
+    qrcode = None
+
 
 class ToolsTestCase(unittest.TestCase):
     'Test tools'
     table = sql.Table('test')
 
     def test_reduce_ids_empty(self):
         'Test reduce_ids empty list'
@@ -728,14 +738,29 @@
 
         domain = [['a.id', '=', 1, 'model']]
         self.assertEqual(unique_value(domain), (True, 'a.id', ['model', 1]))
 
         domain = [['a.b.id', '=', 1, 'model']]
         self.assertEqual(unique_value(domain), (False, None, None))
 
+        domain = [['a', 'in', [1]]]
+        self.assertEqual(unique_value(domain), (True, 'a', 1))
+
+        domain = [['a', 'in', [1, 2]]]
+        self.assertEqual(unique_value(domain), (False, None, None))
+
+        domain = [['a', 'in', []]]
+        self.assertEqual(unique_value(domain), (False, None, None))
+
+        domain = [['a.b', 'in', [1]]]
+        self.assertEqual(unique_value(domain), (False, None, None))
+
+        domain = [['a.id', 'in', [1], 'model']]
+        self.assertEqual(unique_value(domain), (True, 'a.id', ['model', 1]))
+
     def test_evaldomain(self):
         domain = [['x', '>', 5]]
         self.assertTrue(eval_domain(domain, {'x': 6}))
         self.assertFalse(eval_domain(domain, {'x': 4}))
 
         domain = [['x', '>', None]]
         self.assertFalse(eval_domain(domain, {'x': dt.date.today()}))
@@ -1008,10 +1033,44 @@
             ['x.y', 'like', 'A%', 'model_A'],
             ['x.z', 'like', 'B%', 'model_B']]
         self.assertEqual(
             extract_reference_models(domain, 'x'), {'model_A', 'model_B'})
         self.assertEqual(extract_reference_models(domain, 'y'), set())
 
 
+@unittest.skipUnless(barcode, "required barcode")
+class BarcodeTestCase(unittest.TestCase):
+    "Test barcode module"
+
+    def test_generate_svg(self):
+        "Test generate SVG"
+        image = barcode.generate_svg('ean', "8749903790831")
+        self.assertIsInstance(image, BytesIO)
+        self.assertIsNotNone(image.getvalue())
+
+    def test_generate_png(self):
+        "Test generate PNG"
+        image = barcode.generate_png('ean', "8749903790831")
+        self.assertIsInstance(image, BytesIO)
+        self.assertIsNotNone(image.getvalue())
+
+
+@unittest.skipUnless(qrcode, "required qrcode")
+class QRCodeTestCase(unittest.TestCase):
+    "Test qrcode module"
+
+    def test_generate_svg(self):
+        "Test generate SVG"
+        image = qrcode.generate_svg("Tryton")
+        self.assertIsInstance(image, BytesIO)
+        self.assertIsNotNone(image.getvalue())
+
+    def test_generate_png(self):
+        "Test generate PNG"
+        image = qrcode.generate_png("Tryton")
+        self.assertIsInstance(image, BytesIO)
+        self.assertIsNotNone(image.getvalue())
+
+
 def load_tests(loader, tests, pattern):
     tests.addTest(doctest.DocTestSuite(decimal_))
     return tests
```

### Comparing `trytond-6.6.8/trytond/tests/test_transaction.py` & `trytond-6.8.0/trytond/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_tree.py` & `trytond-6.8.0/trytond/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_trigger.py` & `trytond-6.8.0/trytond/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_tryton.py` & `trytond-6.8.0/trytond/tests/test_tryton.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,43 +19,54 @@
 try:
     import pkg_resources
 except ImportError:
     pkg_resources = None
 
 from lxml import etree
 from sql import Table
+from werkzeug.test import Client
 
 from trytond import backend
 from trytond.cache import Cache
 from trytond.config import config, parse_uri
 from trytond.model import (
     ModelSingleton, ModelSQL, ModelStorage, ModelView, Workflow, fields)
 from trytond.model.fields import Function
 from trytond.pool import Pool, isregisteredby
 from trytond.pyson import PYSONDecoder, PYSONEncoder
 from trytond.tools import file_open, find_dir, is_instance_method
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, TransactionError
 from trytond.wizard import StateAction, StateView
 
-__all__ = ['DB_NAME', 'USER', 'CONTEXT',
-    'activate_module', 'ModuleTestCase', 'with_transaction',
-    'doctest_setup', 'doctest_teardown', 'doctest_checker', 'load_doc_tests']
+__all__ = [
+    'CONTEXT',
+    'Client',
+    'DB_NAME',
+    'ModuleTestCase',
+    'USER',
+    'activate_module',
+    'doctest_checker',
+    'doctest_setup',
+    'doctest_teardown',
+    'load_doc_tests',
+    'with_transaction',
+    ]
 
+Pool.test = True
 Pool.start()
 USER = 1
 CONTEXT = {}
 if 'DB_NAME' in os.environ:
     DB_NAME = os.environ['DB_NAME']
 elif backend.name == 'sqlite':
     DB_NAME = ':memory:'
 else:
     DB_NAME = 'test_' + str(int(time.time()))
 os.environ['DB_NAME'] = DB_NAME
 DB_CACHE = os.environ.get('DB_CACHE')
-Pool.test = True
 
 
 def activate_module(modules, lang='en'):
     '''
     Activate modules for the tested database
     '''
     if isinstance(modules, str):
@@ -199,25 +210,33 @@
         return True
 
 
 def with_transaction(user=1, context=None):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            transaction = Transaction()
-            with transaction.start(DB_NAME, user, context=context):
-                try:
-                    result = func(*args, **kwargs)
-                finally:
-                    transaction.rollback()
-                    # Clear remaining tasks
-                    transaction.tasks.clear()
-                    # Drop the cache as the transaction is rollbacked
-                    Cache.drop(DB_NAME)
-                return result
+            extras = {}
+            while True:
+                with Transaction().start(
+                        DB_NAME, user, context=context,
+                        **extras) as transaction:
+                    try:
+                        result = func(*args, **kwargs)
+                    except TransactionError as e:
+                        transaction.rollback()
+                        transaction.tasks.clear()
+                        e.fix(extras)
+                        continue
+                    finally:
+                        transaction.rollback()
+                        # Clear remaining tasks
+                        transaction.tasks.clear()
+                        # Drop the cache as the transaction is rollbacked
+                        Cache.drop(DB_NAME)
+                    return result
         return wrapper
     return decorator
 
 
 class ModuleTestCase(unittest.TestCase):
     'Trytond Test Case'
     module = None
@@ -315,16 +334,20 @@
                 validator.assertValid(tree)
 
                 tree_root = tree.getroottree().getroot()
 
                 for element in tree_root.iter():
                     with self.subTest(element=element):
                         if element.tag in {
-                                'field', 'label', 'separator', 'group'}:
-                            for attr in ['name', 'icon', 'symbol']:
+                                'field', 'label', 'separator', 'group',
+                                'page'}:
+                            attrs = ['name']
+                            if element.tag == 'field':
+                                attrs += ['icon', 'symbol']
+                            for attr in attrs:
                                 field = element.get(attr)
                                 if field:
                                     self.assertIn(field, res['fields'].keys(),
                                         msg='Missing field: %s in %s' % (
                                             field, Model.__name__))
                         if element.tag == 'button':
                             button_name = element.get('name')
@@ -431,15 +454,19 @@
             if not isregisteredby(model, self.module):
                 continue
             for fname, field in model._fields.items():
                 with self.subTest(model=mname, field=fname):
                     for attribute in [
                             'depends', 'on_change', 'on_change_with',
                             'selection_change_with', 'autocomplete']:
-                        depends = getattr(field, attribute, [])
+                        depends = getattr(field, attribute, set())
+                        if attribute == 'depends':
+                            depends |= field.display_depends
+                            depends |= field.edition_depends
+                            depends |= field.validation_depends
                         qualname = '"%s"."%s"."%s"' % (mname, fname, attribute)
                         for depend in depends:
                             test_depend_exists(model, depend, qualname)
                             test_missing_relation(depend, depends, qualname)
                             test_parent_empty(depend, qualname)
                             if attribute != 'depends':
                                 test_missing_parent(
@@ -480,14 +507,16 @@
                         # if pattern is not defined on the model
                         except AttributeError:
                             pass
                     else:
                         getattr(model, attr)()
                 elif attr.startswith('order_'):
                     model.search([], order=[(attr[len('order_'):], None)])
+                elif attr.startswith('domain_'):
+                    model.search([(attr[len('domain_'):], '=', None)])
                 elif any(attr.startswith(p) for p in [
                             'on_change_',
                             'on_change_with_',
                             'autocomplete_']):
                     record = model()
                     getattr(record, attr)()
 
@@ -738,14 +767,17 @@
                         self.assertTrue(getattr(model, func_name, None),
                             msg="Missing method '%(func_name)s' "
                             "on model '%(model)s' for field '%(field)s'" % {
                                 'func_name': func_name,
                                 'model': model.__name__,
                                 'field': field_name,
                                 })
+                        if func_name == field.searcher:
+                            getattr(model, field.searcher)(
+                                field_name, (field_name, '=', None))
 
     @with_transaction()
     def test_ir_action_window(self):
         'Test action windows are correctly defined'
         pool = Pool()
         ModelData = pool.get('ir.model.data')
         ActionWindow = pool.get('ir.action.act_window')
```

### Comparing `trytond-6.6.8/trytond/tests/test_union.py` & `trytond-6.8.0/trytond/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_user.py` & `trytond-6.8.0/trytond/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_wizard.py` & `trytond-6.8.0/trytond/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_workflow.py` & `trytond-6.8.0/trytond/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/test_wsgi.py` & `trytond-6.8.0/trytond/tests/test_wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import unittest
 from unittest.mock import Mock, sentinel
 
-from werkzeug.test import Client
-from werkzeug.wrappers import Response
-
 from trytond.exceptions import TrytonException
+from trytond.protocols.wrappers import Response
+from trytond.tests.test_tryton import Client
 from trytond.wsgi import TrytondWSGI
 
 
 class WSGIAppTestCase(unittest.TestCase):
     'Test WSGI Application'
 
     class TestException(TrytonException):
```

### Comparing `trytond-6.6.8/trytond/tests/tools.py` & `trytond-6.8.0/trytond/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/tree.py` & `trytond-6.8.0/trytond/tests/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/trigger.py` & `trytond-6.8.0/trytond/tests/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/wizard.py` & `trytond-6.8.0/trytond/tests/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/wizard.xml` & `trytond-6.8.0/trytond/tests/wizard.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tests/workflow.py` & `trytond-6.8.0/trytond/tests/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/__init__.py` & `trytond-6.8.0/trytond/tools/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+import posixpath
+
 try:
     from functools import cached_property
 except ImportError:
     from werkzeug.utils import cached_property
 
+try:
+    from werkzeug.security import safe_join
+except ImportError:
+    safe_join = posixpath.join
+
 from .decimal_ import decistmt
 from .misc import (
     escape_wildcard, file_open, find_dir, find_path, firstline,
     get_smtp_server, grouped_slice, is_full_text, is_instance_method,
     lstrip_wildcard, reduce_domain, reduce_ids, remove_forbidden_chars,
     resolve, rstrip_wildcard, slugify, sortable_values, sql_pairing,
     strip_wildcard, unescape_wildcard)
@@ -45,13 +52,14 @@
     is_instance_method,
     lstrip_wildcard,
     reduce_domain,
     reduce_ids,
     remove_forbidden_chars,
     resolve,
     rstrip_wildcard,
+    safe_join,
     slugify,
     sortable_values,
     sql_pairing,
     strip_wildcard,
     unescape_wildcard,
     ]
```

### Comparing `trytond-6.6.8/trytond/tools/decimal_.py` & `trytond-6.8.0/trytond/tools/decimal_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/domain_inversion.py` & `trytond-6.8.0/trytond/tools/domain_inversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -377,24 +377,24 @@
     return simplify(merge(result))
 
 
 def unique_value(domain):
     "Return if unique, the field and the value"
     if (isinstance(domain, list)
             and len(domain) == 1):
-        domain, = domain
-        name = domain[0]
-        value = domain[2]
-        count = 0
-        if len(domain) == 4 and name[-3:] == '.id':
-            count = 1
-            model = domain[3]
-            value = [model, value]
-        if name.count('.') == count and domain[1] == '=':
-            return True, name, value
+        name, operator, value, *model = domain[0]
+        if operator == '=' or (operator == 'in' and len(value) == 1):
+            value = value if operator == '=' else value[0]
+            count = 0
+            if model and name.endswith('.id'):
+                count = 1
+                model = model[0]
+                value = [model, value]
+            if name.count('.') == count:
+                return True, name, value
     return False, None, None
 
 
 def parse(domain):
     if is_leaf(domain):
         return domain
     elif not domain:
```

### Comparing `trytond-6.6.8/trytond/tools/email_.py` & `trytond-6.8.0/trytond/tools/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/immutabledict.py` & `trytond-6.8.0/trytond/tools/immutabledict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/misc.py` & `trytond-6.8.0/trytond/tools/misc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/multivalue.py` & `trytond-6.8.0/trytond/tools/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/singleton.py` & `trytond-6.8.0/trytond/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/string_.py` & `trytond-6.8.0/trytond/tools/string_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tools/timezone.py` & `trytond-6.8.0/trytond/tools/timezone.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/transaction.py` & `trytond-6.8.0/trytond/transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,81 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import logging
 import time
 from collections import defaultdict, deque
+from functools import wraps
 from threading import local
 from weakref import WeakValueDictionary
 
 from sql import Flavor
 
 from trytond.config import config
 from trytond.tools.immutabledict import ImmutableDict
 
+__all__ = ['Transaction',
+    'check_access', 'without_check_access',
+    'active_records', 'inactive_records']
+
+_retry = config.getint('database', 'retry')
 _cache_transaction = config.getint('cache', 'transaction')
 _cache_model = config.getint('cache', 'model')
 _cache_record = config.getint('cache', 'record')
 logger = logging.getLogger(__name__)
 
 
+class TransactionError(Exception):
+    def fix(self, extras):
+        pass
+
+
+class _TransactionLockError(TransactionError):
+    def __init__(self, table):
+        super().__init__()
+        self._table = table
+
+    def fix(self, extras):
+        super().fix(extras)
+        extras.setdefault('_lock_tables', []).append(self._table)
+
+
 def record_cache_size(transaction):
     return transaction.context.get('_record_cache_size', _cache_record)
 
 
+def check_access(func=None, *, _access=True):
+    if func:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            with check_access(_access=_access):
+                return func(*args, **kwargs)
+        return wrapper
+    else:
+        return Transaction().set_context(_check_access=_access)
+
+
+def without_check_access(func=None):
+    return check_access(func=func, _access=False)
+
+
+def active_records(func=None, *, _test=True):
+    if func:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            with active_records(_test=_test):
+                return func(*args, **kwargs)
+        return wrapper
+    else:
+        return Transaction().set_context(active_test=_test)
+
+
+def inactive_records(func=None):
+    return active_records(func=func, _test=False)
+
+
 class _AttributeManager(object):
     '''
     Manage Attribute of transaction
     '''
 
     def __init__(self, **kwargs):
         self.kwargs = kwargs
@@ -50,31 +101,31 @@
     Control the transaction
     '''
 
     _local = _Local()
 
     cache_keys = {'language', 'fuzzy_translation', '_datetime'}
 
-    database = None
-    readonly = False
-    connection = None
-    close = None
-    user = None
-    context = None
-    create_records = None
-    delete_records = None
-    trigger_records = None
-    check_warnings = None
-    timestamp = None
-    started_at = None
-
     def __new__(cls, new=False):
         transactions = cls._local.transactions
         if new or not transactions:
             instance = super(Transaction, cls).__new__(cls)
+            instance.database = None
+            instance.readonly = False
+            instance.connection = None
+            instance.close = None
+            instance.user = None
+            instance.context = None
+            instance.create_records = None
+            instance.delete_records = None
+            instance.trigger_records = None
+            instance.log_records = None
+            instance.check_warnings = None
+            instance.timestamp = None
+            instance.started_at = None
             instance.cache = WeakValueDictionary()
             instance._cache_deque = deque(maxlen=_cache_transaction)
             instance._atexit = []
             transactions.append(instance)
         else:
             instance = transactions[-1]
         return instance
@@ -104,53 +155,72 @@
                     Pool().get(name)._record),
                 default_factory_with_key=True))
         # Keep last used cache references to allow to pre-fill them
         self._cache_deque.append(cache)
         return cache
 
     def start(self, database_name, user, readonly=False, context=None,
-            close=False, autocommit=False):
+            close=False, autocommit=False, **extras):
         '''
         Start transaction
         '''
-        from trytond import backend
-        assert self.user is None
-        assert self.database is None
-        assert self.close is None
-        assert self.context is None
-        # Compute started_at before connect to ensure
-        # it is strictly before all transactions started after
-        # but it may be also before transactions started before
-        self.started_at = self.monotonic_time()
-        if not database_name:
-            database = backend.Database().connect()
-        else:
-            database = backend.Database(database_name).connect()
-        Flavor.set(backend.Database.flavor)
-        self.connection = database.get_connection(readonly=readonly,
-            autocommit=autocommit)
-        self.user = user
-        self.database = database
-        self.readonly = readonly
-        self.close = close
-        self.context = ImmutableDict(context or {})
-        self.create_records = defaultdict(set)
-        self.delete_records = defaultdict(set)
-        self.trigger_records = defaultdict(set)
-        self.check_warnings = set()
-        self.timestamp = {}
-        self.counter = 0
-        self._datamanagers = []
-        if database_name:
-            from trytond.cache import Cache
-            try:
+        try:
+            from trytond import backend
+            assert self.user is None
+            assert self.database is None
+            assert self.close is None
+            assert self.context is None
+            # Compute started_at before connect to ensure
+            # it is strictly before all transactions started after
+            # but it may be also before transactions started before
+            self.started_at = self.monotonic_time()
+            if not database_name:
+                database = backend.Database().connect()
+            else:
+                database = backend.Database(database_name).connect()
+            Flavor.set(backend.Database.flavor)
+            self.user = user
+            self.database = database
+            self.readonly = readonly
+            self.close = close
+            self.context = ImmutableDict(context or {})
+            self.create_records = defaultdict(set)
+            self.delete_records = defaultdict(set)
+            self.trigger_records = defaultdict(set)
+            self.log_records = []
+            self.check_warnings = set()
+            self.timestamp = {}
+            self.counter = 0
+            self._datamanagers = []
+
+            count = 0
+            while True:
+                if count:
+                    time.sleep(0.002 * (_retry - count))
+                self.connection = database.get_connection(readonly=readonly,
+                    autocommit=autocommit)
+                try:
+                    lock_tables = extras.get('_lock_tables', [])
+                    for table in lock_tables:
+                        self.database.lock(self.connection, table)
+                    self._locked_tables = set(lock_tables)
+                except backend.DatabaseOperationalError:
+                    if count < _retry:
+                        self.connection.rollback()
+                        count += 1
+                        logger.debug("Retry: %i", count)
+                        continue
+                    raise
+                break
+            if database_name:
+                from trytond.cache import Cache
                 Cache.sync(self)
-            except BaseException:
-                self.stop(False)
-                raise
+        except BaseException:
+            self.stop(False)
+            raise
         return self
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.stop(type is None)
@@ -176,14 +246,15 @@
                     self.connection = None
                     self.close = None
                     self.user = None
                     self.context = None
                     self.create_records = None
                     self.delete_records = None
                     self.trigger_records = None
+                    self.log_records = None
                     self.timestamp = None
                     self._datamanagers = []
 
                 for func, args, kwargs in self._atexit:
                     func(*args, **kwargs)
         finally:
             transactions.reverse()
@@ -219,27 +290,44 @@
                 ctx['user'] = self.user
         else:
             ctx.pop('user', None)
         self.context = ImmutableDict(ctx)
         self.user = user
         return manager
 
+    def lock_table(self, table):
+        if table not in self._locked_tables:
+            raise _TransactionLockError(table)
+
     def set_current_transaction(self, transaction):
         self._local.transactions.append(transaction)
         return transaction
 
-    def new_transaction(self, autocommit=False, readonly=False):
+    def new_transaction(self, autocommit=False, readonly=False, **extras):
         transaction = Transaction(new=True)
         return transaction.start(self.database.name, self.user,
             context=self.context, close=self.close, readonly=readonly,
-            autocommit=autocommit)
+            autocommit=autocommit, **extras)
+
+    def _store_log_records(self):
+        from trytond.pool import Pool
+        if self.log_records:
+            pool = Pool()
+            Log = pool.get('ir.model.log')
+            with without_check_access():
+                Log.save(self.log_records)
+        self._clear_log_records()
+
+    def _clear_log_records(self):
+        self.log_records.clear()
 
     def commit(self):
         from trytond.cache import Cache
         try:
+            self._store_log_records()
             if self._datamanagers:
                 for datamanager in self._datamanagers:
                     datamanager.tpc_begin(self)
                 for datamanager in self._datamanagers:
                     datamanager.commit(self)
                 for datamanager in self._datamanagers:
                     datamanager.tpc_vote(self)
@@ -263,14 +351,15 @@
     def rollback(self):
         from trytond.cache import Cache
         for cache in self.cache.values():
             cache.clear()
         for datamanager in self._datamanagers:
             datamanager.tpc_abort(self)
         Cache.rollback(self)
+        self._clear_log_records()
         self.connection.rollback()
 
     def join(self, datamanager):
         try:
             idx = self._datamanagers.index(datamanager)
             return self._datamanagers[idx]
         except ValueError:
@@ -285,7 +374,15 @@
         def get_language():
             from trytond.pool import Pool
             Config = Pool().get('ir.configuration')
             return Config.get_language()
         if self.context:
             return self.context.get('language') or get_language()
         return get_language()
+
+    @property
+    def check_access(self):
+        return self.context.get('_check_access', False)
+
+    @property
+    def active_records(self):
+        return self.context.get('active_test', True)
```

### Comparing `trytond-6.6.8/trytond/tryton.rnc` & `trytond-6.8.0/trytond/tryton.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/tryton.rng` & `trytond-6.8.0/trytond/tryton.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/url.py` & `trytond-6.8.0/trytond/url.py`

 * *Files identical despite different names*

### Comparing `trytond-6.6.8/trytond/wizard/wizard.py` & `trytond-6.8.0/trytond/wizard/wizard.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from trytond.model.exceptions import AccessError
 from trytond.model.fields import states_validate
 from trytond.pool import Pool, PoolBase
 from trytond.protocols.jsonrpc import JSONDecoder, JSONEncoder
 from trytond.pyson import PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import cached_property
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.url import URLMixin
 
 
 class Button(object):
     '''
     Define a button on wizard.
     '''
@@ -210,16 +210,26 @@
             'create': RPC(readonly=False),
             'delete': RPC(readonly=False),
             'execute': RPC(readonly=False, check_access=False),
             }
 
         # Copy states
         for attr in dir(cls):
-            if isinstance(getattr(cls, attr), State):
-                setattr(cls, attr, copy.deepcopy(getattr(cls, attr)))
+            if not isinstance(getattr(cls, attr), State):
+                continue
+            state_name = attr
+            state = getattr(cls, state_name)
+            # Copy the original state definition to prevent side-effect with
+            # the mutable attributes
+            for parent_cls in cls.__mro__:
+                parent_state = getattr(parent_cls, state_name, None)
+                if isinstance(parent_state, State):
+                    state = parent_state
+            state = copy.deepcopy(state)
+            setattr(cls, attr, state)
 
     @classmethod
     def __post_setup__(cls):
         super(Wizard, cls).__post_setup__()
         # Set states
         cls.states = {}
         for attr in dir(cls):
@@ -242,15 +252,15 @@
         ActionWizard = pool.get('ir.action.wizard')
         User = pool.get('res.user')
         context = Transaction().context
 
         if Transaction().user == 0:
             return
 
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             model = context.get('active_model')
             if model:
                 Model = pool.get(model)
             if model and model != 'ir.ui.menu':
                 ModelAccess.check(model, 'read')
             models = ActionWizard.get_models(
                 cls.__name__, action_id=context.get('action_id'))
@@ -313,23 +323,32 @@
             - ``actions``: a list of Action to execute
             - ``view``: a dictionary with:
                 - ``fields_view``: a fields/view definition
                 - ``defaults``: a dictionary with default values
                 - ``values``: a dictionary with values
                 - ``buttons``: a list of buttons
         '''
+        transaction = Transaction()
+        counter = transaction.counter
         cls.check_access()
         wizard = cls(session_id)
         for key, values in data.items():
             record = getattr(wizard, key)
             for field, value in values.items():
                 if field == 'id':
                     continue
                 setattr(record, field, value)
-        return wizard._execute(state_name)
+        result = wizard._execute(state_name)
+        # Log before _save increases the counter
+        if transaction.counter != counter and wizard.model:
+            wizard.model.log(
+                wizard.records, 'wizard',
+                f'{cls.__name__}:{state_name}')
+        wizard._save()
+        return result
 
     def _execute(self, state_name):
         if state_name == self.end_state:
             return {}
 
         state = self.states[state_name]
         result = {}
@@ -357,15 +376,14 @@
                 else:
                     do_result = action, {}
             transition = getattr(self, 'transition_%s' % state_name, None)
             if transition:
                 result = self._execute(transition())
             if do_result:
                 result.setdefault('actions', []).append(do_result)
-        self._save()
         return result
 
     def __init__(self, session_id):
         pool = Pool()
         Session = pool.get('ir.session.wizard')
         self._session_id = session_id
         session = Session(session_id)
```

### Comparing `trytond-6.6.8/trytond/worker.py` & `trytond-6.8.0/trytond/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sql import Flavor
 
 from trytond import backend
 from trytond.config import config
 from trytond.exceptions import UserError, UserWarning
 from trytond.pool import Pool
 from trytond.status import processing
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, TransactionError
 
 __all__ = ['work']
 logger = logging.getLogger(__name__)
 
 
 class Queue(object):
     def __init__(self, database_name, mpool):
@@ -66,18 +66,23 @@
     tasks = TaskList()
     selector = selectors.DefaultSelector()
     for queue in queues:
         selector.register(queue.connection, selectors.EVENT_READ)
     try:
         while True:
             timeout = options.timeout
+            # Add some randomness to avoid concurrent pulling
+            time.sleep(0.1 * random.random())
             while len(tasks.filter()) >= processes:
                 time.sleep(0.1)
             for queue in queues:
-                task_id, next_ = queue.pull(options.name)
+                try:
+                    task_id, next_ = queue.pull(options.name)
+                except backend.DatabaseOperationalError:
+                    break
                 if next_ is not None:
                     timeout = min(next_, timeout)
                 if task_id:
                     tasks.append(queue.run(task_id))
                     break
             else:
                 for key, _ in selector.select(timeout=timeout):
@@ -117,31 +122,40 @@
 
     def duration():
         return (time.monotonic() - started) * 1000
     started = time.monotonic()
     name = '<Task %s@%s>' % (task_id, pool.database_name)
     retry = config.getint('database', 'retry')
     try:
-        for count in range(retry, -1, -1):
-            if count != retry:
+        count = 0
+        transaction_extras = {}
+        while True:
+            if count:
                 time.sleep(0.02 * (retry - count))
-            with Transaction().start(pool.database_name, 0) as transaction:
+            with Transaction().start(
+                    pool.database_name, 0,
+                    **transaction_extras) as transaction:
                 try:
                     try:
                         task, = Queue.search([('id', '=', task_id)])
                     except ValueError:
                         # the task was rollbacked, nothing to do
                         break
                     with processing(name):
                         task.run()
                     break
+                except TransactionError as e:
+                    transaction.rollback()
+                    e.fix(transaction_extras)
+                    continue
                 except backend.DatabaseOperationalError:
-                    if count:
+                    if count < retry:
                         transaction.rollback()
-                        logger.debug("Retry: %i", retry - count + 1)
+                        count += 1
+                        logger.debug("Retry: %i", count)
                         continue
                     raise
                 except (UserError, UserWarning) as e:
                     Error.log(task, e)
                     raise
         logger.info("%s in %i ms", name, duration())
     except backend.DatabaseOperationalError:
```

### Comparing `trytond-6.6.8/trytond/wsgi.py` & `trytond-6.8.0/trytond/wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,50 +4,39 @@
 import http.client
 import logging
 import os
 import posixpath
 import sys
 import traceback
 import urllib.parse
+from functools import wraps
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
-from werkzeug.exceptions import HTTPException, InternalServerError, abort
 from werkzeug.routing import BaseConverter, Map, Rule
-from werkzeug.wrappers import Response
 
 try:
     from werkzeug.middleware.proxy_fix import ProxyFix
 
     def NumProxyFix(app, num_proxies):
         return ProxyFix(app,
             x_for=num_proxies, x_proto=num_proxies, x_host=num_proxies,
             x_port=num_proxies, x_prefix=num_proxies)
 except ImportError:
     from werkzeug.contrib.fixers import ProxyFix as NumProxyFix
 try:
-    from werkzeug.security import safe_join
-except ImportError:
-    safe_join = posixpath.join
-try:
     from werkzeug.middleware.shared_data import SharedDataMiddleware
 except ImportError:
     from werkzeug.wsgi import SharedDataMiddleware
 
-import wrapt
-
 from trytond.config import config
 from trytond.protocols.jsonrpc import JSONProtocol
-from trytond.protocols.wrappers import Request
+from trytond.protocols.wrappers import (
+    HTTPStatus, Request, Response, abort, exceptions)
 from trytond.protocols.xmlrpc import XMLProtocol
 from trytond.status import processing
-from trytond.tools import resolve
+from trytond.tools import resolve, safe_join
 
 __all__ = ['TrytondWSGI', 'app']
 
 logger = logging.getLogger(__name__)
 
 
 class Base64Converter(BaseConverter):
@@ -75,25 +64,26 @@
             return func
         return decorator
 
     def error_handler(self, handler):
         self.error_handlers.append(handler)
         return handler
 
-    @wrapt.decorator
-    def auth_required(self, wrapped, instance, args, kwargs):
-        request = args[0]
-        if request.user_id:
-            return wrapped(*args, **kwargs)
-        else:
-            headers = {}
-            if request.headers.get('X-Requested-With') != 'XMLHttpRequest':
-                headers['WWW-Authenticate'] = 'Basic realm="Tryton"'
-            response = Response(None, http.client.UNAUTHORIZED, headers)
-            abort(http.client.UNAUTHORIZED, response=response)
+    def auth_required(self, func):
+        @wraps(func)
+        def wrapper(request, *args, **kwargs):
+            if request.user_id:
+                return func(request, *args, **kwargs)
+            else:
+                headers = {}
+                if request.headers.get('X-Requested-With') != 'XMLHttpRequest':
+                    headers['WWW-Authenticate'] = 'Basic realm="Tryton"'
+                response = Response(None, http.client.UNAUTHORIZED, headers)
+                abort(http.client.UNAUTHORIZED, response=response)
+        return wrapper
 
     def check_request_size(self, request, size=None):
         if request.method not in {'POST', 'PUT', 'PATCH'}:
             return
         if size is None:
             if request.user_id:
                 max_size = config.getint(
@@ -113,15 +103,15 @@
     def dispatch_request(self, request):
         adapter = self.url_map.bind_to_environ(request.environ)
         try:
             endpoint, request.view_args = adapter.match()
             max_request_size = getattr(endpoint, 'max_request_size', None)
             self.check_request_size(request, max_request_size)
             return endpoint(request, **request.view_args)
-        except HTTPException as e:
+        except exceptions.HTTPException as e:
             logger.debug(
                 "Exception when processing %s", request, exc_info=True)
             return e
         except Exception as e:
             logger.debug(
                 "Exception when processing %s", request, exc_info=True)
             tb_s = ''.join(traceback.format_exception(*sys.exc_info()))
@@ -148,17 +138,18 @@
             for cls in self.protocols:
                 if cls.content_type in request.environ.get('CONTENT_TYPE', ''):
                     response = cls.response(data, request)
                     break
             else:
                 if isinstance(data, Exception):
                     try:
-                        response = InternalServerError(original_exception=data)
+                        response = exceptions.InternalServerError(
+                            original_exception=data)
                     except TypeError:
-                        response = InternalServerError(data)
+                        response = exceptions.InternalServerError(data)
                 else:
                     response = Response(data)
         return response
 
     def wsgi_app(self, environ, start_response):
         for cls in self.protocols:
             if cls.content_type in environ.get('CONTENT_TYPE', ''):
@@ -184,15 +175,15 @@
             adapter = self.url_map.bind_to_environ(request.environ)
             endpoint = adapter.match()[0]
             if not getattr(endpoint, 'allow_null_origin', False):
                 abort(HTTPStatus.FORBIDDEN)
 
         with processing(request):
             data = self.dispatch_request(request)
-            if not isinstance(data, (Response, HTTPException)):
+            if not isinstance(data, (Response, exceptions.HTTPException)):
                 response = self.make_response(request, data)
             else:
                 response = data
 
         if origin and isinstance(response, Response):
             response.headers['Access-Control-Allow-Origin'] = origin
             response.headers['Vary'] = 'Origin'
```

### Comparing `trytond-6.6.8/trytond.egg-info/PKG-INFO` & `trytond-6.8.0/trytond.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 6.6.8
+Version: 6.8.0
 Summary: Tryton server
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
-Project-URL: Source Code, https://hg.tryton.org/trytond
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: business application platform ERP
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -38,31 +38,33 @@
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
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: PostgreSQL
 Provides-Extra: graphviz
 Provides-Extra: Levenshtein
 Provides-Extra: BCrypt
 Provides-Extra: Argon2
 Provides-Extra: html2text
 Provides-Extra: weasyprint
 Provides-Extra: coroutine
 Provides-Extra: image
+Provides-Extra: barcode
+Provides-Extra: qrcode
 Provides-Extra: completion
 License-File: LICENSE
 
 trytond
 =======
 
 The server of Tryton.
```

### Comparing `trytond-6.6.8/trytond.egg-info/SOURCES.txt` & `trytond-6.8.0/trytond.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,20 @@
 doc/ref/pool.rst
 doc/ref/pyson.rst
 doc/ref/rpc.rst
 doc/ref/sendmail.rst
 doc/ref/tests.rst
 doc/ref/transaction.rst
 doc/ref/wizard.rst
+doc/ref/tools/barcode.rst
 doc/ref/tools/email.rst
 doc/ref/tools/immutabledict.rst
 doc/ref/tools/index.rst
 doc/ref/tools/misc.rst
+doc/ref/tools/qrcode.rst
 doc/ref/tools/singleton.rst
 doc/ref/tools/timezone.rst
 doc/topics/access_rights.rst
 doc/topics/actions.rst
 doc/topics/backend_types.rst
 doc/topics/bus.rst
 doc/topics/configuration.rst
@@ -274,14 +276,16 @@
 trytond/ir/view/model_data_list.xml
 trytond/ir/view/model_field_access_form.xml
 trytond/ir/view/model_field_access_list.xml
 trytond/ir/view/model_field_form.xml
 trytond/ir/view/model_field_list.xml
 trytond/ir/view/model_form.xml
 trytond/ir/view/model_list.xml
+trytond/ir/view/model_log_form.xml
+trytond/ir/view/model_log_list.xml
 trytond/ir/view/model_print_model_graph_start_form.xml
 trytond/ir/view/module_activate_upgrade_done_form.xml
 trytond/ir/view/module_activate_upgrade_start_form.xml
 trytond/ir/view/module_config_start_form.xml
 trytond/ir/view/module_config_wizard_done_form.xml
 trytond/ir/view/module_config_wizard_first_form.xml
 trytond/ir/view/module_config_wizard_item_list.xml
@@ -451,14 +455,15 @@
 trytond/tests/forbidden.txt
 trytond/tests/history.py
 trytond/tests/import_data.py
 trytond/tests/import_data.xml
 trytond/tests/message.xml
 trytond/tests/mixin.py
 trytond/tests/model.py
+trytond/tests/model_log.py
 trytond/tests/modelsql.py
 trytond/tests/modelstorage.py
 trytond/tests/modelview.py
 trytond/tests/modelview.xml
 trytond/tests/mptt.py
 trytond/tests/multivalue.py
 trytond/tests/path.py
@@ -498,14 +503,15 @@
 trytond/tests/test_history.py
 trytond/tests/test_i18n.py
 trytond/tests/test_importdata.py
 trytond/tests/test_ir.py
 trytond/tests/test_mixins.py
 trytond/tests/test_model.py
 trytond/tests/test_model_index.py
+trytond/tests/test_model_log.py
 trytond/tests/test_modelsingleton.py
 trytond/tests/test_modelsql.py
 trytond/tests/test_modelstorage.py
 trytond/tests/test_modelview.py
 trytond/tests/test_mptt.py
 trytond/tests/test_multivalue.py
 trytond/tests/test_order.py
@@ -535,19 +541,21 @@
 trytond/tests/trigger.py
 trytond/tests/tryton.cfg
 trytond/tests/wizard.py
 trytond/tests/wizard.xml
 trytond/tests/workflow.py
 trytond/tests/workflow.xml
 trytond/tools/__init__.py
+trytond/tools/barcode.py
 trytond/tools/decimal_.py
 trytond/tools/domain_inversion.py
 trytond/tools/email_.py
 trytond/tools/gevent.py
 trytond/tools/immutabledict.py
 trytond/tools/misc.py
 trytond/tools/multivalue.py
+trytond/tools/qrcode.py
 trytond/tools/singleton.py
 trytond/tools/string_.py
 trytond/tools/timezone.py
 trytond/wizard/__init__.py
 trytond/wizard/wizard.py
```

