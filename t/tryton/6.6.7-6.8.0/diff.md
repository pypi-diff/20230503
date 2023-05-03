# Comparing `tmp/tryton-6.6.7.tar.gz` & `tmp/tryton-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-6.6.7.tar", last modified: Wed May  3 16:31:00 2023, max compression
+gzip compressed data, was "tryton-6.8.0.tar", last modified: Mon May  1 12:07:21 2023, max compression
```

## Comparing `tryton-6.6.7.tar` & `tryton-6.8.0.tar`

### file list

```diff
@@ -1,354 +1,357 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.821726 tryton-6.6.7/
--rw-r--r--   0 ced       (1000) ced       (1000)    18192 2023-05-03 16:30:57.000000 tryton-6.6.7/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-05-03 16:30:57.000000 tryton-6.6.7/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 tryton-6.6.7/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-13 16:52:41.000000 tryton-6.6.7/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2260 2023-05-03 16:31:00.821726 tryton-6.6.7/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2022-12-19 12:02:59.000000 tryton-6.6.7/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.738392 tryton-6.6.7/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2067 2023-04-13 16:52:41.000000 tryton-6.6.7/bin/tryton
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2022-12-19 12:02:59.000000 tryton-6.6.7/catalan.nsh
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.725058 tryton-6.6.7/darwin/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.738392 tryton-6.6.7/darwin/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3255 2022-12-19 12:02:59.000000 tryton-6.6.7/darwin/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2022-12-19 12:02:59.000000 tryton-6.6.7/darwin/gtk-3.0/gtk.immodules
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.741725 tryton-6.6.7/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2023-04-13 16:52:41.000000 tryton-6.6.7/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5990 2022-12-19 12:02:59.000000 tryton-6.6.7/doc/glossary.rst
--rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-04-13 16:52:41.000000 tryton-6.6.7/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-13 16:52:41.000000 tryton-6.6.7/doc/installation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-13 16:52:41.000000 tryton-6.6.7/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    18603 2023-04-13 16:52:41.000000 tryton-6.6.7/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2022-12-19 12:02:59.000000 tryton-6.6.7/english.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2022-12-19 12:02:59.000000 tryton-6.6.7/farsi.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2022-12-19 12:02:59.000000 tryton-6.6.7/french.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2022-12-19 12:02:59.000000 tryton-6.6.7/german.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2022-12-19 12:02:59.000000 tryton-6.6.7/make-darwin-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-12-19 12:02:59.000000 tryton-6.6.7/make-win32-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-12-19 12:02:59.000000 tryton-6.6.7/portuguese.nsh
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4684 2023-04-13 16:52:41.000000 tryton-6.6.7/setup-freeze.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-05-03 16:31:00.821726 tryton-6.6.7/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2022-12-19 12:02:59.000000 tryton-6.6.7/setup.nsi
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4271 2023-04-13 16:52:41.000000 tryton-6.6.7/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2022-12-19 12:02:59.000000 tryton-6.6.7/slovenian.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1095 2022-12-19 12:02:59.000000 tryton-6.6.7/spanish.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-13 16:52:41.000000 tryton-6.6.7/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.745059 tryton-6.6.7/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)     1926 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.748392 tryton-6.6.7/tryton/action/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/action/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7009 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/action/main.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2830 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3100 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/client.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/common/
--rw-r--r--   0 ced       (1000) ced       (1000)     2380 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-13 17:12:17.000000 tryton-6.6.7/tryton/common/button.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6607 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/cellrendererbinary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/cellrendererbutton.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/cellrendererclickablepixbuf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/cellrenderercombo.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/cellrendererfloat.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/cellrendererinteger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/cellrenderertext.py
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/cellrenderertoggle.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46177 2023-04-22 21:10:31.000000 tryton-6.6.7/tryton/common/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/completion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19857 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/datetime_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17106 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28942 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/entry_position.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/environment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/focus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/htmltextbuffer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/number_entry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5564 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/popup_menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/richtext.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8186 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/common/underline.py
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/common/widget_style.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6879 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/config.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/tryton/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.725058 tryton-6.6.7/tryton/data/locale/bg/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     8847 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21360 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/bg/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/ca/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18929 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20049 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/ca/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/cs/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     4634 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    17664 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/cs/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/de/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19465 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/de/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20602 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/de/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/es/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19208 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/es/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20537 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/es/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/es_419/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13605 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/et/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.758392 tryton-6.6.7/tryton/data/locale/et/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    13745 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/et/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18301 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/et/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/fa/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16945 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22143 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/fa/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/fi/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13439 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/fi/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/fr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19575 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20653 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/fr/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/hu/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17450 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20290 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/hu/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/id/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/id/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7123 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/id/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    15325 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/id/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/it/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/it/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15330 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/it/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19162 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/it/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/ja_JP/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    36736 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/lo/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/lo/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18768 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    26740 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/lo/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/lt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16567 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20237 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/lt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/nl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18702 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19748 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/nl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/pl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17889 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19569 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/pl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/pt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.761726 tryton-6.6.7/tryton/data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15328 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19756 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/pt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/ro/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18743 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19954 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/ro/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/ru/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    10072 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21763 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/ru/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.728392 tryton-6.6.7/tryton/data/locale/sl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    12361 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18664 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/sl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/tryton/data/locale/tr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13993 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/tr/LC_MESSAGES/tryton.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13160 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/tryton.pot
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/tryton/data/locale/uk/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    23392 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    24571 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/uk/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/tryton/data/locale/zh_CN/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.765059 tryton-6.6.7/tryton/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16910 2023-05-03 16:30:51.000000 tryton-6.6.7/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18628 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/tryton/data/pixmaps/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.785059 tryton-6.6.7/tryton/data/pixmaps/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-add.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-archive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-attach.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-back.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-bookmark.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-cancel.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-clear.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-copy.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-create.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-date.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-delete.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-drag.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-email.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-error.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-exit.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-export.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-filter.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-bold.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-italic.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-format-underline.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-forward.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-history.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-icon.png
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-import.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-info.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-launch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-link.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-log.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-menu.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-note.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-ok.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-print.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-public.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-question.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-refresh.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-remove.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-save.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-search.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-send.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-star-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-star.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-switch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-translate.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-unarchive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-undo.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-warning.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    26698 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.icns
--rw-r--r--   0 ced       (1000) ced       (1000)    62686 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.ico
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/device_cookie.py
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/fingerprints.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.788393 tryton-6.6.7/tryton/gui/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42361 2023-04-22 21:14:38.000000 tryton-6.6.7/tryton/gui/main.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.795059 tryton-6.6.7/tryton/gui/window/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-03 16:30:57.000000 tryton-6.6.7/tryton/gui/window/about.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/board.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28533 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/dblogin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13478 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    35281 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1259 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/infobar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/limit.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-01-15 17:31:04.000000 tryton-6.6.7/tryton/gui/window/nomodal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/preference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/revision.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/tabcontent.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.795059 tryton-6.6.7/tryton/gui/window/view_board/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_board/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5612 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_board/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_board/view_board.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.798393 tryton-6.6.7/tryton/gui/window/view_form/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.798393 tryton-6.6.7/tryton/gui/window/view_form/model/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42655 2023-04-13 16:58:17.000000 tryton-6.6.7/tryton/gui/window/view_form/model/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/model/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25157 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/model/record.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.798393 tryton-6.6.7/tryton/gui/window/view_form/screen/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/screen/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    53392 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/screen/screen.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.801726 tryton-6.6.7/tryton/gui/window/view_form/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5580 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.805060 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9795 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21229 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.815060 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8330 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/checkbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22073 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/dictionary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/image.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12183 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14341 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22369 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1397 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/progressbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/state_widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5760 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/textbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5254 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/url.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10769 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.815060 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/bar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15923 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/graph.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/pie.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51013 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4974 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/list_form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.818393 tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13347 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/editabletree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46851 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/view_form/view/screen_container.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/win_csv.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20653 2023-04-22 21:15:02.000000 tryton-6.6.7/tryton/gui/window/win_export.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19493 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/win_form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/win_import.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/win_search.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/window.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14869 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/gui/window/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13612 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/jsonrpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.818393 tryton-6.6.7/tryton/plugins/
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/plugins/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.818393 tryton-6.6.7/tryton/plugins/translation/
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/plugins/translation/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21766 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5153 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/rpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.818393 tryton-6.6.7/tryton/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43531 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/tests/test_common_domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton/tests/test_common_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/tests/test_common_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6440 2023-04-13 16:52:41.000000 tryton-6.6.7/tryton/translate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2022-12-19 12:02:59.000000 tryton-6.6.7/tryton.desktop
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.748392 tryton-6.6.7/tryton.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2260 2023-05-03 16:30:59.000000 tryton-6.6.7/tryton.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    10479 2023-05-03 16:31:00.000000 tryton-6.6.7/tryton.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-03 16:30:59.000000 tryton-6.6.7/tryton.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:09:54.000000 tryton-6.6.7/tryton.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       69 2023-05-03 16:30:59.000000 tryton-6.6.7/tryton.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        7 2023-05-03 16:30:59.000000 tryton-6.6.7/tryton.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.731725 tryton-6.6.7/win32/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-03 16:31:00.821726 tryton-6.6.7/win32/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2022-12-19 12:02:59.000000 tryton-6.6.7/win32/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)        0 2022-12-19 12:02:59.000000 tryton-6.6.7/win32/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18236 2023-05-01 11:19:08.000000 tryton-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-05-01 11:19:08.000000 tryton-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 tryton-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 tryton-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-01 12:07:21.101585 tryton-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-6.8.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.011584 tryton-6.8.0/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2067 2023-04-15 07:12:15.000000 tryton-6.8.0/bin/tryton
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-01-16 14:00:21.000000 tryton-6.8.0/catalan.nsh
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/darwin/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.011584 tryton-6.8.0/darwin/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-01-16 14:00:21.000000 tryton-6.8.0/darwin/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-01-16 14:00:21.000000 tryton-6.8.0/darwin/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.014917 tryton-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/glossary.rst
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/installation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    18793 2023-04-21 10:10:00.000000 tryton-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-01-16 14:00:21.000000 tryton-6.8.0/english.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-01-16 14:00:21.000000 tryton-6.8.0/farsi.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-01-16 14:00:21.000000 tryton-6.8.0/french.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-01-16 14:00:21.000000 tryton-6.8.0/german.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 tryton-6.8.0/make-darwin-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 tryton-6.8.0/make-win32-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-01-16 14:00:21.000000 tryton-6.8.0/portuguese.nsh
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4684 2023-04-15 07:12:15.000000 tryton-6.8.0/setup-freeze.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-05-01 12:07:21.101585 tryton-6.8.0/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-04-15 07:12:15.000000 tryton-6.8.0/setup.nsi
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4338 2023-04-15 07:12:15.000000 tryton-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-01-16 14:00:21.000000 tryton-6.8.0/slovenian.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-01-16 14:00:21.000000 tryton-6.8.0/spanish.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 tryton-6.8.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.018251 tryton-6.8.0/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1926 2023-05-01 11:19:00.000000 tryton-6.8.0/tryton/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.021584 tryton-6.8.0/tryton/action/
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/action/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6763 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/action/main.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3157 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/client.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/common/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2380 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/common/button.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6607 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererbinary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererbutton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/cellrendererclickablepixbuf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderercombo.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererfloat.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererinteger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderertext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderertoggle.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46398 2023-05-01 07:33:35.000000 tryton-6.8.0/tryton/common/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/completion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/datetime_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28998 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/entry_position.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/environment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/focus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/htmltextbuffer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/number_entry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5776 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/common/popup_menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/richtext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8276 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/underline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/widget_style.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7606 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/config.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/data/locale/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/bg/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8847 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21360 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/ca/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18982 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20106 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/cs/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4634 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    17715 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/de/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19498 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20639 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/es/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19256 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20589 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/es_419/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7108 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    15820 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/et/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13577 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18343 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fa/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16794 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22236 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fi/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    13490 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19662 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20744 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/hu/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17282 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20326 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/id/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6983 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    15314 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/it/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15104 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19228 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ja_JP/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/lo/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18515 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    26787 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/lt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16294 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20304 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/nl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18765 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19815 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/pl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17623 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19642 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/pt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19825 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ro/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19191 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20017 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ru/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10072 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21758 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/sl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    12234 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18742 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/tr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14027 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13211 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/tryton.pot
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/uk/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    23076 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    24539 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/zh_CN/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16690 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18708 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/pixmaps/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.064918 tryton-6.8.0/tryton/data/pixmaps/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-add.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-archive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-attach.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-back.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmark.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-cancel.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-clear.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-copy.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-create.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-date.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-delete.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-drag.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-email.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-error.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-exit.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-export.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-filter.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-bold.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-italic.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-underline.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-forward.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-history.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-import.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-info.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-launch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-link.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-log.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-menu.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-note.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-ok.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-print.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-public.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-question.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-refresh.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-remove.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-save.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-search.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-send.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-star-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-star.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-switch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-translate.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-undo.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-warning.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.icns
+-rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.ico
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/device_cookie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/fingerprints.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.064918 tryton-6.8.0/tryton/gui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42035 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/gui/main.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.074918 tryton-6.8.0/tryton/gui/window/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-01 11:19:08.000000 tryton-6.8.0/tryton/gui/window/about.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/board.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29228 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/dblogin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13478 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    34216 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/infobar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/limit.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/nomodal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/preference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/revision.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/tabcontent.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_board/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/view_board.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_form/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_form/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43599 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/model/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/model/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25729 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/model/record.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.081585 tryton-6.8.0/tryton/gui/window/view_form/screen/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/screen/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    52272 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/screen/screen.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.084918 tryton-6.8.0/tryton/gui/window/view_form/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.084918 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21657 2023-05-01 07:33:35.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.094919 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8330 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22073 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/image.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12565 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14370 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22440 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5687 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/textbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5254 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/url.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/bar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15923 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/graph.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/pie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51013 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6926 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    49457 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/screen_container.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/win_csv.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20797 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/gui/window/win_export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19552 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/win_form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-04-20 14:47:34.000000 tryton-6.8.0/tryton/gui/window/win_import.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/win_search.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14869 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13612 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/jsonrpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/plugins/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/plugins/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/plugins/translation/
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/plugins/translation/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21766 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4903 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/rpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/tryton/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common_domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/tests/test_common_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6440 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/translate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton.desktop
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.021584 tryton-6.8.0/tryton.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    10575 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 tryton-6.8.0/tryton.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       69 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        7 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/win32/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/win32/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-01-16 14:00:21.000000 tryton-6.8.0/win32/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-01-16 14:00:21.000000 tryton-6.8.0/win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-6.6.7/CHANGELOG` & `tryton-6.8.0/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 
-Version 6.6.7 - 2023-05-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.6 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
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
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Include events to logs
+* Add option to disable thread
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Save and Restore tree state on List Form
+* Do record (pre)validation and saving on selection change for list-form views
+* Eagerly read string value of selection fields
+* Do not select first record by default
+* Use ``&`` and ``|`` as boolean operator in search widget
+* Use toggle button and label on translate dialog
+* Manage domain on id in single value list as unique
+* Do not validate domain nor enforce uniqueness for empty fields unless they're required or invisible
+* Display the number of selected records on xxx2Many
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Support authentication services
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `tryton-6.6.7/COPYRIGHT` & `tryton-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/LICENSE` & `tryton-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/PKG-INFO` & `tryton-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 6.6.7
+Version: 6.8.0
 Summary: Tryton desktop client
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
-Project-URL: Source Code, https://hg.tryton.org/tryton
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: business application ERP
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -38,20 +38,20 @@
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Japanese
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: calendar
 License-File: LICENSE
 
 tryton
 ======
 
 The desktop client of Tryton.
```

### Comparing `tryton-6.6.7/bin/tryton` & `tryton-6.8.0/bin/tryton`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/catalan.nsh` & `tryton-6.8.0/catalan.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/darwin/gtk-3.0/gdk-pixbuf.loaders` & `tryton-6.8.0/darwin/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/darwin/gtk-3.0/gtk.immodules` & `tryton-6.8.0/darwin/gtk-3.0/gtk.immodules`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/doc/conf.py` & `tryton-6.8.0/doc/conf.py`

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

### Comparing `tryton-6.6.7/doc/glossary.rst` & `tryton-6.8.0/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/doc/installation.rst` & `tryton-6.8.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/doc/usage.rst` & `tryton-6.8.0/doc/usage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -508,30 +508,34 @@
    For example: ``Name: "Michael:Scott"``
 
    Here it will search with the value ``Michael:Scott``.
 
 Clause composition
 ++++++++++++++++++
 
-The clauses can be composed using the two boolean operators ``and`` and ``or``.
-By default, there is an implicit ``and`` between each clause if no operator is
+The clauses can be composed using the two boolean operators ``&`` (for `logical
+conjunction`_) and ``|`` (for `logical disjunction`_).
+By default, there is an implicit ``&`` between each clause if no operator is
 specified.
 
    For example: ``Name: Michael Amount: 100``
 
-   is the same as ``Name: Michael and Amount: 100``
+   is the same as ``Name: Michael & Amount: 100``
 
-The ``and`` operator has a highest precedence than ``or`` but you can change it
-by using parenthesis.
+The ``&`` operator has a highest precedence than ``|`` but you can change it by
+using parenthesis.
 
-   For example: ``(Name: Michael or Name: Pam) and Amount: 100``
+   For example: ``(Name: Michael | Name: Pam) & Amount: 100``
 
-   is different than ``Name: Michael or Name: Pam and Amount: 100``
+   is different than ``Name: Michael | Name: Pam & Amount: 100``
 
-   which is evaluated as ``Name: Michael or (Name: Pam and Amount: 100)``
+   which is evaluated as ``Name: Michael | (Name: Pam & Amount: 100)``
+
+.. _logical conjunction: https://en.wikipedia.org/wiki/Logical_conjunction
+.. _logical disjunction: https://en.wikipedia.org/wiki/Logical_disjunction
 
 RichText Editor
 ^^^^^^^^^^^^^^^
 
 This feature create a rich text editor with various features that allow for
 text formatting. The features are:
```

### Comparing `tryton-6.6.7/english.nsh` & `tryton-6.8.0/english.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/farsi.nsh` & `tryton-6.8.0/farsi.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/french.nsh` & `tryton-6.8.0/french.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/german.nsh` & `tryton-6.8.0/german.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/portuguese.nsh` & `tryton-6.8.0/portuguese.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/setup-freeze.py` & `tryton-6.8.0/setup-freeze.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/setup.nsi` & `tryton-6.8.0/setup.nsi`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/setup.py` & `tryton-6.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,30 +64,33 @@
 
 version = get_version()
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'tryton'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 dist = setup(name=name,
     version=version,
     description='Tryton desktop client',
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
-        "Source Code": 'https://hg.tryton.org/tryton',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='business application ERP',
     packages=find_packages(),
     package_data=package_data,
     data_files=data_files,
     scripts=['bin/tryton'],
     classifiers=[
@@ -116,23 +119,23 @@
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Japanese',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Office/Business',
         ],
     platforms='any',
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'pycairo',
         "python-dateutil",
         'PyGObject>=3.19',
         ],
     extras_require={
         'calendar': ['GooCalendar>=0.7'],
```

### Comparing `tryton-6.6.7/slovenian.nsh` & `tryton-6.8.0/slovenian.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/spanish.nsh` & `tryton-6.8.0/spanish.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/__init__.py` & `tryton-6.8.0/tryton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-__version__ = "6.6.7"
+__version__ = "6.8.0"
 import locale
 
 import gi
 
 gi.require_version('Gtk', '3.0')
 gi.require_version('Gdk', '3.0')
 gi.require_foreign('cairo')
```

### Comparing `tryton-6.6.7/tryton/action/main.py` & `tryton-6.8.0/tryton/action/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # this repository contains the full copyright notices and license terms.
 import gettext
 import webbrowser
 
 import tryton.rpc as rpc
 from tryton.common import (
     RPCException, RPCExecute, file_open, file_write, message, selection)
-from tryton.config import CONFIG
 from tryton.pyson import PYSONDecoder
 
 _ = gettext.gettext
 
 
 class Action(object):
 
@@ -87,84 +86,74 @@
                 name_suffix += _(',...')
             if name_suffix:
                 return _('%s (%s)') % (name, name_suffix)
             else:
                 return name
 
         data['action_id'] = action['id']
+        params = {
+            'icon': action.get('icon.rec_name') or '',
+            }
         if action['type'] == 'ir.action.act_window':
-            view_ids = []
-            view_mode = None
             if action.get('views', []):
-                view_ids = [x[0] for x in action['views']]
-                view_mode = [x[1] for x in action['views']]
+                params['view_ids'] = [x[0] for x in action['views']]
+                params['view_mode'] = [x[1] for x in action['views']]
             elif action.get('view_id', False):
-                view_ids = [action['view_id'][0]]
+                params['view_ids'] = [action['view_id'][0]]
 
             action.setdefault('pyson_domain', '[]')
             ctx = {
                 'active_model': data.get('model'),
                 'active_id': data.get('id'),
                 'active_ids': data.get('ids') or [],
             }
             ctx.update(rpc.CONTEXT)
             ctx['_user'] = rpc._USER
             decoder = PYSONDecoder(ctx)
-            action_ctx = context.copy()
-            action_ctx.update(
+            params['context'] = context.copy()
+            params['context'].update(
                 decoder.decode(action.get('pyson_context') or '{}'))
-            ctx.update(action_ctx)
+            ctx.update(params['context'])
 
             ctx['context'] = ctx
             decoder = PYSONDecoder(ctx)
-            domain = decoder.decode(action['pyson_domain'])
-            order = decoder.decode(action['pyson_order'])
-            search_value = decoder.decode(action['pyson_search_value'] or '[]')
-            tab_domain = [(n, decoder.decode(d), c)
-                for n, d, c in action['domains']]
+            params['domain'] = decoder.decode(action['pyson_domain'])
+            params['order'] = decoder.decode(action['pyson_order'])
+            params['search_value'] = decoder.decode(
+                action['pyson_search_value'] or '[]')
+            params['tab_domain'] = [
+                (n, decoder.decode(d), c) for n, d, c in action['domains']]
 
             name = action.get('name', '')
             if action.get('keyword', ''):
-                name = add_name_suffix(name, action_ctx)
+                name = add_name_suffix(name, params['context'])
+            params['name'] = name
 
             res_model = action.get('res_model', data.get('res_model'))
-            res_id = action.get('res_id', data.get('res_id'))
+            params['res_id'] = action.get('res_id', data.get('res_id'))
+            params['context_model'] = action.get('context_model')
+            params['context_domain'] = action.get('context_domain')
             limit = action.get('limit')
-            if limit is None:
-                limit = CONFIG['client.limit']
+            if limit is not None:
+                params['limit'] = limit
 
-            Window.create(res_model,
-                view_ids=view_ids,
-                res_id=res_id,
-                domain=domain,
-                context=action_ctx,
-                order=order,
-                mode=view_mode,
-                name=name,
-                limit=limit,
-                search_value=search_value,
-                icon=(action.get('icon.rec_name') or ''),
-                tab_domain=tab_domain,
-                context_model=action['context_model'],
-                context_domain=action['context_domain'])
+            Window.create(res_model, **params)
         elif action['type'] == 'ir.action.wizard':
+            params['context'] = context
+            params['window'] = action.get('window')
             name = action.get('name', '')
             if action.get('keyword', 'form_action') == 'form_action':
                 name = add_name_suffix(name, context)
-            Window.create_wizard(action['wiz_name'], data,
-                direct_print=action.get('direct_print', False),
-                name=name,
-                context=context, icon=(action.get('icon.rec_name') or ''),
-                window=action.get('window', False))
-
+            params['name'] = name
+            Window.create_wizard(action['wiz_name'], data, **params)
         elif action['type'] == 'ir.action.report':
-            Action.exec_report(
-                action['report_name'], data,
-                direct_print=action.get('direct_print', False),
-                context=context)
+            params['direct_print'] = action.get('direct_print', False)
+            params['context'] = context
+            del params['icon']
+            Action.exec_report(action['report_name'], data, **params)
 
         elif action['type'] == 'ir.action.url':
             if action['url']:
                 webbrowser.open(action['url'], new=2)
 
     @staticmethod
     def exec_keyword(keyword, data=None, context=None, warning=True,
```

### Comparing `tryton-6.6.7/tryton/bus.py` & `tryton-6.8.0/tryton/bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 ID = str(uuid.uuid4())
 CHANNELS = [
     'client:%s' % ID,
     ]
 
 
 def listen(connection):
+    if not CONFIG['thread']:
+        return
     listener = threading.Thread(
         target=_listen, args=(connection,), daemon=True)
     listener.start()
 
 
 def _listen(connection):
     bus_timeout = CONFIG['client.bus_timeout']
```

### Comparing `tryton-6.6.7/tryton/client.py` & `tryton-6.8.0/tryton/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     }
     label.required {
         font-weight: bold;
     }
     label.editable {
         font-style: italic;
     }
+    label.warning {
+        color: @warning_color;
+    }
     .window-title, .wizard-title {
         font-size: large;
         font-weight: bold;
     }
     .window-title .status {
         font-size: medium;
         font-weight: normal;
```

### Comparing `tryton-6.6.7/tryton/common/__init__.py` & `tryton-6.8.0/tryton/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/button.py` & `tryton-6.8.0/tryton/common/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,17 @@
             states = record.expr_eval(self.attrs.get('states', {}))
         else:
             states = {}
         if states.get('invisible', False):
             self.hide()
         else:
             self.show()
-        self.set_sensitive(not states.get('readonly', False))
+        self.set_sensitive(
+            not (record.readonly if record else False)
+            and not states.get('readonly', False))
         self._set_icon(states.get('icon', self.attrs.get('icon')))
 
         if self.attrs.get('rule'):
             label = self.label
             tip = self.attrs.get('help', '')
             if record:
                 clicks = record.get_button_clicks(self.attrs['name'])
```

### Comparing `tryton-6.6.7/tryton/common/cellrendererbinary.py` & `tryton-6.8.0/tryton/common/cellrendererbinary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/cellrendererbutton.py` & `tryton-6.8.0/tryton/common/cellrendererbutton.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/cellrendererclickablepixbuf.py` & `tryton-6.8.0/tryton/common/cellrendererclickablepixbuf.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/cellrendererfloat.py` & `tryton-6.8.0/tryton/common/cellrendererfloat.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/cellrendererinteger.py` & `tryton-6.8.0/tryton/common/cellrendererinteger.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/cellrenderertext.py` & `tryton-6.8.0/tryton/common/cellrenderertext.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/common.py` & `tryton-6.8.0/tryton/common/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,37 +19,36 @@
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 try:
     from http import HTTPStatus
 except ImportError:
     from http import client as HTTPStatus
 
-import _thread
 import shlex
 import socket
 import sys
 import traceback
 import urllib.error
 import urllib.parse
 import urllib.request
 import webbrowser
 from functools import lru_cache, wraps
 from string import Template
+from threading import Lock, Thread
 
 import tryton.rpc as rpc
 from tryton.config import CONFIG, PIXMAPS_DIR, TRYTON_ICON
 
 try:
     import ssl
 except ImportError:
     ssl = None
 import zipfile
-from threading import Lock
 
-from gi.repository import Gdk, GdkPixbuf, GLib, GObject, Gtk
+from gi.repository import Gdk, GdkPixbuf, Gio, GLib, GObject, Gtk
 
 from tryton import __version__
 from tryton.exceptions import TrytonError, TrytonServerError
 from tryton.pyson import PYSONEncoder
 
 from .underline import set_underline
 from .widget_style import widget_class
@@ -100,14 +99,16 @@
                 or iconname in cls._local_icons):
             return
         if iconname not in cls._name2id:
             cls.load_icons(refresh=True)
         try:
             icon_ref = (cls._name2id[iconname], iconname)
         except KeyError:
+            logger.error(f"Unknown icon {iconname}")
+            cls._icons[iconname] = None
             return
         idx = cls._tryton_icons.index(icon_ref)
         to_load = slice(max(0, idx - cls.batchnum // 2),
             idx + cls.batchnum // 2)
         ids = [e[0] for e in cls._tryton_icons[to_load]]
         try:
             icons = rpc.execute('model', 'ir.ui.icon', 'read', ids,
@@ -124,21 +125,22 @@
     @classmethod
     def get_pixbuf(cls, iconname, size=16, color=None, badge=None):
         if not iconname:
             return
         colors = CONFIG['icon.colors'].split(',')
         cls.register_icon(iconname)
         if iconname not in cls._pixbufs[(size, badge)]:
+            data = None
             if iconname in cls._icons:
                 data = cls._icons[iconname]
             elif iconname in cls._local_icons:
                 path = cls._local_icons[iconname]
                 with open(path, 'rb') as fp:
                     data = fp.read()
-            else:
+            if not data:
                 logger.error("Unknown icon %s" % iconname)
                 return
             if not color:
                 color = colors[0]
             try:
                 ET.register_namespace('', 'http://www.w3.org/2000/svg')
                 root = ET.fromstring(data)
@@ -435,35 +437,26 @@
     return res
 
 
 def file_selection(title, filename='',
         action=Gtk.FileChooserAction.OPEN, preview=True, multi=False,
         filters=None):
     parent = get_toplevel_window()
-    if action == Gtk.FileChooserAction.OPEN:
-        buttons = (set_underline(_("Cancel")), Gtk.ResponseType.CANCEL,
-            set_underline(_("Select")), Gtk.ResponseType.OK)
-    else:
-        buttons = (set_underline(_("Cancel")), Gtk.ResponseType.CANCEL,
-            set_underline(_("Save")), Gtk.ResponseType.OK)
-    win = Gtk.FileChooserDialog(
+    win = Gtk.FileChooserNative(
         title=title, transient_for=parent, action=action)
-    win.add_buttons(*buttons)
-    win.set_icon(TRYTON_ICON)
     if filename:
         if action in (Gtk.FileChooserAction.SAVE,
                 Gtk.FileChooserAction.CREATE_FOLDER):
             filename = _slugify_filename(filename)
             win.set_current_name(filename)
         else:
             win.set_filename(filename)
     if hasattr(win, 'set_do_overwrite_confirmation'):
         win.set_do_overwrite_confirmation(True)
     win.set_select_multiple(multi)
-    win.set_default_response(Gtk.ResponseType.OK)
     if filters is not None:
         for filt in filters:
             win.add_filter(filt)
 
     def update_preview_cb(win, img):
         have_preview = False
         filename = win.get_preview_filename()
@@ -480,15 +473,15 @@
 
     if preview:
         img_preview = Gtk.Image()
         win.set_preview_widget(img_preview)
         win.connect('update-preview', update_preview_cb, img_preview)
 
     button = win.run()
-    if button != Gtk.ResponseType.OK:
+    if button != Gtk.ResponseType.ACCEPT:
         result = None
     elif not multi:
         result = PurePath(win.get_filename())
     else:
         result = [PurePath(f) for f in win.get_filenames()]
     parent.present()
     win.destroy()
@@ -542,18 +535,16 @@
             for name in zip_file.namelist():
                 ztype = os.path.splitext(name)
                 with zip_file.open(name) as zfile:
                     zfilename = file_write(name, zfile.read())
                     file_open(zfilename, type=ztype, print_p=True)
         return
 
-    if os.name == 'nt':
-        operation = 'open'
-        if print_p:
-            operation = 'print'
+    if hasattr(os, 'startfile'):
+        operation = 'print' if print_p else 'open'
         try:
             os.startfile(os.path.normpath(filename), operation)
         except WindowsError:
             save()
     elif print_p:
         if type in {'odt', 'odp', 'ods', 'odg'}:
             try:
@@ -570,20 +561,28 @@
                     save()
     elif sys.platform == 'darwin':
         try:
             subprocess.Popen(['/usr/bin/open', filename])
         except OSError:
             save()
     else:
+        uri = GLib.filename_to_uri(filename)
         try:
-            subprocess.Popen(['xdg-open', filename])
-        except OSError:
+            Gio.AppInfo.launch_default_for_uri(uri)
+        except GLib.Error:
             save()
 
 
+def webbrowser_open(url):
+    try:
+        Gio.AppInfo.launch_default_for_uri(url)
+    except GLib.Error:
+        webbrowser.open(url)
+
+
 def url_open(uri):
     try:
         return urllib.request.urlopen(uri)
     except urllib.error.URLError:
         if sys.platform == 'win32' and uri.startswith('file://'):
             # There are two ways that Windows UNC filenames can be represented:
             # file://server/folder/data.xml
@@ -636,15 +635,15 @@
     if subject:
         url += "&subject=" + urllib.parse.quote(subject, "")
     if body:
         body = "\r\n".join(body.splitlines())
         url += "&body=" + urllib.parse.quote(body, "")
     if attachment:
         url += "&attachment=" + urllib.parse.quote(attachment, "")
-    webbrowser.open(url, new=1)
+    webbrowser_open(url, new=1)
 
 
 class UniqueDialog(object):
 
     def __init__(self):
         self.running = False
 
@@ -878,36 +877,35 @@
         dialog.vbox.pack_start(
             scrolledwindow, expand=True, fill=True, padding=0)
 
         button_roundup = Gtk.LinkButton.new_with_label(
             CONFIG['bug.url'], _("Report Bug"))
         button_roundup.get_child().set_halign(Gtk.Align.START)
         button_roundup.connect('activate-link',
-            lambda widget: webbrowser.open(CONFIG['bug.url'], new=2))
+            lambda widget: webbrowser_open(CONFIG['bug.url'], new=2))
         dialog.vbox.pack_start(
             button_roundup, expand=False, fill=False, padding=0)
 
         return dialog
 
     def __call__(self, title, details):
         if isinstance(title, Exception):
             title = "%s: %s" % (title.__class__.__name__, title)
         details += '\n' + title
-        log = logging.getLogger(__name__)
-        log.error(details)
+        logger.error(details)
         return super(ErrorDialog, self).__call__(title, details)
 
 
 error = ErrorDialog()
 
 
 def check_version(box, version=__version__):
     def info_bar_response(info_bar, response, box, url):
         if response == Gtk.ResponseType.ACCEPT:
-            webbrowser.open(url)
+            webbrowser_open(url)
         box.remove(info_bar)
 
     class HeadRequest(urllib.request.Request):
         def get_method(self):
             return 'HEAD'
 
     version = version.split('.')
@@ -951,15 +949,15 @@
 
 def open_documentation():
     version = __version__.split('.')[:2]
     if int(version[-1]) % 2:
         version = 'latest'
     else:
         version = '.'.join(version)
-    webbrowser.open(CONFIG['doc.url'] % {
+    webbrowser_open(CONFIG['doc.url'] % {
             'lang': CONFIG['client.lang'],
             'version': version,
             })
 
 
 def to_xml(string):
     return string.replace('&', '&amp;'
@@ -1045,15 +1043,15 @@
         url_parts = list(urlparse(url))
         query = dict(parse_qs(url_parts[4]))
         query['next'] = next_
         if user_id is not None:
             query['renew'] = user_id
         url_parts[4] = urlencode(query)
         url = urlunparse(url_parts)
-        webbrowser.open(url)
+        webbrowser_open(url)
 
         class RequestHandler(BaseHTTPRequestHandler):
             def do_GET(self):
                 self.send_response(200)
                 self.send_header('Content-Type', 'text/html')
                 self.end_headers()
                 try:
@@ -1223,15 +1221,15 @@
         self.callback = callback
 
         if callback:
             # Parent is only useful if it is asynchronous
             # otherwise the cursor is not updated.
             self.parent = get_toplevel_window()
             self._cursor_timeout = GLib.timeout_add(3000, self._set_cursor)
-            _thread.start_new_thread(self.start, ())
+            Thread(target=self.start).run()
             return
         else:
             self.start()
             return self.process()
 
     def _set_cursor(self):
         self._cursor_timeout = None
@@ -1361,22 +1359,37 @@
 
 
 def untimezoned_date(date):
     return timezoned_date(date, reverse=True)
 
 
 def humanize(size, suffix=''):
-    for u in ['', 'K', 'M', 'G', 'T', 'P']:
-        if size <= 1000:
-            if isinstance(size, int) or size.is_integer():
-                size = locale.localize('{0:.0f}'.format(size))
-            else:
-                size = locale.localize('{0:.{1}f}'.format(size, 2).rstrip('0'))
-            return ''.join([size, u, suffix])
-        size /= 1000.0
+    if 0 < abs(size) < 1:
+        for u in ['', 'm', 'µ', 'n', 'p', 'f', 'a', 'z', 'y', 'r', 'q']:
+            if abs(size) >= 0.01:
+                break
+            size *= 1000.0
+        else:
+            size /= 1000.0
+    else:
+        for u in ['', 'k', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y', 'R', 'Q']:
+            if abs(size) <= 1000:
+                break
+            size /= 1000.0
+        else:
+            size *= 1000.0
+    if isinstance(size, int) or size.is_integer():
+        size = locale.localize(str(int(size)))
+    elif abs(size) < 0.01:
+        size = locale.localize(
+            '{0:f}'.format(size).rstrip('0').rstrip('.'))
+    else:
+        size = locale.localize(
+            '{0:.{1}f}'.format(size, 2).rstrip('0').rstrip('.'))
+    return ''.join([size, u, suffix])
 
 
 def get_hostname(netloc):
     if '[' in netloc and ']' in netloc:
         hostname = netloc.split(']')[0][1:]
     elif ':' in netloc:
         hostname = netloc.split(':')[0]
@@ -1441,21 +1454,20 @@
     ellipsis = _('...')
     return string[:length - len(ellipsis)] + ellipsis
 
 
 def get_align(float_, expand=True):
     "Convert float align into Gtk.Align"
     value = float(float_)
+    if expand:
+        return Gtk.Align.FILL
     if value < 0.5:
         return Gtk.Align.START
     elif value == 0.5:
-        if expand:
-            return Gtk.Align.FILL
-        else:
-            return Gtk.Align.CENTER
+        return Gtk.Align.CENTER
     else:
         return Gtk.Align.END
 
 
 def date_format(format_=None):
     return format_ or rpc.CONTEXT.get('locale', {}).get('date', '%x')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tryton-6.6.7/tryton/common/completion.py` & `tryton-6.8.0/tryton/common/completion.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/datetime_.py` & `tryton-6.8.0/tryton/common/datetime_.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,16 +125,17 @@
     def cal_popup_open(self):
         self.parse()
         if self.__date:
             self.__calendar.select_month(
                 self.__date.month - 1, self.__date.year)
             self.__calendar.select_day(self.__date.day)
         self.__cal_popup.set_transient_for(self.get_toplevel())
-        popup_position(self, self.__cal_popup)
+        # Show popup before because position needs the popup allocation
         popup_show(self.__cal_popup)
+        popup_position(self, self.__cal_popup)
 
     def cal_popup_changed(self, calendar):
         year, month, day = self.__calendar.get_date()
         self.__date = datetime.date(year, month + 1, day)
 
         self.update_label()
 
@@ -528,16 +529,27 @@
 
 
 GObject.type_register(DateTime)
 
 
 def popup_position(widget, popup):
     allocation = widget.get_allocation()
+    popup_allocation = popup.get_allocation()
     x, y = widget.get_window().get_root_coords(allocation.x, allocation.y)
-    popup.move(x, y + allocation.height)
+    display = widget.get_display()
+    monitor = display.get_monitor_at_window(widget.get_window())
+    monitor_geometry = monitor.get_geometry()
+    if (monitor_geometry.height
+            < y + allocation.height + popup_allocation.height):
+        y -= popup_allocation.height
+    else:
+        y += allocation.height
+    if monitor_geometry.width < x + popup_allocation.width:
+        x -= popup_allocation.width
+    popup.move(x, y)
 
 
 def popup_show(popup):
     popup.show()
     popup.grab_focus()
     popup.grab_add()
```

### Comparing `tryton-6.6.7/tryton/common/domain_inversion.py` & `tryton-6.8.0/tryton/common/domain_inversion.py`

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

### Comparing `tryton-6.6.7/tryton/common/domain_parser.py` & `tryton-6.8.0/tryton/common/domain_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,18 @@
             break
         else:
             yield token
 
 
 def operatorize(tokens, operator='or'):
     "Convert operators"
-    test = (operator, (operator,))
+    test = {
+        'or': ('|', ('|',)),
+        'and': ('&', ('&',)),
+        }[operator]
     try:
         cur = next(tokens)
         while cur in test:
             cur = next(tokens)
     except StopIteration:
         return
     if isgenerator(cur):
@@ -652,15 +655,15 @@
                 formatted_value = '""'
             return '%s: %s%s' % (quote(field['string']), operator,
                 formatted_value)
 
         if not domain:
             return ''
         if domain[0] in ('AND', 'OR'):
-            nary = ' ' if domain[0] == 'AND' else ' or '
+            nary = ' ' if domain[0] == 'AND' else ' | '
             domain = domain[1:]
         else:
             nary = ' '
         return nary.join(string_(clause) for clause in domain)
 
     def completion(self, input_):
         "Return completion for the input string"
```

### Comparing `tryton-6.6.7/tryton/common/environment.py` & `tryton-6.8.0/tryton/common/environment.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/focus.py` & `tryton-6.8.0/tryton/common/focus.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/htmltextbuffer.py` & `tryton-6.8.0/tryton/common/htmltextbuffer.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/number_entry.py` & `tryton-6.8.0/tryton/common/number_entry.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/popup_menu.py` & `tryton-6.8.0/tryton/common/popup_menu.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from tryton.action import Action
 from tryton.common import RPCException, RPCExecute
 from tryton.common.common import selection
 from tryton.gui.window import Window
 from tryton.gui.window.attachment import Attachment
 from tryton.gui.window.email_ import Email
+from tryton.gui.window.log import Log
 from tryton.gui.window.note import Note
 from tryton.gui.window.view_form.screen import Screen
 
 _ = gettext.gettext
 
 
 def populate(menu, model, record, title='', field=None, context=None):
@@ -52,14 +53,17 @@
         allow_similar = False
         if (event.state & Gdk.ModifierType.CONTROL_MASK
                 or event.state & Gdk.ModifierType.MOD1_MASK):
             allow_similar = True
         with Window(hide_current=True, allow_similar=allow_similar):
             Action.execute(action, data, context=rec.get_context())
 
+    def log(menuitem):
+        Log(load(record))
+
     def attachment(menuitem):
         Attachment(load(record), None)
 
     def note(menuitem):
         Note(load(record), None)
 
     def is_report(action):
@@ -99,14 +103,17 @@
     if len(action_menu):
         action_menu.append(Gtk.SeparatorMenuItem())
     if field:
         edit_item = Gtk.MenuItem(label=_('Edit...'))
         edit_item.connect('activate', edit)
         action_menu.append(edit_item)
         action_menu.append(Gtk.SeparatorMenuItem())
+    log_item = Gtk.MenuItem(label=_("View Logs..."))
+    action_menu.append(log_item)
+    log_item.connect('activate', log)
     attachment_item = Gtk.MenuItem(label=_('Attachments...'))
     action_menu.append(attachment_item)
     attachment_item.connect('activate', attachment)
     note_item = Gtk.MenuItem(label=_('Notes...'))
     action_menu.append(note_item)
     note_item.connect('activate', note)
```

### Comparing `tryton-6.6.7/tryton/common/richtext.py` & `tryton-6.8.0/tryton/common/richtext.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/selection.py` & `tryton-6.8.0/tryton/common/selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         self.selection = selection[:]
         self.help = help_
         self.inactive_selection = []
 
     def update_selection(self, record, field):
         if not field:
             return
+        if not self.selection:
+            self.init_selection()
 
         domain = field.domain_get(record)
         if 'relation' not in self.attrs:
             change_with = self.attrs.get('selection_change_with') or []
             value = record._get_on_change_args(change_with)
             value.pop('id', None)
             self.init_selection(value)
@@ -67,15 +69,15 @@
             fields = ['rec_name']
             help_field = self.attrs.get('help_field')
             if help_field:
                 fields.append(help_field)
             try:
                 result = RPCExecute('model', self.attrs['relation'],
                     'search_read', domain, 0, None, None, fields,
-                    context=context)
+                    context=context, process_exception=False)
             except RPCException:
                 result = False
             if isinstance(result, list):
                 selection = [(x['id'], x['rec_name']) for x in result]
                 if self.nullable_widget:
                     selection.append((None, ''))
                 if help_field:
```

### Comparing `tryton-6.6.7/tryton/common/timedelta.py` & `tryton-6.8.0/tryton/common/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/common/underline.py` & `tryton-6.8.0/tryton/common/underline.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/config.py` & `tryton-6.8.0/tryton/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # this repository contains the full copyright notices and license terms.
 import configparser
 import gettext
 import locale
 import logging
 import optparse
 import os
+import shutil
 import sys
+import tempfile
 
 from gi.repository import GdkPixbuf
 
 from tryton import __version__
 
+logger = logging.getLogger(__name__)
 _ = gettext.gettext
 
 
 def get_config_dir():
     if os.name == 'nt':
         appdata = os.environ['APPDATA']
         if not isinstance(appdata, str):
@@ -64,15 +67,15 @@
             'graph.color': '#3465a4',
             'image.max_size': 10 ** 6,
             'image.cache_size': 1024,
             'doc.url': 'https://docs.tryton.org/en/%(version)s',
             'bug.url': 'https://bugs.tryton.org/',
             'download.url': 'https://downloads.tryton.org/',
             'download.frequency': 60 * 60 * 8,
-            'menu.pane': 200,
+            'menu.pane': 320,
         }
         self.config = {}
         self.options = {}
         self.arguments = []
 
     def parse(self):
         parser = optparse.OptionParser(version=("Tryton %s" % __version__),
@@ -90,14 +93,17 @@
                 "DEBUG, INFO, WARNING, ERROR, CRITICAL"))
         parser.add_option("-o", "--log-ouput", dest="log_output", default=None,
             help=_("specify the file used to output logging information"))
         parser.add_option("-u", "--user", dest="login",
                 help=_("specify the login user"))
         parser.add_option("-s", "--server", dest="host",
                 help=_("specify the server hostname:port"))
+        parser.add_option(
+            '--no-thread', default=True, action='store_false', dest='thread',
+            help=_("disable thread usage"))
         opt, self.arguments = parser.parse_args()
         self.rcfile = opt.config or os.path.join(
             get_config_dir(), 'tryton.conf')
         self.load()
 
         logging_config = {}
         if opt.log_output:
@@ -118,37 +124,48 @@
         logging_config['level'] = loglevels[opt.log_level.upper()]
         logging.basicConfig(**logging_config)
 
         self.options['dev'] = opt.dev
         for arg in ['login', 'host']:
             if getattr(opt, arg):
                 self.options['login.' + arg] = getattr(opt, arg)
+        self.options['thread'] = opt.thread
 
     def save(self):
         try:
             parser = configparser.ConfigParser()
             for entry in list(self.config.keys()):
                 if not len(entry.split('.')) == 2:
                     continue
                 section, name = entry.split('.')
                 if not parser.has_section(section):
                     parser.add_section(section)
                 parser.set(section, name, str(self.config[entry]))
             with open(self.rcfile, 'w') as fp:
                 parser.write(fp)
         except IOError:
-            logging.getLogger(__name__).warn(
-                _('Unable to write config file %s.')
-                % (self.rcfile,))
+            logger.warn("Unable to write config file %s", self.rcfile)
             return False
         return True
 
     def load(self):
         parser = configparser.ConfigParser()
-        parser.read([self.rcfile])
+        try:
+            parser.read([self.rcfile])
+        except configparser.Error:
+            config_dir = os.path.dirname(self.rcfile)
+            with tempfile.NamedTemporaryFile(
+                    delete=False, prefix='tryton_', suffix='.conf',
+                    dir=config_dir) as temp_file:
+                temp_name = temp_file.name
+            shutil.copy(self.rcfile, temp_name)
+            logger.error(
+                f"Failed to parse {self.rcfile}. "
+                f"A backup can be found at {temp_name}", exc_info=True)
+            return
         for section in parser.sections():
             for (name, value) in parser.items(section):
                 if value.lower() == 'true':
                     value = True
                 elif value.lower() == 'false':
                     value = False
                 if section == 'client' and name == 'limit':
```

### Comparing `tryton-6.6.7/tryton/data/locale/bg/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: bg\n"
 "Language-Team: bg <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.6.7/tryton/data/locale/bg/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 msgid "specify the login user"
 msgstr "укажете потребителското име"
 
 #, fuzzy
 msgid "specify the server hostname:port"
 msgstr "укажете адреса на сървъра"
 
-#, fuzzy, python-format
-msgid "Unable to write config file %s."
-msgstr "Не може да запише конфигурационен файл %s!"
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Не може да зададе локални настройки %s"
 
 #, fuzzy
 msgid ", "
@@ -65,20 +64,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "Вашия избор"
 
-msgid "Select"
-msgstr ""
-
-msgid "Save"
-msgstr "Съхраняване"
-
 msgid "Save As..."
 msgstr "Запис като ..."
 
 msgid "Do you want to proceed?"
 msgstr ""
 
 msgid "Always ignore this warning."
@@ -207,14 +200,18 @@
 msgid "Template"
 msgstr "Свързани"
 
 #, fuzzy
 msgid "Edit..."
 msgstr "Изход..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Преглед на логове"
+
 msgid "Attachments..."
 msgstr "Прикачен файл..."
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -624,14 +621,17 @@
 msgid "Select File"
 msgstr "Избор"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Изтриване <Del>"
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 #, fuzzy
 msgid "Preview"
 msgstr "Предишен"
 
@@ -649,36 +649,14 @@
 msgid "Note (%d/%d)"
 msgstr ""
 
 #, fuzzy
 msgid "You have to select one record."
 msgstr "Трябва да изберете един запис!"
 
-msgid "ID:"
-msgstr "ID:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Дата на създаване:"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Дата на създаване:"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Редактиране"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Редактиране"
-
-msgid "Model:"
-msgstr "Модел:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Наистина ли искате да изтриете този запис?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Наистина ли искате да изтриете тези записи?"
 
 #, fuzzy
@@ -741,14 +719,40 @@
 msgid "Search Limit Settings"
 msgstr "Настройки на органичения за търсене"
 
 msgid "Limit:"
 msgstr "Ограничение:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr "Модел:"
+
+msgid "ID:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Дата на създаване:"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Дата на създаване:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Последно променен от:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Дата на последна промяна:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr "Редактиране на потребителски настройки"
 
 msgid "Preference"
@@ -919,14 +923,17 @@
 
 msgid "Name"
 msgstr "Име"
 
 msgid "Open"
 msgstr "Отваряне"
 
+msgid "Save"
+msgstr "Съхраняване"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "Редактиране на избрания запис"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Редактиране на избрания запис"
@@ -1153,28 +1160,24 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-#, fuzzy
-msgid "Week View"
-msgstr "Превключване на изглед"
+msgid "Week"
+msgstr ""
 
 #, fuzzy
-msgid "Month View"
+msgid "Month"
 msgstr "Превключване на изглед"
 
-msgid "Week"
-msgstr ""
-
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr "Изчистване"
 
 msgid "All files"
@@ -1240,9 +1243,12 @@
 msgid "You need to save the record before adding translations."
 msgstr "Трябва да съхраните записа преди да добавите преводи!"
 
 #, fuzzy
 msgid "No other language available."
 msgstr "Няма наличен друг език!"
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Превод на изглед"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ca/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ca\n"
 "Language-Team: ca <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -15,14 +15,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" no és vàlid segons el seu domini."
 
 msgid "\"%s\" is required."
 msgstr "\"%s\" és obligatori."
 
+msgid "#ERROR"
+msgstr "#ERROR"
+
 msgid "%d record imported."
 msgstr "S'ha importat %d registre."
 
 msgid "%d record saved."
 msgstr "S'ha desat %d registre."
 
 msgid "%d records imported."
@@ -282,16 +285,16 @@
 
 msgid "Database:"
 msgstr "Base de dades:"
 
 msgid "Date Format"
 msgstr "Format dates"
 
-msgid "Day View"
-msgstr "Vista de dia"
+msgid "Day"
+msgstr "Dia"
 
 msgid "Default"
 msgstr "Per defecte"
 
 msgid "Delete"
 msgstr "Elimina"
 
@@ -345,23 +348,17 @@
 
 msgid "Edit..."
 msgstr "Edita..."
 
 msgid "Edited at"
 msgstr "Editat el"
 
-msgid "Edited at:"
-msgstr "Editat el:"
-
 msgid "Edited by"
 msgstr "Editat per"
 
-msgid "Edited by:"
-msgstr "Editat per:"
-
 msgid "Edition Shortcuts"
 msgstr "Accessos directes a l'edició"
 
 msgid "Encoding:"
 msgstr "Codificació:"
 
 msgid "Error"
@@ -462,14 +459,20 @@
 
 msgid "Justify"
 msgstr "Justificar"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Combinacions de tecles..."
 
+msgid "Last Modified at:"
+msgstr "Última modificació el:"
+
+msgid "Last Modified by:"
+msgstr "Última modificació per:"
+
 msgid "Launch action"
 msgstr "Executa acció"
 
 msgid "Limit"
 msgstr "Límit"
 
 msgid "Limit:"
@@ -489,14 +492,17 @@
 
 msgid "Listed Records"
 msgstr "Registres llistats"
 
 msgid "Login"
 msgstr "Accedeix"
 
+msgid "Logs (%s)"
+msgstr "Registres (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gestiona..."
 
 msgid "Mark line for deletion/removal"
@@ -504,16 +510,16 @@
 
 msgid "Mark line for removal"
 msgstr "Marcar línia per eliminar"
 
 msgid "Model:"
 msgstr "Model:"
 
-msgid "Month View"
-msgstr "Vista mensual"
+msgid "Month"
+msgstr "Mes"
 
 msgid "Move Cursor"
 msgstr "Mou cursor"
 
 msgid "Move down"
 msgstr "Mou avall"
 
@@ -929,17 +935,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "No s'ha pogut establir l'idioma %s"
 
 msgid "Unable to set view tree state"
 msgstr "No s'ha pogut desar l'estat de la vista d'arbre"
 
-msgid "Unable to write config file %s."
-msgstr "No s'ha pogut escriure el fitxer configuració %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Recupera el registre seleccionat <Ins>"
 
 msgid "Underline"
 msgstr "Subratllat"
 
 msgid "Unknown"
@@ -959,23 +962,23 @@
 
 msgid "Username:"
 msgstr "Nom d'usuari:"
 
 msgid "Value"
 msgstr "Valor"
 
+msgid "View Logs..."
+msgstr "Veure registres..."
+
 msgid "View _Logs..."
 msgstr "Veure _registre..."
 
 msgid "Week"
 msgstr "Setmana"
 
-msgid "Week View"
-msgstr "Vista setmanal"
-
 msgid "What is the name of this export?"
 msgstr "Quin és el nom d'aquesta exportació?"
 
 msgid "Width:"
 msgstr "Amplada:"
 
 msgid "Wizard"
@@ -1088,14 +1091,17 @@
 
 msgid "d"
 msgstr "d"
 
 msgid "development mode"
 msgstr "mode desenvolupament"
 
+msgid "disable thread usage"
+msgstr "desactiva l'ús de fils"
+
 msgid "go back"
 msgstr "vés enrere"
 
 msgid "go forward"
 msgstr "vés endavant"
 
 msgid "h"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ca/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 msgid "specify the login user"
 msgstr "Indica l'usuari"
 
 msgid "specify the server hostname:port"
 msgstr "Indica el nom:port del servidor"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "No s'ha pogut escriure el fitxer configuració %s."
+msgid "disable thread usage"
+msgstr "desactiva l'ús de fils"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "No s'ha pogut establir l'idioma %s"
 
 msgid ", "
 msgstr ", "
@@ -62,20 +61,14 @@
 
 msgid "OK"
 msgstr "D'acord"
 
 msgid "Your selection:"
 msgstr "La vostra selecció:"
 
-msgid "Select"
-msgstr "Selecciona"
-
-msgid "Save"
-msgstr "Desa"
-
 msgid "Save As..."
 msgstr "Desa com..."
 
 msgid "Do you want to proceed?"
 msgstr "Voleu continuar?"
 
 msgid "Always ignore this warning."
@@ -196,14 +189,17 @@
 
 msgid "Template"
 msgstr "Plantilla"
 
 msgid "Edit..."
 msgstr "Edita..."
 
+msgid "View Logs..."
+msgstr "Veure registres..."
+
 msgid "Attachments..."
 msgstr "Adjunts..."
 
 msgid "Notes..."
 msgstr "Notes..."
 
 msgid "Actions..."
@@ -589,14 +585,17 @@
 
 msgid "Select File"
 msgstr "Selecciona un fitxer"
 
 msgid "Remove File"
 msgstr "Elimina fitxer"
 
+msgid "Select"
+msgstr "Selecciona"
+
 msgid "Add..."
 msgstr "Afegeix..."
 
 msgid "Preview"
 msgstr "Previsualitza"
 
 msgid "Previous"
@@ -612,32 +611,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Nota (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Ha de seleccionar un registre."
 
-msgid "ID:"
-msgstr "Identificador:"
-
-msgid "Created by:"
-msgstr "Creat per:"
-
-msgid "Created at:"
-msgstr "Creat el:"
-
-msgid "Edited by:"
-msgstr "Editat per:"
-
-msgid "Edited at:"
-msgstr "Editat el:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Esteu segur que voleu eliminar aquest registre?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Esteu segur que voleu eliminar aquests registres?"
 
 msgid "Records not removed."
@@ -695,14 +676,36 @@
 msgid "Search Limit Settings"
 msgstr "Preferències del límit de cerca"
 
 msgid "Limit:"
 msgstr "Límit:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Registres (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "Identificador:"
+
+msgid "Created by:"
+msgstr "Creat per:"
+
+msgid "Created at:"
+msgstr "Creat el:"
+
+msgid "Last Modified by:"
+msgstr "Última modificació per:"
+
+msgid "Last Modified at:"
+msgstr "Última modificació el:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notes (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Edita preferències d'usuari"
 
 msgid "Preference"
@@ -861,14 +864,17 @@
 
 msgid "Name"
 msgstr "Nom"
 
 msgid "Open"
 msgstr "Obre"
 
+msgid "Save"
+msgstr "Desa"
+
 msgid "Listed Records"
 msgstr "Registres llistats"
 
 msgid "Selected Records"
 msgstr "Registres seleccionats"
 
 msgid "Ignore search limit"
@@ -1082,26 +1088,23 @@
 
 msgid "previous year"
 msgstr "any anterior"
 
 msgid "next year"
 msgstr "l'any següent"
 
-msgid "Day View"
-msgstr "Vista de dia"
-
-msgid "Week View"
-msgstr "Vista setmanal"
-
-msgid "Month View"
-msgstr "Vista mensual"
+msgid "Day"
+msgstr "Dia"
 
 msgid "Week"
 msgstr "Setmana"
 
+msgid "Month"
+msgstr "Mes"
+
 msgid "Select..."
 msgstr "Selecciona..."
 
 msgid "Clear"
 msgstr "Neteja"
 
 msgid "All files"
@@ -1159,9 +1162,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Heu de desar el registre abans d'afegir traduccions."
 
 msgid "No other language available."
 msgstr "No hi ha cap altre idioma disponible."
 
+msgid "#ERROR"
+msgstr "#ERROR"
+
 msgid "Translate view"
 msgstr "Tradueix la vista"
```

### Comparing `tryton-6.6.7/tryton/data/locale/cs/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.6.7/tryton/data/locale/cs/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 msgid "specify the login user"
 msgstr "zadejte uživatelské jméno"
 
 #, fuzzy
 msgid "specify the server hostname:port"
 msgstr "zadejte název hostitele pro server"
 
-#, fuzzy, python-format
-msgid "Unable to write config file %s."
-msgstr "Nelze zapsat konfigurační soubor %s!"
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Nemohu nastavit lokalizaci %s"
 
 #, fuzzy
 msgid ", "
@@ -65,21 +64,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "Váš výběr:"
 
-msgid "Select"
-msgstr ""
-
-#, fuzzy
-msgid "Save"
-msgstr "_Uložit"
-
 msgid "Save As..."
 msgstr "Uložit jako..."
 
 msgid "Do you want to proceed?"
 msgstr ""
 
 msgid "Always ignore this warning."
@@ -209,14 +201,18 @@
 msgstr "_Vytvořit"
 
 #, fuzzy
 msgid "Edit..."
 msgstr "Konec..."
 
 #, fuzzy
+msgid "View Logs..."
+msgstr "Zobrazit záznamy..."
+
+#, fuzzy
 msgid "Attachments..."
 msgstr "Příloha:"
 
 msgid "Notes..."
 msgstr ""
 
 #, fuzzy
@@ -631,14 +627,17 @@
 msgid "Select File"
 msgstr "Výběr"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "_Odstranit"
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 #, fuzzy
 msgid "Preview"
 msgstr "Předchozí"
 
@@ -656,35 +655,14 @@
 msgid "Note (%d/%d)"
 msgstr ""
 
 #, fuzzy
 msgid "You have to select one record."
 msgstr "Musíte vybrat právě jeden záznam!"
 
-msgid "ID:"
-msgstr "ID:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Datum vytvoření:"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Datum vytvoření:"
-
-msgid "Edited by:"
-msgstr ""
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Datum vytvoření:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Opravdu chcete odstranit tento záznam?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Opravdu chcete odstranit tyto záznamy?"
 
 #, fuzzy
@@ -753,14 +731,40 @@
 msgstr ""
 
 #, fuzzy
 msgid "Limit:"
 msgstr "Omezit:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Datum vytvoření:"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Datum vytvoření:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Poslední úpravu provedl:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Datum poslední úpravy:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr "Upravit uživatelské nastavení"
 
 msgid "Preference"
@@ -935,14 +939,18 @@
 msgid "Name"
 msgstr ""
 
 msgid "Open"
 msgstr "Otevřít"
 
 #, fuzzy
+msgid "Save"
+msgstr "_Uložit"
+
+#, fuzzy
 msgid "Listed Records"
 msgstr "Upravit vybraný záznam"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Upravit vybraný záznam"
 
@@ -1169,28 +1177,24 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-#, fuzzy
-msgid "Week View"
-msgstr "Přepnout pohled"
+msgid "Week"
+msgstr ""
 
 #, fuzzy
-msgid "Month View"
+msgid "Month"
 msgstr "Přepnout pohled"
 
-msgid "Week"
-msgstr ""
-
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr "Vymazat"
 
 msgid "All files"
@@ -1257,9 +1261,12 @@
 msgid "You need to save the record before adding translations."
 msgstr "Musíte uložit záznam před přidáváním překladů!"
 
 #, fuzzy
 msgid "No other language available."
 msgstr "Jiný jazyk není k dispozici!"
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Přeložit pohled"
```

### Comparing `tryton-6.6.7/tryton/data/locale/de/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -15,14 +15,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" liegt nicht im gültigen Wertebereich (Domain)."
 
 msgid "\"%s\" is required."
 msgstr "In Feld \"%s\" ist ein Eintrag erforderlich."
 
+msgid "#ERROR"
+msgstr "#FEHLER"
+
 msgid "%d record imported."
 msgstr "%d Datensatz importiert."
 
 msgid "%d record saved."
 msgstr "%d Datensatz gespeichert."
 
 msgid "%d records imported."
@@ -282,16 +285,16 @@
 
 msgid "Database:"
 msgstr "Datenbank:"
 
 msgid "Date Format"
 msgstr "Datumsformat"
 
-msgid "Day View"
-msgstr "Tagesansicht"
+msgid "Day"
+msgstr "Tag"
 
 msgid "Default"
 msgstr "Standard"
 
 msgid "Delete"
 msgstr "Löschen"
 
@@ -345,23 +348,17 @@
 
 msgid "Edit..."
 msgstr "Bearbeiten..."
 
 msgid "Edited at"
 msgstr "Bearbeitet um"
 
-msgid "Edited at:"
-msgstr "Zuletzt bearbeitet am:"
-
 msgid "Edited by"
 msgstr "Bearbeitet von"
 
-msgid "Edited by:"
-msgstr "Bearbeitet von:"
-
 msgid "Edition Shortcuts"
 msgstr "Tastenkombinationen Bearbeitung"
 
 msgid "Encoding:"
 msgstr "Zeichenkodierung:"
 
 msgid "Error"
@@ -462,14 +459,20 @@
 
 msgid "Justify"
 msgstr "Blocksatz"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Tastenkombinationen..."
 
+msgid "Last Modified at:"
+msgstr "Zuletzt verändert am:"
+
+msgid "Last Modified by:"
+msgstr "Zuletzt verändert von:"
+
 msgid "Launch action"
 msgstr "Aktion ausführen"
 
 msgid "Limit"
 msgstr "Limit"
 
 msgid "Limit:"
@@ -489,14 +492,17 @@
 
 msgid "Listed Records"
 msgstr "Angezeigte Datensätze"
 
 msgid "Login"
 msgstr "Log-in"
 
+msgid "Logs (%s)"
+msgstr "Logs (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Verwalten..."
 
 msgid "Mark line for deletion/removal"
@@ -504,16 +510,16 @@
 
 msgid "Mark line for removal"
 msgstr "Zeile zum Entfernen markieren"
 
 msgid "Model:"
 msgstr "Modell:"
 
-msgid "Month View"
-msgstr "Monatsansicht"
+msgid "Month"
+msgstr "Monat"
 
 msgid "Move Cursor"
 msgstr "Cursor bewegen"
 
 msgid "Move down"
 msgstr "Nach unten bewegen"
 
@@ -932,17 +938,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Kann locale %s nicht setzen."
 
 msgid "Unable to set view tree state"
 msgstr "Kann Sicht für den Menübaum nicht anwenden."
 
-msgid "Unable to write config file %s."
-msgstr "Kann Konfigurationsdatei '%s' nicht schreiben."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Löschung der ausgewählten Datensätze rückgängig machen <Einfg>"
 
 msgid "Underline"
 msgstr "Unterstrichen"
 
 msgid "Unknown"
@@ -962,23 +965,23 @@
 
 msgid "Username:"
 msgstr "Anmeldename:"
 
 msgid "Value"
 msgstr "Wert"
 
+msgid "View Logs..."
+msgstr "Logs anzeigen..."
+
 msgid "View _Logs..."
 msgstr "_Protokoll ansehen..."
 
 msgid "Week"
 msgstr "Woche"
 
-msgid "Week View"
-msgstr "Wochenansicht"
-
 msgid "What is the name of this export?"
 msgstr "Wie soll der Name des Exports lauten?"
 
 msgid "Width:"
 msgstr "Breite:"
 
 msgid "Wizard"
@@ -1093,14 +1096,17 @@
 
 msgid "d"
 msgstr "t"
 
 msgid "development mode"
 msgstr "Entwicklungsmodus"
 
+msgid "disable thread usage"
+msgstr "Threading deaktivieren"
+
 msgid "go back"
 msgstr "Rückwärts bewegen"
 
 msgid "go forward"
 msgstr "Vorwärts bewegen"
 
 msgid "h"
```

### Comparing `tryton-6.6.7/tryton/data/locale/de/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 msgid "specify the login user"
 msgstr "Anmeldename angeben"
 
 msgid "specify the server hostname:port"
 msgstr "Den Server mit Hostname:Port angeben."
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Kann Konfigurationsdatei '%s' nicht schreiben."
+msgid "disable thread usage"
+msgstr "Threading deaktivieren"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Kann locale %s nicht setzen."
 
 msgid ", "
 msgstr ", "
@@ -62,20 +61,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Ihre Auswahl:"
 
-msgid "Select"
-msgstr "Auswählen"
-
-msgid "Save"
-msgstr "Speichern"
-
 msgid "Save As..."
 msgstr "Speichern unter..."
 
 msgid "Do you want to proceed?"
 msgstr "Fortfahren?"
 
 msgid "Always ignore this warning."
@@ -198,14 +191,17 @@
 
 msgid "Template"
 msgstr "Vorlage"
 
 msgid "Edit..."
 msgstr "Bearbeiten..."
 
+msgid "View Logs..."
+msgstr "Logs anzeigen..."
+
 msgid "Attachments..."
 msgstr "Anhänge..."
 
 msgid "Notes..."
 msgstr "Notizen..."
 
 msgid "Actions..."
@@ -596,14 +592,17 @@
 
 msgid "Select File"
 msgstr "Datei auswählen"
 
 msgid "Remove File"
 msgstr "Datei entfernen"
 
+msgid "Select"
+msgstr "Auswählen"
+
 msgid "Add..."
 msgstr "Hinzufügen..."
 
 msgid "Preview"
 msgstr "Vorschau"
 
 msgid "Previous"
@@ -619,32 +618,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Notiz (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Ein Datensatz muss ausgewählt werden."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Erstellt von:"
-
-msgid "Created at:"
-msgstr "Erstellt am:"
-
-msgid "Edited by:"
-msgstr "Bearbeitet von:"
-
-msgid "Edited at:"
-msgstr "Zuletzt bearbeitet am:"
-
-msgid "Model:"
-msgstr "Modell:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Möchten Sie diesen Datensatz wirklich löschen?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Möchten Sie diese Datensätze wirklich löschen?"
 
 msgid "Records not removed."
@@ -702,14 +683,36 @@
 msgid "Search Limit Settings"
 msgstr "Einstellung Suchlimit"
 
 msgid "Limit:"
 msgstr "Limit:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Logs (%s)"
+
+msgid "Model:"
+msgstr "Modell:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Erstellt von:"
+
+msgid "Created at:"
+msgstr "Erstellt am:"
+
+msgid "Last Modified by:"
+msgstr "Zuletzt verändert von:"
+
+msgid "Last Modified at:"
+msgstr "Zuletzt verändert am:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notizen (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Benutzereinstellungen bearbeiten"
 
 msgid "Preference"
@@ -868,14 +871,17 @@
 
 msgid "Name"
 msgstr "Name"
 
 msgid "Open"
 msgstr "Öffnen"
 
+msgid "Save"
+msgstr "Speichern"
+
 msgid "Listed Records"
 msgstr "Angezeigte Datensätze"
 
 msgid "Selected Records"
 msgstr "Ausgewählte Datensätze"
 
 msgid "Ignore search limit"
@@ -1089,26 +1095,23 @@
 
 msgid "previous year"
 msgstr "Vorheriges Jahr"
 
 msgid "next year"
 msgstr "Nächstes Jahr"
 
-msgid "Day View"
-msgstr "Tagesansicht"
-
-msgid "Week View"
-msgstr "Wochenansicht"
-
-msgid "Month View"
-msgstr "Monatsansicht"
+msgid "Day"
+msgstr "Tag"
 
 msgid "Week"
 msgstr "Woche"
 
+msgid "Month"
+msgstr "Monat"
+
 msgid "Select..."
 msgstr "Auswählen..."
 
 msgid "Clear"
 msgstr "Leeren"
 
 msgid "All files"
@@ -1168,9 +1171,12 @@
 msgstr ""
 "Der Datensatz muss gespeichert werden, bevor eine Übersetzung hinzugefügt "
 "werden kann."
 
 msgid "No other language available."
 msgstr "Keine weitere Sprache verfügbar."
 
+msgid "#ERROR"
+msgstr "#FEHLER"
+
 msgid "Translate view"
 msgstr "Aktuelle Sicht übersetzen"
```

### Comparing `tryton-6.6.7/tryton/data/locale/es/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -15,14 +15,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" no es válido según su dominio."
 
 msgid "\"%s\" is required."
 msgstr "\"%s\" es obligatorio."
 
+msgid "#ERROR"
+msgstr "#ERROR"
+
 msgid "%d record imported."
 msgstr "Se ha importado %d registro."
 
 msgid "%d record saved."
 msgstr "Se ha guardado %d registro."
 
 msgid "%d records imported."
@@ -282,16 +285,16 @@
 
 msgid "Database:"
 msgstr "Base de datos:"
 
 msgid "Date Format"
 msgstr "Formato fecha"
 
-msgid "Day View"
-msgstr "Vista de día"
+msgid "Day"
+msgstr "Día"
 
 msgid "Default"
 msgstr "Por defecto"
 
 msgid "Delete"
 msgstr "Eliminar"
 
@@ -345,23 +348,17 @@
 
 msgid "Edit..."
 msgstr "Editar..."
 
 msgid "Edited at"
 msgstr "Editado el"
 
-msgid "Edited at:"
-msgstr "Editado el:"
-
 msgid "Edited by"
 msgstr "Editado por"
 
-msgid "Edited by:"
-msgstr "Editado por:"
-
 msgid "Edition Shortcuts"
 msgstr "Atajos de edición"
 
 msgid "Encoding:"
 msgstr "Codificación:"
 
 msgid "Error"
@@ -462,14 +459,20 @@
 
 msgid "Justify"
 msgstr "Justificar"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Combinaciones de teclas..."
 
+msgid "Last Modified at:"
+msgstr "Última modificación el:"
+
+msgid "Last Modified by:"
+msgstr "Última modificación por:"
+
 msgid "Launch action"
 msgstr "Ejecutar acción"
 
 msgid "Limit"
 msgstr "Límite"
 
 msgid "Limit:"
@@ -489,14 +492,17 @@
 
 msgid "Listed Records"
 msgstr "Registros listados"
 
 msgid "Login"
 msgstr "Acceder"
 
+msgid "Logs (%s)"
+msgstr "Registros (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gestionar..."
 
 msgid "Mark line for deletion/removal"
@@ -504,16 +510,16 @@
 
 msgid "Mark line for removal"
 msgstr "Marcar para eliminar"
 
 msgid "Model:"
 msgstr "Modelo:"
 
-msgid "Month View"
-msgstr "Vista mensual"
+msgid "Month"
+msgstr "Mes"
 
 msgid "Move Cursor"
 msgstr "Mover cursor"
 
 msgid "Move down"
 msgstr "Mover abajo"
 
@@ -929,17 +935,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "No se ha podido establecer el idioma %s"
 
 msgid "Unable to set view tree state"
 msgstr "No se ha podido establecer el estado de expansión del árbol"
 
-msgid "Unable to write config file %s."
-msgstr "No se ha podido escribir el archivo de configuración %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Recuperar registro seleccionado <Ins>"
 
 msgid "Underline"
 msgstr "Subrayado"
 
 msgid "Unknown"
@@ -959,23 +962,23 @@
 
 msgid "Username:"
 msgstr "Nombre de usuario:"
 
 msgid "Value"
 msgstr "Valor"
 
+msgid "View Logs..."
+msgstr "Ver registros..."
+
 msgid "View _Logs..."
 msgstr "Ver _registro..."
 
 msgid "Week"
 msgstr "Semana"
 
-msgid "Week View"
-msgstr "Vista semanal"
-
 msgid "What is the name of this export?"
 msgstr "¿Cuál es el nombre de esta exportación?"
 
 msgid "Width:"
 msgstr "Anchura:"
 
 msgid "Wizard"
@@ -1088,14 +1091,17 @@
 
 msgid "d"
 msgstr "d"
 
 msgid "development mode"
 msgstr "Modo desarrollo"
 
+msgid "disable thread usage"
+msgstr "desactivar el uso de hilos"
+
 msgid "go back"
 msgstr "retroceder"
 
 msgid "go forward"
 msgstr "ir adelante"
 
 msgid "h"
```

### Comparing `tryton-6.6.7/tryton/data/locale/es/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 
 msgid "specify the login user"
 msgstr "Indica el usuario"
 
 msgid "specify the server hostname:port"
 msgstr "Indica el nombre:puerto del servidor"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "No se ha podido escribir el archivo de configuración %s."
+msgid "disable thread usage"
+msgstr "desactivar el uso de hilos"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "No se ha podido establecer el idioma %s"
 
 msgid ", "
 msgstr ", "
@@ -66,20 +65,14 @@
 
 msgid "OK"
 msgstr "Aceptar"
 
 msgid "Your selection:"
 msgstr "Su selección:"
 
-msgid "Select"
-msgstr "Seleccionar"
-
-msgid "Save"
-msgstr "Guardar"
-
 msgid "Save As..."
 msgstr "Guardar como..."
 
 msgid "Do you want to proceed?"
 msgstr "¿Desea continuar?"
 
 msgid "Always ignore this warning."
@@ -200,14 +193,17 @@
 
 msgid "Template"
 msgstr "Plantilla"
 
 msgid "Edit..."
 msgstr "Editar..."
 
+msgid "View Logs..."
+msgstr "Ver registros..."
+
 msgid "Attachments..."
 msgstr "Adjuntos..."
 
 msgid "Notes..."
 msgstr "Notas..."
 
 msgid "Actions..."
@@ -593,14 +589,17 @@
 
 msgid "Select File"
 msgstr "Seleccionar un archivo"
 
 msgid "Remove File"
 msgstr "Eliminar archivo"
 
+msgid "Select"
+msgstr "Seleccionar"
+
 msgid "Add..."
 msgstr "Añadir..."
 
 msgid "Preview"
 msgstr "Previsualizar"
 
 msgid "Previous"
@@ -616,32 +615,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Nota (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Debe elegir un registro."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Creado por:"
-
-msgid "Created at:"
-msgstr "Creado el:"
-
-msgid "Edited by:"
-msgstr "Editado por:"
-
-msgid "Edited at:"
-msgstr "Editado el:"
-
-msgid "Model:"
-msgstr "Modelo:"
-
 msgid "Are you sure to remove this record?"
 msgstr "¿Está seguro que quiere eliminar este registro?"
 
 msgid "Are you sure to remove those records?"
 msgstr "¿Está seguro que quiere eliminar estos registros?"
 
 msgid "Records not removed."
@@ -699,14 +680,36 @@
 msgid "Search Limit Settings"
 msgstr "Preferencias del límite de búsqueda"
 
 msgid "Limit:"
 msgstr "Límite:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Registros (%s)"
+
+msgid "Model:"
+msgstr "Modelo:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Creado por:"
+
+msgid "Created at:"
+msgstr "Creado el:"
+
+msgid "Last Modified by:"
+msgstr "Última modificación por:"
+
+msgid "Last Modified at:"
+msgstr "Última modificación el:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notas (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Editar preferencias de usuario"
 
 msgid "Preference"
@@ -865,14 +868,17 @@
 
 msgid "Name"
 msgstr "Nombre"
 
 msgid "Open"
 msgstr "Abrir"
 
+msgid "Save"
+msgstr "Guardar"
+
 msgid "Listed Records"
 msgstr "Registros listados"
 
 msgid "Selected Records"
 msgstr "Registros seleccionados"
 
 msgid "Ignore search limit"
@@ -1086,26 +1092,23 @@
 
 msgid "previous year"
 msgstr "año anterior"
 
 msgid "next year"
 msgstr "año próximo"
 
-msgid "Day View"
-msgstr "Vista de día"
-
-msgid "Week View"
-msgstr "Vista semanal"
-
-msgid "Month View"
-msgstr "Vista mensual"
+msgid "Day"
+msgstr "Día"
 
 msgid "Week"
 msgstr "Semana"
 
+msgid "Month"
+msgstr "Mes"
+
 msgid "Select..."
 msgstr "Seleccionar…"
 
 msgid "Clear"
 msgstr "Limpiar"
 
 msgid "All files"
@@ -1163,9 +1166,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Debe guardar el registro antes de añadir traducciones."
 
 msgid "No other language available."
 msgstr "No hay otro idioma disponible."
 
+msgid "#ERROR"
+msgstr "#ERROR"
+
 msgid "Translate view"
 msgstr "Traducir vista"
```

### Comparing `tryton-6.6.7/tryton/data/locale/es_419/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Translations template for tryton.
-# Copyright (C) 2016 Tryton
+# Copyright (C) 2018 Tryton
 # This file is distributed under the same license as the tryton project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2018.
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgid "specify alternate config file"
 msgstr ""
 
 msgid "development mode"
@@ -22,24 +22,24 @@
 
 msgid "specify the login user"
 msgstr ""
 
 msgid "specify the server hostname:port"
 msgstr ""
 
-#, python-format
-msgid "Unable to write config file %s."
+msgid "disable thread usage"
 msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
+#, fuzzy
 msgid ", "
-msgstr ""
+msgstr ", "
 
 msgid ",..."
 msgstr ""
 
 #, python-format
 msgid "%s (%s)"
 msgstr ""
@@ -61,20 +61,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr ""
 
-msgid "Select"
-msgstr ""
-
-msgid "Save"
-msgstr ""
-
 msgid "Save As..."
 msgstr ""
 
 msgid "Do you want to proceed?"
 msgstr ""
 
 msgid "Always ignore this warning."
@@ -101,15 +95,15 @@
 msgid "See the modified version"
 msgstr ""
 
 msgid "Write Anyway"
 msgstr ""
 
 msgid "Save your current version"
-msgstr "Guardar tu versión actual"
+msgstr ""
 
 #, python-format
 msgid "Compare: %s"
 msgstr ""
 
 msgid "Close"
 msgstr ""
@@ -141,16 +135,17 @@
 
 msgid "Not found."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+#, fuzzy
 msgid "..."
-msgstr ""
+msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
 msgid "<i>Create...</i>"
 msgstr ""
 
@@ -195,14 +190,17 @@
 
 msgid "Template"
 msgstr ""
 
 msgid "Edit..."
 msgstr ""
 
+msgid "View Logs..."
+msgstr ""
+
 msgid "Attachments..."
 msgstr ""
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -486,15 +484,15 @@
 msgid "Close Tab"
 msgstr ""
 
 msgid "modularity, scalability and security"
 msgstr ""
 
 msgid "translator-credits"
-msgstr "Sebastian Marro"
+msgstr ""
 
 #, python-format
 msgid "Attachments (%s)"
 msgstr ""
 
 msgid "Profile Editor"
 msgstr ""
@@ -586,14 +584,17 @@
 
 msgid "Select File"
 msgstr ""
 
 msgid "Remove File"
 msgstr ""
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 msgid "Preview"
 msgstr ""
 
 msgid "Previous"
@@ -609,36 +610,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr ""
 
-msgid "ID:"
-msgstr ""
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Fecha creación:"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Fecha creación:"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Editar"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Editar"
-
-msgid "Model:"
-msgstr ""
-
 msgid "Are you sure to remove this record?"
 msgstr ""
 
 msgid "Are you sure to remove those records?"
 msgstr ""
 
 msgid "Records not removed."
@@ -694,14 +673,36 @@
 msgid "Search Limit Settings"
 msgstr ""
 
 msgid "Limit:"
 msgstr ""
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr ""
+
+msgid "ID:"
+msgstr ""
+
+msgid "Created by:"
+msgstr ""
+
+msgid "Created at:"
+msgstr ""
+
+msgid "Last Modified by:"
+msgstr ""
+
+msgid "Last Modified at:"
+msgstr ""
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr ""
 
 msgid "Preference"
@@ -860,14 +861,17 @@
 
 msgid "Name"
 msgstr ""
 
 msgid "Open"
 msgstr ""
 
+msgid "Save"
+msgstr ""
+
 msgid "Listed Records"
 msgstr ""
 
 msgid "Selected Records"
 msgstr ""
 
 msgid "Ignore search limit"
@@ -982,29 +986,25 @@
 
 msgid "Wizard"
 msgstr ""
 
 msgid "ID"
 msgstr ""
 
-#, fuzzy
 msgid "Created by"
-msgstr "Fecha creación:"
+msgstr ""
 
-#, fuzzy
 msgid "Created at"
-msgstr "Fecha creación:"
+msgstr ""
 
-#, fuzzy
 msgid "Edited by"
-msgstr "Editar"
+msgstr ""
 
-#, fuzzy
 msgid "Edited at"
-msgstr "Editar"
+msgstr ""
 
 msgid "Unable to set view tree state"
 msgstr ""
 
 #, python-format
 msgid "\"%s\" is not valid according to its domain."
 msgstr ""
@@ -1016,16 +1016,17 @@
 #, python-format
 msgid "The values of \"%s\" are not valid."
 msgstr ""
 
 msgid "Pre-validation"
 msgstr ""
 
+#, fuzzy
 msgid ":"
-msgstr ""
+msgstr ":"
 
 msgid "Image Size"
 msgstr ""
 
 msgid "Width:"
 msgstr ""
 
@@ -1043,16 +1044,17 @@
 
 msgid "Copy"
 msgstr ""
 
 msgid "Paste"
 msgstr ""
 
+#, fuzzy
 msgid ".."
-msgstr ""
+msgstr ".."
 
 msgid "Open filters"
 msgstr ""
 
 msgid "Show bookmarks of filters"
 msgstr ""
 
@@ -1085,24 +1087,21 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
+msgid "Week"
 msgstr ""
 
-msgid "Month View"
-msgstr ""
-
-msgid "Week"
+msgid "Month"
 msgstr ""
 
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr ""
@@ -1154,17 +1153,20 @@
 msgid "Translation"
 msgstr ""
 
 msgid "Edit"
 msgstr ""
 
 msgid "Fuzzy"
-msgstr "Revisión"
+msgstr ""
 
 msgid "You need to save the record before adding translations."
 msgstr ""
 
 msgid "No other language available."
 msgstr ""
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tryton-6.6.7/tryton/data/locale/et/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: et\n"
 "Language-Team: et <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -228,17 +228,14 @@
 
 msgid "Database:"
 msgstr "Andmebaas:"
 
 msgid "Date Format"
 msgstr "Kuupäevaformaat"
 
-msgid "Day View"
-msgstr "Päeva vaade"
-
 msgid "Default"
 msgstr "Vaikimisi"
 
 msgid "Delete"
 msgstr "Kustuta"
 
 msgid "Delete selected record"
@@ -375,26 +372,26 @@
 
 msgid "Link"
 msgstr "Link"
 
 msgid "Login"
 msgstr "Logi sisse"
 
+msgid "Logs (%s)"
+msgstr "Palgid (%s)"
+
 msgid "M"
 msgstr "K"
 
 msgid "Manage..."
 msgstr "Halda..."
 
 msgid "Model:"
 msgstr "Mudel:"
 
-msgid "Month View"
-msgstr "Kuu vaade"
-
 msgid "Move down"
 msgstr "Liigu alla"
 
 msgid "Move down of one page"
 msgstr "Liigu lehekülg alla"
 
 msgid "Move left"
@@ -719,17 +716,14 @@
 
 msgid "True"
 msgstr "Tõene"
 
 msgid "Unable to set locale %s"
 msgstr "Ei saa seadistada lokaati %s"
 
-msgid "Unable to write config file %s."
-msgstr "Ei saa kirjutada konfiguratsioonifaili %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Taasta valitud kirje <Ins>"
 
 msgid "Underline"
 msgstr "Allajoonitud"
 
 msgid "Unknown"
@@ -752,17 +746,14 @@
 
 msgid "View _Logs..."
 msgstr "Vaata _logisid"
 
 msgid "Week"
 msgstr "Nädal"
 
-msgid "Week View"
-msgstr "Nädala vaade"
-
 msgid "Width:"
 msgstr "Laius:"
 
 msgid "Wizard"
 msgstr "Nõustaja"
 
 msgid "Write Anyway"
```

### Comparing `tryton-6.6.7/tryton/data/locale/et/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "määra kasutaja sisselogimise tunnus"
 
 msgid "specify the server hostname:port"
 msgstr "määra server:port"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Ei saa kirjutada konfiguratsioonifaili %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Ei saa seadistada lokaati %s"
 
 msgid ", "
 msgstr ", "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Teie valik:"
 
-msgid "Select"
-msgstr "Vali"
-
-msgid "Save"
-msgstr "Salvesta"
-
 msgid "Save As..."
 msgstr "Salvesta nimega..."
 
 msgid "Do you want to proceed?"
 msgstr "Kas soovid jätkata?"
 
 msgid "Always ignore this warning."
@@ -200,14 +193,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "Seo"
 
 msgid "Edit..."
 msgstr "Muuda..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Vaata _logisid"
+
 msgid "Attachments..."
 msgstr "Manused..."
 
 msgid "Notes..."
 msgstr "Märkused..."
 
 msgid "Actions..."
@@ -603,14 +600,17 @@
 msgid "Select File"
 msgstr "Vali kõik"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Eemalda <Del>"
 
+msgid "Select"
+msgstr "Vali"
+
 msgid "Add..."
 msgstr "Lisa..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "Eelmine"
 
@@ -627,36 +627,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Märkus (%d%d)"
 
 msgid "You have to select one record."
 msgstr "Pead valima vähemasti ühe rea."
 
-msgid "ID:"
-msgstr "ID"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Loomise kuupäev"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Loomise kuupäev"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Muuda"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Muuda"
-
-msgid "Model:"
-msgstr "Mudel:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Oled kindel, et kustutada see kirje?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Oled kindel, et kustutada need kirjed?"
 
 msgid "Records not removed."
@@ -714,14 +692,40 @@
 msgid "Search Limit Settings"
 msgstr "Otsingupiirangu seaded"
 
 msgid "Limit:"
 msgstr "Limiit"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Palgid (%s)"
+
+msgid "Model:"
+msgstr "Mudel:"
+
+msgid "ID:"
+msgstr "ID"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Loomise kuupäev"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Loomise kuupäev"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Muutja:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Muutmise kuupäev:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Märkused (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Muuda kasutaja eelistusi"
 
 msgid "Preference"
@@ -882,14 +886,17 @@
 
 msgid "Name"
 msgstr "Nimi"
 
 msgid "Open"
 msgstr "Ava"
 
+msgid "Save"
+msgstr "Salvesta"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "Muuda valitud kirjet"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Muuda valitud kirjet"
@@ -1109,26 +1116,24 @@
 
 msgid "previous year"
 msgstr "eelmine aasta"
 
 msgid "next year"
 msgstr "järgmine aasta"
 
-msgid "Day View"
-msgstr "Päeva vaade"
-
-msgid "Week View"
-msgstr "Nädala vaade"
-
-msgid "Month View"
-msgstr "Kuu vaade"
+msgid "Day"
+msgstr ""
 
 msgid "Week"
 msgstr "Nädal"
 
+#, fuzzy
+msgid "Month"
+msgstr "Kuu vaade"
+
 msgid "Select..."
 msgstr "Vali..."
 
 msgid "Clear"
 msgstr "Tühjenda"
 
 msgid "All files"
@@ -1186,9 +1191,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Kirje tuleb salvestada enne tõlke lisamist."
 
 msgid "No other language available."
 msgstr "Teisi keeli pole saadaval."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Tõlgi vaade"
```

### Comparing `tryton-6.6.7/tryton/data/locale/fa/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -348,26 +348,26 @@
 
 msgid "Link"
 msgstr "پیوند"
 
 msgid "Login"
 msgstr "ورود به سیستم"
 
+msgid "Logs (%s)"
+msgstr "سیاهههای مربوط (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "مدیریت..."
 
 msgid "Model:"
 msgstr "مدل:"
 
-msgid "Month View"
-msgstr "نمایش ماه"
-
 msgid "Move Cursor"
 msgstr "حرکت مکان نما"
 
 msgid "Move down"
 msgstr "حرکت به پایین"
 
 msgid "Move down of one page"
@@ -692,17 +692,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "قادر به تنظیم محلی: \"%s\" نیست"
 
 msgid "Unable to set view tree state"
 msgstr "قادر به تنظیم حالت نمایش درختی نیست"
 
-msgid "Unable to write config file %s."
-msgstr "قادر به نوشتن در فایل پیکربندی \"%s\" نیست."
-
 msgid "Undelete selected record <Ins>"
 msgstr "بازگردانی فایل انتخابی <Ins>"
 
 msgid "Unknown"
 msgstr "نامعلوم"
 
 msgid "Unmark line for deletion"
@@ -722,17 +719,14 @@
 
 msgid "View _Logs..."
 msgstr "_مشاهده گزارشات..."
 
 msgid "Week"
 msgstr "هفته"
 
-msgid "Week View"
-msgstr "نمایش هفته"
-
 msgid "What is the name of this export?"
 msgstr "نام این فایل استخراجی چیست؟"
 
 msgid "Width:"
 msgstr "عرض:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/fa/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "تعیین ورود به سیستم کاربر"
 
 msgid "specify the server hostname:port"
 msgstr "تعیین نام میزبان سرور : درگاه"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "قادر به نوشتن در فایل پیکربندی \"%s\" نیست."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "قادر به تنظیم محلی: \"%s\" نیست"
 
 msgid ", "
 msgstr "، "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr "بلی"
 
 msgid "Your selection:"
 msgstr "انتخاب شما:"
 
-msgid "Select"
-msgstr "انتخاب"
-
-msgid "Save"
-msgstr "ذخیره"
-
 msgid "Save As..."
 msgstr "ذخیره با نام..."
 
 msgid "Do you want to proceed?"
 msgstr "آیا می خواهید پردازش شود؟"
 
 msgid "Always ignore this warning."
@@ -200,14 +193,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "مرتبط"
 
 msgid "Edit..."
 msgstr "ویرایش..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "_مشاهده گزارشات..."
+
 msgid "Attachments..."
 msgstr "پیوست ها..."
 
 msgid "Notes..."
 msgstr "یادداشت ها..."
 
 msgid "Actions..."
@@ -608,14 +605,17 @@
 msgid "Select File"
 msgstr "انتخاب همه"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "حذف <Del>"
 
+msgid "Select"
+msgstr "انتخاب"
+
 msgid "Add..."
 msgstr "افزودن..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "قبلی"
 
@@ -632,36 +632,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr "شما باید یک پرونده را انتخاب کنید."
 
-msgid "ID:"
-msgstr "شناسه:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "تاریخ ایجاد"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "تاریخ ایجاد"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "ویرایش"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "ویرایش"
-
-msgid "Model:"
-msgstr "مدل:"
-
 msgid "Are you sure to remove this record?"
 msgstr "برای حذف این پرونده اطمینان کامل دارید؟"
 
 msgid "Are you sure to remove those records?"
 msgstr "برای حذف این پرونده ها اطمینان کامل دارید؟"
 
 msgid "Records not removed."
@@ -719,14 +697,40 @@
 msgid "Search Limit Settings"
 msgstr "تنظیمات جستجو محدود"
 
 msgid "Limit:"
 msgstr "محدودیت:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "سیاهههای مربوط (%s)"
+
+msgid "Model:"
+msgstr "مدل:"
+
+msgid "ID:"
+msgstr "شناسه:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "تاریخ ایجاد"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "تاریخ ایجاد"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "آخرین تغییرات بوسیله:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "تاریخ آخرین تغییرات:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "یادداشت ها(%s)"
 
 msgid "Edit User Preferences"
 msgstr "ویرایش ظاهر برنامه کاربر"
 
 msgid "Preference"
@@ -887,14 +891,17 @@
 
 msgid "Name"
 msgstr "نام"
 
 msgid "Open"
 msgstr "باز کردن"
 
+msgid "Save"
+msgstr "ذخیره"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "ویرایش پرونده انتخابی <F2>"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "ویرایش پرونده انتخابی <F2>"
@@ -1115,26 +1122,24 @@
 
 msgid "previous year"
 msgstr "سال قبل"
 
 msgid "next year"
 msgstr "سال بعد"
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "نمایش هفته"
-
-msgid "Month View"
-msgstr "نمایش ماه"
-
 msgid "Week"
 msgstr "هفته"
 
+#, fuzzy
+msgid "Month"
+msgstr "نمایش ماه"
+
 msgid "Select..."
 msgstr "انتخاب..."
 
 msgid "Clear"
 msgstr "پاک کردن"
 
 msgid "All files"
@@ -1194,9 +1199,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "قبل از اضافه کردن ترجمه ها شما باید پرونده را ذخیره کنید."
 
 msgid "No other language available."
 msgstr "هیچ زبان دیگری در دسترس نیست."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "نمایش ترجمه"
```

### Comparing `tryton-6.6.7/tryton/data/locale/fi/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/tryton.pot`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-# Translations template for tryton.
-# Copyright (C) 2018 Tryton
-# This file is distributed under the same license as the tryton project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2018.
-msgid ""
-msgstr "Content-Type: text/plain; charset=utf-8\n"
-
 msgid "specify alternate config file"
 msgstr ""
 
 msgid "development mode"
 msgstr ""
 
 msgid "logging everything at INFO level"
@@ -22,25 +15,23 @@
 
 msgid "specify the login user"
 msgstr ""
 
 msgid "specify the server hostname:port"
 msgstr ""
 
-#, python-format
-msgid "Unable to write config file %s."
+msgid "disable thread usage"
 msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
-#, fuzzy
 msgid ", "
-msgstr ", "
+msgstr ""
 
 msgid ",..."
 msgstr ""
 
 #, python-format
 msgid "%s (%s)"
 msgstr ""
@@ -62,20 +53,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr ""
 
-msgid "Select"
-msgstr ""
-
-msgid "Save"
-msgstr ""
-
 msgid "Save As..."
 msgstr ""
 
 msgid "Do you want to proceed?"
 msgstr ""
 
 msgid "Always ignore this warning."
@@ -142,17 +127,16 @@
 
 msgid "Not found."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
-#, fuzzy
 msgid "..."
-msgstr "..."
+msgstr ""
 
 msgid "<i>Search...</i>"
 msgstr ""
 
 msgid "<i>Create...</i>"
 msgstr ""
 
@@ -197,14 +181,17 @@
 
 msgid "Template"
 msgstr ""
 
 msgid "Edit..."
 msgstr ""
 
+msgid "View Logs..."
+msgstr ""
+
 msgid "Attachments..."
 msgstr ""
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -588,14 +575,17 @@
 
 msgid "Select File"
 msgstr ""
 
 msgid "Remove File"
 msgstr ""
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 msgid "Preview"
 msgstr ""
 
 msgid "Previous"
@@ -611,32 +601,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr ""
 
-msgid "ID:"
-msgstr ""
-
-msgid "Created by:"
-msgstr ""
-
-msgid "Created at:"
-msgstr ""
-
-msgid "Edited by:"
-msgstr ""
-
-msgid "Edited at:"
-msgstr ""
-
-msgid "Model:"
-msgstr ""
-
 msgid "Are you sure to remove this record?"
 msgstr ""
 
 msgid "Are you sure to remove those records?"
 msgstr ""
 
 msgid "Records not removed."
@@ -692,14 +664,36 @@
 msgid "Search Limit Settings"
 msgstr ""
 
 msgid "Limit:"
 msgstr ""
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr ""
+
+msgid "ID:"
+msgstr ""
+
+msgid "Created by:"
+msgstr ""
+
+msgid "Created at:"
+msgstr ""
+
+msgid "Last Modified by:"
+msgstr ""
+
+msgid "Last Modified at:"
+msgstr ""
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr ""
 
 msgid "Preference"
@@ -858,14 +852,17 @@
 
 msgid "Name"
 msgstr ""
 
 msgid "Open"
 msgstr ""
 
+msgid "Save"
+msgstr ""
+
 msgid "Listed Records"
 msgstr ""
 
 msgid "Selected Records"
 msgstr ""
 
 msgid "Ignore search limit"
@@ -1010,17 +1007,16 @@
 #, python-format
 msgid "The values of \"%s\" are not valid."
 msgstr ""
 
 msgid "Pre-validation"
 msgstr ""
 
-#, fuzzy
 msgid ":"
-msgstr ":"
+msgstr ""
 
 msgid "Image Size"
 msgstr ""
 
 msgid "Width:"
 msgstr ""
 
@@ -1038,17 +1034,16 @@
 
 msgid "Copy"
 msgstr ""
 
 msgid "Paste"
 msgstr ""
 
-#, fuzzy
 msgid ".."
-msgstr ".."
+msgstr ""
 
 msgid "Open filters"
 msgstr ""
 
 msgid "Show bookmarks of filters"
 msgstr ""
 
@@ -1081,24 +1076,21 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr ""
-
-msgid "Month View"
+msgid "Week"
 msgstr ""
 
-msgid "Week"
+msgid "Month"
 msgstr ""
 
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr ""
@@ -1158,9 +1150,13 @@
 
 msgid "You need to save the record before adding translations."
 msgstr ""
 
 msgid "No other language available."
 msgstr ""
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr ""
+
```

### Comparing `tryton-6.6.7/tryton/data/locale/fr/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -15,14 +15,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "« %s » n'est pas valide selon son domaine."
 
 msgid "\"%s\" is required."
 msgstr "« %s » est requis."
 
+msgid "#ERROR"
+msgstr "#ERREUR"
+
 msgid "%d record imported."
 msgstr "%d enregistrement importé."
 
 msgid "%d record saved."
 msgstr "%d enregistrement sauvé."
 
 msgid "%d records imported."
@@ -282,16 +285,16 @@
 
 msgid "Database:"
 msgstr "Base de données :"
 
 msgid "Date Format"
 msgstr "Format de date"
 
-msgid "Day View"
-msgstr "Vue jour"
+msgid "Day"
+msgstr "Jour"
 
 msgid "Default"
 msgstr "Défaut"
 
 msgid "Delete"
 msgstr "Supprimer"
 
@@ -345,23 +348,17 @@
 
 msgid "Edit..."
 msgstr "Éditer..."
 
 msgid "Edited at"
 msgstr "Édité le"
 
-msgid "Edited at:"
-msgstr "Édité le :"
-
 msgid "Edited by"
 msgstr "Édité par"
 
-msgid "Edited by:"
-msgstr "Édité par :"
-
 msgid "Edition Shortcuts"
 msgstr "Éditer les raccourcis"
 
 msgid "Encoding:"
 msgstr "Codage :"
 
 msgid "Error"
@@ -462,14 +459,20 @@
 
 msgid "Justify"
 msgstr "Justifier"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Raccourcis clavier..."
 
+msgid "Last Modified at:"
+msgstr "Dernière modification à :"
+
+msgid "Last Modified by:"
+msgstr "Dernière modification par :"
+
 msgid "Launch action"
 msgstr "Lancer une action"
 
 msgid "Limit"
 msgstr "Limite"
 
 msgid "Limit:"
@@ -489,14 +492,17 @@
 
 msgid "Listed Records"
 msgstr "Enregistrements listés"
 
 msgid "Login"
 msgstr "Connexion"
 
+msgid "Logs (%s)"
+msgstr "Journaux (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gérer..."
 
 msgid "Mark line for deletion/removal"
@@ -504,16 +510,16 @@
 
 msgid "Mark line for removal"
 msgstr "Marquer la ligne pour enlèvement"
 
 msgid "Model:"
 msgstr "Modèle :"
 
-msgid "Month View"
-msgstr "Vue mois"
+msgid "Month"
+msgstr "Mois"
 
 msgid "Move Cursor"
 msgstr "Déplacer le curseur"
 
 msgid "Move down"
 msgstr "Déplacer vers le bas"
 
@@ -930,17 +936,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Impossible de sélectionner la locale %s"
 
 msgid "Unable to set view tree state"
 msgstr "Impossible de définir l'état de la vue arbre"
 
-msgid "Unable to write config file %s."
-msgstr "Impossible d'écrire le fichier de configuration %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Restaurer l'enregistrement sélectionné<Ins>"
 
 msgid "Underline"
 msgstr "Souligné"
 
 msgid "Unknown"
@@ -960,23 +963,23 @@
 
 msgid "Username:"
 msgstr "Nom d'utilisateur :"
 
 msgid "Value"
 msgstr "Valeur"
 
+msgid "View Logs..."
+msgstr "Voir les journaux..."
+
 msgid "View _Logs..."
-msgstr "Voir les _Logs..."
+msgstr "Voir les _journaux..."
 
 msgid "Week"
 msgstr "Semaine"
 
-msgid "Week View"
-msgstr "Vue semaine"
-
 msgid "What is the name of this export?"
 msgstr "Quel est le nom de cet export ?"
 
 msgid "Width:"
 msgstr "Largeur :"
 
 msgid "Wizard"
@@ -1090,14 +1093,17 @@
 
 msgid "d"
 msgstr "j"
 
 msgid "development mode"
 msgstr "mode développement"
 
+msgid "disable thread usage"
+msgstr "désactiver l'utilisation des threads"
+
 msgid "go back"
 msgstr "revenir"
 
 msgid "go forward"
 msgstr "avancer"
 
 msgid "h"
```

### Comparing `tryton-6.6.7/tryton/data/locale/fr/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 msgid "specify the login user"
 msgstr "spécifier l'identifiant de l'utilisateur"
 
 msgid "specify the server hostname:port"
 msgstr "spécifier le nom du serveur:port"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Impossible d'écrire le fichier de configuration %s."
+msgid "disable thread usage"
+msgstr "désactiver l'utilisation des threads"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Impossible de sélectionner la locale %s"
 
 msgid ", "
 msgstr ", "
@@ -62,20 +61,14 @@
 
 msgid "OK"
 msgstr "Valider"
 
 msgid "Your selection:"
 msgstr "Votre sélection :"
 
-msgid "Select"
-msgstr "Sélectionner"
-
-msgid "Save"
-msgstr "Sauver"
-
 msgid "Save As..."
 msgstr "Enregistrer sous..."
 
 msgid "Do you want to proceed?"
 msgstr "Souhaitez-vous continuer ?"
 
 msgid "Always ignore this warning."
@@ -198,14 +191,17 @@
 
 msgid "Template"
 msgstr "Modèle"
 
 msgid "Edit..."
 msgstr "Éditer..."
 
+msgid "View Logs..."
+msgstr "Voir les journaux..."
+
 msgid "Attachments..."
 msgstr "Attachements..."
 
 msgid "Notes..."
 msgstr "Notes..."
 
 msgid "Actions..."
@@ -593,14 +589,17 @@
 
 msgid "Select File"
 msgstr "Choisir un fichier"
 
 msgid "Remove File"
 msgstr "Supprimer le fichier"
 
+msgid "Select"
+msgstr "Sélectionner"
+
 msgid "Add..."
 msgstr "Ajouter..."
 
 msgid "Preview"
 msgstr "Aperçu"
 
 msgid "Previous"
@@ -616,32 +615,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Note (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Vous devez sélectionner un enregistrement."
 
-msgid "ID:"
-msgstr "ID :"
-
-msgid "Created by:"
-msgstr "Crée par :"
-
-msgid "Created at:"
-msgstr "Crée le :"
-
-msgid "Edited by:"
-msgstr "Édité par :"
-
-msgid "Edited at:"
-msgstr "Édité le :"
-
-msgid "Model:"
-msgstr "Modèle :"
-
 msgid "Are you sure to remove this record?"
 msgstr "Êtes-vous sûr de vouloir supprimer cet enregistrement ?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Êtes-vous sûr de vouloir supprimer ces enregistrements ?"
 
 msgid "Records not removed."
@@ -699,14 +680,36 @@
 msgid "Search Limit Settings"
 msgstr "Limite de recherche"
 
 msgid "Limit:"
 msgstr "Limite :"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Journaux (%s)"
+
+msgid "Model:"
+msgstr "Modèle :"
+
+msgid "ID:"
+msgstr "ID :"
+
+msgid "Created by:"
+msgstr "Crée par :"
+
+msgid "Created at:"
+msgstr "Crée le :"
+
+msgid "Last Modified by:"
+msgstr "Dernière modification par :"
+
+msgid "Last Modified at:"
+msgstr "Dernière modification à :"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notes (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Éditer les préférences utilisateur"
 
 msgid "Preference"
@@ -763,15 +766,15 @@
 msgid "_Duplicate"
 msgstr "_Dupliquer"
 
 msgid "_Delete..."
 msgstr "Su_pprimer..."
 
 msgid "View _Logs..."
-msgstr "Voir les _Logs..."
+msgstr "Voir les _journaux..."
 
 msgid "Show revisions..."
 msgstr "Afficher les révisions..."
 
 msgid "A_ttachments..."
 msgstr "_Pièce jointes..."
 
@@ -865,14 +868,17 @@
 
 msgid "Name"
 msgstr "Nom"
 
 msgid "Open"
 msgstr "Ouvrir"
 
+msgid "Save"
+msgstr "Sauver"
+
 msgid "Listed Records"
 msgstr "Enregistrements listés"
 
 msgid "Selected Records"
 msgstr "Enregistrements sélectionnés"
 
 msgid "Ignore search limit"
@@ -1086,26 +1092,23 @@
 
 msgid "previous year"
 msgstr "année précédente"
 
 msgid "next year"
 msgstr "année suivante"
 
-msgid "Day View"
-msgstr "Vue jour"
-
-msgid "Week View"
-msgstr "Vue semaine"
-
-msgid "Month View"
-msgstr "Vue mois"
+msgid "Day"
+msgstr "Jour"
 
 msgid "Week"
 msgstr "Semaine"
 
+msgid "Month"
+msgstr "Mois"
+
 msgid "Select..."
 msgstr "Sélectionner..."
 
 msgid "Clear"
 msgstr "Effacer"
 
 msgid "All files"
@@ -1164,9 +1167,12 @@
 msgid "You need to save the record before adding translations."
 msgstr ""
 "Vous devez sauvegarder l'enregistrement avant d'ajouter des traductions."
 
 msgid "No other language available."
 msgstr "Pas d'autre langue disponible."
 
+msgid "#ERROR"
+msgstr "#ERREUR"
+
 msgid "Translate view"
 msgstr "Traduire la vue"
```

### Comparing `tryton-6.6.7/tryton/data/locale/hu/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu\n"
 "Language-Team: hu <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -291,23 +291,17 @@
 
 msgid "Edit..."
 msgstr "Módosítás…"
 
 msgid "Edited at"
 msgstr "Módosítás dátuma"
 
-msgid "Edited at:"
-msgstr "Módosítás dátuma:"
-
 msgid "Edited by"
 msgstr "Módosította"
 
-msgid "Edited by:"
-msgstr "Módosította:"
-
 msgid "Edition Shortcuts"
 msgstr "Szerkesztés gyorsbillentyűi"
 
 msgid "Encoding:"
 msgstr "Kódolás:"
 
 msgid "Error"
@@ -435,17 +429,14 @@
 
 msgid "Mark line for removal"
 msgstr "Sor törlésre jelölése"
 
 msgid "Model:"
 msgstr "Elem:"
 
-msgid "Month View"
-msgstr "Havi nézet"
-
 msgid "Move Cursor"
 msgstr "Lépkedés a listaelemek között"
 
 msgid "Move down"
 msgstr "Le"
 
 msgid "Move down of one page"
@@ -858,17 +849,14 @@
 
 msgid "View _Logs..."
 msgstr "Nap_ló megtekintése…"
 
 msgid "Week"
 msgstr "Hét"
 
-msgid "Week View"
-msgstr "Heti nézet"
-
 msgid "What is the name of this export?"
 msgstr "Mi legyen az oszloplista neve?"
 
 msgid "Width:"
 msgstr "Szélesség:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/hu/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "adja meg a felhasználónevet"
 
 msgid "specify the server hostname:port"
 msgstr "adja meg a kiszolgálónév:portot"
 
-#, fuzzy, python-format
-msgid "Unable to write config file %s."
-msgstr "Nem lehet a következő konfigurációs fájlba írni: „%s”"
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Nem lehet beállítani a %s nyelvet"
 
 #, fuzzy
 msgid ", "
@@ -63,20 +62,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Kiválasztva"
 
-msgid "Select"
-msgstr "Kiválaszt"
-
-msgid "Save"
-msgstr "Mentés"
-
 msgid "Save As..."
 msgstr "Mentés másként…"
 
 msgid "Do you want to proceed?"
 msgstr "Akarja folyatni?"
 
 msgid "Always ignore this warning."
@@ -201,14 +194,18 @@
 
 msgid "Template"
 msgstr "Sablon"
 
 msgid "Edit..."
 msgstr "Módosítás…"
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Nap_ló megtekintése…"
+
 msgid "Attachments..."
 msgstr "Mellékletek..."
 
 msgid "Notes..."
 msgstr "Jegyzetek..."
 
 msgid "Actions..."
@@ -597,14 +594,17 @@
 #, fuzzy
 msgid "Select File"
 msgstr "Mind kijelölése"
 
 msgid "Remove File"
 msgstr "Fájl eltávolítása"
 
+msgid "Select"
+msgstr "Kiválaszt"
+
 msgid "Add..."
 msgstr "Hozzáadás..."
 
 msgid "Preview"
 msgstr "Előnézet"
 
 msgid "Previous"
@@ -620,32 +620,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Jegyzet (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Ki kell választania egy rekordot."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Létrehozta:"
-
-msgid "Created at:"
-msgstr "Létrehozás dátuma:"
-
-msgid "Edited by:"
-msgstr "Módosította:"
-
-msgid "Edited at:"
-msgstr "Módosítás dátuma:"
-
-msgid "Model:"
-msgstr "Elem:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Biztos törölni szeretné?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Biztos törölni szeretné?"
 
 msgid "Records not removed."
@@ -703,14 +685,38 @@
 msgid "Search Limit Settings"
 msgstr "Keresett rekordok számának korlátozása"
 
 msgid "Limit:"
 msgstr "Korlát:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr "Elem:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Létrehozta:"
+
+msgid "Created at:"
+msgstr "Létrehozás dátuma:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Utolsó módosítás"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Módosítás dátuma "
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr "Felhasználói beállítások szerkesztése"
 
 msgid "Preference"
@@ -869,14 +875,17 @@
 
 msgid "Name"
 msgstr "Név"
 
 msgid "Open"
 msgstr "Megnyitás"
 
+msgid "Save"
+msgstr "Mentés"
+
 msgid "Listed Records"
 msgstr "A listán szereplő összes rekordot"
 
 msgid "Selected Records"
 msgstr "Csak a kiválasztott rekordokat"
 
 msgid "Ignore search limit"
@@ -1092,26 +1101,24 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "Heti nézet"
-
-msgid "Month View"
-msgstr "Havi nézet"
-
 msgid "Week"
 msgstr "Hét"
 
+#, fuzzy
+msgid "Month"
+msgstr "Havi nézet"
+
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr "Törlés"
 
 msgid "All files"
@@ -1169,9 +1176,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "El kell menteni a rekordot mielőtt hozzáadja a fordítást."
 
 msgid "No other language available."
 msgstr "Másik nyelv nem elérhető."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Nézet lefordítása"
```

### Comparing `tryton-6.6.7/tryton/data/locale/id/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: id\n"
 "Language-Team: id <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -156,23 +156,17 @@
 
 msgid "Edit..."
 msgstr "Sunting..."
 
 msgid "Edited at"
 msgstr "Disunting pada"
 
-msgid "Edited at:"
-msgstr "Disunting pada:"
-
 msgid "Edited by"
 msgstr "Disunting oleh"
 
-msgid "Edited by:"
-msgstr "Disunting oleh:"
-
 msgid "False"
 msgstr "Salah"
 
 msgid "Files"
 msgstr "Berkas-Berkas"
 
 msgid "Foreground Color"
@@ -210,14 +204,17 @@
 
 msgid "Limit"
 msgstr "Batasan"
 
 msgid "Link"
 msgstr "Tautan"
 
+msgid "Logs (%s)"
+msgstr "Log (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "Move Cursor"
@@ -400,17 +397,14 @@
 
 msgid "True"
 msgstr "Benar"
 
 msgid "Unable to check for new version."
 msgstr "Tidak dapat memeriksa versi baru."
 
-msgid "Unable to write config file %s."
-msgstr "Tidak dapat menulis file konfigurasi %s."
-
 msgid "Underline"
 msgstr "Garis Bawah"
 
 msgid "Value"
 msgstr "Nilai"
 
 msgid "Week"
```

### Comparing `tryton-6.6.7/tryton/data/locale/id/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 
 msgid "specify the login user"
 msgstr "tentukan user login"
 
 msgid "specify the server hostname:port"
 msgstr "tentukan nama host server:port"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Tidak dapat menulis file konfigurasi %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
 msgid ", "
 msgstr ", "
@@ -58,20 +57,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Pilihan Anda:"
 
-msgid "Select"
-msgstr "Pilih"
-
-msgid "Save"
-msgstr "Simpan"
-
 msgid "Save As..."
 msgstr "Simpan Sebagai..."
 
 msgid "Do you want to proceed?"
 msgstr "Apakah Anda ingin melanjutkan?"
 
 msgid "Always ignore this warning."
@@ -193,14 +186,17 @@
 
 msgid "Template"
 msgstr "Templat"
 
 msgid "Edit..."
 msgstr "Sunting..."
 
+msgid "View Logs..."
+msgstr ""
+
 msgid "Attachments..."
 msgstr ""
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -586,14 +582,17 @@
 
 msgid "Select File"
 msgstr "Pilih Berkas"
 
 msgid "Remove File"
 msgstr "Hapus Berkas"
 
+msgid "Select"
+msgstr "Pilih"
+
 msgid "Add..."
 msgstr ""
 
 msgid "Preview"
 msgstr "Pratinjau"
 
 msgid "Previous"
@@ -609,32 +608,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Catatan (%d/%d)"
 
 msgid "You have to select one record."
 msgstr ""
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Dibuat oleh:"
-
-msgid "Created at:"
-msgstr "Dibuat pada:"
-
-msgid "Edited by:"
-msgstr "Disunting oleh:"
-
-msgid "Edited at:"
-msgstr "Disunting pada:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr ""
 
 msgid "Are you sure to remove those records?"
 msgstr ""
 
 msgid "Records not removed."
@@ -690,14 +671,36 @@
 msgid "Search Limit Settings"
 msgstr ""
 
 msgid "Limit:"
 msgstr ""
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Log (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Dibuat oleh:"
+
+msgid "Created at:"
+msgstr "Dibuat pada:"
+
+msgid "Last Modified by:"
+msgstr ""
+
+msgid "Last Modified at:"
+msgstr ""
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr ""
 
 msgid "Preference"
@@ -856,14 +859,17 @@
 
 msgid "Name"
 msgstr "Nama"
 
 msgid "Open"
 msgstr "Buka"
 
+msgid "Save"
+msgstr "Simpan"
+
 msgid "Listed Records"
 msgstr ""
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Pilih satu warna"
 
@@ -1078,26 +1084,23 @@
 
 msgid "previous year"
 msgstr "tahun sebelumnya"
 
 msgid "next year"
 msgstr "tahun berikutnya"
 
-msgid "Day View"
-msgstr ""
-
-msgid "Week View"
-msgstr ""
-
-msgid "Month View"
+msgid "Day"
 msgstr ""
 
 msgid "Week"
 msgstr "Pekan"
 
+msgid "Month"
+msgstr ""
+
 msgid "Select..."
 msgstr "Pilih..."
 
 msgid "Clear"
 msgstr "Bersihkan"
 
 msgid "All files"
@@ -1155,9 +1158,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr ""
 
 msgid "No other language available."
 msgstr "Tidak ada bahasa lain yang tersedia."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr ""
```

### Comparing `tryton-6.6.7/tryton/data/locale/it/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -267,20 +267,14 @@
 
 msgid "Edit User Preferences"
 msgstr "Modifica le preferenze dell'utente"
 
 msgid "Edit..."
 msgstr "Modifica..."
 
-msgid "Edited at:"
-msgstr "Modifica il:"
-
-msgid "Edited by:"
-msgstr "Modificato da:"
-
 msgid "Encoding:"
 msgstr "Codifica:"
 
 msgid "Error"
 msgstr "Errore"
 
 msgid "Error processing the file at field %s."
@@ -375,14 +369,17 @@
 
 msgid "Listed Records"
 msgstr "Record elencati"
 
 msgid "Login"
 msgstr "Accedi"
 
+msgid "Logs (%s)"
+msgstr "Registri (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gestisci..."
 
 msgid "Mark line for deletion/removal"
@@ -390,17 +387,14 @@
 
 msgid "Mark line for removal"
 msgstr "Contrassegnare la linea per la rimozione"
 
 msgid "Model:"
 msgstr "Modello:"
 
-msgid "Month View"
-msgstr "Vista mensile"
-
 msgid "Move Cursor"
 msgstr "Sposta cursore"
 
 msgid "Move down"
 msgstr "Spostati giù"
 
 msgid "Move down of one page"
@@ -743,17 +737,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Impossibile impostare la localizzazione %s"
 
 msgid "Unable to set view tree state"
 msgstr "Impossibile configurare la vista ad albero"
 
-msgid "Unable to write config file %s."
-msgstr "Impossibile scrivere il file di configurazione %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Non eliminare il record selezionato <Ins>"
 
 msgid "Unknown"
 msgstr "Sconosciuto"
 
 msgid "Unmark line for deletion"
@@ -776,17 +767,14 @@
 
 msgid "View _Logs..."
 msgstr "Visualizza_Log..."
 
 msgid "Week"
 msgstr "Settimana"
 
-msgid "Week View"
-msgstr "Vista settimanale"
-
 msgid "What is the name of this export?"
 msgstr "Qual è il nome di questa esportazione?"
 
 msgid "Wizard"
 msgstr "Wizard"
 
 msgid "Working now on the duplicated record(s)."
```

### Comparing `tryton-6.6.7/tryton/data/locale/it/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 msgid "specify the login user"
 msgstr "specifica l'utente di accesso"
 
 msgid "specify the server hostname:port"
 msgstr "specifica hostname:porta del server"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Impossibile scrivere il file di configurazione %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Impossibile impostare la localizzazione %s"
 
 msgid ", "
 msgstr ", "
@@ -62,20 +61,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "La tua selezione:"
 
-msgid "Select"
-msgstr "Seleziona"
-
-msgid "Save"
-msgstr "Salva"
-
 msgid "Save As..."
 msgstr "Salva come..."
 
 msgid "Do you want to proceed?"
 msgstr "Procedere?"
 
 msgid "Always ignore this warning."
@@ -200,14 +193,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "Collegato"
 
 msgid "Edit..."
 msgstr "Modifica..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Visualizza_Log..."
+
 msgid "Attachments..."
 msgstr "Allegati..."
 
 msgid "Notes..."
 msgstr "Appunti..."
 
 msgid "Actions..."
@@ -598,14 +595,17 @@
 msgid "Select File"
 msgstr "Seleziona tutto"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "_Rimuovi"
 
+msgid "Select"
+msgstr "Seleziona"
+
 msgid "Add..."
 msgstr "Inserisci..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "Precedente"
 
@@ -622,32 +622,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Appunto (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Devi selezionare un record."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Creato da:"
-
-msgid "Created at:"
-msgstr "Creato il:"
-
-msgid "Edited by:"
-msgstr "Modificato da:"
-
-msgid "Edited at:"
-msgstr "Modifica il:"
-
-msgid "Model:"
-msgstr "Modello:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Sei sicuro di rimuovere questo record?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Sei sicuro di rimuovere questi records?"
 
 msgid "Records not removed."
@@ -705,14 +687,38 @@
 msgid "Search Limit Settings"
 msgstr "Impostazione dei limiti di ricerca"
 
 msgid "Limit:"
 msgstr "Limite:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Registri (%s)"
+
+msgid "Model:"
+msgstr "Modello:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Creato da:"
+
+msgid "Created at:"
+msgstr "Creato il:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Ultima modifica a:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Ultima data di modifica:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Appunti (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Modifica le preferenze dell'utente"
 
 msgid "Preference"
@@ -873,14 +879,17 @@
 
 msgid "Name"
 msgstr "Nome"
 
 msgid "Open"
 msgstr "Apri"
 
+msgid "Save"
+msgstr "Salva"
+
 msgid "Listed Records"
 msgstr "Record elencati"
 
 msgid "Selected Records"
 msgstr "Record selezionati"
 
 msgid "Ignore search limit"
@@ -1100,26 +1109,24 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "Vista settimanale"
-
-msgid "Month View"
-msgstr "Vista mensile"
-
 msgid "Week"
 msgstr "Settimana"
 
+#, fuzzy
+msgid "Month"
+msgstr "Vista mensile"
+
 msgid "Select..."
 msgstr "Seleziona..."
 
 msgid "Clear"
 msgstr "Pulisci"
 
 msgid "All files"
@@ -1180,9 +1187,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "È necessario salvare il record prima di aggiungere le traduzioni."
 
 msgid "No other language available."
 msgstr "Nessun altra lingua è disponibile."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Traduci vista"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja_JP\n"
 "Language-Team: ja_JP <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/locale/lo/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lo\n"
 "Language-Team: lo <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -282,23 +282,23 @@
 
 msgid "Link"
 msgstr "ເຊື່ອມໂຍງ"
 
 msgid "Login"
 msgstr "ເຂົ້າສູ່ລະບົບ"
 
+msgid "Logs (%s)"
+msgstr "ໄມ້ທ່ອນ (%s)"
+
 msgid "M"
 msgstr "ດ"
 
 msgid "Model:"
 msgstr "ແບບ:"
 
-msgid "Month View"
-msgstr "ເບິ່ງເປັນເດືອນ"
-
 msgid "Move Cursor"
 msgstr "ຍ້າຍ ເຄິກເຊີຣ໌"
 
 msgid "Move down"
 msgstr "ຍ້າຍລົງ"
 
 msgid "Move down of one page"
@@ -573,17 +573,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "ບໍ່ສາມາດຕັ້ງຄ່າ ທ້ອງຖິ່ນ %s ໄດ້."
 
 msgid "Unable to set view tree state"
 msgstr "ບໍ່ສາມາດຕັ້ງຄ່າສະຖານະມູມມອງແບບຕົ້ນໄມ້ໄດ້"
 
-msgid "Unable to write config file %s."
-msgstr "ບໍ່ສາມາດ ຂຽນ ຟາຍລ໌ ຕັ້ງຄ່າ (config file) %s ນີ້ໄດ້."
-
 msgid "Undelete selected record <Ins>"
 msgstr "ຍົກເລີກການລຶບແຖວທີ່ເລືອກ"
 
 msgid "Unknown"
 msgstr "ບໍ່ຮູ້"
 
 msgid "Unmark line for deletion"
@@ -603,17 +600,14 @@
 
 msgid "View _Logs..."
 msgstr "ເບິ່ງ_ບັນທຶກ..."
 
 msgid "Week"
 msgstr "ອາທິດ"
 
-msgid "Week View"
-msgstr "ເບິ່ງເປັນລາຍອາທິດ"
-
 msgid "What is the name of this export?"
 msgstr "ຊື່ຂອງການສົ່ງອອກນີ້ແມ່ນຫຍັງ?"
 
 msgid "Width:"
 msgstr "ຄວາມກວ້າງ:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/lo/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 msgid "specify the login user"
 msgstr "ລະບຸ ຜູ້ເຂົ້າໃຊ້ງານ"
 
 #, fuzzy
 msgid "specify the server hostname:port"
 msgstr "ລະບຸ ທີ່ຢູ່ ຂອງ ເຄື່ອງແມ່ຂ່າຍ"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "ບໍ່ສາມາດ ຂຽນ ຟາຍລ໌ ຕັ້ງຄ່າ (config file) %s ນີ້ໄດ້."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "ບໍ່ສາມາດຕັ້ງຄ່າ ທ້ອງຖິ່ນ %s ໄດ້."
 
 msgid ", "
 msgstr ","
@@ -64,20 +63,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "ການເລືອກຂອງທ່ານ:"
 
-msgid "Select"
-msgstr "ເລືອກ..."
-
-msgid "Save"
-msgstr "ບັນທຶກ"
-
 msgid "Save As..."
 msgstr "ບັນທຶກເປັນ..."
 
 msgid "Do you want to proceed?"
 msgstr "ທ່ານຕ້ອງການດຳເນີນການຕໍ່ໄປບໍ່?"
 
 msgid "Always ignore this warning."
@@ -203,14 +196,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "ທີ່ກ່ຽວພັນ"
 
 msgid "Edit..."
 msgstr "ແກ້ໄຂ..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "ເບິ່ງ_ບັນທຶກ..."
+
 msgid "Attachments..."
 msgstr "ຄັດຕິດ..."
 
 msgid "Notes..."
 msgstr "ໝາຍເຫດ..."
 
 msgid "Actions..."
@@ -622,14 +619,17 @@
 msgid "Select File"
 msgstr "ເລືອກທັງໝົດ"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "ເອົາອອກ"
 
+msgid "Select"
+msgstr "ເລືອກ..."
+
 msgid "Add..."
 msgstr ""
 
 #, fuzzy
 msgid "Preview"
 msgstr "ກ່ອນໜ້າ"
 
@@ -646,36 +646,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr "ທ່ານຕ້ອງໄດ້ເລືອກ ໜຶ່ງແຖວຂໍ້ມູນ."
 
-msgid "ID:"
-msgstr "ເລກລໍາດັບ:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "ວັນທີສ້າງ"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "ວັນທີສ້າງ"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "ແກ້ໄຂ"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "ແກ້ໄຂ"
-
-msgid "Model:"
-msgstr "ແບບ:"
-
 msgid "Are you sure to remove this record?"
 msgstr "ທ່ານແນ່ໃຈບໍ່ທີ່ຈະລຶບແຖວຂໍ້ມູນນີ້?"
 
 msgid "Are you sure to remove those records?"
 msgstr "ທ່ານແນ່ໃຈບໍ່ທີ່ຈະລຶບແຖວຂໍ້ມູນເຫຼົ່ານີ້?"
 
 msgid "Records not removed."
@@ -731,14 +709,40 @@
 msgid "Search Limit Settings"
 msgstr "ການຕັ້ງຄ່າຂີດຈຳກັດການຊອກຫາ"
 
 msgid "Limit:"
 msgstr "ຂີດຈຳກັດ:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "ໄມ້ທ່ອນ (%s)"
+
+msgid "Model:"
+msgstr "ແບບ:"
+
+msgid "ID:"
+msgstr "ເລກລໍາດັບ:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "ວັນທີສ້າງ"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "ວັນທີສ້າງ"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "ປັບປ່ຽນລ້າສຸດ ໂດຍ:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "ວັນທີປັບປ່ຽນລ້າສຸດ:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "ບັນທຶກ (%s)"
 
 msgid "Edit User Preferences"
 msgstr "ແກ້ໄຂການຕັ້ງຄ່າຜູ້ໃຊ້ງານ"
 
 msgid "Preference"
@@ -901,14 +905,17 @@
 
 msgid "Name"
 msgstr "ຊື່"
 
 msgid "Open"
 msgstr "ໄຂ"
 
+msgid "Save"
+msgstr "ບັນທຶກ"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "ແກ້ໄຂ ແຖວຂໍ້ມູນ ທີ່ເລືອກ <F2>"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "ແກ້ໄຂ ແຖວຂໍ້ມູນ ທີ່ເລືອກ <F2>"
@@ -1129,26 +1136,24 @@
 
 msgid "previous year"
 msgstr "ປີກ່ອນ"
 
 msgid "next year"
 msgstr "ປີຕໍ່ໄປ"
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "ເບິ່ງເປັນລາຍອາທິດ"
-
-msgid "Month View"
-msgstr "ເບິ່ງເປັນເດືອນ"
-
 msgid "Week"
 msgstr "ອາທິດ"
 
+#, fuzzy
+msgid "Month"
+msgstr "ເບິ່ງເປັນເດືອນ"
+
 msgid "Select..."
 msgstr "ເລືອກ..."
 
 msgid "Clear"
 msgstr "ໃຫ້ເປົ່າ"
 
 msgid "All files"
@@ -1209,9 +1214,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "ທ່ານຕ້ອງບັນທຶກຂໍ້ມູນໄວ້ກ່ອນຈຶ່ງເພີ່ມການແປເຂົ້າໄປໄດ້."
 
 msgid "No other language available."
 msgstr "ບໍ່ມີພາສາອື່ນໃຫ້ໃຊ້."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "ມູມມອງການແປ"
```

### Comparing `tryton-6.6.7/tryton/data/locale/lt/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lt\n"
 "Language-Team: lt <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -232,17 +232,14 @@
 
 msgid "Database:"
 msgstr "Duomenų bazė:"
 
 msgid "Date Format"
 msgstr "Datos formatas"
 
-msgid "Day View"
-msgstr "Dienos rodinys"
-
 msgid "Default"
 msgstr "Numatytasis"
 
 msgid "Delete"
 msgstr "Naikinti"
 
 msgid "Delete selected record <Del>"
@@ -280,23 +277,17 @@
 
 msgid "Edit..."
 msgstr "Keisti..."
 
 msgid "Edited at"
 msgstr "Taisymo data"
 
-msgid "Edited at:"
-msgstr "Keitimo data:"
-
 msgid "Edited by"
 msgstr "Taisęs naudotojas"
 
-msgid "Edited by:"
-msgstr "Pakeitęs naudotojas:"
-
 msgid "Encoding:"
 msgstr "Koduotė:"
 
 msgid "Error"
 msgstr "Klaida"
 
 msgid "Error processing the file at field %s."
@@ -403,14 +394,17 @@
 
 msgid "Listed Records"
 msgstr "Rodomi įrašai"
 
 msgid "Login"
 msgstr "Prisijungti"
 
+msgid "Logs (%s)"
+msgstr "Rąstai (%s)"
+
 msgid "M"
 msgstr "mėn."
 
 msgid "Manage..."
 msgstr "Valdyti..."
 
 msgid "Mark line for deletion/removal"
@@ -418,17 +412,14 @@
 
 msgid "Mark line for removal"
 msgstr "Pažymėti eilutę pašalinimui"
 
 msgid "Model:"
 msgstr "Modelis:"
 
-msgid "Month View"
-msgstr "Mėnesio rodinys"
-
 msgid "Move Cursor"
 msgstr "Paslinkti žymeklį"
 
 msgid "Move down"
 msgstr "Paslinkti į apačią"
 
 msgid "Move down of one page"
@@ -783,17 +774,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Nepavyko nustatyti lokalės %s"
 
 msgid "Unable to set view tree state"
 msgstr "Nepavyko nustatyti hierarchinio sąrašo rodinio"
 
-msgid "Unable to write config file %s."
-msgstr "Negalima įrašyti konfigūracinį failą %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Atkurti pasirinktą įrašą <Ins>"
 
 msgid "Underline"
 msgstr "Pabrauktas"
 
 msgid "Unknown"
@@ -819,17 +807,14 @@
 
 msgid "View _Logs..."
 msgstr "Žiūrėti _žurnalus..."
 
 msgid "Week"
 msgstr "Savaitė"
 
-msgid "Week View"
-msgstr "Savaitės rodinys"
-
 msgid "What is the name of this export?"
 msgstr "Kokiu pavadinimu išsaugoti šį eksportavimo šabloną?"
 
 msgid "Width:"
 msgstr "Plotis:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/lt/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "nurodyti naudotoją"
 
 msgid "specify the server hostname:port"
 msgstr "nurodyti tarnybinę stotį pavadinimas:prievadas"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Negalima įrašyti konfigūracinį failą %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Nepavyko nustatyti lokalės %s"
 
 msgid ", "
 msgstr ", "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr "Gerai"
 
 msgid "Your selection:"
 msgstr "Jūsų pasirinkimas:"
 
-msgid "Select"
-msgstr "Pasirinkti"
-
-msgid "Save"
-msgstr "Išsaugoti"
-
 msgid "Save As..."
 msgstr "Įrašyti kaip..."
 
 msgid "Do you want to proceed?"
 msgstr "Ar tikrai norite vykdyti?"
 
 msgid "Always ignore this warning."
@@ -200,14 +193,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "Susijęs"
 
 msgid "Edit..."
 msgstr "Keisti..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Žiūrėti _žurnalus..."
+
 msgid "Attachments..."
 msgstr "Priedai..."
 
 msgid "Notes..."
 msgstr "Pastabos..."
 
 msgid "Actions..."
@@ -605,14 +602,17 @@
 msgid "Select File"
 msgstr "Pasirinkti viską"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Šalinti <Del>"
 
+msgid "Select"
+msgstr "Pasirinkti"
+
 msgid "Add..."
 msgstr "Sukurti naują..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "Buvęs"
 
@@ -629,34 +629,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Pastaba (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Pasirinkite bent vieną įrašą."
 
-msgid "ID:"
-msgstr "ID:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Sukūręs naudotojas"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Sukūrimo data"
-
-msgid "Edited by:"
-msgstr "Pakeitęs naudotojas:"
-
-msgid "Edited at:"
-msgstr "Keitimo data:"
-
-msgid "Model:"
-msgstr "Modelis:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Ar tikrai norite ištrinti šį įrašą?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Ar tikrai norite ištrinti šiuos įrašus?"
 
 msgid "Records not removed."
@@ -714,14 +694,40 @@
 msgid "Search Limit Settings"
 msgstr "Paieškos ribojimo nustatymai"
 
 msgid "Limit:"
 msgstr "Riba:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Rąstai (%s)"
+
+msgid "Model:"
+msgstr "Modelis:"
+
+msgid "ID:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Sukūręs naudotojas"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Sukūrimo data"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Paskutinį kartą redagavo:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Paskutinio redagavimo data:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Pastabos (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Keisti naudotojo nustatymus"
 
 msgid "Preference"
@@ -882,14 +888,17 @@
 
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgid "Open"
 msgstr "Atvėrimas"
 
+msgid "Save"
+msgstr "Išsaugoti"
+
 msgid "Listed Records"
 msgstr "Rodomi įrašai"
 
 msgid "Selected Records"
 msgstr "Pasirinkti įrašai"
 
 msgid "Ignore search limit"
@@ -1105,26 +1114,24 @@
 
 msgid "previous year"
 msgstr "praeiti metai"
 
 msgid "next year"
 msgstr "kiti metai"
 
-msgid "Day View"
-msgstr "Dienos rodinys"
-
-msgid "Week View"
-msgstr "Savaitės rodinys"
-
-msgid "Month View"
-msgstr "Mėnesio rodinys"
+msgid "Day"
+msgstr ""
 
 msgid "Week"
 msgstr "Savaitė"
 
+#, fuzzy
+msgid "Month"
+msgstr "Mėnesio rodinys"
+
 msgid "Select..."
 msgstr "Pasirinkti..."
 
 msgid "Clear"
 msgstr "Valyti"
 
 msgid "All files"
@@ -1184,9 +1191,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Išsaugokite įrašą prieš pridedant vertimą."
 
 msgid "No other language available."
 msgstr "Nėra kitų kalbų."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Išversti rodinį"
```

### Comparing `tryton-6.6.7/tryton/data/locale/nl/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -15,14 +15,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" is niet geldig volgens zijn domein."
 
 msgid "\"%s\" is required."
 msgstr "\"%s\" is vereist."
 
+msgid "#ERROR"
+msgstr "#FOUT"
+
 msgid "%d record imported."
 msgstr "%d record geïmporteerd."
 
 msgid "%d record saved."
 msgstr "%d record opgeslagen."
 
 msgid "%d records imported."
@@ -282,16 +285,16 @@
 
 msgid "Database:"
 msgstr "Database:"
 
 msgid "Date Format"
 msgstr "Datum formaat"
 
-msgid "Day View"
-msgstr "Dagweergave"
+msgid "Day"
+msgstr "Dag"
 
 msgid "Default"
 msgstr "Standaard"
 
 msgid "Delete"
 msgstr "Verwijderen"
 
@@ -345,23 +348,17 @@
 
 msgid "Edit..."
 msgstr "Bewerken..."
 
 msgid "Edited at"
 msgstr "Bewerkt op"
 
-msgid "Edited at:"
-msgstr "Bewerkt op:"
-
 msgid "Edited by"
 msgstr "Bewerkt door"
 
-msgid "Edited by:"
-msgstr "Bewerkt door:"
-
 msgid "Edition Shortcuts"
 msgstr "Bewerk snelkoppelingen"
 
 msgid "Encoding:"
 msgstr "Codering:"
 
 msgid "Error"
@@ -462,14 +459,20 @@
 
 msgid "Justify"
 msgstr "Uitvullen"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Sneltoetsen..."
 
+msgid "Last Modified at:"
+msgstr "Laatst gewijzigd om:"
+
+msgid "Last Modified by:"
+msgstr "Laatst aangepast door:"
+
 msgid "Launch action"
 msgstr "Actie uitvoeren"
 
 msgid "Limit"
 msgstr "Limiet"
 
 msgid "Limit:"
@@ -489,14 +492,17 @@
 
 msgid "Listed Records"
 msgstr "Weergegeven records"
 
 msgid "Login"
 msgstr "Inlognaam"
 
+msgid "Logs (%s)"
+msgstr "Logboeken (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Beheren..."
 
 msgid "Mark line for deletion/removal"
@@ -504,16 +510,16 @@
 
 msgid "Mark line for removal"
 msgstr "Markeer regel voor verwijderen"
 
 msgid "Model:"
 msgstr "Model:"
 
-msgid "Month View"
-msgstr "Maandweergave"
+msgid "Month"
+msgstr "Maand"
 
 msgid "Move Cursor"
 msgstr "Beweeg cursor"
 
 msgid "Move down"
 msgstr "Naar beneden"
 
@@ -929,17 +935,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Kan omgeving %s niet instellen"
 
 msgid "Unable to set view tree state"
 msgstr "Kan weergave boomstructuur niet instellen"
 
-msgid "Unable to write config file %s."
-msgstr "Kan configuratiebestand %s niet opslaan."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Verwijderen van geselecteerde record <Ins> ongedaan maken"
 
 msgid "Underline"
 msgstr "Onderstrepen"
 
 msgid "Unknown"
@@ -959,23 +962,23 @@
 
 msgid "Username:"
 msgstr "Gebruikersnaam:"
 
 msgid "Value"
 msgstr "Waarde"
 
+msgid "View Logs..."
+msgstr "Bekijk Logboek..."
+
 msgid "View _Logs..."
 msgstr "Bekijk _logboek..."
 
 msgid "Week"
 msgstr "Week"
 
-msgid "Week View"
-msgstr "Weekoverzicht"
-
 msgid "What is the name of this export?"
 msgstr "Wat is de naam voor deze export?"
 
 msgid "Width:"
 msgstr "Breedte:"
 
 msgid "Wizard"
@@ -1088,14 +1091,17 @@
 
 msgid "d"
 msgstr "d"
 
 msgid "development mode"
 msgstr "Ontwikkelingsmodus"
 
+msgid "disable thread usage"
+msgstr "schakel gebruik van threads uit"
+
 msgid "go back"
 msgstr "ga terug"
 
 msgid "go forward"
 msgstr "ga vooruit"
 
 msgid "h"
```

### Comparing `tryton-6.6.7/tryton/data/locale/nl/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 msgid "specify the login user"
 msgstr "specificeer de inlog gebruiker"
 
 msgid "specify the server hostname:port"
 msgstr "specificeer de hostnaam:poort"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Kan configuratiebestand %s niet opslaan."
+msgid "disable thread usage"
+msgstr "schakel gebruik van threads uit"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Kan omgeving %s niet instellen"
 
 msgid ", "
 msgstr ", "
@@ -62,20 +61,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Uw selectie:"
 
-msgid "Select"
-msgstr "Selecteer"
-
-msgid "Save"
-msgstr "Opslaan"
-
 msgid "Save As..."
 msgstr "Opslaan als..."
 
 msgid "Do you want to proceed?"
 msgstr "Doorgaan?"
 
 msgid "Always ignore this warning."
@@ -196,14 +189,17 @@
 
 msgid "Template"
 msgstr "Sjabloon"
 
 msgid "Edit..."
 msgstr "Bewerken..."
 
+msgid "View Logs..."
+msgstr "Bekijk Logboek..."
+
 msgid "Attachments..."
 msgstr "Bijlagen..."
 
 msgid "Notes..."
 msgstr "Notities..."
 
 msgid "Actions..."
@@ -589,14 +585,17 @@
 
 msgid "Select File"
 msgstr "Selecteer bestand"
 
 msgid "Remove File"
 msgstr "Bestand verwijderen"
 
+msgid "Select"
+msgstr "Selecteer"
+
 msgid "Add..."
 msgstr "Toevoegen..."
 
 msgid "Preview"
 msgstr "Voorbeeld"
 
 msgid "Previous"
@@ -612,32 +611,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Notitie (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "U moet één record selecteren."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Aangemaakt door:"
-
-msgid "Created at:"
-msgstr "Aanmaakdatum:"
-
-msgid "Edited by:"
-msgstr "Bewerkt door:"
-
-msgid "Edited at:"
-msgstr "Bewerkt op:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Weet u zeker dat u dit record wilt verwijderen?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Weet u zeker dat u deze records wilt verwijderen?"
 
 msgid "Records not removed."
@@ -695,14 +676,36 @@
 msgid "Search Limit Settings"
 msgstr "Zoek limiet instellen"
 
 msgid "Limit:"
 msgstr "Limiet:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Logboeken (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Aangemaakt door:"
+
+msgid "Created at:"
+msgstr "Aanmaakdatum:"
+
+msgid "Last Modified by:"
+msgstr "Laatst aangepast door:"
+
+msgid "Last Modified at:"
+msgstr "Laatst gewijzigd om:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notities (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Voorkeuren gebruiker aanpassen"
 
 msgid "Preference"
@@ -861,14 +864,17 @@
 
 msgid "Name"
 msgstr "Naam"
 
 msgid "Open"
 msgstr "Openen"
 
+msgid "Save"
+msgstr "Opslaan"
+
 msgid "Listed Records"
 msgstr "Weergegeven records"
 
 msgid "Selected Records"
 msgstr "Geselecteerde records"
 
 msgid "Ignore search limit"
@@ -1082,26 +1088,23 @@
 
 msgid "previous year"
 msgstr "vorig jaar"
 
 msgid "next year"
 msgstr "volgend jaar"
 
-msgid "Day View"
-msgstr "Dagweergave"
-
-msgid "Week View"
-msgstr "Weekoverzicht"
-
-msgid "Month View"
-msgstr "Maandweergave"
+msgid "Day"
+msgstr "Dag"
 
 msgid "Week"
 msgstr "Week"
 
+msgid "Month"
+msgstr "Maand"
+
 msgid "Select..."
 msgstr "Selecteer ..."
 
 msgid "Clear"
 msgstr "Wissen"
 
 msgid "All files"
@@ -1159,9 +1162,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "U moet de record opslaan voordat u vertalingen kunt toevoegen."
 
 msgid "No other language available."
 msgstr "Geen andere taal beschikbaar."
 
+msgid "#ERROR"
+msgstr "#FOUT"
+
 msgid "Translate view"
 msgstr "Vertaal weergave"
```

### Comparing `tryton-6.6.7/tryton/data/locale/pl/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -274,17 +274,14 @@
 
 msgid "Database:"
 msgstr "Baza danych:"
 
 msgid "Date Format"
 msgstr "Format daty"
 
-msgid "Day View"
-msgstr "Widok dnia"
-
 msgid "Default"
 msgstr "Domyślnie"
 
 msgid "Delete"
 msgstr "Usuń"
 
 msgid "Delete selected record"
@@ -331,23 +328,17 @@
 
 msgid "Edit..."
 msgstr "Edycja..."
 
 msgid "Edited at"
 msgstr "Data modyfikacji"
 
-msgid "Edited at:"
-msgstr "Data modyfikacji:"
-
 msgid "Edited by"
 msgstr "Zmodyfikował"
 
-msgid "Edited by:"
-msgstr "Zmodyfikował:"
-
 msgid "Edition Shortcuts"
 msgstr "Skróty edycji"
 
 msgid "Encoding:"
 msgstr "Kodowanie:"
 
 msgid "Error"
@@ -466,14 +457,17 @@
 
 msgid "Listed Records"
 msgstr "Wymienione rekordy"
 
 msgid "Login"
 msgstr "Login"
 
+msgid "Logs (%s)"
+msgstr "Logi (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Zarządzaj..."
 
 msgid "Mark line for deletion/removal"
@@ -481,17 +475,14 @@
 
 msgid "Mark line for removal"
 msgstr "Zaznacz wiersz do usunięcia"
 
 msgid "Model:"
 msgstr "Model:"
 
-msgid "Month View"
-msgstr "Widok miesiąca"
-
 msgid "Move Cursor"
 msgstr "Przesuń kursor"
 
 msgid "Move down"
 msgstr "Przesuń w dół"
 
 msgid "Move down of one page"
@@ -891,17 +882,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Nie można ustawić lokalizacji %s"
 
 msgid "Unable to set view tree state"
 msgstr "Brak możliwości ustawienia stanu widoku drzewa"
 
-msgid "Unable to write config file %s."
-msgstr "Nie można zapisać pliku konfiguracyjnego %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Przywróć zaznaczony rekord <Ins>"
 
 msgid "Underline"
 msgstr "Podkreślenie"
 
 msgid "Unknown"
@@ -927,17 +915,14 @@
 
 msgid "View _Logs..."
 msgstr "Przeglądaj dziennik..."
 
 msgid "Week"
 msgstr "Tydzień"
 
-msgid "Week View"
-msgstr "Widok tygodnia"
-
 msgid "What is the name of this export?"
 msgstr "Jaka jest nazwa tego eksportu?"
 
 msgid "Width:"
 msgstr "Szerokość:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/pl/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "podaj login użytkownika"
 
 msgid "specify the server hostname:port"
 msgstr "podaj nazwę:port serwera"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Nie można zapisać pliku konfiguracyjnego %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Nie można ustawić lokalizacji %s"
 
 msgid ", "
 msgstr ", "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Twoje zaznaczenie:"
 
-msgid "Select"
-msgstr "Wybierz"
-
-msgid "Save"
-msgstr "Zapisz"
-
 msgid "Save As..."
 msgstr "Zapisz jako..."
 
 msgid "Do you want to proceed?"
 msgstr "Czy chcesz kontynuować?"
 
 msgid "Always ignore this warning."
@@ -198,14 +191,18 @@
 
 msgid "Template"
 msgstr "Szablon"
 
 msgid "Edit..."
 msgstr "Edycja..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Przeglądaj dziennik..."
+
 msgid "Attachments..."
 msgstr "Załączniki..."
 
 msgid "Notes..."
 msgstr "Notatki..."
 
 msgid "Actions..."
@@ -594,14 +591,17 @@
 msgid "Select File"
 msgstr "Zaznacz wszystko"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Usuń <Del>"
 
+msgid "Select"
+msgstr "Wybierz"
+
 msgid "Add..."
 msgstr "Dodaj..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "Poprzedni"
 
@@ -618,32 +618,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Notatka (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Musisz wybrać jeden rekord."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Utworzył:"
-
-msgid "Created at:"
-msgstr "Data utworzenia:"
-
-msgid "Edited by:"
-msgstr "Zmodyfikował:"
-
-msgid "Edited at:"
-msgstr "Data modyfikacji:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Czy na pewno usunąć wybrany rekord?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Czy na pewno usunąć wybrane rekordy?"
 
 msgid "Records not removed."
@@ -701,14 +683,38 @@
 msgid "Search Limit Settings"
 msgstr "Ustawienia limitu wyszukiwania"
 
 msgid "Limit:"
 msgstr "Limit:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Logi (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Utworzył:"
+
+msgid "Created at:"
+msgstr "Data utworzenia:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Autor ostatniej modyfikacji:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Data ostatniej modyfikacji:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notatki (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Edytuj preferencje użytkownika"
 
 msgid "Preference"
@@ -867,14 +873,17 @@
 
 msgid "Name"
 msgstr "Nazwa"
 
 msgid "Open"
 msgstr "Otwórz"
 
+msgid "Save"
+msgstr "Zapisz"
+
 msgid "Listed Records"
 msgstr "Wymienione rekordy"
 
 msgid "Selected Records"
 msgstr "Wybrane rekordy"
 
 msgid "Ignore search limit"
@@ -1089,26 +1098,24 @@
 
 msgid "previous year"
 msgstr "poprzedni rok"
 
 msgid "next year"
 msgstr "następny rok"
 
-msgid "Day View"
-msgstr "Widok dnia"
-
-msgid "Week View"
-msgstr "Widok tygodnia"
-
-msgid "Month View"
-msgstr "Widok miesiąca"
+msgid "Day"
+msgstr ""
 
 msgid "Week"
 msgstr "Tydzień"
 
+#, fuzzy
+msgid "Month"
+msgstr "Widok miesiąca"
+
 msgid "Select..."
 msgstr "Wybierz..."
 
 msgid "Clear"
 msgstr "Wyczyść"
 
 msgid "All files"
@@ -1166,9 +1173,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Musisz zapisać rekord przed dodaniem tłumaczeń."
 
 msgid "No other language available."
 msgstr "Brak innych języków."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Widok tłumaczenia"
```

### Comparing `tryton-6.6.7/tryton/data/locale/pt/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pt\n"
 "Language-Team: pt <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -357,26 +357,26 @@
 
 msgid "List/Tree Shortcuts"
 msgstr "Atalhos da tela de Lista/Árvore"
 
 msgid "Login"
 msgstr "Entrar"
 
+msgid "Logs (%s)"
+msgstr "Histórico (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gerenciar..."
 
 msgid "Model:"
 msgstr "Modelo:"
 
-msgid "Month View"
-msgstr "Visão Mensal"
-
 msgid "Move Cursor"
 msgstr "Mover cursor"
 
 msgid "Move down"
 msgstr "Mover para baixo"
 
 msgid "Move down of one page"
@@ -737,17 +737,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Não foi possível definir as configurações regionais %s"
 
 msgid "Unable to set view tree state"
 msgstr "Não foi possível definir o estado da visão em árvore"
 
-msgid "Unable to write config file %s."
-msgstr "Não foi possível gravar o arquivo de configuração %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Recuperar o registro selecionado <Ins>"
 
 msgid "Unknown"
 msgstr "Desconhecido"
 
 msgid "Unmark line for deletion"
@@ -767,17 +764,14 @@
 
 msgid "View _Logs..."
 msgstr "Ver _Logs..."
 
 msgid "Week"
 msgstr "Semana"
 
-msgid "Week View"
-msgstr "Visão Semanal"
-
 msgid "What is the name of this export?"
 msgstr "Qual é o nome dessa exportação?"
 
 msgid "Width:"
 msgstr "Largura:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/pt/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 
 msgid "specify the login user"
 msgstr "Especifique o nome do usuário"
 
 msgid "specify the server hostname:port"
 msgstr "Especifique o servidor hostname:porta"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Não foi possível gravar o arquivo de configuração %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Não foi possível definir as configurações regionais %s"
 
 msgid ", "
 msgstr ", "
@@ -63,20 +62,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Sua seleção:"
 
-msgid "Select"
-msgstr "Selecionar"
-
-msgid "Save"
-msgstr "Gravar"
-
 msgid "Save As..."
 msgstr "Salvar como..."
 
 msgid "Do you want to proceed?"
 msgstr "Você deseja prosseguir?"
 
 msgid "Always ignore this warning."
@@ -202,14 +195,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "Relacionar"
 
 msgid "Edit..."
 msgstr "Editar..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Ver _Logs..."
+
 msgid "Attachments..."
 msgstr "Anexos..."
 
 msgid "Notes..."
 msgstr "Notas..."
 
 msgid "Actions..."
@@ -607,14 +604,17 @@
 msgid "Select File"
 msgstr "Selecionar todos"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Remover <Del>"
 
+msgid "Select"
+msgstr "Selecionar"
+
 msgid "Add..."
 msgstr "Adicionar..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "Anterior"
 
@@ -631,36 +631,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr "Você precisa selecionar um registo."
 
-msgid "ID:"
-msgstr "ID:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Data de criação"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Data de criação"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Editar"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Editar"
-
-msgid "Model:"
-msgstr "Modelo:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Você tem certeza que deseja apagar este registro?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Você tem certeza que deseja apagar estes registros?"
 
 msgid "Records not removed."
@@ -718,14 +696,40 @@
 msgid "Search Limit Settings"
 msgstr "Preferências de limite de buscas"
 
 msgid "Limit:"
 msgstr "Limite:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Histórico (%s)"
+
+msgid "Model:"
+msgstr "Modelo:"
+
+msgid "ID:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Data de criação"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Data de criação"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Última Modificação por:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Data da última modificação:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Notas (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Editar preferências do usuário"
 
 msgid "Preference"
@@ -886,14 +890,17 @@
 
 msgid "Name"
 msgstr "Nome"
 
 msgid "Open"
 msgstr "Abrir"
 
+msgid "Save"
+msgstr "Gravar"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "Editar o registro selecionado <F2>"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Editar o registro selecionado <F2>"
@@ -1114,26 +1121,24 @@
 
 msgid "previous year"
 msgstr "ano anterior"
 
 msgid "next year"
 msgstr "próximo ano"
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "Visão Semanal"
-
-msgid "Month View"
-msgstr "Visão Mensal"
-
 msgid "Week"
 msgstr "Semana"
 
+#, fuzzy
+msgid "Month"
+msgstr "Visão Mensal"
+
 msgid "Select..."
 msgstr "Selecionar..."
 
 msgid "Clear"
 msgstr "Limpar"
 
 msgid "All files"
@@ -1193,9 +1198,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Você precisa salvar o registro antes de adicionar traduções."
 
 msgid "No other language available."
 msgstr "Não há outros idiomas disponíveis."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Traduzir visão"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ro/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ro\n"
 "Language-Team: ro <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -16,14 +16,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" nu este valid conform domeniului său."
 
 msgid "\"%s\" is required."
 msgstr "\"%s\" este obligatoriu."
 
+msgid "#ERROR"
+msgstr "#EROARE"
+
 msgid "%d record imported."
 msgstr "înregistrare %d importată."
 
 msgid "%d record saved."
 msgstr "inregistrare %d salvata."
 
 msgid "%d records imported."
@@ -40,14 +43,17 @@
 
 msgid "%s (string)"
 msgstr "%s (string)"
 
 msgid "%s%%"
 msgstr "%s%%"
 
+msgid "%s/Record Name"
+msgstr "%s/Denumire Înregistrare"
+
 msgid ", "
 msgstr ", "
 
 msgid ",..."
 msgstr ",..."
 
 msgid ".."
@@ -242,15 +248,18 @@
 msgid "Copy _URL..."
 msgstr "Copiază _URL ..."
 
 msgid "Copy selected text"
 msgstr "Copiere text selectat"
 
 msgid "Could not connect to the server."
-msgstr "Nu s-a putut conecta la server."
+msgstr "Nu s-a putut efectua conexiunea la server."
+
+msgid "Could not get a session."
+msgstr "Nu s-a putut găsi o sesiune."
 
 msgid "Create a new record"
 msgstr "Creați o înregistrare nouă"
 
 msgid "Create a new record <F3>"
 msgstr "Creați o nouă înregistrare <F3>"
 
@@ -277,16 +286,16 @@
 
 msgid "Database:"
 msgstr "Bază de date:"
 
 msgid "Date Format"
 msgstr "Formatul datei"
 
-msgid "Day View"
-msgstr "Visualizare zi"
+msgid "Day"
+msgstr "Zi"
 
 msgid "Default"
 msgstr "Implicit"
 
 msgid "Delete"
 msgstr "Ștergere"
 
@@ -296,15 +305,15 @@
 msgid "Delete selected record <Del>"
 msgstr "Ștergeți înregistrarea selectată <Del>"
 
 msgid "Delimiter:"
 msgstr "Delimitator:"
 
 msgid "Detection failed"
-msgstr "Detectarea a eșuat"
+msgstr "Detecție eșuată"
 
 msgid "Digits"
 msgstr "Cifre"
 
 msgid "Display format"
 msgstr "Formatul afisare"
 
@@ -313,14 +322,17 @@
 
 msgid "Displayed value"
 msgstr "Valoarea afișată"
 
 msgid "Do you want to proceed?"
 msgstr "Doriți să continuați?"
 
+msgid "Documentation..."
+msgstr "Documentație..."
+
 msgid "Download"
 msgstr "Descarca"
 
 msgid "E-Mail..."
 msgstr "E-Mail..."
 
 msgid "E-mail %s"
@@ -337,23 +349,17 @@
 
 msgid "Edit..."
 msgstr "Editare..."
 
 msgid "Edited at"
 msgstr "Editat la"
 
-msgid "Edited at:"
-msgstr "Editat la:"
-
 msgid "Edited by"
 msgstr "Editat de"
 
-msgid "Edited by:"
-msgstr "Editat de:"
-
 msgid "Edition Shortcuts"
 msgstr "Comenzi rapide de ediție"
 
 msgid "Encoding:"
 msgstr "Codifiere:"
 
 msgid "Error"
@@ -443,25 +449,31 @@
 msgid "Images"
 msgstr "Imagini"
 
 msgid "Import failed"
 msgstr "Import eşuat"
 
 msgid "Incompatible version of the server."
-msgstr "Versiunea incompatibilă a serverului."
+msgstr "Versiune incompatibila a serverului."
 
 msgid "Italic"
 msgstr "Cursiv"
 
 msgid "Justify"
 msgstr "Margini"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Comenzi rapide..."
 
+msgid "Last Modified at:"
+msgstr "Ultima Modificare la:"
+
+msgid "Last Modified by:"
+msgstr "Modificat de:"
+
 msgid "Launch action"
 msgstr "Lansare acțiune"
 
 msgid "Limit"
 msgstr "Limită"
 
 msgid "Limit:"
@@ -481,14 +493,17 @@
 
 msgid "Listed Records"
 msgstr "Înregistrări enumerate"
 
 msgid "Login"
 msgstr "Autentificare"
 
+msgid "Logs (%s)"
+msgstr "Jurnale (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Manage..."
 msgstr "Gestionare..."
 
 msgid "Mark line for deletion/removal"
@@ -496,16 +511,16 @@
 
 msgid "Mark line for removal"
 msgstr "Selectare linia pentru eliminare"
 
 msgid "Model:"
 msgstr "Model:"
 
-msgid "Month View"
-msgstr "Vizualizare lunară"
+msgid "Month"
+msgstr "Lună"
 
 msgid "Move Cursor"
 msgstr "Mutare cursor"
 
 msgid "Move down"
 msgstr "Mutre în jos"
 
@@ -559,14 +574,20 @@
 
 msgid "No other language available."
 msgstr "Nu există altă limbă disponibilă."
 
 msgid "No result found."
 msgstr "Niciun rezultat găsit."
 
+msgid "Not Found."
+msgstr "Niciun rezultat găsit."
+
+msgid "Not found."
+msgstr "Nimic găsit."
+
 msgid "Note (%d/%d)"
 msgstr "Notă (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Note (%s)"
 
 msgid "Notes..."
@@ -915,17 +936,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Imposibil de setat regiunea locală %s"
 
 msgid "Unable to set view tree state"
 msgstr "Imposibil de setat starea arborelui de vizualizare"
 
-msgid "Unable to write config file %s."
-msgstr "Imposibil de scris fișierul de configurare %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Anulare stergere pentru înregistrarea selectată <Ins>"
 
 msgid "Underline"
 msgstr "Subliniere"
 
 msgid "Unknown"
@@ -945,23 +963,23 @@
 
 msgid "Username:"
 msgstr "Utilizator:"
 
 msgid "Value"
 msgstr "Valoare"
 
+msgid "View Logs..."
+msgstr "Vizualizare Jurnale..."
+
 msgid "View _Logs..."
 msgstr "Vizualizare_jurnalele ..."
 
 msgid "Week"
 msgstr "Săptămână"
 
-msgid "Week View"
-msgstr "Visualizare saptamana"
-
 msgid "What is the name of this export?"
 msgstr "Care este numele acestui export?"
 
 msgid "Width:"
 msgstr "Lăţime:"
 
 msgid "Wizard"
@@ -1074,14 +1092,17 @@
 
 msgid "d"
 msgstr "d"
 
 msgid "development mode"
 msgstr "mod de dezvoltare"
 
+msgid "disable thread usage"
+msgstr "dezactivare utilizarea thread-urilor"
+
 msgid "go back"
 msgstr "întoarcre"
 
 msgid "go forward"
 msgstr "mergi inainte"
 
 msgid "h"
@@ -1104,14 +1125,17 @@
 
 msgid "s"
 msgstr "s"
 
 msgid "specify alternate config file"
 msgstr "specificare alt fisier de configurare"
 
+msgid "specify the file used to output logging information"
+msgstr "specificare fișier pentru scriere informaţii în jurnal"
+
 msgid "specify the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 msgstr "specificați nivelul jurnalului: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 
 msgid "specify the login user"
 msgstr "specificati utilizatorul"
 
 msgid "specify the server hostname:port"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ro/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 msgid "logging everything at INFO level"
 msgstr "logare totul la nivel INFO"
 
 msgid "specify the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 msgstr "specificați nivelul jurnalului: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 
 msgid "specify the file used to output logging information"
-msgstr ""
+msgstr "specificare fișier pentru scriere informaţii în jurnal"
 
 msgid "specify the login user"
 msgstr "specificati utilizatorul"
 
 msgid "specify the server hostname:port"
 msgstr "specificați numele gazdă server: port"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Imposibil de scris fișierul de configurare %s."
+msgid "disable thread usage"
+msgstr "dezactivare utilizarea thread-urilor"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Imposibil de setat regiunea locală %s"
 
 msgid ", "
 msgstr ", "
@@ -58,20 +57,14 @@
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
 msgstr "Selecția dvs.:"
 
-msgid "Select"
-msgstr "Selectați"
-
-msgid "Save"
-msgstr "Salvare"
-
 msgid "Save As..."
 msgstr "Salvare că..."
 
 msgid "Do you want to proceed?"
 msgstr "Doriți să continuați?"
 
 msgid "Always ignore this warning."
@@ -126,26 +119,23 @@
 
 msgid "A new version is available!"
 msgstr "O nouă versiune este disponibilă!"
 
 msgid "Download"
 msgstr "Descarca"
 
-#, fuzzy
 msgid "Could not get a session."
-msgstr "Nu s-a putut conecta la server."
+msgstr "Nu s-a putut găsi o sesiune."
 
 msgid "Too many requests. Try again later."
 msgstr "Prea multe cereri. Încercați mai târziu."
 
-#, fuzzy
 msgid "Not found."
-msgstr "Niciun rezultat găsit."
+msgstr "Nimic găsit."
 
-#, fuzzy
 msgid "Not Found."
 msgstr "Niciun rezultat găsit."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
@@ -195,14 +185,17 @@
 
 msgid "Template"
 msgstr "Șablon"
 
 msgid "Edit..."
 msgstr "Editare..."
 
+msgid "View Logs..."
+msgstr "Vizualizare Jurnale..."
+
 msgid "Attachments..."
 msgstr "Atașamente..."
 
 msgid "Notes..."
 msgstr "Note..."
 
 msgid "Actions..."
@@ -306,17 +299,16 @@
 
 msgid "Check Version"
 msgstr "Verificare versiune"
 
 msgid "Options"
 msgstr "Opțiuni"
 
-#, fuzzy
 msgid "Documentation..."
-msgstr "Acțiuni..."
+msgstr "Documentație..."
 
 msgid "Keyboard Shortcuts..."
 msgstr "Comenzi rapide..."
 
 msgid "About..."
 msgstr "Despre..."
 
@@ -520,18 +512,18 @@
 msgid "Fetching databases list"
 msgstr "Obținerea listei de baze de date"
 
 msgid "Username:"
 msgstr "Utilizator:"
 
 msgid "Incompatible version of the server."
-msgstr "Versiunea incompatibilă a serverului."
+msgstr "Versiune incompatibila a serverului."
 
 msgid "Could not connect to the server."
-msgstr "Nu s-a putut conecta la server."
+msgstr "Nu s-a putut efectua conexiunea la server."
 
 msgid "Login"
 msgstr "Autentificare"
 
 msgid "_Cancel"
 msgstr "_Anulare"
 
@@ -589,14 +581,17 @@
 
 msgid "Select File"
 msgstr "Selectare Fişier"
 
 msgid "Remove File"
 msgstr "Eliminare Fişier"
 
+msgid "Select"
+msgstr "Selectați"
+
 msgid "Add..."
 msgstr "Adăuga..."
 
 msgid "Preview"
 msgstr "Previzualizare"
 
 msgid "Previous"
@@ -612,32 +607,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Notă (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Trebuie selectaa o singura înregistrare."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Creat de:"
-
-msgid "Created at:"
-msgstr "Creat la:"
-
-msgid "Edited by:"
-msgstr "Editat de:"
-
-msgid "Edited at:"
-msgstr "Editat la:"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Sigur eliminați această înregistrare?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Sigur eliminați această înregistrare?"
 
 msgid "Records not removed."
@@ -695,14 +672,36 @@
 msgid "Search Limit Settings"
 msgstr "Setări limită de căutare"
 
 msgid "Limit:"
 msgstr "Limită:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Jurnale (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Creat de:"
+
+msgid "Created at:"
+msgstr "Creat la:"
+
+msgid "Last Modified by:"
+msgstr "Modificat de:"
+
+msgid "Last Modified at:"
+msgstr "Ultima Modificare la:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Note (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Editare Preferințe utilizator"
 
 msgid "Preference"
@@ -861,14 +860,17 @@
 
 msgid "Name"
 msgstr "Denumire"
 
 msgid "Open"
 msgstr "Deschidere"
 
+msgid "Save"
+msgstr "Salvare"
+
 msgid "Listed Records"
 msgstr "Înregistrări enumerate"
 
 msgid "Selected Records"
 msgstr "Înregistrări selectate"
 
 msgid "Ignore search limit"
@@ -881,17 +883,17 @@
 msgid "%s (string)"
 msgstr "%s (string)"
 
 #, python-format
 msgid "%s (model name)"
 msgstr "%s (model name)"
 
-#, fuzzy, python-format
+#, python-format
 msgid "%s/Record Name"
-msgstr "%s (denmire inregistrare)"
+msgstr "%s/Denumire Înregistrare"
 
 msgid "What is the name of this export?"
 msgstr "Care este numele acestui export?"
 
 #, python-format
 msgid "Override '%s' definition?"
 msgstr "Trecere peste definiția '%s'?"
@@ -950,15 +952,15 @@
 msgid "Lines to Skip:"
 msgstr "Rânduri de sarit:"
 
 msgid "You must select an import file first."
 msgstr "Mai întâi trebuie să selectați un fișier de import."
 
 msgid "Detection failed"
-msgstr "Detectarea a eșuat"
+msgstr "Detecție eșuată"
 
 #, python-format
 msgid "Error processing the file at field %s."
 msgstr "Eroare la procesarea fișierului în câmpul %s."
 
 msgid "Error"
 msgstr "Eroare"
@@ -1082,26 +1084,23 @@
 
 msgid "previous year"
 msgstr "anul precedent"
 
 msgid "next year"
 msgstr "anul urmator"
 
-msgid "Day View"
-msgstr "Visualizare zi"
-
-msgid "Week View"
-msgstr "Visualizare saptamana"
-
-msgid "Month View"
-msgstr "Vizualizare lunară"
+msgid "Day"
+msgstr "Zi"
 
 msgid "Week"
 msgstr "Săptămână"
 
+msgid "Month"
+msgstr "Lună"
+
 msgid "Select..."
 msgstr "Selectare..."
 
 msgid "Clear"
 msgstr "Golire"
 
 msgid "All files"
@@ -1159,9 +1158,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Trebuie să salvați înregistrarea înainte de a adăuga traduceri."
 
 msgid "No other language available."
 msgstr "Nu există altă limbă disponibilă."
 
+msgid "#ERROR"
+msgstr "#EROARE"
+
 msgid "Translate view"
 msgstr "Traducere vedere"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ru/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.6.7/tryton/data/locale/ru/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 msgid "specify the login user"
 msgstr "указать имя пользователя"
 
 #, fuzzy
 msgid "specify the server hostname:port"
 msgstr "укажите имя сервера"
 
-#, fuzzy, python-format
-msgid "Unable to write config file %s."
-msgstr "Невозможно записать файл конфигурации %s!"
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Не удается установить локализацию %s"
 
 #, fuzzy
 msgid ", "
@@ -66,20 +65,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "Ваш выбор:"
 
-msgid "Select"
-msgstr ""
-
-msgid "Save"
-msgstr "Сохранить"
-
 msgid "Save As..."
 msgstr "Сохранить как..."
 
 msgid "Do you want to proceed?"
 msgstr "Вы хотите продолжить?"
 
 msgid "Always ignore this warning."
@@ -211,14 +204,18 @@
 msgid "Template"
 msgstr "Связанные"
 
 #, fuzzy
 msgid "Edit..."
 msgstr "_Выход..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Просмотр изменений"
+
 msgid "Attachments..."
 msgstr "Вложения..."
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -629,14 +626,17 @@
 msgid "Select File"
 msgstr "Выбор"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Удалить <Del>"
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 #, fuzzy
 msgid "Preview"
 msgstr "Предыдущий"
 
@@ -654,36 +654,14 @@
 msgid "Note (%d/%d)"
 msgstr ""
 
 #, fuzzy
 msgid "You have to select one record."
 msgstr "Вы должны выбрать одну запись!"
 
-msgid "ID:"
-msgstr "Номер строки"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Дата создания"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Дата создания"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Редактировать"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Редактировать"
-
-msgid "Model:"
-msgstr "Модель:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Вы уверены что хотите удалить эту запись?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Вы уверены что хотите удалить эти записи?"
 
 #, fuzzy
@@ -746,14 +724,40 @@
 msgid "Search Limit Settings"
 msgstr "Настройки ограничения поиска"
 
 msgid "Limit:"
 msgstr "Кол-во записей"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr ""
+
+msgid "Model:"
+msgstr "Модель:"
+
+msgid "ID:"
+msgstr "Номер строки"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Дата создания"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Дата создания"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Изменена пользователем:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Дата изменения:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr "Изменить настройки пользователя"
 
 msgid "Preference"
@@ -922,14 +926,17 @@
 
 msgid "Name"
 msgstr "Имя"
 
 msgid "Open"
 msgstr "Открыть"
 
+msgid "Save"
+msgstr "Сохранить"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "Изменить выбранную запись <F2>"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Изменить выбранную запись <F2>"
@@ -1155,28 +1162,24 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-#, fuzzy
-msgid "Week View"
-msgstr "Переключить вид"
+msgid "Week"
+msgstr ""
 
 #, fuzzy
-msgid "Month View"
+msgid "Month"
 msgstr "Переключить вид"
 
-msgid "Week"
-msgstr ""
-
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr "Очистить"
 
 msgid "All files"
@@ -1239,9 +1242,12 @@
 msgid "You need to save the record before adding translations."
 msgstr "Необходимо сохранить запись перед добавлением перевода!"
 
 #, fuzzy
 msgid "No other language available."
 msgstr "Отсутствуют другие доступные языки!"
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Перевод текущего окна"
```

### Comparing `tryton-6.6.7/tryton/data/locale/sl/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: sl\n"
 "Language-Team: sl <LL@li.org>\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
@@ -283,23 +283,23 @@
 
 msgid "Link"
 msgstr "Povezava"
 
 msgid "Login"
 msgstr "Prijava"
 
+msgid "Logs (%s)"
+msgstr "Dnevniki (%s)"
+
 msgid "M"
 msgstr "M"
 
 msgid "Model:"
 msgstr "Model:"
 
-msgid "Month View"
-msgstr "Mesečno"
-
 msgid "Move Cursor"
 msgstr "Premiki"
 
 msgid "Move down"
 msgstr "Premik dol"
 
 msgid "Move down of one page"
@@ -582,17 +582,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Ni možno nastaviti krajevnih nastavitev %s"
 
 msgid "Unable to set view tree state"
 msgstr "Ni možno nastaviti stanja obrazca"
 
-msgid "Unable to write config file %s."
-msgstr "Ni možno zapisati konfiguracijske datoteke %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Povrni izbran zapis <Ins>"
 
 msgid "Unknown"
 msgstr "Neznano"
 
 msgid "Unmark line for deletion"
@@ -612,17 +609,14 @@
 
 msgid "View _Logs..."
 msgstr "Poglej dnevni_k..."
 
 msgid "Week"
 msgstr "Teden"
 
-msgid "Week View"
-msgstr "Tedensko"
-
 msgid "What is the name of this export?"
 msgstr "Kako se imenuje ta izvoz?"
 
 msgid "Width:"
 msgstr "Širina:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/sl/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "določi uporabniško ime"
 
 msgid "specify the server hostname:port"
 msgstr "določi ime in vrata strežniškega gostitelja"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Ni možno zapisati konfiguracijske datoteke %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Ni možno nastaviti krajevnih nastavitev %s"
 
 msgid ", "
 msgstr ", "
@@ -63,20 +62,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "Vaša izbira:"
 
-msgid "Select"
-msgstr "Izberi"
-
-msgid "Save"
-msgstr "Shrani"
-
 msgid "Save As..."
 msgstr "Shrani kot..."
 
 msgid "Do you want to proceed?"
 msgstr "Ali želite nadaljevati?"
 
 msgid "Always ignore this warning."
@@ -202,14 +195,18 @@
 #, fuzzy
 msgid "Template"
 msgstr "Veza"
 
 msgid "Edit..."
 msgstr "Uredi ..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Poglej dnevni_k..."
+
 msgid "Attachments..."
 msgstr "Priponke..."
 
 msgid "Notes..."
 msgstr "Zabeležke ..."
 
 msgid "Actions..."
@@ -621,14 +618,17 @@
 msgid "Select File"
 msgstr "Izberi vse"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "Odstrani <Del>"
 
+msgid "Select"
+msgstr "Izberi"
+
 msgid "Add..."
 msgstr ""
 
 #, fuzzy
 msgid "Preview"
 msgstr "Prejšnji"
 
@@ -645,36 +645,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr "En zapis mora biti izbran."
 
-msgid "ID:"
-msgstr "ID:"
-
-#, fuzzy
-msgid "Created by:"
-msgstr "Ustvarjeno"
-
-#, fuzzy
-msgid "Created at:"
-msgstr "Ustvarjeno"
-
-#, fuzzy
-msgid "Edited by:"
-msgstr "Uredi"
-
-#, fuzzy
-msgid "Edited at:"
-msgstr "Uredi"
-
-msgid "Model:"
-msgstr "Model:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Ali res želiš izbrisati ta zapis?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Ali res želiš izbrisati te zapise?"
 
 msgid "Records not removed."
@@ -731,14 +709,41 @@
 
 msgid "Search Limit Settings"
 msgstr "Nastavitev omejitev iskanja"
 
 msgid "Limit:"
 msgstr "Omejitev:"
 
+# ?
+#, python-format
+msgid "Logs (%s)"
+msgstr "Dnevniki (%s)"
+
+msgid "Model:"
+msgstr "Model:"
+
+msgid "ID:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Created by:"
+msgstr "Ustvarjeno"
+
+#, fuzzy
+msgid "Created at:"
+msgstr "Ustvarjeno"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "Nazadnje popravil:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "Nazadnje popravljeno:"
+
 #, python-format
 msgid "Notes (%s)"
 msgstr "Zabeležke (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Uredi uporabniške nastavitve"
 
@@ -900,14 +905,17 @@
 
 msgid "Name"
 msgstr "Naziv"
 
 msgid "Open"
 msgstr "Odpri"
 
+msgid "Save"
+msgstr "Shrani"
+
 #, fuzzy
 msgid "Listed Records"
 msgstr "Uredi izbran zapis <F2>"
 
 #, fuzzy
 msgid "Selected Records"
 msgstr "Uredi izbran zapis <F2>"
@@ -1128,26 +1136,24 @@
 
 msgid "previous year"
 msgstr "Prejšnje leto"
 
 msgid "next year"
 msgstr "naslednje leto"
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
-msgstr "Tedensko"
-
-msgid "Month View"
-msgstr "Mesečno"
-
 msgid "Week"
 msgstr "Teden"
 
+#, fuzzy
+msgid "Month"
+msgstr "Mesečno"
+
 msgid "Select..."
 msgstr "Izberi ..."
 
 msgid "Clear"
 msgstr "Počisti"
 
 msgid "All files"
@@ -1208,9 +1214,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Pred dodajanjem prevodov morate zapis shraniti."
 
 msgid "No other language available."
 msgstr "Drugih jezikov ni na voljo."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Prevedi pogled"
```

### Comparing `tryton-6.6.7/tryton/data/locale/tr/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -39,14 +39,17 @@
 
 msgid "Do you want to proceed?"
 msgstr "İlerlemek istiyor musunuz?"
 
 msgid "Error"
 msgstr "Hata"
 
+msgid "Logs (%s)"
+msgstr "Günlükler (%s)"
+
 msgid "No action defined."
 msgstr "İşlem belirtilmedi."
 
 msgid "Report Bug"
 msgstr "Hatayı Raporla"
 
 msgid "Select your action"
@@ -54,17 +57,14 @@
 
 msgid "Selection"
 msgstr "Seçim"
 
 msgid "Unable to set locale %s"
 msgstr "Lokal %s ayarlanamadı"
 
-msgid "Unable to write config file %s."
-msgstr "Config dosyasına %s yazılamadı"
-
 msgid "Write Anyway"
 msgstr "Tüm Durumlarda Yaz"
 
 msgid "Your selection:"
 msgstr "Seçiminiz:"
 
 msgid "development mode"
```

### Comparing `tryton-6.6.7/tryton/data/locale/tr/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "Giriş kullanıcısını belirle"
 
 msgid "specify the server hostname:port"
 msgstr "Server hostname belirle: port"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Config dosyasına %s yazılamadı"
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Lokal %s ayarlanamadı"
 
 msgid ", "
 msgstr ", "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr ""
 
 msgid "Your selection:"
 msgstr "Seçiminiz:"
 
-msgid "Select"
-msgstr ""
-
-msgid "Save"
-msgstr ""
-
 #, fuzzy
 msgid "Save As..."
 msgstr "Save As..."
 
 msgid "Do you want to proceed?"
 msgstr "İlerlemek istiyor musunuz?"
 
@@ -197,14 +190,17 @@
 
 msgid "Template"
 msgstr ""
 
 msgid "Edit..."
 msgstr ""
 
+msgid "View Logs..."
+msgstr ""
+
 msgid "Attachments..."
 msgstr ""
 
 msgid "Notes..."
 msgstr ""
 
 msgid "Actions..."
@@ -591,14 +587,17 @@
 #, fuzzy
 msgid "Select File"
 msgstr "Seçim"
 
 msgid "Remove File"
 msgstr ""
 
+msgid "Select"
+msgstr ""
+
 msgid "Add..."
 msgstr ""
 
 msgid "Preview"
 msgstr ""
 
 msgid "Previous"
@@ -614,32 +613,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr ""
 
 msgid "You have to select one record."
 msgstr ""
 
-msgid "ID:"
-msgstr ""
-
-msgid "Created by:"
-msgstr ""
-
-msgid "Created at:"
-msgstr ""
-
-msgid "Edited by:"
-msgstr ""
-
-msgid "Edited at:"
-msgstr ""
-
-msgid "Model:"
-msgstr ""
-
 msgid "Are you sure to remove this record?"
 msgstr ""
 
 msgid "Are you sure to remove those records?"
 msgstr ""
 
 msgid "Records not removed."
@@ -695,14 +676,36 @@
 msgid "Search Limit Settings"
 msgstr ""
 
 msgid "Limit:"
 msgstr ""
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "Günlükler (%s)"
+
+msgid "Model:"
+msgstr ""
+
+msgid "ID:"
+msgstr ""
+
+msgid "Created by:"
+msgstr ""
+
+msgid "Created at:"
+msgstr ""
+
+msgid "Last Modified by:"
+msgstr ""
+
+msgid "Last Modified at:"
+msgstr ""
+
+#, python-format
 msgid "Notes (%s)"
 msgstr ""
 
 msgid "Edit User Preferences"
 msgstr ""
 
 msgid "Preference"
@@ -861,14 +864,17 @@
 
 msgid "Name"
 msgstr ""
 
 msgid "Open"
 msgstr ""
 
+msgid "Save"
+msgstr ""
+
 msgid "Listed Records"
 msgstr ""
 
 msgid "Selected Records"
 msgstr ""
 
 msgid "Ignore search limit"
@@ -1082,24 +1088,21 @@
 
 msgid "previous year"
 msgstr ""
 
 msgid "next year"
 msgstr ""
 
-msgid "Day View"
+msgid "Day"
 msgstr ""
 
-msgid "Week View"
+msgid "Week"
 msgstr ""
 
-msgid "Month View"
-msgstr ""
-
-msgid "Week"
+msgid "Month"
 msgstr ""
 
 msgid "Select..."
 msgstr ""
 
 msgid "Clear"
 msgstr ""
@@ -1159,9 +1162,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr ""
 
 msgid "No other language available."
 msgstr ""
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr ""
```

### Comparing `tryton-6.6.7/tryton/data/locale/uk/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -277,17 +277,14 @@
 
 msgid "Database:"
 msgstr "База даних:"
 
 msgid "Date Format"
 msgstr "Формат дати"
 
-msgid "Day View"
-msgstr "Вид дня"
-
 msgid "Default"
 msgstr "За замовчуванням"
 
 msgid "Delete"
 msgstr "Видалити"
 
 msgid "Delete selected record"
@@ -337,23 +334,17 @@
 
 msgid "Edit..."
 msgstr "Редагувати..."
 
 msgid "Edited at"
 msgstr "Коли змінено"
 
-msgid "Edited at:"
-msgstr "Коли змінено:"
-
 msgid "Edited by"
 msgstr "Ким змінено"
 
-msgid "Edited by:"
-msgstr "Ким змінено:"
-
 msgid "Edition Shortcuts"
 msgstr "Комбінації клавіш для редагування"
 
 msgid "Encoding:"
 msgstr "Кодування:"
 
 msgid "Error"
@@ -481,14 +472,17 @@
 
 msgid "Listed Records"
 msgstr "Записи списку"
 
 msgid "Login"
 msgstr "Логін"
 
+msgid "Logs (%s)"
+msgstr "колоди (%s)"
+
 msgid "M"
 msgstr "М"
 
 msgid "Manage..."
 msgstr "Керування..."
 
 msgid "Mark line for deletion/removal"
@@ -496,17 +490,14 @@
 
 msgid "Mark line for removal"
 msgstr "Позначити рядок для видалення"
 
 msgid "Model:"
 msgstr "Модель:"
 
-msgid "Month View"
-msgstr "Вид місяця"
-
 msgid "Move Cursor"
 msgstr "Переміщення курсора"
 
 msgid "Move down"
 msgstr "Перемістити вниз"
 
 msgid "Move down of one page"
@@ -915,17 +906,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "Неможливо встановити локалізацію %s"
 
 msgid "Unable to set view tree state"
 msgstr "Неможливо встановити стан дерева"
 
-msgid "Unable to write config file %s."
-msgstr "Неможливо записати конфігураційний файл %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "Відновити вибраний запис <Ins>"
 
 msgid "Underline"
 msgstr "Підкреслений"
 
 msgid "Unknown"
@@ -951,17 +939,14 @@
 
 msgid "View _Logs..."
 msgstr "Перегляд _журналів..."
 
 msgid "Week"
 msgstr "Тиждень"
 
-msgid "Week View"
-msgstr "Вид тижня"
-
 msgid "What is the name of this export?"
 msgstr "Як називається цей експорт?"
 
 msgid "Width:"
 msgstr "Ширина:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/uk/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 
 msgid "specify the login user"
 msgstr "вкажіть логін користувача"
 
 msgid "specify the server hostname:port"
 msgstr "вкажіть ім'я сервера:порт"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "Неможливо записати конфігураційний файл %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Неможливо встановити локалізацію %s"
 
 msgid ", "
 msgstr ", "
@@ -58,20 +57,14 @@
 
 msgid "OK"
 msgstr "Гаразд"
 
 msgid "Your selection:"
 msgstr "Ваш вибір:"
 
-msgid "Select"
-msgstr "Вибрати"
-
-msgid "Save"
-msgstr "Зберегти"
-
 msgid "Save As..."
 msgstr "Зберегти як..."
 
 msgid "Do you want to proceed?"
 msgstr "Ви бажаєте продовжити?"
 
 msgid "Always ignore this warning."
@@ -195,14 +188,18 @@
 
 msgid "Template"
 msgstr "Шаблон"
 
 msgid "Edit..."
 msgstr "Редагувати..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "Перегляд _журналів..."
+
 msgid "Attachments..."
 msgstr "Вкладення..."
 
 msgid "Notes..."
 msgstr "Примітки..."
 
 msgid "Actions..."
@@ -591,14 +588,17 @@
 
 msgid "Select File"
 msgstr "Вибрати файл"
 
 msgid "Remove File"
 msgstr "Видалити файл"
 
+msgid "Select"
+msgstr "Вибрати"
+
 msgid "Add..."
 msgstr "Додати..."
 
 msgid "Preview"
 msgstr "Перегляд"
 
 msgid "Previous"
@@ -614,32 +614,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "Примітка (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "Ви повинні вибрати один запис."
 
-msgid "ID:"
-msgstr "ID:"
-
-msgid "Created by:"
-msgstr "Ким створено:"
-
-msgid "Created at:"
-msgstr "Коли створено:"
-
-msgid "Edited by:"
-msgstr "Ким змінено:"
-
-msgid "Edited at:"
-msgstr "Коли змінено:"
-
-msgid "Model:"
-msgstr "Модель:"
-
 msgid "Are you sure to remove this record?"
 msgstr "Ви впевнені, що бажаєте видалити цей запис?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Ви впевнені, що бажаєте видалити ці записи?"
 
 msgid "Records not removed."
@@ -697,14 +679,36 @@
 msgid "Search Limit Settings"
 msgstr "Налаштування обмеження пошуку"
 
 msgid "Limit:"
 msgstr "Кількість записів:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "колоди (%s)"
+
+msgid "Model:"
+msgstr "Модель:"
+
+msgid "ID:"
+msgstr "ID:"
+
+msgid "Created by:"
+msgstr "Ким створено:"
+
+msgid "Created at:"
+msgstr "Коли створено:"
+
+msgid "Last Modified by:"
+msgstr ""
+
+msgid "Last Modified at:"
+msgstr ""
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "Примітки (%s)"
 
 msgid "Edit User Preferences"
 msgstr "Змінити налаштування користувача"
 
 msgid "Preference"
@@ -863,14 +867,17 @@
 
 msgid "Name"
 msgstr "Ім'я"
 
 msgid "Open"
 msgstr "Відкрити"
 
+msgid "Save"
+msgstr "Зберегти"
+
 msgid "Listed Records"
 msgstr "Записи списку"
 
 msgid "Selected Records"
 msgstr "Вибрані записи"
 
 msgid "Ignore search limit"
@@ -1084,26 +1091,24 @@
 
 msgid "previous year"
 msgstr "попередній рік"
 
 msgid "next year"
 msgstr "наступний рік"
 
-msgid "Day View"
-msgstr "Вид дня"
-
-msgid "Week View"
-msgstr "Вид тижня"
-
-msgid "Month View"
-msgstr "Вид місяця"
+msgid "Day"
+msgstr ""
 
 msgid "Week"
 msgstr "Тиждень"
 
+#, fuzzy
+msgid "Month"
+msgstr "Вид місяця"
+
 msgid "Select..."
 msgstr "Вибрати..."
 
 msgid "Clear"
 msgstr "Очистити"
 
 msgid "All files"
@@ -1161,9 +1166,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "Треба зберегти запис перед додаванням перекладів."
 
 msgid "No other language available."
 msgstr "Немає іншої мови."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "Переклад вкладки"
```

### Comparing `tryton-6.6.7/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo` & `tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-03 18:30+0200\n"
+"POT-Creation-Date: 2023-05-01 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -273,17 +273,14 @@
 
 msgid "Database:"
 msgstr "数据库:"
 
 msgid "Date Format"
 msgstr "日期格式"
 
-msgid "Day View"
-msgstr "日视图"
-
 msgid "Default"
 msgstr "默认设置"
 
 msgid "Delete"
 msgstr "删除"
 
 msgid "Delete selected record"
@@ -330,23 +327,17 @@
 
 msgid "Edit..."
 msgstr "编辑..."
 
 msgid "Edited at"
 msgstr "编辑时间"
 
-msgid "Edited at:"
-msgstr "编辑于:"
-
 msgid "Edited by"
 msgstr "编辑人"
 
-msgid "Edited by:"
-msgstr "编辑者:"
-
 msgid "Edition Shortcuts"
 msgstr "编辑快捷方式"
 
 msgid "Encoding:"
 msgstr "编码:"
 
 msgid "Error"
@@ -465,14 +456,17 @@
 
 msgid "Listed Records"
 msgstr "已列出记录"
 
 msgid "Login"
 msgstr "登录"
 
+msgid "Logs (%s)"
+msgstr "日志（%s）"
+
 msgid "M"
 msgstr "月"
 
 msgid "Manage..."
 msgstr "管理..."
 
 msgid "Mark line for deletion/removal"
@@ -480,17 +474,14 @@
 
 msgid "Mark line for removal"
 msgstr "标记要删除的行"
 
 msgid "Model:"
 msgstr "模型:"
 
-msgid "Month View"
-msgstr "月视图"
-
 msgid "Move Cursor"
 msgstr "光标移动"
 
 msgid "Move down"
 msgstr "下移"
 
 msgid "Move down of one page"
@@ -890,17 +881,14 @@
 
 msgid "Unable to set locale %s"
 msgstr "无法设置 locale %s"
 
 msgid "Unable to set view tree state"
 msgstr "无法设置视图树状态"
 
-msgid "Unable to write config file %s."
-msgstr "无法写入配置文件 %s."
-
 msgid "Undelete selected record <Ins>"
 msgstr "已选记录取消删除 <Ins>"
 
 msgid "Underline"
 msgstr "下划线"
 
 msgid "Unknown"
@@ -926,17 +914,14 @@
 
 msgid "View _Logs..."
 msgstr "日志(_V)..."
 
 msgid "Week"
 msgstr "周"
 
-msgid "Week View"
-msgstr "周视图"
-
 msgid "What is the name of this export?"
 msgstr "导出设置的名称是?"
 
 msgid "Width:"
 msgstr "宽度:"
 
 msgid "Wizard"
```

### Comparing `tryton-6.6.7/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po` & `tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
 msgid "specify the login user"
 msgstr "设置登录用户"
 
 msgid "specify the server hostname:port"
 msgstr "设置服务器主机名:端口号"
 
-#, python-format
-msgid "Unable to write config file %s."
-msgstr "无法写入配置文件 %s."
+msgid "disable thread usage"
+msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "无法设置 locale %s"
 
 msgid ", "
 msgstr ", "
@@ -61,20 +60,14 @@
 
 msgid "OK"
 msgstr "确定"
 
 msgid "Your selection:"
 msgstr "已选择:"
 
-msgid "Select"
-msgstr "选择"
-
-msgid "Save"
-msgstr "保存"
-
 msgid "Save As..."
 msgstr "另存为..."
 
 msgid "Do you want to proceed?"
 msgstr "继续此项操作 ?"
 
 msgid "Always ignore this warning."
@@ -198,14 +191,18 @@
 
 msgid "Template"
 msgstr "模板"
 
 msgid "Edit..."
 msgstr "编辑..."
 
+#, fuzzy
+msgid "View Logs..."
+msgstr "日志(_V)..."
+
 msgid "Attachments..."
 msgstr "附件..."
 
 msgid "Notes..."
 msgstr "注释..."
 
 msgid "Actions..."
@@ -594,14 +591,17 @@
 msgid "Select File"
 msgstr "全选"
 
 #, fuzzy
 msgid "Remove File"
 msgstr "删除 <Del>"
 
+msgid "Select"
+msgstr "选择"
+
 msgid "Add..."
 msgstr "添加..."
 
 #, fuzzy
 msgid "Preview"
 msgstr "向前"
 
@@ -618,32 +618,14 @@
 #, python-format
 msgid "Note (%d/%d)"
 msgstr "批注 (%d/%d)"
 
 msgid "You have to select one record."
 msgstr "需要选择一条记录."
 
-msgid "ID:"
-msgstr "标识:"
-
-msgid "Created by:"
-msgstr "创建者:"
-
-msgid "Created at:"
-msgstr "创建日期:"
-
-msgid "Edited by:"
-msgstr "编辑者:"
-
-msgid "Edited at:"
-msgstr "编辑于:"
-
-msgid "Model:"
-msgstr "模型:"
-
 msgid "Are you sure to remove this record?"
 msgstr "确定要删除这条记录吗？"
 
 msgid "Are you sure to remove those records?"
 msgstr "确定要删除这些记录？"
 
 msgid "Records not removed."
@@ -701,14 +683,38 @@
 msgid "Search Limit Settings"
 msgstr "设置查询限制"
 
 msgid "Limit:"
 msgstr "限制:"
 
 #, python-format
+msgid "Logs (%s)"
+msgstr "日志（%s）"
+
+msgid "Model:"
+msgstr "模型:"
+
+msgid "ID:"
+msgstr "标识:"
+
+msgid "Created by:"
+msgstr "创建者:"
+
+msgid "Created at:"
+msgstr "创建日期:"
+
+#, fuzzy
+msgid "Last Modified by:"
+msgstr "最近更改:"
+
+#, fuzzy
+msgid "Last Modified at:"
+msgstr "最近更改日期:"
+
+#, python-format
 msgid "Notes (%s)"
 msgstr "注释(%s)"
 
 msgid "Edit User Preferences"
 msgstr "编辑用户偏好"
 
 msgid "Preference"
@@ -867,14 +873,17 @@
 
 msgid "Name"
 msgstr "名称"
 
 msgid "Open"
 msgstr "打开"
 
+msgid "Save"
+msgstr "保存"
+
 msgid "Listed Records"
 msgstr "已列出记录"
 
 msgid "Selected Records"
 msgstr "已选记录"
 
 msgid "Ignore search limit"
@@ -1089,26 +1098,24 @@
 
 msgid "previous year"
 msgstr "上一年度"
 
 msgid "next year"
 msgstr "下一年度"
 
-msgid "Day View"
-msgstr "日视图"
-
-msgid "Week View"
-msgstr "周视图"
-
-msgid "Month View"
-msgstr "月视图"
+msgid "Day"
+msgstr ""
 
 msgid "Week"
 msgstr "周"
 
+#, fuzzy
+msgid "Month"
+msgstr "月视图"
+
 msgid "Select..."
 msgstr "选择..."
 
 msgid "Clear"
 msgstr "清除"
 
 msgid "All files"
@@ -1166,9 +1173,12 @@
 
 msgid "You need to save the record before adding translations."
 msgstr "请先保存已翻译条目，然后再增加新翻译 ."
 
 msgid "No other language available."
 msgstr "没有其他可翻译语言."
 
+msgid "#ERROR"
+msgstr ""
+
 msgid "Translate view"
 msgstr "翻译视图"
```

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/LICENSE` & `tryton-6.8.0/tryton/data/pixmaps/tryton/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-icon.png` & `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.png`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/tryton-unarchive.svg` & `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.icns` & `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.icns`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.ico` & `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.ico`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/data/pixmaps/tryton/tryton.svg` & `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.svg`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/device_cookie.py` & `tryton-6.8.0/tryton/device_cookie.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/fingerprints.py` & `tryton-6.8.0/tryton/fingerprints.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/main.py` & `tryton-6.8.0/tryton/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import logging
 import os
 import sys
 import threading
 import traceback
 import webbrowser
+from functools import partial
 from urllib.parse import parse_qsl, unquote, urlparse
 
 from gi.repository import Gdk, GdkPixbuf, Gio, GLib, Gtk
 
 import tryton.common as common
 import tryton.plugins
 import tryton.rpc as rpc
@@ -121,15 +122,15 @@
 
     def do_activate(self):
         if self.window:
             self.window.present()
             return
 
         self.window = Gtk.ApplicationWindow(application=self, title="Tryton")
-        self.window.set_default_size(960, 720)
+        self.window.set_default_size(1280, 960)
         self.window.maximize()
         self.window.set_position(Gtk.WindowPosition.CENTER)
         self.window.set_resizable(True)
         self.window.set_icon(TRYTON_ICON)
         self.window.connect("destroy", self.on_quit)
         self.window.connect("delete_event", self.on_quit)
         common.setup_window(self.window)
@@ -171,17 +172,18 @@
             '<tryton>/Form/Save', Gdk.KEY_S, Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
             '<tryton>/Form/Duplicate', Gdk.KEY_D,
             Gdk.ModifierType.CONTROL_MASK | Gdk.ModifierType.SHIFT_MASK)
         Gtk.AccelMap.add_entry(
             '<tryton>/Form/Delete', Gdk.KEY_D, Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
-            '<tryton>/Form/Next', Gdk.KEY_Page_Down, 0)
+            '<tryton>/Form/Next', Gdk.KEY_Down, Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
-            '<tryton>/Form/Previous', Gdk.KEY_Page_Up, 0)
+            '<tryton>/Form/Previous',
+            Gdk.KEY_Up, Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
             '<tryton>/Form/Switch View', Gdk.KEY_L,
             Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
             '<tryton>/Form/Close', Gdk.KEY_W, Gdk.ModifierType.CONTROL_MASK)
         Gtk.AccelMap.add_entry(
             '<tryton>/Form/Reload', Gdk.KEY_R, Gdk.ModifierType.CONTROL_MASK)
@@ -517,27 +519,33 @@
     def get_preferences(self):
         RPCContextReload()
         try:
             prefs = RPCExecute('model', 'res.user', 'get_preferences', False)
         except RPCException:
             prefs = {}
 
-        threads = []
-        for target in (
-                common.IconFactory.load_icons,
-                common.MODELACCESS.load_models,
-                common.MODELHISTORY.load_history,
-                common.MODELNOTIFICATION.load_names,
-                common.VIEW_SEARCH.load_searches,
-                ):
-            t = threading.Thread(target=target)
-            threads.append(t)
-            t.start()
-        for t in threads:
-            t.join()
+        targets = [
+            common.IconFactory.load_icons,
+            common.MODELACCESS.load_models,
+            common.MODELHISTORY.load_history,
+            common.MODELNOTIFICATION.load_names,
+            common.VIEW_SEARCH.load_searches,
+            ]
+        if CONFIG['thread']:
+            threads = []
+            for target in targets:
+                t = threading.Thread(target=target)
+                threads.append(t)
+                t.start()
+            for t in threads:
+                t.join()
+        else:
+            for target in targets:
+                target()
+
         if prefs and 'language_direction' in prefs:
             translate.set_language_direction(prefs['language_direction'])
             CONFIG['client.language_direction'] = \
                 prefs['language_direction']
         self.sig_win_menu(prefs=prefs)
         for action_id in prefs.get('actions', []):
             Action.execute(action_id, {})
@@ -949,14 +957,15 @@
         # Using idle_add because the Gtk.TreeView grabs the focus at the
         # end of the event
         GLib.idle_add(set_cursor)
         for dialog in current_form.dialogs:
             dialog.show()
 
     def _open_url(self, url):
+        loads = partial(json.loads, object_hook=object_hook)
         urlp = urlparse(url)
         if not urlp.scheme == 'tryton':
             return
         urlp = urlparse('http' + url[6:])
         database, path = list(map(unquote,
             (urlp.path[1:].split('/', 1) + [''])[:2]))
         if not path:
@@ -971,96 +980,80 @@
                 return
 
         def open_model(path):
             attributes = {}
             model, path = (path.split('/', 1) + [''])[:2]
             if not model:
                 return
-            res_id = None
-            mode = None
+            attributes = {}
             try:
-                view_ids = json.loads(params.get('views', '[]'))
+                attributes['view_ids'] = loads(params.get('views', '[]'))
                 if 'limit' in params:
-                    attributes['limit'] = json.loads(
-                        params.get('limit', 'null'))
-                name = json.loads(params.get('name', '""'))
-                search_value = json.loads(params.get('search_value', '[]'),
-                    object_hook=object_hook)
-                domain = json.loads(params.get('domain', '[]'),
-                    object_hook=object_hook)
-                context = json.loads(params.get('context', '{}'),
-                    object_hook=object_hook)
-                context_model = params.get('context_model')
-                tab_domain = json.loads(params.get('tab_domain', '[]'),
-                    object_hook=object_hook)
+                    attributes['limit'] = loads(params.get('limit', 'null'))
+                attributes['name'] = loads(params.get('name', '""'))
+                attributes['search_value'] = loads(
+                    params.get('search_value', '[]'))
+                attributes['domain'] = loads(params.get('domain', '[]'))
+                attributes['context'] = loads(params.get('context', '{}'))
+                attributes['context_model'] = params.get('context_model')
+                attributes['tab_domain'] = loads(
+                    params.get('tab_domain', '[]'))
             except ValueError:
                 return
             if path:
                 try:
-                    res_id = int(path)
+                    attributes['res_id'] = int(path)
                 except ValueError:
                     return
-                mode = ['form', 'tree']
+                attributes['mode'] = ['form', 'tree']
             try:
-                Window.create(model,
-                    view_ids=view_ids,
-                    res_id=res_id,
-                    domain=domain,
-                    context=context,
-                    context_model=context_model,
-                    mode=mode,
-                    name=name,
-                    search_value=search_value,
-                    tab_domain=tab_domain,
-                    **attributes)
+                Window.create(model, **attributes)
             except Exception:
                 # Prevent crashing the client
                 return
 
         def open_wizard(wizard):
+            attributes = {}
             if not wizard:
                 return
             try:
-                data = json.loads(params.get('data', '{}'),
-                    object_hook=object_hook)
-                direct_print = json.loads(params.get('direct_print', 'false'))
-                name = json.loads(params.get('name', '""'))
-                window = json.loads(params.get('window', 'false'))
-                context = json.loads(params.get('context', '{}'),
-                    object_hook=object_hook)
+                attributes['data'] = loads(params.get('data', '{}'))
+                attributes['direct_print'] = loads(
+                    params.get('direct_print', 'false'))
+                attributes['name'] = loads(params.get('name', '""'))
+                attributes['window'] = loads(params.get('window', 'false'))
+                attributes['context'] = loads(params.get('context', '{}'))
             except ValueError:
                 return
             try:
-                Window.create_wizard(
-                    wizard, data, direct_print=direct_print, name=name,
-                    context=context, window=window)
+                Window.create_wizard(wizard, **attributes)
             except Exception:
                 # Prevent crashing the client
                 return
 
         def open_report(report):
+            attributes = {}
             if not report:
                 return
             try:
-                data = json.loads(params.get('data'), object_hook=object_hook)
-                direct_print = json.loads(params.get('direct_print', 'false'))
-                context = json.loads(params.get('context', '{}'),
-                    object_hook=object_hook)
+                attributes['data'] = loads(params.get('data', '{}'))
+                attributes['direct_print'] = loads(
+                    params.get('direct_print', 'false'))
+                attributes['context'] = loads(params.get('context', '{}'))
             except ValueError:
                 return
             try:
-                Action.exec_report(
-                    report, data, direct_print=direct_print, context=context)
+                Action.exec_report(report, **attributes)
             except Exception:
                 # Prevent crashing the client
                 return
 
         def open_url():
             try:
-                url = json.loads(params.get('url', 'false'))
+                url = loads(params.get('url', 'false'))
             except ValueError:
                 return
             if url:
                 webbrowser.open(url, new=2)
 
         if type_ == 'model':
             open_model(path)
```

### Comparing `tryton-6.6.7/tryton/gui/window/about.py` & `tryton-6.8.0/tryton/gui/window/about.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/attachment.py` & `tryton-6.8.0/tryton/gui/window/attachment.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/board.py` & `tryton-6.8.0/tryton/gui/window/board.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/dblogin.py` & `tryton-6.8.0/tryton/gui/window/dblogin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import configparser
 import gettext
 import logging
 import os
+import shutil
+import tempfile
 import threading
 
 from gi.repository import GLib, GObject, Gtk
 
 import tryton.common as common
 import tryton.rpc as rpc
 from tryton import __version__
@@ -280,17 +282,21 @@
         version = rpc.server_version(host, port)
         if not version:
             return None
         return version.split('.')[:2] == __version__.split('.')[:2]
 
     def refresh_databases(self, host, port):
         self.dbs_updated = threading.Event()
-        threading.Thread(target=self.refresh_databases_start,
-            args=(host, port)).start()
-        GLib.timeout_add(100, self.refresh_databases_end, host, port)
+        if CONFIG['thread']:
+            threading.Thread(target=self.refresh_databases_start,
+                args=(host, port)).start()
+            GLib.timeout_add(100, self.refresh_databases_end, host, port)
+        else:
+            self.refresh_databases_start(host, port)
+            self.refresh_databases_end(host, port)
 
     def refresh_databases_start(self, host, port):
         dbs = None
         try:
             dbs = rpc.db_list(host, port)
         except Exception:
             pass
@@ -478,28 +484,39 @@
         label_username = Gtk.Label(
             label=set_underline(_("User name:")),
             use_underline=True, halign=Gtk.Align.END, margin=3)
         label_username.set_mnemonic_widget(self.entry_login)
         grid.attach(label_username, 0, 5, 1, 1)
 
         # Profile information
-        self.profile_cfg = os.path.join(get_config_dir(), 'profiles.cfg')
+        config_dir = get_config_dir()
+        self.profile_cfg = os.path.join(config_dir, 'profiles.cfg')
         self.profiles = configparser.ConfigParser()
-        if not os.path.exists(self.profile_cfg):
+        try:
+            self.profiles.read(self.profile_cfg)
+        except configparser.Error:
+            # reset self.profiles as parsing errors may leave wrong data in
+            # the parser
+            self.profiles = configparser.ConfigParser()
+            with tempfile.NamedTemporaryFile(
+                    delete=False, prefix='profiles_', suffix='.cfg',
+                    dir=config_dir) as temp_file:
+                temp_name = temp_file.name
+            shutil.copy(self.profile_cfg, temp_name)
+            logger.error(
+                f"Failed to parse {self.profiles_cfg}. "
+                f"A backup can be found at {temp_name}",
+                exc_info=True)
+        if not self.profiles.sections():
             short_version = '.'.join(__version__.split('.', 2)[:2])
             name = 'demo%s.tryton.org' % short_version
             self.profiles.add_section(name)
             self.profiles.set(name, 'host', name)
             self.profiles.set(name, 'database', 'demo%s' % short_version)
             self.profiles.set(name, 'username', 'demo')
-        else:
-            try:
-                self.profiles.read(self.profile_cfg)
-            except configparser.ParsingError:
-                logger.error("Fail to parse profiles.cfg", exc_info=True)
         for section in self.profiles.sections():
             active = all(self.profiles.has_option(section, option)
                 for option in ('host', 'database'))
             self.profile_store.append([section, active])
 
         self.services = []
         self.service_base = ''
```

### Comparing `tryton-6.6.7/tryton/gui/window/email_.py` & `tryton-6.8.0/tryton/gui/window/email_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/form.py` & `tryton-6.8.0/tryton/gui/window/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 "Form"
 import csv
-import datetime
 import gettext
 import locale
 import os
 import tempfile
 from itertools import zip_longest
 
 from gi.repository import Gdk, GLib, Gtk
 
 import tryton.common as common
 from tryton import plugins
 from tryton.action import Action
-from tryton.common import (
-    RPCException, RPCExecute, message, sur, sur_3b, timezoned_date)
+from tryton.common import RPCException, RPCExecute, sur, sur_3b
 from tryton.common.common import selection as selection_
 from tryton.common.popup_menu import popup
 from tryton.common.underline import set_underline
 from tryton.gui import Main
 from tryton.gui.window import Window
 from tryton.gui.window.attachment import Attachment
 from tryton.gui.window.email_ import Email
+from tryton.gui.window.log import Log
 from tryton.gui.window.note import Note
 from tryton.gui.window.revision import Revision
 from tryton.gui.window.view_form.screen import Screen
 from tryton.gui.window.win_export import WinExport
 from tryton.gui.window.win_import import WinImport
 
 from .tabcontent import TabContent
@@ -71,15 +70,15 @@
             if self.screen.current_view.view_type == 'form':
                 self.sig_new(None, autosave=False)
             if self.screen.current_view.view_type \
                     in ('tree', 'graph', 'calendar'):
                 self.screen.search_filter()
 
         self.update_revision()
-        self.activate_save()
+        self.set_buttons_sensitive()
 
     def get_toolbars(self):
         try:
             return RPCExecute('model', self.model, 'view_toolbar_get',
                 context=self.screen.context)
         except RPCException:
             return {}
@@ -291,45 +290,16 @@
         self.screen.switch_view()
 
     def sig_logs(self, widget=None):
         current_record = self.screen.current_record
         if not current_record or current_record.id < 0:
             self.info_bar_add(
                 _('You have to select one record.'), Gtk.MessageType.INFO)
-            return False
-
-        fields = [
-            ('id', _('ID:')),
-            ('create_uid.rec_name', _('Created by:')),
-            ('create_date', _('Created at:')),
-            ('write_uid.rec_name', _('Edited by:')),
-            ('write_date', _('Edited at:')),
-        ]
-
-        try:
-            data = RPCExecute('model', self.model, 'read', [current_record.id],
-                [x[0] for x in fields], context=self.screen.context)[0]
-        except RPCException:
             return
-        date_format = self.screen.context.get('date_format', '%x')
-        datetime_format = date_format + ' %H:%M:%S.%f'
-        message_str = ''
-        for (key, label) in fields:
-            value = data
-            keys = key.split('.')
-            name = keys.pop(-1)
-            for key in keys:
-                value = value.get(key + '.', {})
-            value = (value or {}).get(name, '/')
-            if isinstance(value, datetime.datetime):
-                value = timezoned_date(value).strftime(datetime_format)
-            message_str += '%s %s\n' % (label, value)
-        message_str += _('Model:') + ' ' + self.model
-        message(message_str)
-        return True
+        Log(current_record)
 
     def sig_revision(self, widget=None):
         if not self.modified_save():
             return
         current_id = (self.screen.current_record.id
             if self.screen.current_record else None)
         try:
@@ -370,32 +340,37 @@
                 self.name, 80 - len(revision_label)) + revision_label
             tooltip = self.name + revision_label
         else:
             label = common.ellipsize(self.name, 80)
             tooltip = self.name
         self.title.set_text(label)
         tooltips.set_tip(self.title, tooltip)
-        self.set_buttons_sensitive(revision)
+        self.set_buttons_sensitive()
 
-    def set_buttons_sensitive(self, revision=None):
+    def set_buttons_sensitive(self):
+        revision = self.screen.context.get('_datetime')
         if not revision:
             access = common.MODELACCESS[self.model]
+            modified = self.screen.modified()
             for name, sensitive in [
-                    ('new', access['create']),
-                    ('save', access['create'] or access['write']),
+                    ('new', access['create'] and not modified),
+                    ('save',
+                        (access['create'] or access['write'])
+                        and modified and not self.screen.readonly),
                     ('remove', access['delete']),
                     ('copy', access['create']),
                     ('import', access['create']),
+                    ('action', access['write'] and not self.screen.readonly),
                     ]:
                 if name in self.buttons:
                     self.buttons[name].props.sensitive = sensitive
                 if name in self.menu_buttons:
                     self.menu_buttons[name].props.sensitive = sensitive
         else:
-            for name in ['new', 'save', 'remove', 'copy', 'import']:
+            for name in ['new', 'save', 'remove', 'copy', 'import', 'action']:
                 if name in self.buttons:
                     self.buttons[name].props.sensitive = False
                 if name in self.menu_buttons:
                     self.menu_buttons[name].props.sensitive = False
 
     def sig_remove(self, widget=None):
         if (not common.MODELACCESS[self.model]['delete']
@@ -463,15 +438,15 @@
         if not common.MODELACCESS[self.model]['create']:
             return
         if autosave:
             if not self.modified_save():
                 return
         self.screen.new()
         self.info_bar_clear()
-        self.activate_save()
+        self.set_buttons_sensitive()
 
     def sig_copy(self, widget=None):
         if not common.MODELACCESS[self.model]['create']:
             return
         if not self.modified_save():
             return
         if self.screen.copy():
@@ -498,22 +473,22 @@
             return False
 
     def sig_previous(self, widget=None):
         if not self.modified_save():
             return
         self.screen.display_prev()
         self.info_bar_clear()
-        self.activate_save()
+        self.set_buttons_sensitive()
 
     def sig_next(self, widget=None):
         if not self.modified_save():
             return
         self.screen.display_next()
         self.info_bar_clear()
-        self.activate_save()
+        self.set_buttons_sensitive()
 
     def sig_reload(self, test_modified=True):
         if test_modified:
             if not self.modified_save():
                 return False
         else:
             self.screen.save_tree_state(store=False)
@@ -527,15 +502,14 @@
                 if record.id == record_id:
                     self.screen.current_record = record
                     set_cursor = True
                     break
         self.screen.display(set_cursor=set_cursor)
         self.info_bar_clear()
         self.set_buttons_sensitive()
-        self.activate_save()
         self.screen.count_tab_domain()
         return True
 
     def sig_action(self, widget):
         if self.buttons['action'].props.sensitive:
             self.buttons['action'].props.active = True
 
@@ -597,27 +571,24 @@
             if button_id in self.menu_buttons:
                 self.menu_buttons[button_id].props.sensitive = sensitive
 
         name = str(position) if position else '_'
         selected = len(self.screen.selected_records)
         if selected > 1:
             name += '#%i' % selected
-        for button_id in ('print', 'relate', 'email', 'open', 'save',
-                'attach'):
+        for button_id in ['print', 'relate', 'email', 'open', 'attach']:
             button = self.buttons[button_id]
             can_be_sensitive = getattr(button, '_can_be_sensitive', True)
             if button_id in {'print', 'relate', 'email', 'open'}:
                 action_type = button_id
                 if button_id == 'open':
                     action_type = 'print'
                 can_be_sensitive |= any(
                     b.attrs.get('keyword', 'action') == action_type
                     for b in self.screen.get_buttons())
-            elif button_id == 'save':
-                can_be_sensitive &= not self.screen.readonly
             set_sensitive(button_id, bool(position) and can_be_sensitive)
         set_sensitive('switch', self.screen.number_of_views > 1)
         set_sensitive('remove', self.screen.deletable)
         set_sensitive('previous', self.screen.has_prev())
         set_sensitive('next', self.screen.has_next())
 
         if size < max_size:
@@ -625,28 +596,28 @@
                 name, common.humanize(size), common.humanize(max_size))
             if max_size >= self.screen.count_limit:
                 msg += "+"
         else:
             msg = "%s/%s" % (name, common.humanize(size))
         self.status_label.set_text(msg)
         self.info_bar_clear()
-        self.activate_save()
+        self.set_buttons_sensitive()
         self.refresh_attachment_preview()
 
     def record_modified(self):
         def _record_modified():
             # As it is called via idle_add, the form could have been destroyed
             # in the meantime.
             if self.widget_get().props.window:
-                self.activate_save()
+                self.set_buttons_sensitive()
         GLib.idle_add(_record_modified)
         self.info_bar_refresh()
 
     def record_saved(self):
-        self.activate_save()
+        self.set_buttons_sensitive()
         self.refresh_resources()
 
     def modified_save(self):
         self.screen.save_tree_state()
         self.screen.current_view.set_value()
         if self.screen.modified():
             value = sur_3b(
@@ -689,17 +660,14 @@
                 if self.screen.context_screen else None),
             'id': record_id,
             'ids': record_ids,
             'paths': record_paths,
         }
         Action.execute(action, data, context=self.screen.local_context)
 
-    def activate_save(self):
-        self.buttons['save'].props.sensitive = self.screen.modified()
-
     def sig_win_close(self, widget):
         Main().sig_win_close(widget)
 
     def create_toolbar(self, toolbars):
         gtktoolbar = super(Form, self).create_toolbar(toolbars)
 
         attach_btn = self.buttons['attach']
```

### Comparing `tryton-6.6.7/tryton/gui/window/infobar.py` & `tryton-6.8.0/tryton/gui/window/infobar.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,39 @@
 
     toolbar = None
 
     def create_info_bar(self):
         self.__box = Gtk.VBox()
         self.__box.show()
         self.__messages = set()
+        self.__kinds = {}
         return self.__box
 
-    def info_bar_add(self, message, type_=Gtk.MessageType.ERROR):
+    def info_bar_add(self, message, type_=Gtk.MessageType.ERROR, kind=None):
         if not message:
             return
         key = (message, type_)
         if key not in self.__messages:
             info_bar = Gtk.InfoBar()
             self.__box.pack_start(info_bar, False, False, 0)
             area = info_bar.get_content_area()
             area.add(Gtk.Label(label=message))
             info_bar.set_show_close_button(True)
             info_bar.connect('response', self.__response, key)
             info_bar.set_message_type(type_)
             info_bar.show_all()
+            self.__kinds[info_bar] = kind
 
     def __response(self, widget, response, key):
         self.__messages.add(key)
         self.__box.remove(widget)
 
-    def info_bar_refresh(self):
+    def info_bar_refresh(self, kind=None):
         for child in self.__box.get_children():
-            self.__box.remove(child)
+            if self.__kinds[child] == kind:
+                self.__box.remove(child)
+                del self.__kinds[child]
 
     def info_bar_clear(self):
-        self.info_bar_refresh()
+        for kind in set(self.__kinds.values()):
+            self.info_bar_refresh(kind=kind)
         self.__messages.clear()
```

### Comparing `tryton-6.6.7/tryton/gui/window/limit.py` & `tryton-6.8.0/tryton/gui/window/limit.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/nomodal.py` & `tryton-6.8.0/tryton/gui/window/nomodal.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/note.py` & `tryton-6.8.0/tryton/gui/window/note.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/preference.py` & `tryton-6.8.0/tryton/gui/window/preference.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/revision.py` & `tryton-6.8.0/tryton/gui/window/revision.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/tabcontent.py` & `tryton-6.8.0/tryton/gui/window/tabcontent.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_board/action.py` & `tryton-6.8.0/tryton/gui/window/view_board/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,18 +118,14 @@
             def callback(result):
                 if result:
                     self.screen.current_record.save()
                 else:
                     self.screen.current_record.cancel()
             WinForm(self.screen, callback, title=self.title.get_text())
 
-    def set_value(self, mode, model_field):
-        self.screen.current_view.set_value()
-        return True
-
     def display(self):
         self.screen.search_filter(self.screen.screen_container.get_text())
 
     def record_message(self, *args):
         self.view.active_changed(self)
 
     def _get_active(self):
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_board/view_board.py` & `tryton-6.8.0/tryton/gui/window/view_board/view_board.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/model/field.py` & `tryton-6.8.0/tryton/gui/window/view_form/model/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,28 +91,38 @@
                     and not bool(int(state_attrs.get('readonly') or 0))):
                 return False
         return True
 
     def validate(self, record, softvalidation=False, pre_validate=None):
         if self.attrs.get('readonly'):
             return True
+        state_attrs = self.get_state_attrs(record)
+        is_required = bool(int(state_attrs.get('required') or 0))
+        is_invisible = bool(int(state_attrs.get('invisible') or 0))
         invalid = False
-        self.get_state_attrs(record)['domain_readonly'] = False
+        state_attrs['domain_readonly'] = False
         domain = simplify(self.validation_domains(record, pre_validate))
         if not softvalidation:
             if not self.check_required(record):
                 invalid = 'required'
         if isinstance(domain, bool):
             if not domain:
                 invalid = 'domain'
         elif domain == [('id', '=', None)]:
             invalid = 'domain'
         else:
+            screen_domain, _ = self.domains_get(record, pre_validate)
             unique, leftpart, value = unique_value(domain)
-            if unique:
+            unique_from_screen, _, _ = unique_value(screen_domain)
+            if (self._is_empty(record)
+                    and not is_required
+                    and not is_invisible
+                    and not unique_from_screen):
+                pass
+            elif unique:
                 # If the inverted domain is so constraint that only one value
                 # is possible we should use it. But we must also pay attention
                 # to the fact that the original domain might be a 'OR' domain
                 # and thus not preventing the modification of fields.
                 if value is False:
                     # XXX to remove once server domains are fixed
                     value = None
@@ -128,19 +138,18 @@
                     if domain_readonly:
                         for leaf in localize_domain(original_domain[1:]):
                             constraintfields.add(leaf[0])
                     if localpart != 'id' or recordpart not in constraintfields:
                         setdefault = False
                 if setdefault and not pre_validate:
                     self.set_client(record, value)
-                    self.get_state_attrs(record)['domain_readonly'] = (
-                        domain_readonly)
+                    state_attrs['domain_readonly'] = domain_readonly
             if not eval_domain(domain, EvalEnvironment(record)):
                 invalid = domain
-        self.get_state_attrs(record)['invalid'] = invalid
+        state_attrs['invalid'] = invalid
         return not invalid
 
     def set(self, record, value):
         record.value[self.name] = value
 
     def get(self, record):
         return record.value.get(self.name, self._default)
@@ -350,14 +359,19 @@
         value = super(TimeDeltaField, self).get_client(record)
         return common.timedelta.format(value, self.converter(record.group))
 
 
 class FloatField(Field):
     _default = None
 
+    def __init__(self, attrs):
+        super().__init__(attrs)
+        self._digits = {}
+        self._symbol = {}
+
     def _is_empty(self, record):
         return self.get(record) is None
 
     def get(self, record):
         return record.value.get(self.name, self._default)
 
     def digits(self, record, factor=1):
@@ -365,22 +379,26 @@
         if isinstance(digits, str):
             if digits not in record.group.fields:
                 return
             digits_field = record.group.fields[digits]
             digits_name = digits_field.attrs.get('relation')
             digits_id = digits_field.get(record)
             if digits_name and digits_id is not None and digits_id >= 0:
-                try:
-                    digits = RPCExecute(
-                        'model', digits_name, 'get_digits', digits_id)
-                except RPCException:
-                    logger.warn(
-                        "Fail to fetch digits for %s,%s",
-                        digits_name, digits_id)
-                    return
+                if digits_id in self._digits:
+                    digits = self._digits[digits_id]
+                else:
+                    try:
+                        digits = RPCExecute(
+                            'model', digits_name, 'get_digits', digits_id)
+                    except RPCException:
+                        logger.warn(
+                            "Fail to fetch digits for %s,%s",
+                            digits_name, digits_id)
+                        return
+                    self._digits[digits_id] = digits
             else:
                 return
         if not digits or any(d is None for d in digits):
             return
         shift = int(round(math.log(abs(factor), 10)))
         return (digits[0] + shift, digits[1] - shift)
 
@@ -392,18 +410,22 @@
                 sign = -1
             elif value == 0:
                 sign = 0
             symbol_field = record.group.fields[symbol]
             symbol_name = symbol_field.attrs.get('relation')
             symbol_id = symbol_field.get(record)
             if symbol_name and symbol_id is not None and symbol_id >= 0:
+                if symbol_id in self._symbol:
+                    return self._symbol[symbol_id]
                 try:
-                    return RPCExecute(
+                    result = RPCExecute(
                         'model', symbol_name, 'get_symbol', symbol_id, sign,
                         context=record.get_context())
+                    self._symbol[symbol_id] = result
+                    return result
                 except RPCException:
                     logger.warn(
                         "Fail to fetch symbol for %s,%s",
                         symbol_name, symbol_id)
         return '', 1
 
     def convert(self, value):
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/model/group.py` & `tryton-6.8.0/tryton/gui/window/view_form/model/group.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/model/record.py` & `tryton-6.8.0/tryton/gui/window/view_form/model/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,19 @@
         self.next = {}  # Used in Group list
         self.value = {}
         self.autocompletion = {}
         self.exception = False
         self.destroyed = False
 
     def __getitem__(self, name):
+        self.load(name)
+        if name != '*':
+            return self.group.fields[name]
+
+    def load(self, name, process_exception=True):
         if not self.destroyed and self.id >= 0 and name not in self._loaded:
             id2record = {
                 self.id: self,
                 }
             if name == '*':
                 loading = 'eager'
                 views = set()
@@ -70,17 +75,21 @@
                     if field.attrs.get('loading', 'eager') == 'eager')
             else:
                 fields = self.group.fields.items()
 
             fnames = [fname for fname, field in fields
                 if fname not in self._loaded
                 and (not views or (views & field.views))]
-            fnames.extend(('%s.rec_name' % fname for fname in fnames[:]
-                    if self.group.fields[fname].attrs['type']
-                    in ('many2one', 'one2one', 'reference')))
+            for fname in list(fnames):
+                f_attrs = self.group.fields[fname].attrs
+                if f_attrs['type'] in {'many2one', 'one2one', 'reference'}:
+                    fnames.append('%s.rec_name' % fname)
+                elif (f_attrs['type'] == 'selection'
+                        and f_attrs.get('loading', 'lazy') == 'eager'):
+                    fnames.append('%s:string' % fname)
             if 'rec_name' not in fnames:
                 fnames.append('rec_name')
             fnames.extend(['_timestamp', '_write', '_delete'])
 
             record_context = self.get_context()
             if loading == 'eager':
                 limit = CONFIG['client.limit'] // min(len(fnames), 10)
@@ -122,15 +131,16 @@
             ctx = record_context.copy()
             ctx.update(dict(('%s.%s' % (self.model_name, fname), 'size')
                     for fname, field in self.group.fields.items()
                     if field.attrs['type'] == 'binary' and fname in fnames))
             exception = False
             try:
                 values = RPCExecute('model', self.model_name, 'read',
-                    list(id2record.keys()), fnames, context=ctx)
+                    list(id2record.keys()), fnames, context=ctx,
+                    process_exception=process_exception)
             except RPCException:
                 values = [{'id': x} for x in id2record]
                 default_values = dict((f, None) for f in fnames)
                 for value in values:
                     value.update(default_values)
                 self.exception = exception = True
             id2value = dict((value['id'], value) for value in values)
@@ -138,16 +148,14 @@
                 if not record.exception:
                     record.exception = exception
                 value = id2value.get(id)
                 if record and not record.destroyed and value:
                     for key in record.modified_fields:
                         value.pop(key, None)
                     record.set(value, modified=False)
-        if name != '*':
-            return self.group.fields[name]
 
     def __repr__(self):
         return '<Record %s@%s at %s>' % (self.id, self.model_name, id(self))
 
     @property
     def modified(self):
         if self.modified_fields:
@@ -236,14 +244,15 @@
 
     deleted = property(get_deleted)
 
     def get_readonly(self):
         return (self.deleted
             or self.removed
             or self.exception
+            or self.group.readonly
             or not self._write)
 
     readonly = property(get_readonly)
 
     @property
     def deletable(self):
         return self._delete
@@ -460,21 +469,25 @@
             if fieldname in {'_write', '_delete'}:
                 setattr(self, fieldname, value)
                 continue
             if fieldname not in self.group.fields:
                 if fieldname == 'rec_name':
                     self.value['rec_name'] = value
                 continue
-            if isinstance(self.group.fields[fieldname], fields.O2MField):
+            field = self.group.fields[fieldname]
+            if isinstance(field, fields.O2MField):
                 later[fieldname] = value
                 continue
-            if isinstance(self.group.fields[fieldname], (fields.M2OField,
-                        fields.ReferenceField)):
+            if isinstance(field, (fields.M2OField, fields.ReferenceField)):
                 related = fieldname + '.'
                 self.value[related] = val.get(related) or {}
+            elif (isinstance(field, fields.SelectionField)
+                    and fieldname + ':string' in val):
+                related = fieldname + ':string'
+                self.value[related] = val[related]
             self.group.fields[fieldname].set(self, value)
             self._loaded.add(fieldname)
             fieldnames.append(fieldname)
         for fieldname, value in later.items():
             self.group.fields[fieldname].set(self, value)
             self._loaded.add(fieldname)
         if validate:
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/screen/screen.py` & `tryton-6.8.0/tryton/gui/window/view_form/screen/screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -418,18 +418,15 @@
         self.group.screens.append(self)
         self.parent = group.parent
         self.parent_name = group.parent_name
         if self.parent:
             self.filter_widget = None
             self.order = None
         self.__group.add_fields(fields)
-        if len(group):
-            self.current_record = group[0]
-        else:
-            self.current_record = None
+        self.current_record = None
         for name, views in fields_views.items():
             self.__group.fields[name].views.update(views)
         self.__group.exclude_field = self.exclude_field
 
     group = property(__get_group, __set_group)
 
     def new_group(self, context=None):
@@ -448,22 +445,22 @@
                 window.record_modified()
         if display:
             self.display()
 
     def record_notify(self, notifications):
         for window in self.windows:
             if isinstance(window, InfoBar):
-                window.info_bar_refresh()
+                window.info_bar_refresh('notification')
                 for type_, message in notifications:
                     type_ = {
                         'info': Gtk.MessageType.INFO,
                         'warning': Gtk.MessageType.WARNING,
                         'error': Gtk.MessageType.ERROR,
                         }.get(type_, Gtk.MessageType.WARNING)
-                    window.info_bar_add(message, type_)
+                    window.info_bar_add(message, type_, 'notification')
 
     def record_message(self, position, size, max_size, record_id):
         for window in self.windows:
             if hasattr(window, 'record_message'):
                 window.record_message(position, size, max_size, record_id)
 
     def record_saved(self):
@@ -482,15 +479,15 @@
     def __get_current_record(self):
         if (self.__current_record is not None
                 and self.__current_record.group is None):
             self.__current_record = None
         return self.__current_record
 
     def __set_current_record(self, record):
-        if self.__current_record == record:
+        if self.__current_record == record and record:
             return
         self.__current_record = record
         if record:
             try:
                 pos = self.group.index(record) + self.offset + 1
             except ValueError:
                 # XXX offset?
@@ -785,19 +782,14 @@
             return
         if delete:
             # Must delete children records before parent
             records.sort(key=lambda r: r.depth, reverse=True)
             if not self.group.delete(records):
                 return False
 
-        top_record = records[0]
-        top_group = top_record.group
-        idx = top_group.index(top_record)
-        path = top_record.get_path(self.group)
-
         for record in records:
             # set current model to None to prevent __select_changed
             # to save the previous_model as it can be already deleted.
             self.current_record = None
             record.group.remove(
                 record, remove=remove, modified=False,
                 force_remove=force_remove)
@@ -811,23 +803,15 @@
                 if record in record.group.record_removed:
                     record.group.record_removed.remove(record)
                 if record.parent:
                     # Save parent without deleted children
                     record.parent.save(force_reload=False)
                 record.destroy()
 
-        if idx > 0:
-            record = top_group[idx - 1]
-            path = path[:-1] + ((path[-1][0], record.id,),)
-        else:
-            path = path[:-1]
-        if path:
-            self.current_record = self.group.get_by_path(path)
-        elif len(self.group):
-            self.current_record = self.group[0]
+        self.current_record = None
         self.set_cursor()
         self.display()
         return True
 
     def copy(self):
         ids = [r.id for r in self.selected_records]
         try:
@@ -836,48 +820,51 @@
         except RPCException:
             return False
         self.load(new_ids, position=self.new_position)
         return True
 
     def set_tree_state(self):
         view = self.current_view
-        if view.view_type not in ('tree', 'form'):
+        if view.view_type not in {'tree', 'form', 'list-form'}:
             return
         if id(view) in self.tree_states_done:
             return
         if view.view_type == 'form' and self.tree_states_done:
             return
-        if (view.view_type == 'tree'
-                and not view.attributes.get('tree_state', False)):
+        if (view.view_type in {'tree', 'list-form'}
+                and not int(view.attributes.get('tree_state', False))):
             # Mark as done to not set later when the view_type change
             self.tree_states_done.add(id(view))
         parent = self.parent.id if self.parent else None
         if parent is not None and parent < 0:
             return
         expanded_nodes, selected_nodes = [], []
-        state = self.tree_states[parent][view.children_field]
-        if state:
-            expanded_nodes, selected_nodes = state
-        if state is None and CONFIG['client.save_tree_state']:
-            json_domain = self.get_tree_domain(parent)
-            try:
-                expanded_nodes, selected_nodes = RPCExecute('model',
-                    'ir.ui.view_tree_state', 'get',
-                    self.model_name, json_domain,
-                    view.children_field)
-                expanded_nodes = json.loads(expanded_nodes)
-                selected_nodes = json.loads(selected_nodes)
-            except RPCException:
-                logger.warn(
-                    'Unable to get view tree state for %s',
-                    self.model_name)
-            self.tree_states[parent][view.children_field] = (
-                expanded_nodes, selected_nodes)
-        if view.view_type == 'tree':
-            view.expand_nodes(expanded_nodes)
+        if view.view_type in {'tree', 'list-form'}:
+            state = self.tree_states[parent][view.children_field]
+            if state:
+                expanded_nodes, selected_nodes = state
+            if (state is None
+                    and CONFIG['client.save_tree_state']
+                    and int(view.attributes.get('tree_state', False))):
+                json_domain = self.get_tree_domain(parent)
+                try:
+                    expanded_nodes, selected_nodes = RPCExecute('model',
+                        'ir.ui.view_tree_state', 'get',
+                        self.model_name, json_domain,
+                        view.children_field)
+                    expanded_nodes = json.loads(expanded_nodes)
+                    selected_nodes = json.loads(selected_nodes)
+                except RPCException:
+                    logger.warn(
+                        'Unable to get view tree state for %s',
+                        self.model_name)
+                self.tree_states[parent][view.children_field] = (
+                    expanded_nodes, selected_nodes)
+            if view.view_type == 'tree':
+                view.expand_nodes(expanded_nodes)
             view.select_nodes(selected_nodes)
         else:
             if selected_nodes:
                 record = None
                 for node in selected_nodes[0]:
                     new_record = self.group.get(node)
                     if node < 0 and -node < len(self.group):
@@ -905,17 +892,20 @@
                 if len(self.views) == 1 and self.current_record:
                     path = self.current_record.id
                     if path < 0:
                         path = -self.current_record.group.index(
                             self.current_record)
                     self.tree_states[parent][view.children_field] = (
                         [], [[path]])
-            elif view.view_type == 'tree':
-                view.save_width()
-                paths = view.get_expanded_paths()
+            elif view.view_type in {'tree', 'list-form'}:
+                if view.view_type == 'tree':
+                    view.save_width()
+                    paths = view.get_expanded_paths()
+                else:
+                    paths = []
                 selected_paths = view.get_selected_paths()
                 self.tree_states[parent][view.children_field] = (
                     paths, selected_paths)
                 if (store
                         and int(view.attributes.get('tree_state', False))
                         and CONFIG['client.save_tree_state']):
                     json_domain = self.get_tree_domain(parent)
@@ -955,15 +945,15 @@
     def display(self, res_id=None, set_cursor=False):
         if res_id:
             self.current_record = self.group.get(res_id)
         else:
             if (self.current_record
                     and self.current_record in self.current_record.group):
                 pass
-            elif self.group and self.current_view.view_type != 'calendar':
+            elif self.group and self.current_view.view_type == 'form':
                 self.current_record = self.group[0]
             else:
                 self.current_record = None
         if self.views:
             self.search_active(self.current_view.view_type
                 in ('tree', 'graph', 'calendar'))
             for view in self.views:
@@ -982,27 +972,15 @@
                 self.set_cursor(reset_view=False)
         self.set_tree_state()
         # Force record_message
         self.current_record = self.current_record
 
     def _get_next_record(self, test=False):
         view = self.current_view
-        if view.view_type == 'tree' and len(self.group):
-            range_ = view.treeview.get_visible_range()
-            if range_ and not test:
-                start, end = range_
-                vadjustment = view.treeview.get_vadjustment()
-                vadjustment.set_value(
-                    vadjustment.props.value + vadjustment.props.page_increment)
-                model = view.treeview.get_model()
-                iter_ = model.get_iter(end)
-                return model.get_value(iter_, 0)
-            else:
-                return self.group[-1]
-        elif (view.view_type == 'form'
+        if (view.view_type in {'tree', 'form'}
                 and self.current_record
                 and self.current_record.group):
             group = self.current_record.group
             record = self.current_record
             while group:
                 children = record.children_group(view.children_field)
                 if children:
@@ -1069,27 +1047,15 @@
         self.set_cursor(reset_view=False)
         self.current_record = self._get_next_record()
         self.set_cursor(reset_view=False)
         view.display()
 
     def _get_prev_record(self, test=False):
         view = self.current_view
-        if view.view_type == 'tree' and len(self.group):
-            range_ = view.treeview.get_visible_range()
-            if range_ and not test:
-                start, end = range_
-                vadjustment = view.treeview.get_vadjustment()
-                vadjustment.set_value(
-                    vadjustment.props.value - vadjustment.props.page_increment)
-                model = view.treeview.get_model()
-                iter_ = model.get_iter(start)
-                return model.get_value(iter_, 0)
-            else:
-                return self.group[0]
-        elif (view.view_type == 'form'
+        if (view.view_type in {'tree', 'form'}
                 and self.current_record
                 and self.current_record.group):
             group = self.current_record.group
             record = self.current_record
             idx = group.index(record) - 1
             if idx >= 0:
                 record = group[idx]
@@ -1179,15 +1145,17 @@
     @property
     def selected_paths(self):
         if self.current_view and self.current_view.view_type == 'tree':
             return self.current_view.get_selected_paths()
 
     @property
     def listed_records(self):
-        if self.current_view and self.current_view.view_type == 'tree':
+        if (self.current_view
+                and self.current_view.view_type in {
+                    'tree', 'calendar', 'list-form'}):
             return self.current_view.listed_records
         elif self.current_record:
             return [self.current_record]
         else:
             return []
 
     @property
@@ -1205,15 +1173,16 @@
     def on_change(self, fieldname, attr):
         self.current_record.on_change(fieldname, attr)
         self.display()
 
     def get_buttons(self):
         'Return active buttons for the current view'
         def is_active(record, button):
-            if button.attrs.get('type', 'class') == 'instance':
+            if (record.readonly
+                    or button.attrs.get('type', 'class') == 'instance'):
                 return False
             states = record.expr_eval(button.attrs.get('states', {}))
             return not (states.get('invisible') or states.get('readonly'))
 
         if not self.selected_records:
             return []
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/__init__.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/calendar_.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,29 +37,18 @@
         self.calendar_fields = []
 
     def _parse_calendar(self, node, attributes):
         for child in node.childNodes:
             self.parse(child)
         goocalendar = Calendar_(
             self.view.attributes, self.view, self.calendar_fields)
-        scrolledwindow = Gtk.ScrolledWindow()
-        scrolledwindow.add(goocalendar)
         toolbar = Toolbar(goocalendar)
-        self.view.widget.pack_start(
-            toolbar, expand=False, fill=False, padding=0)
-        self.view.widget.pack_start(
-            scrolledwindow, expand=True, fill=True, padding=0)
         self.view.widgets['goocalendar'] = goocalendar
         self.view.widgets['toolbar'] = toolbar
 
-        if attributes.get('height') or attributes.get('width'):
-            scrolledwindow.set_size_request(
-                int(attributes.get('width', -1)),
-                int(attributes.get('height', -1)))
-
     def _parse_field(self, node, attributes):
         self.calendar_fields.append(attributes)
 
 
 class ViewCalendar(View):
     editable = False
     creatable = False
@@ -81,14 +70,33 @@
         goocalendar.connect('page-changed', self.on_page_changed, toolbar)
         goocalendar.connect('event-pressed', self.on_event_pressed)
         goocalendar.connect('event-activated', self.on_event_activated)
         goocalendar.connect('event-released', self.on_event_released)
         goocalendar.connect('day-pressed', self.on_day_pressed)
         goocalendar.connect('day-activated', self.on_day_activated)
 
+        self.widget.pack_start(toolbar, expand=False, fill=False, padding=0)
+        vp = Gtk.Viewport()
+        vp.set_shadow_type(Gtk.ShadowType.NONE)
+        vp.add(goocalendar)
+        self.scroll = scroll = Gtk.ScrolledWindow()
+        scroll.add(vp)
+        scroll.set_policy(
+            Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
+        scroll.set_placement(Gtk.CornerType.TOP_LEFT)
+        viewport = Gtk.Viewport()
+        viewport.set_shadow_type(Gtk.ShadowType.ETCHED_IN)
+        viewport.add(scroll)
+        self.widget.pack_start(viewport, expand=True, fill=True, padding=0)
+
+        if self.attributes.get('height') or self.attributes.get('width'):
+            scroll.set_size_request(
+                int(self.attributes.get('width', -1)),
+                int(self.attributes.get('height', -1)))
+
     def on_page_changed(self, goocalendar, day, toolbar):
         toolbar.update_displayed_date()
         if goocalendar.update_domain():
             self.screen.search_filter()
 
     def on_view_changed(self, goocalendar, view, toolbar):
         toolbar.update_displayed_date()
@@ -166,7 +174,12 @@
         self.widgets['goocalendar'].display(self.group)
 
     def set_cursor(self, new=False, reset_view=True):
         pass
 
     def get_fields(self):
         return []
+
+    @property
+    def listed_records(self):
+        event_store = self.widgets['goocalendar'].event_store
+        return [e.record for e in event_store.get_events()]
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,36 +104,37 @@
         self.insert(next_year, -1)
 
         blank_widget = Gtk.ToolItem()
         blank_widget.set_expand(True)
         self.insert(blank_widget, -1)
 
         day_button = Gtk.RadioToolButton()
-        day_button.set_label(_('Day View'))
+        day_button.set_label(_("Day"))
         day_button.connect("clicked", self.on_day_button_clicked)
         day_button.add_accelerator(
             "clicked", self.accel_group, Gdk.KEY_d,
             Gdk.ModifierType.MODIFIER_MASK, Gtk.AccelFlags.VISIBLE)
-        self.insert(day_button, -1)
 
         week_button = Gtk.RadioToolButton.new_from_widget(day_button)
-        week_button.set_label(_('Week View'))
+        week_button.set_label(_("Week"))
         week_button.connect("clicked", self.on_week_button_clicked)
         week_button.add_accelerator(
             "clicked", self.accel_group, Gdk.KEY_w,
             Gdk.ModifierType.MODIFIER_MASK, Gtk.AccelFlags.VISIBLE)
-        self.insert(week_button, -1)
 
         month_button = Gtk.RadioToolButton.new_from_widget(week_button)
-        month_button.set_label_widget(Gtk.Label(label=_('Month View')))
+        month_button.set_label_widget(Gtk.Label(label=_("Month")))
         month_button.connect("clicked", self.on_month_button_clicked)
         month_button.add_accelerator(
             "clicked", self.accel_group, Gdk.KEY_m,
             Gdk.ModifierType.MODIFIER_MASK, Gtk.AccelFlags.VISIBLE)
+
         self.insert(month_button, -1)
+        self.insert(week_button, -1)
+        self.insert(day_button, -1)
         buttons = {
             'month': month_button,
             'week': week_button,
             'day': day_button,
             }
         buttons[self.goocalendar.view].set_active(True)
         self.update_displayed_date()
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,21 +275,26 @@
     def _parse_separator(self, node, attributes):
         name = attributes.get('name')
         if name and name == self.exclude_field:
             self.container.add(None, attributes)
             return
         vbox = VBox(attrs=attributes)
         if attributes.get('string'):
+            attributes.setdefault('xexpand', 0)
+            attributes.setdefault('xalign', 0)
+            attributes.setdefault('yalign', 0.5)
             label = Label(label=attributes['string'], attrs=attributes)
             label.set_halign(get_align(
-                    attributes.get('xalign', 0.0),
-                    bool(attributes.get('xexpand', True))))
+                    attributes['xalign'],
+                    bool(attributes.get('xexpand'))))
             label.set_valign(get_align(
-                    attributes.get('yalign', 0.5),
-                    bool(attributes.get('yexpand', False))))
+                    attributes['yalign'],
+                    bool(attributes.get('yexpand'))))
+            label.props.xalign = float(attributes['xalign'])
+            label.props.yalign = float(attributes['yalign'])
             vbox.pack_start(label, expand=True, fill=True, padding=0)
             self.view.state_widgets.append(label)
             if name:
                 self._mnemonics[name] = label
         vbox.pack_start(Gtk.HSeparator(), expand=True, fill=True, padding=0)
         self.view.state_widgets.append(vbox)
         self.container.add(vbox, attributes)
@@ -299,21 +304,25 @@
         if name and name == self.exclude_field:
             self.container.add(None, attributes)
             return
         if CONFIG['client.modepda']:
             attributes['xalign'] = 0.0
 
         attributes.setdefault('xexpand', 0)
+        attributes.setdefault('xalign', 1)
+        attributes.setdefault('yalign', 0.5)
         label = Label(label=attributes.get('string', ''), attrs=attributes)
         label.set_halign(get_align(
-                attributes.get('xalign', 1.0),
+                attributes['xalign'],
                 bool(attributes.get('xexpand'))))
         label.set_valign(get_align(
                 attributes.get('yalign', 0.5),
                 bool(attributes.get('yexpand'))))
+        label.props.xalign = float(attributes['xalign'])
+        label.props.yalign = float(attributes['yalign'])
         label.set_angle(int(attributes.get('angle', 0)))
         self.view.state_widgets.append(label)
         self.container.add(label, attributes)
         if name:
             self._mnemonics[name] = label
 
     def _parse_newline(self, node, attributes):
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/binary.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/binary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/calendar_.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/char.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/char.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/checkbox.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/dictionary.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/document.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/document.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/float.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/float.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/image.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/image.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/integer.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/integer.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/many2many.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2many.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
         tooltips.set_tip(self.but_add, _('Add existing record'))
         self.but_add.connect('clicked', self._sig_add)
         self.but_add.add(common.IconFactory.get_image(
                 'tryton-add', Gtk.IconSize.SMALL_TOOLBAR))
         self.but_add.set_relief(Gtk.ReliefStyle.NONE)
         hbox.pack_start(self.but_add, expand=False, fill=False, padding=0)
 
+        self.label = Gtk.Label(label='(_/0)')
+        hbox.pack_start(self.label, expand=False, fill=False, padding=0)
+
         self.but_remove = Gtk.Button(can_focus=False)
         tooltips.set_tip(self.but_remove, _('Remove selected record'))
         self.but_remove.connect('clicked', self._sig_remove)
         self.but_remove.add(common.IconFactory.get_image(
                 'tryton-remove', Gtk.IconSize.SMALL_TOOLBAR))
         self.but_remove.set_relief(Gtk.ReliefStyle.NONE)
         hbox.pack_start(self.but_remove, expand=False, fill=False, padding=0)
@@ -275,16 +278,22 @@
         self.but_add.set_sensitive(bool(
                 not self._readonly
                 and not size_limit))
         self.but_remove.set_sensitive(bool(
                 not self._readonly
                 and self._position))
 
-    def record_message(self, position, *args):
+    def record_message(self, position, size, *args):
         self._position = position
+        name = str(position) if position else '_'
+        selected = len(self.screen.selected_records)
+        if selected > 1:
+            name += '#%i' % selected
+        name = '(%s/%s)' % (name, common.humanize(size))
+        self.label.set_text(name)
         self._set_button_sensitive()
 
     def display(self):
         super(Many2Many, self).display()
         if not self.field:
             self.screen.new_group()
             self.screen.current_record = None
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/many2one.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2one.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from .widget import Widget
 
 _ = gettext.gettext
 
 
 class Many2One(Widget):
+    default_width_chars = 12
 
     def __init__(self, view, attrs):
         super(Many2One, self).__init__(view, attrs)
 
         self.widget = Gtk.HBox(spacing=0)
         self.widget.set_property('sensitive', True)
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/multiselection.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/one2many.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2many.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         tooltips.set_tip(self.but_pre, _('Previous'))
         self.but_pre.connect('clicked', self._sig_previous)
         self.but_pre.add(common.IconFactory.get_image(
                 'tryton-back', Gtk.IconSize.SMALL_TOOLBAR))
         self.but_pre.set_relief(Gtk.ReliefStyle.NONE)
         hbox.pack_start(self.but_pre, expand=False, fill=False, padding=0)
 
-        self.label = Gtk.Label(label='(0,0)')
+        self.label = Gtk.Label(label='(_/0)')
         hbox.pack_start(self.label, expand=False, fill=False, padding=0)
 
         self.but_next = Gtk.Button(can_focus=False)
         tooltips.set_tip(self.but_next, _('Next'))
         self.but_next.connect('clicked', self._sig_next)
         self.but_next.add(common.IconFactory.get_image(
                 'tryton-forward', Gtk.IconSize.SMALL_TOOLBAR))
@@ -507,20 +507,20 @@
             exclude_field=self.attrs.get('relation_field'))
         win.screen.search_filter(quote(text))
         win.show()
 
     def record_message(self, position, size, *args):
         self._position = position
         self._length = size
-        if self._position:
-            name = str(self._position)
-        else:
-            name = '_'
-        line = '(%s/%s)' % (name, self._length)
-        self.label.set_text(line)
+        name = str(position) if position else '_'
+        selected = len(self.screen.selected_records)
+        if selected > 1:
+            name += '#%i' % selected
+        name = '(%s/%s)' % (name, common.humanize(size))
+        self.label.set_text(name)
         self._set_button_sensitive()
 
     def display(self):
         super(One2Many, self).display()
 
         self._set_button_sensitive()
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/progressbar.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/pyson.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/reference.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/reference.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/richtextbox.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/selection.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/state_widget.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/textbox.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/textbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,14 @@
         textview = widget.get_children()[-1].get_child()
         textview.set_editable(not value)
         textview.props.sensitive = not value
 
     def _readonly_set(self, value):
         super(TextBox, self)._readonly_set(value)
         self.textview.set_editable(not value)
-        if self.button:
-            self.button.set_sensitive(not value)
 
     @property
     def modified(self):
         if self.record and self.field:
             return self.field.get_client(self.record) != self.get_value()
         return False
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/timedelta.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/url.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/url.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/form_gtk/widget.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tryton.gui.window.nomodal import NoModal
 
 _ = gettext.gettext
 
 
 class Widget(object):
     expand = False
-    default_width_chars = 25
+    default_width_chars = 8
 
     def __init__(self, view, attrs):
         super(Widget, self).__init__()
         self.view = view
         self.attrs = attrs
         self.widget = None
         self.mnemonic_widget = None
@@ -200,25 +200,23 @@
             widget = self.widget.translate_widget()
             label.set_mnemonic_widget(widget)
             self.widget.translate_widget_set(widget, fuzzy_value)
             self.widget.translate_widget_set_readonly(widget, True)
             widget.set_vexpand(self.widget.expand)
             widget.set_hexpand(True)
             grid.attach(widget, 1, i, 1, 1)
-            editing = Gtk.CheckButton()
+            editing = Gtk.ToggleButton(label=_("Edit"))
             editing.connect('toggled', self.editing_toggled, widget)
             editing.props.sensitive = not readonly
-            tooltips.set_tip(editing, _('Edit'))
             grid.attach(editing, 2, i, 1, 1)
-            fuzzy = Gtk.CheckButton()
-            fuzzy.set_active(value != fuzzy_value)
-            fuzzy.props.sensitive = False
-            tooltips.set_tip(fuzzy, _('Fuzzy'))
-            grid.attach(fuzzy, 4, i, 1, 1)
-            self.widgets[language['code']] = (widget, editing, fuzzy)
+            if value != fuzzy_value:
+                fuzzy = Gtk.Label(_("Fuzzy"))
+                widget_class(fuzzy, 'warning', True)
+                grid.attach(fuzzy, 4, i, 1, 1)
+            self.widgets[language['code']] = (widget, editing)
 
         tooltips.enable()
         vbox = Gtk.VBox()
         vbox.pack_start(grid, expand=self.widget.expand, fill=True, padding=0)
         viewport = Gtk.Viewport()
         viewport.set_shadow_type(Gtk.ShadowType.NONE)
         viewport.add(vbox)
@@ -237,15 +235,15 @@
     def editing_toggled(self, editing, widget):
         self.widget.translate_widget_set_readonly(widget,
             not editing.get_active())
 
     def response(self, win, response):
         if response == Gtk.ResponseType.OK:
             for code, widget in self.widgets.items():
-                widget, editing, fuzzy = widget
+                widget, editing = widget
                 if not editing.get_active():
                     continue
                 value = self.widget.translate_widget_get(widget)
                 context = dict(
                     language=code,
                     fuzzy_translation=False,
                     )
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/graph.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/bar.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/bar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/graph.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/line.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/line.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/graph_gtk/pie.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/pie.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/list.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/list.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/list_form.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/list_form.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from gi.repository import Gio, GObject, Gtk
+from gi.repository import Gio, GLib, GObject, Gtk
 
 from tryton.common import common
 
 from . import View
 from .form import ViewForm
 
 
@@ -115,14 +115,18 @@
 
     @property
     def selected_records(self):
         selected_rows = self.listbox.get_selected_rows()
         return [
             self._model.get_item(r.get_index()).record for r in selected_rows]
 
+    @property
+    def listed_records(self):
+        return list(self._model.group)
+
     def group_list_changed(self, group, action, *args):
         if action == 'record-added':
             record, position = args
             self._model.emit('items-changed', position, 0, 1)
             self._view_forms.insert(position, self._view_forms.pop())
         elif action == 'record-removed':
             record, position = args
@@ -131,25 +135,77 @@
 
     def set_cursor(self, new=False, reset_view=True):
         for idx, form in enumerate(self._view_forms):
             if form.record == self.record:
                 self._select_show_row(idx)
                 break
 
-    def _row_selected(self, listbox, row):
-        if not row:
+    def get_selected_paths(self):
+        return [[r.id] for r in self.selected_records]
+
+    def select_nodes(self, nodes):
+        if not nodes:
             return
-        self.record = self._model.get_item(row.get_index()).record
+        nodes = {n[0] for n in nodes}
+        self.listbox.handler_block_by_func(self.select_nodes)
+        self.listbox.unselect_all()
+        for idx, view_form in enumerate(self._view_forms):
+            if view_form.record.id in nodes:
+                row = self.listbox.get_row_at_index(idx)
+                if not row:
+                    continue
+                self.listbox.select_row(row)
+        self.listbox.handler_unblock_by_func(self.select_nodes)
+
+    def _row_selected(self, listbox, row):
+        previous_record = self.record
+        if (previous_record
+                and previous_record not in previous_record.group):
+            previous_record = None
+
+        if row:
+            self.record = self._model.get_item(row.get_index()).record
+        else:
+            self.record = None
+
+        def go_previous():
+            self.record = previous_record
+            self.set_cursor()
+
+        def save():
+            if not previous_record.destroyed:
+                if not previous_record.save():
+                    go_previous()
+
+        def pre_validate():
+            if not previous_record.destroyed:
+                if not previous_record.pre_validate():
+                    go_previous()
+
+        if previous_record and previous_record != self.record:
+            if not self.screen.parent:
+                if not previous_record.validate(self.get_fields()):
+                    go_previous()
+                    return True
+                GLib.idle_add(save)
+            elif self.screen.pre_validate:
+                GLib.idle_add(pre_validate)
 
     @common.idle_add
     def _select_show_row(self, index):
         # translate_coordinates requires that both widgets are realized
         if not self.listbox.get_realized():
             return
-        self.listbox.unselect_all()
+        # unselect_all triggers a loop in _row_selected if the record is not
+        # valid
+        self.listbox.handler_block_by_func(self._select_show_row)
+        try:
+            self.listbox.unselect_all()
+        finally:
+            self.listbox.handler_unblock_by_func(self._select_show_row)
         row = self.listbox.get_row_at_index(index)
         if not row or not row.get_realized():
             return
         self.listbox.select_row(row)
         y_position = row.translate_coordinates(self.listbox, 0, 0)[1]
         y_size = row.get_allocated_height()
         vadjustment = self.widget.get_vadjustment()
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/editabletree.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import gettext
+import logging
 from itertools import chain, cycle, islice
 
 from gi.repository import Gdk, GLib, Gtk
 
 from tryton.common import MODELACCESS
 from tryton.common.datetime_ import Date, Time
 
 _ = gettext.gettext
+logger = logging.getLogger(__name__)
 
 
 def focusable_cells(column, editable=True):
     for cell in column.get_cells():
         if (not editable
                 or (isinstance(cell, (
                             Gtk.CellRendererText,
@@ -47,15 +49,22 @@
             columns.reverse()
         current_idx = columns.index(column) + 1
         for column in islice(cycle(columns), current_idx,
                 len(columns) + current_idx):
             if not column.name:
                 continue
             widget = self.view.get_column_widget(column)
-            field = record[column.name]
+            try:
+                record.load(column.name, process_exception=False)
+            except Exception:
+                logger.error(
+                    f"Error loading '{column.name}' for {record}",
+                    exc_info=True)
+                return (None, None)
+            field = record.group.fields[column.name]
             field.state_set(record, states=('readonly', 'invisible'))
             invisible = field.get_state_attrs(record).get('invisible', False)
             if not column.get_visible():
                 invisible = True
             if editable:
                 readonly = widget.attrs.get('readonly',
                     field.get_state_attrs(record).get('readonly', False))
@@ -79,15 +88,16 @@
     leaving_record_events = (
         Gdk.KEY_Up, Gdk.KEY_Down, Gdk.KEY_Return)
     leaving_events = leaving_record_events + (
         Gdk.KEY_Tab, Gdk.KEY_ISO_Left_Tab, Gdk.KEY_KP_Enter)
 
     def on_quit_cell(
             self, current_record, column, renderer, value, callback=None):
-        field = current_record[column.name]
+        current_record.load(column.name, process_exception=False)
+        field = current_record.group.fields[column.name]
         widget = self.view.get_column_widget(column)
 
         # The value has not changed and is valid ... do nothing.
         if value == widget.get_textual_value(current_record) \
                 and field.validate(current_record):
             if callback:
                 callback()
@@ -267,15 +277,15 @@
                 else:
                     entry.set_active_text(value)
                 entry.handler_unblock(entry.editing_done_id)
             self.on_open_remote(record, column,
                 create=(event.keyval == Gdk.KEY_F3), value=value,
                 callback=callback)
         else:
-            field = record[column.name]
+            field = record.group.fields[column.name]
             if isinstance(entry, Gtk.Entry):
                 entry.set_max_length(int(field.attrs.get('size', 0)))
             record.modified_fields.setdefault(column.name)
             return False
 
         return True
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/list_gtk/widget.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 import gettext
+import logging
 import os
 import webbrowser
 from functools import partial, wraps
 from weakref import WeakKeyDictionary
 
 from gi.repository import Gdk, GLib, Gtk
 
@@ -27,14 +28,15 @@
     PopdownMixin, SelectionMixin, selection_shortcuts)
 from tryton.config import CONFIG
 from tryton.gui.window.view_form.screen import Screen
 from tryton.gui.window.win_form import WinForm
 from tryton.gui.window.win_search import WinSearch
 
 _ = gettext.gettext
+logger = logging.getLogger(__name__)
 
 COLORS = {n: v for n, v in zip(
         ['muted', 'success', 'warning', 'danger'],
         CONFIG['tree.colors'].split(','))}
 
 
 def send_keys(renderer, editable, position, treeview):
@@ -46,14 +48,31 @@
             # "changed" signal is also triggered by text editing
             # so only trigger editing-done if a row is active
             if combobox.get_active_iter():
                 treeview.on_editing_done(combobox, renderer)
         editable.connect('changed', changed)
 
 
+def catch_errors(error_value=_('#ERROR')):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(self, record):
+            if record.exception:
+                return error_value
+            try:
+                return func(self, record)
+            except Exception:
+                logger.error(
+                    f"Error calling {func.__name__} for {self} with {record}",
+                    exc_info=True)
+                return error_value
+        return wrapper
+    return decorator
+
+
 def realized(func):
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         has_been_realized = _REALIZED.get(self.view.treeview, False)
         if not has_been_realized:
             has_been_realized = self.view.treeview.get_realized()
@@ -139,15 +158,15 @@
         field = record.group.fields[self.attrs['name']]
         return record, field
 
     def _get_record_field_from_iter(self, iter_, store=None):
         if not store:
             store = self.view.treeview.get_model()
         record = store.get_value(iter_, 0)
-        field = record[self.attrs['name']]
+        field = record.group.fields[self.attrs['name']]
         return record, field
 
     def _set_visual(self, cell, record):
         visual = record.expr_eval(self.attrs.get('visual'))
         if not visual:
             visual = record.expr_eval(self.view.attributes.get('visual'))
         background = COLORS.get(visual) if visual != 'muted' else None
@@ -326,17 +345,17 @@
                 cell.set_property('activatable', False)
         self._set_visual(cell, record)
 
     def open_remote(self, record, create, changed=False, text=None,
             callback=None):
         raise NotImplementedError
 
+    @catch_errors()
     def get_textual_value(self, record):
-        if not record:
-            return ''
+        record.load(self.attrs['name'], process_exception=False)
         return record[self.attrs['name']].get_client(record)
 
     def value_from_text(self, record, text, callback=None):
         field = record[self.attrs['name']]
         field.set_client(record, text)
         if callback:
             callback()
@@ -392,17 +411,17 @@
 
     @property
     def suffixes(self):
         if self.symbol:
             return [self.renderer_suffix]
         return []
 
+    @catch_errors()
     def get_textual_value(self, record):
-        if not record:
-            return ''
+        record.load(self.attrs['name'], process_exception=False)
         return record[self.attrs['name']].get_client(
             record, factor=self.factor, grouping=self.grouping)
 
     def value_from_text(self, record, text, callback=None):
         field = record[self.attrs['name']]
         field.set_client(record, text, factor=self.factor)
         if callback:
@@ -460,17 +479,17 @@
 
     def get_format(self, record, field):
         if field and record:
             return field.date_format(record)
         else:
             return '%x'
 
+    @catch_errors()
     def get_textual_value(self, record):
-        if not record:
-            return ''
+        record.load(self.attrs['name'], process_exception=False)
         value = record[self.attrs['name']].get_client(record)
         if value:
             return value.strftime(self.renderer.props.format)
         else:
             return ''
 
 
@@ -483,17 +502,17 @@
 
     def get_format(self, record, field):
         if field and record:
             return field.time_format(record)
         else:
             return '%X'
 
+    @catch_errors()
     def get_textual_value(self, record):
-        if not record:
-            return ''
+        record.load(self.attrs['name'], process_exception=False)
         value = record[self.attrs['name']].get_client(record)
         if value is not None:
             if isinstance(value, datetime.datetime):
                 value = value.time()
             return value.strftime(self.renderer.props.format)
         else:
             return ''
@@ -545,15 +564,17 @@
     def prefixes(self):
         return filter(None, [self.renderer_open])
 
     @property
     def suffixes(self):
         return [self.renderer_save, self.renderer_select]
 
+    @catch_errors()
     def get_textual_value(self, record):
+        record.load(self.attrs['name'], process_exception=False)
         field = record[self.attrs['name']]
         if hasattr(field, 'get_size'):
             size = field.get_size(record)
         else:
             size = len(field.get(record))
         return common.humanize(size, 'B') if size else ''
 
@@ -600,14 +621,19 @@
     def attrs(self):
         return self.binary.attrs
 
     @property
     def view(self):
         return self.binary.view
 
+    @catch_errors(False)
+    def _fetch_data(self, record):
+        record.fetch(self.attrs['name'], process_exception=False)
+        return True
+
 
 class _BinarySave(_BinaryIcon):
     icon_name = 'tryton-save'
 
     def __init__(self, binary):
         super().__init__(binary)
         pixbuf = common.IconFactory.get_pixbuf(
@@ -627,14 +653,17 @@
             with open(filename, 'wb') as fp:
                 fp.write(self.binary.get_data(record, field))
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         record, field = self._get_record_field_from_iter(iter_, store)
+        if not self._fetch_data(record):
+            cell.set_property('visible', False)
+            return
         if hasattr(field, 'get_size'):
             size = field.get_size(record)
         else:
             size = len(field.get(record))
         field.state_set(record, states=['invisible'])
         invisible = field.get_state_attrs(record).get('invisible', False)
         cell.set_property('visible', not invisible and size)
@@ -667,14 +696,17 @@
                             record, os.path.basename(filename))
             GLib.idle_add(_select)
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         record, field = self._get_record_field_from_iter(iter_, store)
+        if not self._fetch_data(record):
+            cell.set_property('visible', False)
+            return
         if hasattr(field, 'get_size'):
             size = field.get_size(record)
         else:
             size = len(field.get(record))
         if size:
             icon = 'tryton-clear'
         else:
@@ -706,14 +738,17 @@
         GLib.idle_add(file_open, file_path, type_)
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         super().setter(column, cell, store, iter_)
         record, field = self._get_record_field_from_iter(iter_, store)
+        if not self._fetch_data(record):
+            cell.set_property('visible', False)
+            return
         filename_field = record.group.fields.get(self.attrs.get('filename'))
         filename = filename_field.get(record)
         if not filename:
             cell.set_property('visible', False)
 
 
 class Image(GenericText):
@@ -727,30 +762,41 @@
         self.width = int(attrs.get('width', 300))
         self.renderer.set_fixed_size(self.width, self.height)
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         record, field = self._get_record_field_from_iter(iter_, store)
+        value = self._get_data(record)
+        if value is None:
+            cell.set_property('pixbuf', None)
+            return
+        pixbuf = data2pixbuf(value)
+        if pixbuf:
+            pixbuf = common.resize_pixbuf(pixbuf, self.width, self.height)
+        cell.set_property('pixbuf', pixbuf)
+        self._set_visual(cell, record)
+
+    @catch_errors(None)
+    def _get_data(self, record):
+        record.load(self.attrs['name'], process_exception=False)
+        field = record[self.attrs['name']]
         value = field.get_client(record)
         if isinstance(value, int):
             if value > CONFIG['image.max_size']:
                 value = None
             else:
                 value = field.get_data(record)
-        pixbuf = data2pixbuf(value)
-        if pixbuf:
-            pixbuf = common.resize_pixbuf(pixbuf, self.width, self.height)
-        cell.set_property('pixbuf', pixbuf)
-        self._set_visual(cell, record)
+        return value
 
+    @catch_errors()
     def get_textual_value(self, record):
-        if not record:
-            return ''
-        return str(record[self.attrs['name']].get_size(record))
+        record.load(self.attrs['name'], process_exception=False)
+        field = record[self.attrs['name']]
+        return str(field.get_size(record))
 
 
 class M2O(GenericText):
 
     def __init__(self, view, attrs, renderer=None):
         if renderer is None and int(attrs.get('completion', 1)):
             renderer = partial(CellRendererTextCompletion, self.set_completion)
@@ -970,17 +1016,19 @@
 class O2O(M2O):
     pass
 
 
 class O2M(GenericText):
     align = 0.5
 
+    @catch_errors()
     def get_textual_value(self, record):
-        return '( ' + str(len(record[self.attrs['name']]
-                .get_eval(record))) + ' )'
+        record.load(self.attrs['name'], process_exception=False)
+        field = record[self.attrs['name']]
+        return '( ' + str(len(field.get_eval(record))) + ' )'
 
     def value_from_text(self, record, text, callback=None):
         if callback:
             callback()
 
     def open_remote(self, record, create=True, changed=False, text=None,
             callback=None):
@@ -1041,24 +1089,32 @@
 
 class Selection(GenericText, SelectionMixin, PopdownMixin):
 
     def __init__(self, *args, **kwargs):
         if 'renderer' not in kwargs:
             kwargs['renderer'] = CellRendererCombo
         super(Selection, self).__init__(*args, **kwargs)
-        self.init_selection()
-        # Use a variable let Python holding reference when calling set_property
-        model = self.get_popdown_model(self.selection)[0]
-        self.renderer.set_property('model', model)
-        self.renderer.set_property('text-column', 0)
+        if self.view and self.view.editable:
+            self.init_selection()
+            # Use a variable let Python holding reference when calling
+            # set_property
+            model = self.get_popdown_model(self.selection)[0]
+            self.renderer.set_property('model', model)
+            self.renderer.set_property('text-column', 0)
 
     def get_value(self, record, field):
         return field.get(record)
 
+    @catch_errors()
     def get_textual_value(self, record):
+        related = self.attrs['name'] + ':string'
+        if not self.view.editable and related in record.value:
+            return record.value[related]
+
+        record.load(self.attrs['name'], process_exception=False)
         field = record[self.attrs['name']]
         self.update_selection(record, field)
         value = self.get_value(record, field)
         text = dict(self.selection).get(value, '')
         if value and not text:
             text = self.get_inactive_selection(value)
         return text
@@ -1115,27 +1171,34 @@
         return False
 
 
 class MultiSelection(GenericText, SelectionMixin):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.init_selection()
+        if self.view and self.view.editable:
+            self.init_selection()
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         super().setter(column, cell, store, iter_, user_data=user_data)
         cell.set_property('editable', False)
 
     def value_from_text(self, record, text, callback=None):
         if callback:
             callback()
 
+    @catch_errors()
     def get_textual_value(self, record):
+        related = self.attrs['name'] + ':string'
+        if not self.view.editable and related in record.value:
+            return ";".join(record.value[related])
+
+        record.load(self.attrs['name'], process_exception=False)
         field = record[self.attrs['name']]
         self.update_selection(record, field)
         selection = dict(self.selection)
         values = []
         for value in field.get_eval(record):
             text = selection.get(value, '')
             values.append(text)
@@ -1176,14 +1239,15 @@
             str_ = ''
         return model, (id_, str_)
 
     def id_from_value(self, value):
         _, value = value.split(',')
         return int(value)
 
+    @catch_errors()
     def get_textual_value(self, record):
         value = super().get_textual_value(record)
         if value:
             model, value = value
         else:
             value = ''
         return value
@@ -1217,16 +1281,19 @@
         super().__init__(view, attrs)
         self.renderer.props.editable = False
 
     def setter(self, column, cell, store, iter_, user_data=None):
         super().setter(column, cell, store, iter_, user_data=None)
         cell.props.editable = False
 
+    @catch_errors()
     def get_textual_value(self, record):
-        return '(%s)' % len(record[self.attrs['name']].get_client(record))
+        record.load(self.attrs['name'], process_exception=False)
+        field = record[self.attrs['name']]
+        return '(%s)' % len(field.get_client(record))
 
 
 class ProgressBar(Cell):
     align = 0.5
     orientations = {
         'left_to_right': (Gtk.Orientation.HORIZONTAL, False),
         'right_to_left': (Gtk.Orientation.HORIZONTAL, True),
@@ -1260,16 +1327,19 @@
         cell.set_property('value', value * 100)
         self._set_visual(cell, record)
 
     def open_remote(self, record, create, changed=False, text=None,
             callback=None):
         raise NotImplementedError
 
+    @catch_errors()
     def get_textual_value(self, record):
-        return record[self.attrs['name']].get_client(record, factor=100) or ''
+        record.load(self.attrs['name'], process_exception=False)
+        field = record[self.attrs['name']]
+        return field.get_client(record, factor=100) or ''
 
     def value_from_text(self, record, text, callback=None):
         field = record[self.attrs['name']]
         field.set_client(record, float(text))
         if callback:
             callback()
```

### Comparing `tryton-6.6.7/tryton/gui/window/view_form/view/screen_container.py` & `tryton-6.8.0/tryton/gui/window/view_form/view/screen_container.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/win_csv.py` & `tryton-6.8.0/tryton/gui/window/win_csv.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/win_export.py` & `tryton-6.8.0/tryton/gui/window/win_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,44 +367,48 @@
                 except RPCException:
                     data = []
 
             if self.saveas.get_active():
                 fname = common.file_selection(_('Save As...'),
                         action=Gtk.FileChooserAction.SAVE)
                 if fname:
-                    self.export_csv(fname, data, paths)
+                    self.export_csv(fname, data, paths, header=header)
             else:
                 fileno, fname = tempfile.mkstemp(
                     '.csv', common.slugify(self.name) + '_')
-                if self.export_csv(fname, data, paths, popup=False):
+                if self.export_csv(
+                        fname, data, paths, popup=False, header=header):
                     os.close(fileno)
                     common.file_open(fname, 'csv')
                 else:
                     os.close(fileno)
         self.destroy()
 
-    def export_csv(self, fname, data, paths, popup=True):
+    def export_csv(self, fname, data, paths, popup=True, header=False):
         encoding = self.csv_enc.get_active_text() or 'utf_8_sig'
         locale_format = self.csv_locale.get_active()
 
         try:
             writer = csv.writer(
                 open(fname, 'w', encoding=encoding, newline=''),
                 quotechar=self.get_quotechar(),
                 delimiter=self.get_delimiter())
             for row, path in zip_longest(data, paths or []):
                 indent = len(path) - 1 if path else 0
                 if row:
                     writer.writerow(self.format_row(
                             row, indent=indent, locale_format=locale_format))
             if popup:
-                if len(data) == 1:
-                    common.message(_('%d record saved.') % len(data))
+                size = len(data)
+                if header:
+                    size -= 1
+                if size <= 1:
+                    common.message(_('%d record saved.') % size)
                 else:
-                    common.message(_('%d records saved.') % len(data))
+                    common.message(_('%d records saved.') % size)
             return True
         except (IOError, UnicodeEncodeError, csv.Error) as exception:
             common.warning(str(exception), _('Export failed'))
             return False
 
     @classmethod
     def format_row(cls, line, indent=0, locale_format=True):
```

### Comparing `tryton-6.6.7/tryton/gui/window/win_form.py` & `tryton-6.8.0/tryton/gui/window/win_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 _ = gettext.gettext
 
 
 class WinForm(NoModal, InfoBar):
     "Form window"
 
-    def __init__(self, screen, callback, view_type='form',
+    def __init__(self, screen, callback=None, view_type='form',
             new=False, many=0, domain=None, context=None,
             save_current=False, title='', rec_name=None):
         tooltips = common.Tooltips()
         NoModal.__init__(self)
         self.screen = screen
         self.callback = callback
         self.many = many
@@ -341,15 +341,15 @@
 
         win = WinSearch(model_name, callback, sel_multi=True,
             context=self.context, domain=domain)
         win.screen.search_filter(quote(value))
         win.show()
 
     def record_message(self, position, size, *args):
-        self.activate_save()
+        self.set_buttons_sensitive()
         if self.view_type != 'tree':
             return
         name = '_'
         access = common.MODELACCESS[self.screen.model_name]
         deletable = True
         if self.screen.current_record:
             deletable = self.screen.current_record.deletable
@@ -376,18 +376,18 @@
             self.but_pre.set_sensitive(False)
             if self.domain is not None:
                 self.but_remove.set_sensitive(False)
         line = '(%s/%s)' % (name, position)
         self.label.set_text(line)
 
     def record_modified(self, *args):
-        self.activate_save()
+        self.set_buttons_sensitive()
         self.info_bar_refresh()
 
-    def activate_save(self):
+    def set_buttons_sensitive(self):
         modified = self.screen.modified()
         # Keep sensible as change could have been trigger by a Many2One edition
         sensitive = modified or self.but_ok.props.sensitive
         self.but_ok.props.sensitive = sensitive
         self.win.set_default_response(
             Gtk.ResponseType.OK if sensitive else Gtk.ResponseType.CANCEL)
 
@@ -444,15 +444,16 @@
                 record.reload()
                 record.set_modified()
             if added:
                 record.modified_fields.setdefault('id')
             result = False
         else:
             result = response_id not in cancel_responses
-        self.callback(result)
+        if self.callback:
+            self.callback(result)
         self.destroy()
 
     def new(self):
         self.screen.new()
         self._initial_value = None
         self.screen.current_view.display()
         self.screen.set_cursor(new=True)
```

### Comparing `tryton-6.6.7/tryton/gui/window/win_import.py` & `tryton-6.8.0/tryton/gui/window/win_import.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/win_search.py` & `tryton-6.8.0/tryton/gui/window/win_search.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/window.py` & `tryton-6.8.0/tryton/gui/window/window.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/gui/window/wizard.py` & `tryton-6.8.0/tryton/gui/window/wizard.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/jsonrpc.py` & `tryton-6.8.0/tryton/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/plugins/__init__.py` & `tryton-6.8.0/tryton/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/plugins/translation/__init__.py` & `tryton-6.8.0/tryton/plugins/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/pyson.py` & `tryton-6.8.0/tryton/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/rpc.py` & `tryton-6.8.0/tryton/rpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,48 +41,47 @@
 
 context_reset()
 
 
 def db_list(host, port):
     try:
         connection = ServerProxy(host, port)
-        logging.getLogger(__name__).info('common.db.list()')
+        logger.info('common.db.list()')
         result = connection.common.db.list()
-        logging.getLogger(__name__).debug(repr(result))
+        logger.debug('%r', result)
         return result
     except Fault as exception:
-        logging.getLogger(__name__).debug(exception.faultCode)
+        logger.debug(exception.faultCode)
         if exception.faultCode == str(HTTPStatus.FORBIDDEN.value):
             return []
         else:
             return None
 
 
 def server_version(host, port):
     try:
         connection = ServerProxy(host, port)
-        logging.getLogger(__name__).info(
-            'common.server.version(None, None)')
+        logger.info('common.server.version(None, None)')
         result = connection.common.server.version()
-        logging.getLogger(__name__).debug(repr(result))
+        logger.debug('%r', result)
         return result
     except Exception as e:
-        logging.getLogger(__name__).error(e)
+        logger.exception(e)
         return None
 
 
 def authentication_services(host, port):
     try:
         connection = ServerProxy(host, port)
         logger.info('common.authentication.services()')
         services = connection.common.authentication.services()
-        logger.debug(repr(services))
+        logger.debug('%r', services)
         return connection.url, services
     except Exception as e:
-        logger.error(e)
+        logger.exception(e)
         return '', []
 
 
 def set_service_session(parameters):
     from tryton import common
     global CONNECTION, _USER
     host = CONFIG['login.host']
@@ -115,33 +114,32 @@
     hostname = common.get_hostname(host)
     port = common.get_port(host)
     database = CONFIG['login.db']
     username = CONFIG['login.login']
     language = CONFIG['client.lang']
     parameters['device_cookie'] = device_cookie.get()
     connection = ServerProxy(hostname, port, database)
-    logging.getLogger(__name__).info('common.db.login(%s, %s, %s)'
-        % (username, 'x' * 10, language))
+    logger.info('common.db.login(%s, %s, %s)', username, 'x' * 10, language)
     result = connection.common.db.login(username, parameters, language)
-    logging.getLogger(__name__).debug(repr(result))
+    logger.debug('%r', result)
     _USER = result[0]
     session = ':'.join(map(str, [username] + result))
     if CONNECTION is not None:
         CONNECTION.close()
     CONNECTION = ServerPool(
         hostname, port, database, session=session, cache=not CONFIG['dev'])
     device_cookie.renew()
     bus.listen(CONNECTION)
 
 
 def logout():
     global CONNECTION, _USER
     if CONNECTION is not None:
         try:
-            logging.getLogger(__name__).info('common.db.logout()')
+            logger.info('common.db.logout()')
             with CONNECTION() as conn:
                 conn.common.db.logout()
         except (Fault, socket.error, http.client.CannotSendRequest):
             pass
         CONNECTION.close()
         CONNECTION = None
     _USER = None
@@ -150,19 +148,19 @@
 def execute(*args):
     global CONNECTION, _USER
     if CONNECTION is None:
         raise TrytonServerError('403')
     try:
         name = '.'.join(args[:3])
         args = args[3:]
-        logging.getLogger(__name__).info('%s%s' % (name, args))
+        logger.info('%s%r', name, args)
         with CONNECTION() as conn:
             result = getattr(conn, name)(*args)
     except (http.client.CannotSendRequest, socket.error) as exception:
         raise TrytonServerUnavailable(*exception.args)
-    logging.getLogger(__name__).debug(repr(result))
+    logger.debug('%r', result)
     return result
 
 
 def clear_cache(prefix=None):
     if CONNECTION:
         CONNECTION.clear_cache(prefix)
```

### Comparing `tryton-6.6.7/tryton/tests/test_common_domain_parser.py` & `tryton-6.8.0/tryton/tests/test_common_domain_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,39 +525,39 @@
         a = ('a', 'a', 'a')
         b = ('b', 'b', 'b')
         c = ('c', 'c', 'c')
         null_ = ('d', None, 'x')
         double_null_ = ('e', None, None)
         for value, result in (
                 (['a'], ['a']),
-                (['a', 'or', 'b'], [['OR', 'a', 'b']]),
-                (['a', 'or', 'b', 'or', 'c'], [['OR', ['OR', 'a', 'b'], 'c']]),
-                (['a', 'b', 'or', 'c'], ['a', ['OR', 'b', 'c']]),
-                (['a', 'or', 'b', 'c'], [['OR', 'a', 'b'], 'c']),
+                (['a', '|', 'b'], [['OR', 'a', 'b']]),
+                (['a', '|', 'b', '|', 'c'], [['OR', ['OR', 'a', 'b'], 'c']]),
+                (['a', 'b', '|', 'c'], ['a', ['OR', 'b', 'c']]),
+                (['a', '|', 'b', 'c'], [['OR', 'a', 'b'], 'c']),
                 (['a', iter(['b', 'c'])], ['a', ['b', 'c']]),
                 (['a', iter(['b', 'c']), 'd'], ['a', ['b', 'c'], 'd']),
-                (['a', 'or', iter(['b', 'c'])], [['OR', 'a', ['b', 'c']]]),
-                (['a', 'or', iter(['b', 'c']), 'd'],
+                (['a', '|', iter(['b', 'c'])], [['OR', 'a', ['b', 'c']]]),
+                (['a', '|', iter(['b', 'c']), 'd'],
                     [['OR', 'a', ['b', 'c']], 'd']),
-                (['a', iter(['b', 'c']), 'or', 'd'],
+                (['a', iter(['b', 'c']), '|', 'd'],
                     ['a', ['OR', ['b', 'c'], 'd']]),
-                (['a', 'or', iter(['b', 'or', 'c'])],
+                (['a', '|', iter(['b', '|', 'c'])],
                     [['OR', 'a', [['OR', 'b', 'c']]]]),
-                (['or'], []),
-                (['or', 'a'], ['a']),
-                (['a', iter(['or', 'b'])], ['a', ['b']]),
-                (['a', 'or', 'or', 'b'], [['OR', 'a', 'b']]),
-                (['or', 'or', 'a'], ['a']),
-                (['or', 'or', 'a', 'b'], ['a', 'b']),
-                (['or', 'or', 'a', 'or', 'b'], [['OR', 'a', 'b']]),
-                (['a', iter(['b', 'or', 'c'])], ['a', [['OR', 'b', 'c']]]),
-                ([a, iter([b, ('or',), c])], [a, [['OR', b, c]]]),
-                (['a', iter(['b', 'or'])], ['a', [['OR', 'b']]]),
+                (['|'], []),
+                (['|', 'a'], ['a']),
+                (['a', iter(['|', 'b'])], ['a', ['b']]),
+                (['a', '|', '|', 'b'], [['OR', 'a', 'b']]),
+                (['|', '|', 'a'], ['a']),
+                (['|', '|', 'a', 'b'], ['a', 'b']),
+                (['|', '|', 'a', '|', 'b'], [['OR', 'a', 'b']]),
+                (['a', iter(['b', '|', 'c'])], ['a', [['OR', 'b', 'c']]]),
+                ([a, iter([b, ('|',), c])], [a, [['OR', b, c]]]),
+                (['a', iter(['b', '|'])], ['a', [['OR', 'b']]]),
                 ([null_], [null_]),
-                ([null_, 'or', double_null_], [['OR', null_, double_null_]]),
+                ([null_, '|', double_null_], [['OR', null_, double_null_]]),
                 ):
             self.assertEqual(
                 rlist(operatorize(iter(value))), result,
                 msg="operatorize(%r)" % value)
 
     def test_stringable(self):
         "Test stringable"
@@ -692,22 +692,22 @@
                 ('name', 'ilike', '%Doe%'),
                 ('name', 'ilike', '%Jane%')]),
             'Name: Doe Name: Jane')
         self.assertEqual(
             dom.string(['OR',
                 ('name', 'ilike', '%Doe%'),
                 ('name', 'ilike', '%Jane%')]),
-            'Name: Doe or Name: Jane')
+            'Name: Doe | Name: Jane')
         self.assertEqual(
             dom.string([
                 ('name', 'ilike', '%Doe%'),
                 ['OR',
                     ('name', 'ilike', '%John%'),
                     ('name', 'ilike', '%Jane%')]]),
-            'Name: Doe (Name: John or Name: Jane)')
+            'Name: Doe (Name: John | Name: Jane)')
         self.assertEqual(dom.string([]), '')
         self.assertEqual(
             dom.string([('surname', 'ilike', '%Doe%')]), '"(Sur)Name": Doe')
         self.assertEqual(
             dom.string([('date', '>=', dt.date(2012, 10, 24))]),
             dt.date(2012, 10, 24).strftime('Date: >=%x'))
         self.assertEqual(dom.string([('selection', '=', '')]), 'Selection: ')
@@ -1117,18 +1117,18 @@
         self.assertEqual(list(dom.completion('Nam')), ['Name: '])
         self.assertEqual(list(dom.completion('Name:')), ['Name: '])
         self.assertEqual(list(dom.completion('Name: foo')), [])
         self.assertEqual(list(dom.completion('Name: !=')), [])
         self.assertEqual(list(dom.completion('Name: !=foo')), [])
         self.assertEqual(list(dom.completion('')), ['Name: '])
         self.assertEqual(list(dom.completion(' ')), ['', 'Name: '])
-        self.assertEqual(list(dom.completion('Name: foo or')), ['Name: foo'])
+        self.assertEqual(list(dom.completion('Name: foo |')), ['Name: foo'])
         self.assertEqual(
-            list(dom.completion('Name: foo (Name: foo or N')),
-            ['Name: foo (Name: foo or Name: '])
+            list(dom.completion('Name: foo (Name: foo | N')),
+            ['Name: foo (Name: foo | Name: '])
 
     def test_completion_many2one(self):
         "Test completion many2one"
         dom = DomainParser({
                 'relation': {
                     'name': 'relation',
                     'string': "Relation",
```

### Comparing `tryton-6.6.7/tryton/tests/test_common_selection.py` & `tryton-6.8.0/tryton/tests/test_common_selection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/tests/test_common_timedelta.py` & `tryton-6.8.0/tryton/tests/test_common_timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton/translate.py` & `tryton-6.8.0/tryton/translate.py`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton.desktop` & `tryton-6.8.0/tryton.desktop`

 * *Files identical despite different names*

### Comparing `tryton-6.6.7/tryton.egg-info/PKG-INFO` & `tryton-6.8.0/tryton.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 6.6.7
+Version: 6.8.0
 Summary: Tryton desktop client
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
-Project-URL: Source Code, https://hg.tryton.org/tryton
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: business application ERP
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -38,20 +38,20 @@
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Japanese
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: calendar
 License-File: LICENSE
 
 tryton
 ======
 
 The desktop client of Tryton.
```

### Comparing `tryton-6.6.7/tryton.egg-info/SOURCES.txt` & `tryton-6.8.0/tryton.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 tryton/data/pixmaps/tryton/tryton-format-bold.svg
 tryton/data/pixmaps/tryton/tryton-format-color-text.svg
 tryton/data/pixmaps/tryton/tryton-format-italic.svg
 tryton/data/pixmaps/tryton/tryton-format-underline.svg
 tryton/data/pixmaps/tryton/tryton-forward.svg
 tryton/data/pixmaps/tryton/tryton-history.svg
 tryton/data/pixmaps/tryton/tryton-icon.png
+tryton/data/pixmaps/tryton/tryton-icon.svg
 tryton/data/pixmaps/tryton/tryton-import.svg
 tryton/data/pixmaps/tryton/tryton-info.svg
 tryton/data/pixmaps/tryton/tryton-launch.svg
 tryton/data/pixmaps/tryton/tryton-link.svg
 tryton/data/pixmaps/tryton/tryton-log.svg
 tryton/data/pixmaps/tryton/tryton-menu.svg
 tryton/data/pixmaps/tryton/tryton-note.svg
@@ -194,14 +195,15 @@
 tryton/gui/window/attachment.py
 tryton/gui/window/board.py
 tryton/gui/window/dblogin.py
 tryton/gui/window/email_.py
 tryton/gui/window/form.py
 tryton/gui/window/infobar.py
 tryton/gui/window/limit.py
+tryton/gui/window/log.py
 tryton/gui/window/nomodal.py
 tryton/gui/window/note.py
 tryton/gui/window/preference.py
 tryton/gui/window/revision.py
 tryton/gui/window/tabcontent.py
 tryton/gui/window/win_csv.py
 tryton/gui/window/win_export.py
@@ -263,12 +265,13 @@
 tryton/gui/window/view_form/view/graph_gtk/pie.py
 tryton/gui/window/view_form/view/list_gtk/__init__.py
 tryton/gui/window/view_form/view/list_gtk/editabletree.py
 tryton/gui/window/view_form/view/list_gtk/widget.py
 tryton/plugins/__init__.py
 tryton/plugins/translation/__init__.py
 tryton/tests/__init__.py
+tryton/tests/test_common.py
 tryton/tests/test_common_domain_parser.py
 tryton/tests/test_common_selection.py
 tryton/tests/test_common_timedelta.py
 win32/gtk-3.0/gdk-pixbuf.loaders
 win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-6.6.7/win32/gtk-3.0/gdk-pixbuf.loaders` & `tryton-6.8.0/win32/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

