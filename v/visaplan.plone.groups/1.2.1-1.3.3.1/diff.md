# Comparing `tmp/visaplan.plone.groups-1.2.1.tar.gz` & `tmp/visaplan.plone.groups-1.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.plone.groups-1.2.1.tar", last modified: Tue Jan 12 15:40:35 2021, max compression
+gzip compressed data, was "dist/visaplan.plone.groups-1.3.3.1.tar", last modified: Wed May  3 14:48:10 2023, max compression
```

## Comparing `visaplan.plone.groups-1.2.1.tar` & `visaplan.plone.groups-1.3.3.1.tar`

### file list

```diff
@@ -1,97 +1,115 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-08-27 14:33:33.000000 visaplan.plone.groups-1.2.1/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      674 2018-08-27 14:38:07.000000 visaplan.plone.groups-1.2.1/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       86 2018-08-27 14:37:58.000000 visaplan.plone.groups-1.2.1/docs/index.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/sql/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      294 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/sql/update-0001.sql
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      261 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      965 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/ajax.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8277 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/board.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24771 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/browser.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      800 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      314 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/crumbs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      605 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/fullpage.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7655 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/new-thread.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4641 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/oldcrumbs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9782 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/thread-reply.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      960 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/utils.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9164 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/ajax.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24062 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/browser.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1346 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      316 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/crumbs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6500 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/fullpage.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3494 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/gdmacros.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1760 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/group_administration_learning_progress_view.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3711 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/group_administration_user_view.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2668 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/group_administration_view.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7293 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/oldcrumbs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      234 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-animations.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13484 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-articles.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-audios.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      243 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-binaries.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      231 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-courses.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      327 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-events.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      232 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-formulas.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      260 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-glossaries.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      792 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-images.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      235 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-literatures.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      229 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-news.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-standards.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-tables.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-videos.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1041 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/utils.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1193 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/update-0001.sql
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      279 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/update-0002.sql
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2046 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/update-0003.sql
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      431 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/ajax.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   113033 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/browser.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1693 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/cache.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      585 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1895 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/configure_groupsharing.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      311 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/fullpage.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    15337 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/utils.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/resource/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1942 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/resource/group-desktop.js
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2679 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/browser.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      364 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11011 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/utils.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       62 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      523 2020-08-27 13:15:15.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/ajax.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      272 2020-06-09 22:53:22.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      440 2020-08-27 13:15:15.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/fullpage.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    49460 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/group-desktop.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       70 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      433 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.2.1/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9723 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3794 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-09-13 07:22:08.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      133 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4273 2021-01-12 15:40:30.000000 visaplan.plone.groups-1.2.1/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-08-27 14:33:33.000000 visaplan.plone.groups-1.2.1/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-02-27 09:37:12.000000 visaplan.plone.groups-1.2.1/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2114 2019-07-30 22:42:32.000000 visaplan.plone.groups-1.2.1/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-01-12 13:46:39.000000 visaplan.plone.groups-1.2.1/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1152 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6492 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.2.1/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9723 2021-01-12 15:40:35.000000 visaplan.plone.groups-1.2.1/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-08-27 14:33:33.000000 visaplan.plone.groups-1.3.3.1/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      674 2018-08-27 14:38:07.000000 visaplan.plone.groups-1.3.3.1/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       86 2018-08-27 14:37:58.000000 visaplan.plone.groups-1.3.3.1/docs/index.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/sql/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      294 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/sql/update-0001.sql
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      261 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      965 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/ajax.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8277 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/board.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    24079 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/browser.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1336 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      415 2023-05-02 15:23:58.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/crumbs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      605 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/fullpage.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8362 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/groupboard.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1335 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/interface.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7874 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/new-thread.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4619 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/oldcrumbs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     9782 2021-01-13 12:38:28.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/thread-reply.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      960 2021-01-13 12:38:28.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/utils.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     9164 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/ajax.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    24268 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/browser.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1348 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      417 2023-05-02 15:23:58.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/crumbs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6500 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/fullpage.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3494 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/gdmacros.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1760 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/group_administration_learning_progress_view.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4396 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/group_administration_user_view.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3175 2022-03-28 14:52:49.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/group_administration_view.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1396 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/interface.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7715 2023-01-21 00:10:39.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/oldcrumbs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      234 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-animations.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13256 2023-01-21 00:01:15.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-articles.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-audios.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      243 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-binaries.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      231 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-courses.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      327 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-events.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      232 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-formulas.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      260 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-glossaries.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      792 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-images.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      235 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-literatures.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      229 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-news.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-standards.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-tables.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      230 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-videos.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1041 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/utils.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1193 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/update-0001.sql
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      279 2018-08-27 14:42:09.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/update-0002.sql
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2046 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/update-0003.sql
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      431 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/ajax.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    92884 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/browser.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1693 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/cache.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      587 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1895 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/configure_groupsharing.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      311 2020-06-09 22:53:23.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/fullpage.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5745 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/interface.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10257 2022-03-28 14:52:49.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/utils.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/infofact/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      336 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/infofact/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2863 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/infofact/_coursemap.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3724 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/infofact/_member.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/resource/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1942 2021-01-13 12:38:28.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/resource/group-desktop.js
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2679 2020-12-17 17:52:33.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/browser.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      364 2021-01-13 12:38:28.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11291 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/utils.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       62 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      523 2020-08-27 13:15:15.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/ajax.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1026 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      617 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/fullpage.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    17812 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/group-desktop.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8439 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/group-macros.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    17486 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/mycalendar.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      594 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/mycalendar.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11865 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/myfellows.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4926 2023-05-02 15:23:58.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/myfellows.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       70 2022-03-28 14:52:26.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2634 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/_base_pio.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3104 2023-04-20 18:29:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/_base_tools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      604 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/_idxnames.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18487 2023-05-02 15:23:58.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/base.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      433 2021-11-18 18:18:50.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      455 2023-01-20 23:59:13.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/interfaces.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2020-09-24 15:44:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13922 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4564 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-09-13 07:22:08.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      170 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7302 2023-05-03 14:48:00.000000 visaplan.plone.groups-1.3.3.1/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-08-27 14:33:33.000000 visaplan.plone.groups-1.3.3.1/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-02-27 09:37:12.000000 visaplan.plone.groups-1.3.3.1/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2114 2019-07-30 22:42:32.000000 visaplan.plone.groups-1.3.3.1/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        8 2023-05-03 11:40:54.000000 visaplan.plone.groups-1.3.3.1/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1588 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7156 2023-05-03 11:11:14.000000 visaplan.plone.groups-1.3.3.1/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13922 2023-05-03 14:48:10.000000 visaplan.plone.groups-1.3.3.1/PKG-INFO
```

### Comparing `visaplan.plone.groups-1.2.1/docs/LICENSE.GPL` & `visaplan.plone.groups-1.3.3.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/docs/LICENSE.rst` & `visaplan.plone.groups-1.3.3.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/ajax.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/ajax.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/board.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/board.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/browser.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,111 +8,69 @@
 from six.moves.urllib.parse import quote_plus
 
 __author__ = "enrico"
 __date__ = "$29.04.2013 15:48:48$"
 # Standard library:
 from datetime import datetime
 
+# Zope:
+from AccessControl import Unauthorized
+from Products.CMFCore.utils import getToolByName
+from Products.Five import BrowserView
+from zope.interface import implements
+
 # visaplan:
-from visaplan.plone.base import BrowserView, Interface, implements
-from visaplan.plone.tools.context import message
+from visaplan.plone.tools.context import message as tell_user
 from visaplan.tools.coding import safe_decode
-# from visaplan.tools.debug import trace_this
 
 # Local imports:
+from ..base import GroupsBase
+from .interface import IGroupBoard
 from .utils import getsavedkey, make_getUserName
 
 # Logging / Debugging:
 import logging
 
 logger = logging.getLogger('unitracc@@groupboard')
 
 
-class IGroupBoard(Interface):
+class Browser(GroupsBase):
     """
+    Oh well.
 
+    We'll try to turn this dinosaur in some more satisfactionary BrowserView.
     """
+    implements(IGroupBoard)
 
-    def viewBoard(self):
-        """
-        generelle Ansicht des Forums
-        """
-
-    def newThread(self):
-        """
-        neues Thema eröffnen
-        """
-
-    def replyThread(self, tid=None):
-        """
-        Antwort auf ein Thema schreiben
-        """
-
-    def save(self):
-        """
-        Neues Thema speichern
-        """
-
-    def save_reply(self):
-        """
-        Speichern einer Antwort
-        """
-
-    def get_messages(self, group_id=None, subject_id=None, all=None):
-        """
-        Hole alle Nachrichten aus der Datenbank.
-        Falls Gruppe angegeben nur für Gruppe.
-        Falls subject_id angegeben hole Thema für
-        antwort ausgabe.
-        """
-
-    def get_group_id(self, subject_id):
-        """
-        Ermittle die Gruppen-ID für den angegebenen Thread
-        """
-
-    def editThread(self):
-        """
-        Einen Thread inklusive Titel bearbeiten
-        """
-
-    def delete_thread(self):
-        """
-        Einen Thread löschen.
-        """
-
-    def delete_post(self, mid=None, tid=None, withoutreturn=None):
+    def data(self):
         """
-        Delete a single message
+        data for the the ./groupboard.pt template
         """
+        g = self.my_groups_old(grouped=1)
+        return {
+            'groups': g,
+            }
 
-
-class Browser(BrowserView):
-    """
-
-    """
-    implements(IGroupBoard)
     # ---------- Funktionen für die Views --------------
 
     def viewBoard(self):
         """
         Funktion zur Seite;
-        gf: templates/board.pt
+        gf: ./board.pt
         """
         context = self.context
         form = context.restrictedTraverse('board')()
         return form
 
     def newThread(self):
         """
-        neues Thema eröffnen
+        neues Thema eröffnen; gf: ./new-thread.pt
         """
-        context = self.context
-        gid = context.REQUEST.get('gid', None)
-        form = context.restrictedTraverse('new-thread')(group=gid)
+        gid = self.current_group_id()  # request/gid
+        form = self.context.restrictedTraverse('new-thread')(group=gid)
         return form
 
     def replyThread(self):
         """
         Antwort auf ein Thema schreiben
 
         ACHTUNG - Es wird manchmal ein Request mit tid='' ausgelöst (#499) --
@@ -128,17 +86,15 @@
                 logger.error('@@gb.replyThread: tid ist %(tid)r (%(request)r)',
                              locals())
                 doit = handle_falsy_tid >= 2
             else:
                 logger.warn('@@gb.replyThread: tid ist %(tid)r (%(request)r)',
                              locals())
                 doit = handle_falsy_tid >= 1
-            if doit and 0:
-                from pdb import set_trace
-                set_trace()
+            if doit and 0: from pdb import set_trace; set_trace()
         else:
             doit = 1
 
         if doit:
             # (gf) thread-reply.pt
             form = context.restrictedTraverse('thread-reply')(tid=tid)
             return form
@@ -163,41 +119,44 @@
             return
         form = context.restrictedTraverse('new-thread')(group=thread['group_uid'],
                                                         subject=thread['thread_subject'],
                                                         tid=thread['id'],
                                                         content=first['message'],
                                                         mid=first['id'])
         return form
-    # ---- Funktionen für das Holen und aufbereiten der Daten -----
+    # ---- Funktionen für das Holen und Aufbereiten der Daten -----
 
     def get_group_id(self, subject_id):
         """
         Ermittle die Gruppen-ID für den angegebenen Thread
         """
         context = self.context
         with context.getAdapter('sqlwrapper') as sql:
             rows = sql.select('groupboard_thread',
                               query_data={'id': subject_id},
                               maxrows=1)
             for row in rows:
                 return row['group_uid']  # eine Id, *keine* UID
 
-    # @trace_this
     def get_messages(self,  # ------------------- [ get_messages ... [
                      group_id=None, subject_id=None, all=None):
         """
         Hole alle Nachrichten aus der Datenbank.
         Falls Gruppe angegeben nur für Gruppe.
         Falls subject_id angegeben hole Thema für
         antwort ausgabe.
         """
         context = self.context
         getBrowser = context.getBrowser
         author = getBrowser('author')
-        me = getBrowser('auth').getId()
+        pm = getToolByName(context, 'portal_membership')
+        if pm.isAnonymousUser():
+            raise Unauthorized
+        user = pm.getAuthenticatedMember()
+        me = user.getId()
         groupsharing = getBrowser('groupsharing')
         result = {}
         read = []
         new = []
         getAdapter = context.getAdapter
         getUserName = make_getUserName(getBrowser=getBrowser)
         with getAdapter('sqlwrapper') as sql:
@@ -268,18 +227,17 @@
                     logger.error(message_)
                     desktop_path = getBrowser('unitraccfeature').desktop_path()
                     url = desktop_path + '/@@groupboard/viewBoard'
                     return context.REQUEST.RESPONSE.redirect(url)
 
                 group_uid = group_id
             else:
-                # Hole alle Threads in denen ich Gruppenmitglied bin.
-                groups = getBrowser('groupdesktop').getInfo()['groups']
-                group_uid = list(set(filter(None,
-                                            [group['id'] for group in groups])))
+                # Hole die Threads aller Gruppen, in denen ich Mitglied bin
+                group_uid = [theid for theid in user.getGroups()
+                             if theid != 'AuthenticatedUsers']
             threads = sql.select(table="groupboard_thread",
                                  query_data={'group_uid': group_uid})
             delete_right = self.can_delete()
 
             # ----------------------------------- ... get_messages ...
             for thread in threads:
 
@@ -336,59 +294,61 @@
             return result  # -------------------- ] ... get_messages ]
 
     def get_message(self, tid, mid):
         if not mid or not tid:
             logger.warn('get_message(): tid=%(tid)r, mid=%(mid)r', locals())
             return
         with self.context.getAdapter('sqlwrapper') as sql:
-            message = sql.select('groupboard_messages',
+            msg_item = sql.select('groupboard_messages',
                                  ['user_id', 'message_text'],
                                  "WHERE id=%(mid)s and thread_id=%(tid)s",
                                  {'mid': mid, 'tid': tid},
                                  1)[0]
-        if not self.can_edit(message):
+        if not self.can_edit(msg_item):
             return
-        return message['message_text']
+        return msg_item['message_text']
 
     def save(self, subject=None):
         """
         Speichern eines neuen Themas
         """
         context = self.context
         form = context.REQUEST.form
         if form.get('tid'):
             return self.edit_thread()
 
         group = form.get('group')
         subject = form.get('subject')
-        message = form.get('content', '  ')
+        message_text = form.get('content', '  ')
         boardrules = form.get('boardrules')
         desktop_path = context.getBrowser('unitraccfeature').desktop_path()
-        errors = []
+        errors = []  # i.e., numbers of the respective inputs
         if not group:
             errors.append("1")
+        elif not self.can_access_group(group):
+            errors.append('1')
         if not subject:
             errors.append("2")
-        if not message:
+        if not message_text:
             errors.append("3")
         if not boardrules:
             errors.append("4")
 
         if errors:
             error = ",".join(errors)
             url = ('%s/@@groupboard/newThread?error=%s'
                    '&group=%s&subject=%s&content=%s'
                    % (desktop_path,
                       error,
                       group,
                       quote_plus(subject),
-                      quote_plus(message)))
+                      quote_plus(message_text)))
             return context.REQUEST.RESPONSE.redirect(url)
         with context.getAdapter('sqlwrapper') as sql:
-            # Neues Thema Speichern
+            # Neues Thema speichern
             values = {'group_uid': group,
                       'thread_subject': subject,
                       }
             # Update eine vorhandenen Themas
             try:
                 sql.insert("groupboard_thread", values)
             except:
@@ -401,38 +361,38 @@
             tid = sql.select(table="groupboard_thread",
                              fields=['id'],
                              where=where,
                              query_data=values,
                              maxrows=1)[0]['id']
             user_id = context.getBrowser('auth').getId()
             values = {'thread_id': tid,
-                      'message_text': message,
+                      'message_text': message_text,
                       'message_date': now,
                       }
             values['user_id'] = user_id
 
             # Die Nachricht speichern
             table = "groupboard_messages"
             sql.insert(table, values)
 
         # Verweis auf das Gruppenforum für die Gruppe
         # in der das Thema geschrieben wurde
-        url = '%s/@@groupboard/replyThread?tid=%s' % (
-               desktop_path, tid,
+        url = '%s/@@groupboard/replyThread?group=%s&tid=%s' % (
+               desktop_path, group, tid,
                )
         return context.REQUEST.RESPONSE.redirect(url)
 
     def save_reply(self):
         """
         Speichern einer Antwort
         """
         context = self.context
         desktop_path = context.getBrowser('unitraccfeature').desktop_path()
         subject = context.REQUEST.form['tid']
-        message = context.REQUEST.form.get('reply')
+        message_text = context.REQUEST.form.get('reply')
         mid = context.REQUEST.form.get('mid')
         boardrules = context.REQUEST.form.get('boardrules', False)
         error = not boardrules
         redirect = context.REQUEST.RESPONSE.redirect
         if error:
             if mid:
                 url = ('%s/@@groupboard/replyThread?tid=%s&mid=%s&error=%s'
@@ -440,28 +400,28 @@
                             subject,
                             mid,
                             error)
             else:
                 url = ('%s/@@groupboard/replyThread?tid=%s&reply=%s&error=%s'
                        ) % (desktop_path,
                             subject,
-                            quote_plus(message),
+                            quote_plus(message_text),
                             error)
             return redirect(url)
-        if not message:
+        if not message_text:
             url = ('%s/@@groupboard/replyThread?tid=%s&reply=%s'
                    % (desktop_path,
                       subject,
-                      quote_plus(message),
+                      quote_plus(message_text),
                       ))
             return redirect(url)
         user_id = context.getBrowser('auth').getId()
         now = datetime.now()
         values = {'thread_id': subject,
-                  'message_text': message,
+                  'message_text': message_text,
                   }
 
         # Die Nachricht speichern
         with context.getAdapter('sqlwrapper') as sql:
             table = "groupboard_messages"
             if mid:
                 sql.update(table,
@@ -530,16 +490,16 @@
         with context.getAdapter('sqlwrapper') as sql:
             messages = self.get_messages(subject_id=thread, all=True)
             all_messages = []
             all_messages.extend(x for x in messages['replys'])
             all_messages.append(messages['first'])
 
             query = {'tid': thread}
-            for message in all_messages:
-                self.delete_post(mid=message['id'],
+            for msg_item in all_messages:
+                self.delete_post(mid=msg_item['id'],
                                  tid=thread,
                                  withoutreturn=True)
             # delete Thread
             table = "groupboard_thread"
             where = "WHERE id=%(tid)s"
             sql.delete(table, where, query)
         desktop_path = context.getBrowser('unitraccfeature').desktop_path()
@@ -550,56 +510,56 @@
         """
         Ganzen Thread bearbeiten
         """
         context = self.context
         form = context.REQUEST.form
         group = form.get('group')
         subject = form.get('subject')
-        message = form.get('content', '  ')
+        message_text = form.get('content', '  ')
         _ = context.getAdapter('translate')
         tid = form.get('tid')
         mid = form.get('mid')
         boardrules = form.get('boardrules')
         desktop_path = context.getBrowser('unitraccfeature').desktop_path()
         error = boardrules is None
         url = ('%s/@@groupboard/editThread?tid=%s&mid=%s'
                '&group=%s&subject=%s&content=%s'
                ) % (desktop_path,
                    tid,
                    mid,
                    group,
                    quote_plus(subject),
-                   quote_plus(message))
-        if not group or not subject or not message or not boardrules:
+                   quote_plus(message_text))
+        if not group or not subject or not message_text or not boardrules:
             url += '&error=%s' % error
             return context.REQUEST.RESPONSE.redirect(url)
 
         with context.getAdapter('sqlwrapper') as sql:
             group_uid = sql.select("groupboard_thread",
                                    ['group_uid'],
                                    "WHERE id=%(tid)s",
                                    form,
                                    1)[0]['group_uid']
-            # Neues Thema Speichern
+            # Neues Thema speichern
             values = {'thread_subject': subject,
                       }
             if group != group_uid:
                 values['group_uid'] = group
             # Update eine vorhandenen Themas
             where = "WHERE id=%(tid)s"
             try:
                 sql.update("groupboard_thread", values, where, form)
             except:
                 print("Thema '%s' bereits vorhanden." % subject)
-                message(context,
+                tell_user(context,
                         _("Subject exists already in group."), 'error')
                 return context.REQUEST.RESPONSE.redirect(url)
 
             # Daten für Nachricht zusammenbauen
-            values = {'thread_id': tid, 'message_text': message}
+            values = {'thread_id': tid, 'message_text': message_text}
 
             # Die Nachricht speichern
             table = "groupboard_messages"
             where = "WHERE id=%(mid)s and thread_id=%(tid)s"
             sql.update(table, values, where, form)
             # Verweis auf das Thread
 
@@ -626,21 +586,15 @@
             message_WHERE = "WHERE id=%(mid)s and thread_id=%(tid)s"
             sql.delete(message_table, message_WHERE, query)
 
         if not withoutreturn:
             return self.replyThread()
 
     def has_access(self, group_id):
-        context = self.context
-        groups = context.getBrowser('groupdesktop').getInfo()['groups']
-
-        if group_id in [x['id'] for x in groups]:
-            return True
-        else:
-            return False
+        return self.can_access_group(group_id)
 
     def isBoardManager(self, context=None, getAdapter=None):
         """
         Ist der aktive Benutzer ein Board-Manager?
         """
         if getAdapter is None:
             if context is None:
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/fullpage.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/fullpage.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/new-thread.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/new-thread.pt`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,40 @@
       i18n:domain="plone">
 
     <metal:block fill-slot="top_slot"
              tal:define="dummy python:request.set('disable_border',1);" />
     <metal:no-ads fill-slot="column_two_slot"/>
     <metal:no-ads fill-slot="column_one_slot"/>
     <head>
-        <metal:js fill-slot="head_slot">
-        <metal:js define-macro="chosen-js">
-        <script type="text/javascript">
-        function filterOptions(){
-            handleOverLay(true);
-            $("#go_to_groupdesktop").submit();
-        }
-        $(document).ready(function () {
-            $('select.chosen').chosen().change(filterOptions);
-        });
-        </script>
-      </metal:js>
-      </metal:js>
     </head>
     <body>
-        <metal:cr_outer fill-slot="breadcrumb">
-            <metal:breadcrumb use-macro="here/crumbs/macros/main"/>
-
-        </metal:cr_outer>
-
+<!--
+gf links:
+- ./browser.py (@@groupboard)
+- ../../../../../../visaplan.UnitraccSkins/src/visaplan/UnitraccSkins/skins/unitracc_templates/main_template.pt
+
+Remarks:
+- Why do we consider both gid and group request vars?!
+  Since no reason was documented, we'll use the one given by the form field
+  name.
+  -->
         <metal:main fill-slot="main"
                     tal:define="
 gid request/gid|options/gid|nothing;
-group request/group|options/group|nothing;
+group request/group|options/group|gid;
 subject request/subject|options/subject|nothing;
 content request/content|options/content|nothing;
 mid options/mid|nothing;
-errors python:request.get('error','') ;
-error python: errors.split(',');
+error python:(request.get('error') or '').split(',');
 tid request/tid | nothing;
 gs python:here.getBrowser('groupsharing');
 groupboard python:here.getBrowser('groupboard');
+data       python:groupboard.data();
 guidelinesuid groupboard/get_guidelines;
-groups python:(not gid and not group) and gs.voc_get_explicit_group_memberships_for_auth();
+groups python:gs.voc_get_explicit_group_memberships_for_auth();
 ">
             <div class="area-title">
                 <h1 i18n:translate="" tal:condition="not: tid">
                     Create a new thread
                 </h1>
                 <h1 tal:condition="tid" i18n:translate="">
                     Edit thread
@@ -65,46 +57,52 @@
                            tal:condition="tid">
                             Edit a thread for your working group
                         </p>
                     </div>
                 </div>
                 <div class="new-thread">
                     <form method="POST" action="@@groupboard/save"
-                          tal:condition="python: gid or group or groups">
+                          tal:condition="python:group or groups">
                         <input type="hidden" name="mid"
                                tal:condition="mid"
                                tal:attributes="value mid"/>
                         <input type="hidden" name="tid"
                                tal:condition="tid"
                                tal:attributes="value tid"/>
                         <div class="field"
-                             tal:define="groups python:gs.voc_get_explicit_group_memberships_for_auth();">
+                             tal:define="
+group python:None if group == 'None' else group;
+gid   group;
+name      string:group;
+optgroups python:data['groups'];
+class     string:chosen;
+">
                             <label
                                 tal:attributes="class python:'1' in error and 'text-error' or ''">
                                 <i class="glyphicon glyphicon-exclamation-sign"></i>
                                 <tal:block i18n:translate="">Working group</tal:block>
                             </label>
                             <select name="group" class="chosen"
-                                    tal:condition="python:not gid"
+                                metal:use-macro="here/group-macros/macros/group-selector-grouped"
                                     data-placeholder="Choose one ..."
                                     i18n:attributes="data-placeholder"
                                     style="width:50%">
-                                <option></option>
+                                <option
+                                    tal:replace="nothing"
+                                    metal:fill-slot="empty-selection"></option>
                                 <tal:loop tal:repeat="row groups">
                                 <option tal:attributes="value python:row[0];
                                                         selected python:row[0]==group or ''"
                                         tal:content="python:row[1]"
                                         i18n:translate=""/>
                                 </tal:loop>
                             </select>
-                            <tal:block tal:condition="gid">
-                                <input type="hidden" tal:attributes="value gid|group"
-                                       name="group">
-
-                                <p tal:define="title python:gs.get_group_info_by_id(gid)"
+                            <tal:block tal:condition="group">
+                                <p tal:define="title python:gs.get_group_info_by_id(group)"
+                                   tal:on-error="string:Oops - error getting group info! (${group})"
                                    tal:content="structure title/group_title"
                                    i18n:translate=""/>
                             </tal:block>
                         </div>
 
                         <div id="archetypes-fieldname-title" class="field">
                             <label tal:attributes="class python:'2' in error and 'text-error' or ''">
@@ -138,16 +136,25 @@
                             <textarea tal:content="content" name="content" class="thread-content col-md-7" rows="15"></textarea>
                         </div>
                         <div>
                             <input type="submit" value="Store" class="btn btn-primary" i18n:attributes="value">
                             <input type="reset" value="Reset" class="btn btn-default" i18n:attributes="value">
                         </div>
                     </form>
-                    <p tal:condition="python: not gid and not group and not groups"
+                    <p tal:condition="python: not group and not groups"
                        i18n:translate="">
                         You must be member of a group to create a thread.
                     </p>
                 </div>
             </div>
+        <script type="text/javascript">
+        function filterOptions(){
+            handleOverLay(true);
+            $("#go_to_groupdesktop").submit();
+        }
+        $(document).ready(function () {
+            $('select.chosen').chosen().change(filterOptions);
+        });
+        </script>
         </metal:main>
     </body>
 </html>
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/oldcrumbs.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/oldcrumbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     Erzeuge keinen eigenen Krümel, sondern ermittle die Gruppen-ID
     aus der Thread-ID *vor* dem Aufruf der Parents!
 
     Es wird allerdings der Gruppenschreibtischkrümel sichergestellt
     und der Gruppenforum-Krümel hinter diesen sortiert.
     """
     def __call__(self, crumbs, hub, info):
-        # set_trace()
         if info['gid'] is None:
             tid = info['request_var'].get('tid')
             if tid is not None:
                 info['gid'] = hub['groupboard'].get_group_id(tid)
         BaseCrumb.__call__(self, crumbs, hub, info)
 
     def tweak(self, crumbs, hub, info):
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/thread-reply.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/thread-reply.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupboard/utils.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupboard/utils.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/ajax.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/ajax.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/browser.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,77 @@
 # -*- coding: utf-8 -*- Umlaute: ÄÖÜäöüß
 # Python compatibility:
 from __future__ import absolute_import
 
-# visaplan:
-from visaplan.plone.base import BrowserView, Interface, implements
-
 try:
     # Zope:
     from Globals import DevelopmentMode
-    DevelopmentMode = 1  # nur [bugfix]
 except ImportError:
     # Hotfix for Zope 4; how to properly replace this?
     DevelopmentMode = False
+
 # Zope:
 from AccessControl import Unauthorized
 from Products.CMFCore.utils import getToolByName
+from zope.component import getMultiAdapter
+from zope.interface import implements
 
 # visaplan:
 from visaplan.plone.base.permissions import ManageCourses, ManageGroups
 from visaplan.plone.base.typestr import pluralize
 from visaplan.plone.infohubs import make_hubs
+from visaplan.plone.infohubs.hubs2 import context_and_form_tuple
+from visaplan.plone.tools.groups import (
+    build_groups_set,
+    get_all_members,
+    groupinfo_factory,
+    is_direct_member__factory,
+    is_member_of__factory,
+    is_member_of_any,
+    userinfo_factory,
+    )
+from visaplan.tools.classes import Proxy
+from visaplan.tools.coding import safe_decode
+from visaplan.tools.dates import make_date_formatter
+from visaplan.tools.lands0 import list_of_strings
 from visaplan.tools.minifuncs import gimme_True, makeBool
 from visaplan.tools.profile import StopWatch
 
 # Local imports:
+from .._idxnames import getExcludeFromNav
+from ..base import GroupsBase
+from ..groupsharing.utils import (
+    datefromform,
+    default_dates_dict,
+    getcoursetitle,
+    getgrouptitle,
+    gettitle,
+    journal_text,
+    make_break_at_row,
+    make_keyfunction,
+    makedate,
+    )
+from .interface import IGroupDesktop
 from .utils import make_authorfilter, make_groupfilter
+# TODO: generate the split_group_id function,
+#       using data depending on the installed packages.
+#       Implement make_group_id_splitter in v.p.tools.groups.
 from visaplan.plone.groups.unitraccgroups.utils import (
+    ALL_GROUP_SUFFIXES,
+    ALUMNI_SUFFIX,
     LEARNER_SUFFIX,
+    pretty_group_title,
     split_group_id,
     )
 
 # Logging / Debugging:
 from visaplan.plone.tools.log import getLogSupport
+from visaplan.tools.debug import pp
 
 logger, debug_active, DEBUG = getLogSupport('groupdesktop')
-# Logging / Debugging:
-from visaplan.tools.debug import pp
 
 sw_kwargs = {'enable': bool(debug_active),
              }
 
 
 # ------------------------------------------------------ [ Daten ... [
 # TODO: die folgenden beiden Listen sollten inzwischen obsolet sein;
@@ -48,79 +80,37 @@
                            # nicht zur Bearbeitung, also kein Schreibtisch:
                            'group_academic_accounts',
                            # ... Vortraege Reader:
                            'group_1255c69f5497ffb66ab21dfb9108ec4e_Reader',
                            # HTML-Autoren:
                            'group_1cc0c081bceacc480da7af79f1fb70d4',
                            ]
+BORING_GROUPS = set(['AuthenticatedUsers'])
 ANONYMOUS_GROUPS = [
                     # Evaluation Reinigung I Reader (UNITRACC-421):
                     'group_04c187b106643685b2f51201e12d534a',
                     ]
 # siehe auch @@groupsharing.BORING_GROUPS
 # ------------------------------------------------------ ] ... Daten ]
 
 
-class IGroupDesktop(Interface):
-
-    def getInfo(topic=None,
-                tid=None,
-                portal_type=None,
-                get_members=0):
-        """
-        Gib ein Python-Dictionary zurueck, das interessante
-        Informationen fuer den Gruppenschreibtisch enthaelt
-        """
-
-    def getLoopDicts(gid=None, topic=None, exclude=None):
-        """
-        Gib Dictionarys fuer group-desktop zurueck
-        """
-
-    def getGroupsBlacklist():
-        """
-        Gib die Gruppen zurueck, die *keine* Gruppenschreibtische erzeugen
-        """
-
-    def groupProvidesMembers(gid):
-        """
-        Stellt die uebergebene Gruppe ueber ihren Gruppenschreibtisch
-        die Visitenkarten ihrer Mitglieder zur Verfuegung?
-        """
-
-    def can_view_group_administration(group_id, user_id=None):
-        """
-        Kann Benutzer Gruppenschreibtisch administrieren? ja/nein
-        """
-
-    def auth_view_group_administration(group_id, user_id=None):
-        """
-        Kann Benutzer Gruppenschreibtisch administrieren? ja/nein;
-        wenn nein -> Unauthorized-Exception
-        """
-
-    def set_end_of_group_membership_to_today():
-        """
-        Mitgliedschaft durch Gruppenadministrator beeenden.
-        """
-
-
-class Browser(BrowserView):
+class Browser(GroupsBase):
 
     implements(IGroupDesktop)
 
     @staticmethod
     def isValid(gid):
         """
         Prüfe, ob die übergebene Gruppen-ID sinnvoll erscheint
         """
         if not gid:
             return False
         return gid != 'None'
 
+    # data for ../views/group-desktop.pt
     def getInfo(self,
                 topic=None,
                 tid=None,
                 portal_type=None,
                 get_members=0,
                 get_breadcrumbs=0,
                 **kwargs):
@@ -164,32 +154,37 @@
 
         strings -- wenn topic uebergeben, das Ergebnis von
                    self.getLoopDicts(..., topic) (das in diesem Fall ein einzelnes
                    dict zurueckgibt, keine Sequenz)
         """
         with StopWatch('@@groupdesktop.getInfo',
                        **sw_kwargs) as stopwatch:
-            context = self.context
-            mt = getToolByName(context, 'portal_membership')
+            mt = getToolByName(self.context, 'portal_membership')
             if mt.isAnonymousUser():
                 raise Unauthorized()
 
             hub = kwargs.pop('hub', None)
             info = kwargs.pop('info', None)
-            if hub is None:
-                assert info is None
-                hub, info = make_hubs(context)
-            else:
+            caft_kw = {
+                'amend': True,
+                }
+            if hub is not None:
                 assert info is not None
-
-            rc = hub['rc']
-
-            request = context.REQUEST
-            form = request.form
-            gid = info['gid']
+                caft_kw.update({
+                    'hub': hub,
+                    'info': info,
+                    })
+            else:
+                assert info is None
+                caft_kw.update({
+                    'context': self.context,
+                    })
+            hub, info, context, form = \
+                context_and_form_tuple(**caft_kw)
+            gid = info['gid'] = self.current_group_id()
             subpages = None
             user_id = info['user_id']
 
             if debug_active:
                 DEBUG('getInfo(topic=%r, tid=%r, portal_type=%r, get_members=%r)',
                         topic, tid, portal_type, get_members)
             if tid is not None:
@@ -202,53 +197,55 @@
                 if tid is None:
                     tid = strings['page']
                 if portal_type is None:
                     portal_type = strings['portal_type']
             else:
                 strings = None
 
-            if 0 and 'devel':
-                # Logging / Debugging:
-                import pdb
-                pdb.set_trace()
+            if 0 and 'devel': set_trace()
             _ = mogrify = hub['translate']
 
             baseurl = hub['unitraccfeature'].desktop_path()
 
-            # wird von getGroups gefüllt:
-            current = {}
             courses = []
             # groups: Gruppen für die Schreibtischauswahl
             #         Es dürfen nur Gruppen ausgegeben werden ...
             #         - deren Schreibtisch-Flag aktiv ist
             #         - zu denen eine *direkte* Mitgliedschaft besteht
             #         - (um die Auswahl des pers. Schreibtischs jedenfalls
             #           funktional zu machen:) Die aktuell gewählte Gruppe
-            stopwatch.lap('Kurse und Gruppen besorgen ...')
-            courses, dt_groups = \
-                    hub['groupsharing'].get_courses_and_desktop_groups(
-                            user_id, gid or None)
-            stopwatch.lap('Kurse und Gruppen')
-            if 0:
-                pp((('courses:', courses),
-                    ('dt_groups:', dt_groups),
-                    ))
-            for dic in dt_groups:
-                if dic['id'] == gid:
-                    # nicht einfach zuweisen, wg. pot. Änderung:
-                    current.update(dic)
-                if dic['group_manager'] == user_id:
-                    dic['group_title'] = _('${group_title} (Group manager)',
-                                           mapping=dic)
+            gs = context.restrictedTraverse('@@groupsharing')
+            # gs.get_courses_and_desktop_groups(user_id, None)
+            # mygroups = gs.get_user_and_all_groups(user_id)[1]
+            groups = self.my_groups_old(user_id, grouped=1)
+            pg = getToolByName(context, 'portal_groups')
+
+            checkperm = getToolByName(context, 'portal_membership').checkPermission
+            manage_any = checkperm(ManageGroups, context)
+
+            stopwatch.lap('Nur Gruppen')
+
+            # dt_groups = self.admin_or_desktop_groups(grouped=0)
             stopwatch.lap('Gruppentitel')
 
+            if gid is None:
+                current = None
+            else:
+                gi = groupinfo_factory(context, pretty=1, forlist=1)
+                current = gi(gid)
+                get_group = pg.getGroupById
+                go = get_group(gid)
+                current['group_desktop'] = (1 if go
+                                                 and go.getProperty('group_desktop')
+                                            else 0)
+
             members = []  # ... der Gruppe <gid>
             # nur 'natuerliche Personen', also keine Gruppen:
             if (get_members
-                and gid is not None
+                and current is not None
                 # Desktop-Flag -> Mitglieder werden ausgegeben:
                 and current.get('group_desktop')
                 ):
                 memberids = []
                 gsle = hub['author'].getShortListEntry
                 for brain in self.getGroupMembers(gid, user_id):
                     try:
@@ -276,15 +273,15 @@
                     elif member['id'] in memberids:
                         logger.error('Doppelter Benutzer "%(id)s"!', member)
                         continue
                     memberids.append(member['id'])
                     members.append(member)
                 stopwatch.lap('Mitgliederliste')
 
-            rslt = {'groups': dt_groups,
+            rslt = {'groups': groups, # dt_groups,
                     'members': members,
                     'current': current or None,
                     'gid': gid,
                     'calendar': gid
                     and {'url': '%(baseurl)s/our-calendar?gid=%(gid)s' % locals(),
                          'label': 'Group calendar',
                          }
@@ -293,15 +290,15 @@
                          },
                     'userid': user_id,
                     'desktopurl': baseurl,
                     'baseurl': baseurl,
                     'devmode': DevelopmentMode,
                     'verbose': DevelopmentMode and makeBool(form.get('verbose', 'no')),
                     'strings': strings,
-                    'courses': courses,
+                    # 'courses': courses, --> see @@mycourses
                     'info': info, # aus make_hubs-Aufruf
                     }
             return rslt
 
     def getGroupMembers(self, groupId, myId=None):
         """
         Gib alle Mitglieder der Gruppe mit der uebergebenen ID zurueck,
@@ -328,15 +325,15 @@
             pass
         else:
             checkperm = getToolByName(context, 'portal_membership').checkPermission
             if not checkperm(ManageGroups, context):
                 logger.info('User %r nicht in Gruppe, keine Perm. "Manage Groups"'
                             % (myId,))
                 return []
-        query = {'getExcludeFromNav': False,
+        query = {getExcludeFromNav: False,  # WIP: change index name
                  'portal_type': 'UnitraccAuthor',
                  'Creator': mids,
                  }
         pc = getToolByName(context, 'portal_user_catalog')
         rslt = pc(query)
         return rslt
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/configure.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
        ../views/configure.zcml)
     -->
   <browser:page
       for="*"
       name="groupdesktop"
       class=".browser.Browser"
       permission="zope2.View"
-      allowed_interface=".browser.IGroupDesktop"
+      allowed_interface=".interface.IGroupDesktop"
       />
 
     <browser:page
              for="*"
              name="gdmacros"
              template="gdmacros.pt"
              permission="zope2.View"
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/fullpage.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/fullpage.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/gdmacros.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/gdmacros.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/group_administration_learning_progress_view.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/group_administration_learning_progress_view.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/group_administration_user_view.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/group_administration_view.pt`

 * *Files 27% similar despite different names*

```diff
@@ -41,192 +41,159 @@
 00000280: 6172 696e 6720 6e6f 6361 6c6c 3a63 6f6e  aring nocall:con
 00000290: 7465 7874 2f40 4067 726f 7570 7368 6172  text/@@groupshar
 000002a0: 696e 673b 0a20 2020 2020 2020 2020 2020  ing;.           
 000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002c0: 2020 6772 6f75 705f 696e 666f 2070 7974    group_info pyt
 000002d0: 686f 6e3a 6772 6f75 7073 6861 7269 6e67  hon:groupsharing
 000002e0: 2e67 6574 5f67 726f 7570 5f69 6e66 6f5f  .get_group_info_
-000002f0: 6279 5f69 6428 6769 6429 3b0a 2020 2020  by_id(gid);.    
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2020 2020 2020 2067 726f 7570 5f6d           group_m
-00000320: 656d 6265 7273 6869 7073 2070 7974 686f  emberships pytho
-00000330: 6e3a 6772 6f75 7073 6861 7269 6e67 2e67  n:groupsharing.g
-00000340: 6574 5f65 7870 6c69 6369 745f 6772 6f75  et_explicit_grou
-00000350: 705f 6d65 6d62 6572 7368 6970 7328 6769  p_memberships(gi
-00000360: 6429 3b0a 2020 2020 2020 2020 2020 2020  d);.            
-00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000380: 2022 3e0a 0a20 2020 203c 6831 2063 6c61   ">..    <h1 cla
-00000390: 7373 3d22 646f 6375 6d65 6e74 4669 7273  ss="documentFirs
-000003a0: 7448 6561 6469 6e67 220a 2020 2020 2020  tHeading".      
-000003b0: 2020 6931 386e 3a74 7261 6e73 6c61 7465    i18n:translate
-000003c0: 3d22 223e 0a20 2020 2020 2020 204d 616e  ="">.        Man
-000003d0: 6167 6520 6772 6f75 7020 6d65 6d62 6572  age group member
-000003e0: 7368 6970 7320 666f 720a 2020 2020 2020  ships for.      
-000003f0: 2020 3c74 616c 3a62 6c6f 636b 2074 616c    <tal:block tal
-00000400: 3a63 6f6e 7465 6e74 3d22 6772 6f75 705f  :content="group_
-00000410: 696e 666f 2f67 726f 7570 5f74 6974 6c65  info/group_title
-00000420: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000430: 2020 2020 2069 3138 6e3a 6e61 6d65 3d22       i18n:name="
-00000440: 7661 6c75 6522 3e0a 2020 2020 2020 2020  value">.        
-00000450: 2020 2020 4772 7570 7065 6e2d 4944 0a20      Gruppen-ID. 
-00000460: 2020 2020 2020 203c 2f74 616c 3a62 6c6f         </tal:blo
-00000470: 636b 3e0a 2020 2020 3c2f 6831 3e0a 0a20  ck>.    </h1>.. 
-00000480: 2020 203c 7461 626c 6520 636c 6173 733d     <table class=
-00000490: 2274 6162 6c65 2074 6162 6c65 2d62 6f72  "table table-bor
-000004a0: 6465 7265 6420 6461 7461 7462 2074 6162  dered datatb tab
-000004b0: 6c65 2d73 6f72 7465 6422 3e0a 2020 2020  le-sorted">.    
-000004c0: 3c74 6865 6164 3e0a 2020 2020 3c74 723e  <thead>.    <tr>
-000004d0: 0a20 2020 2020 2020 203c 7468 2069 3138  .        <th i18
-000004e0: 6e3a 7472 616e 736c 6174 653d 2222 3e0a  n:translate="">.
-000004f0: 2020 2020 2020 2020 2020 2020 5479 7065              Type
-00000500: 0a20 2020 2020 2020 203c 2f74 683e 0a20  .        </th>. 
-00000510: 2020 2020 2020 203c 7468 2069 3138 6e3a         <th i18n:
-00000520: 7472 616e 736c 6174 653d 226c 6162 656c  translate="label
-00000530: 5f6c 6f67 696e 5f6e 616d 6522 3e0a 2020  _login_name">.  
-00000540: 2020 2020 2020 2020 2020 4c6f 6769 6e20            Login 
-00000550: 4e61 6d65 0a20 2020 2020 2020 203c 2f74  Name.        </t
-00000560: 683e 0a20 2020 2020 2020 203c 7468 2069  h>.        <th i
-00000570: 3138 6e3a 7472 616e 736c 6174 653d 2222  18n:translate=""
-00000580: 3e0a 2020 2020 2020 2020 2020 2020 4e61  >.            Na
-00000590: 6d65 0a20 2020 2020 2020 203c 2f74 683e  me.        </th>
-000005a0: 0a20 2020 2020 2020 203c 7468 2069 3138  .        <th i18
-000005b0: 6e3a 7472 616e 736c 6174 653d 2222 3e0a  n:translate="">.
-000005c0: 2020 2020 2020 2020 2020 2020 4d65 6d62              Memb
-000005d0: 6572 2073 696e 6365 0a20 2020 2020 2020  er since.       
-000005e0: 203c 2f74 683e 0a20 2020 2020 2020 203c   </th>.        <
-000005f0: 7468 2069 3138 6e3a 7472 616e 736c 6174  th i18n:translat
-00000600: 653d 2222 3e0a 2020 2020 2020 2020 2020  e="">.          
-00000610: 2020 4d65 6d62 6572 2074 696c 6c0a 2020    Member till.  
-00000620: 2020 2020 2020 3c2f 7468 3e0a 2020 2020        </th>.    
-00000630: 2020 2020 3c74 6820 6931 386e 3a74 7261      <th i18n:tra
-00000640: 6e73 6c61 7465 3d22 223e 0a20 2020 2020  nslate="">.     
-00000650: 2020 2020 2020 2041 6374 696f 6e73 0a20         Actions. 
-00000660: 2020 2020 2020 203c 2f74 683e 0a20 2020         </th>.   
-00000670: 203c 2f74 723e 0a20 2020 203c 2f74 6865   </tr>.    </the
-00000680: 6164 3e0a 2020 2020 3c74 626f 6479 3e0a  ad>.    <tbody>.
-00000690: 2020 2020 3c74 7220 7461 6c3a 7265 7065      <tr tal:repe
-000006a0: 6174 3d22 6469 6374 5f20 6772 6f75 705f  at="dict_ group_
-000006b0: 6d65 6d62 6572 7368 6970 7322 3e0a 2020  memberships">.  
-000006c0: 2020 2020 2020 2020 2020 3c74 643e 0a20            <td>. 
-000006d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000006e0: 7461 6c3a 626c 6f63 6b20 7461 6c3a 6465  tal:block tal:de
-000006f0: 6669 6e65 3d22 7479 2070 7974 686f 6e3a  fine="ty python:
-00000700: 6469 6374 5f5b 2774 7970 6527 5d22 0a20  dict_['type']". 
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2020 2020 7461 6c3a 636f            tal:co
-00000730: 6e64 6974 696f 6e3d 2274 7922 0a20 2020  ndition="ty".   
-00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000750: 2020 2020 2020 2020 7461 6c3a 636f 6e74          tal:cont
-00000760: 656e 743d 2270 7974 686f 6e3a 7479 2e74  ent="python:ty.t
-00000770: 6974 6c65 2829 220a 2020 2020 2020 2020  itle()".        
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2069 3138 6e3a 7472 616e 736c 6174     i18n:translat
-000007a0: 653d 2222 0a20 2020 2020 2020 2020 2020  e="".           
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 7461 6c3a 6f6e 2d65 7272 6f72 3d22 7479  tal:on-error="ty
-000007d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000007e0: 2020 2042 656e 7574 7a65 720a 2020 2020     Benutzer.    
-000007f0: 2020 2020 2020 2020 2020 2020 3c2f 7461              </ta
-00000800: 6c3a 626c 6f63 6b3e 0a20 2020 2020 2020  l:block>.       
-00000810: 2020 2020 203c 2f74 643e 0a20 2020 2020       </td>.     
-00000820: 2020 2020 2020 203c 7464 3e0a 2020 2020         <td>.    
-00000830: 2020 2020 2020 2020 2020 2020 3c74 616c              <tal
-00000840: 3a62 6c6f 636b 2074 616c 3a63 6f6e 7465  :block tal:conte
-00000850: 6e74 3d22 6469 6374 5f2f 6964 222f 3e0a  nt="dict_/id"/>.
-00000860: 2020 2020 2020 2020 2020 2020 3c2f 7464              </td
-00000870: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-00000880: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00000890: 2020 203c 7461 6c3a 626c 6f63 6b20 7461     <tal:block ta
-000008a0: 6c3a 636f 6e74 656e 743d 2264 6963 745f  l:content="dict_
-000008b0: 2f74 6974 6c65 222f 3e0a 2020 2020 2020  /title"/>.      
-000008c0: 2020 2020 2020 3c2f 7464 3e0a 2020 2020        </td>.    
-000008d0: 2020 2020 2020 2020 3c74 643e 0a20 2020          <td>.   
-000008e0: 2020 2020 2020 2020 2020 2020 203c 7461               <ta
-000008f0: 6c3a 626c 6f63 6b20 7461 6c3a 636f 6e64  l:block tal:cond
-00000900: 6974 696f 6e3d 2264 6963 745f 2f73 7461  ition="dict_/sta
-00000910: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
-00000920: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000930: 616c 3a63 6f6e 7465 6e74 3d22 6469 6374  al:content="dict
-00000940: 5f2f 7374 6172 7422 2f3e 0a20 2020 2020  _/start"/>.     
-00000950: 2020 2020 2020 203c 2f74 643e 0a20 2020         </td>.   
-00000960: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
-00000970: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00000980: 616c 3a62 6c6f 636b 2074 616c 3a63 6f6e  al:block tal:con
-00000990: 6469 7469 6f6e 3d22 6469 6374 5f2f 656e  dition="dict_/en
-000009a0: 6473 220a 2020 2020 2020 2020 2020 2020  ds".            
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000009c0: 616c 3a63 6f6e 7465 6e74 3d22 6469 6374  al:content="dict
-000009d0: 5f2f 656e 6473 222f 3e0a 0a20 2020 2020  _/ends"/>..     
-000009e0: 2020 2020 2020 203c 2f74 643e 0a20 2020         </td>.   
-000009f0: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
-00000a00: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000a10: 6976 2063 6c61 7373 3d22 6274 6e2d 6772  iv class="btn-gr
-00000a20: 6f75 7022 3e0a 2020 2020 2020 2020 2020  oup">.          
-00000a30: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
-00000a40: 6e20 636c 6173 733d 2262 746e 2062 746e  n class="btn btn
-00000a50: 2d64 6566 6175 6c74 2064 726f 7064 6f77  -default dropdow
-00000a60: 6e2d 746f 6767 6c65 2220 6461 7461 2d74  n-toggle" data-t
-00000a70: 6f67 676c 653d 2264 726f 7064 6f77 6e22  oggle="dropdown"
-00000a80: 3e3c 7370 616e 2063 6c61 7373 3d22 6361  ><span class="ca
-00000a90: 7265 7422 3e3c 2f73 7061 6e3e 3c2f 6275  ret"></span></bu
-00000aa0: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
-00000ab0: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
-00000ac0: 6173 733d 2264 726f 7064 6f77 6e2d 6d65  ass="dropdown-me
-00000ad0: 6e75 223e 0a20 2020 2020 2020 2020 2020  nu">.           
-00000ae0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-00000af0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000b00: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00000b10: 2074 616c 3a63 6f6e 6469 7469 6f6e 3d22   tal:condition="
-00000b20: 6469 6374 5f2f 656d 6169 6c20 7c20 6e6f  dict_/email | no
-00000b30: 7468 696e 6722 0a20 2020 2020 2020 2020  thing".         
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2020 2020 6872 6566 3d22 6d61 696c        href="mail
-00000b60: 746f 3a68 6569 6e7a 406b 756e 7a22 0a20  to:heinz@kunz". 
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00000b90: 6c3a 6174 7472 6962 7574 6573 3d22 6872  l:attributes="hr
-00000ba0: 6566 2073 7472 696e 673a 6d61 696c 746f  ef string:mailto
-00000bb0: 3a24 7b64 6963 745f 2f65 6d61 696c 7d22  :${dict_/email}"
-00000bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 6931 386e 3a74 7261 6e73 6c61 7465 3d22  i18n:translate="
-00000bf0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c10: 2020 2043 6f6e 7461 6374 0a20 2020 2020     Contact.     
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 2020 2020 3c61 2063 6c61 7373          <a class
-00000c60: 3d22 636f 6e66 6972 6d2d 6765 6e65 7261  ="confirm-genera
-00000c70: 6c22 0a20 2020 2020 2020 2020 2020 2020  l".             
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 6872 6566 3d22 2322 0a20 2020 2020    href="#".     
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 2020 2020 2020 7461 6c3a 6174            tal:at
-00000cc0: 7472 6962 7574 6573 3d22 6872 6566 2073  tributes="href s
-00000cd0: 7472 696e 673a 247b 636f 6e74 6578 742f  tring:${context/
-00000ce0: 6162 736f 6c75 7465 5f75 726c 7d2f 4040  absolute_url}/@@
-00000cf0: 6772 6f75 7064 6573 6b74 6f70 2f73 6574  groupdesktop/set
-00000d00: 5f65 6e64 5f6f 665f 6772 6f75 705f 6d65  _end_of_group_me
-00000d10: 6d62 6572 7368 6970 5f74 6f5f 746f 6461  mbership_to_toda
-00000d20: 793f 6769 643d 247b 6769 647d 2675 7365  y?gid=${gid}&use
-00000d30: 725f 6964 3d24 7b64 6963 745f 2f69 647d  r_id=${dict_/id}
-00000d40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2069 3138 6e3a 7472 616e 736c 6174 653d   i18n:translate=
-00000d70: 2222 3e0a 2020 2020 2020 2020 2020 2020  "">.            
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 2020 2020 456e 6420 6d65 6d62 6572 7368      End membersh
-00000da0: 6970 0a20 2020 2020 2020 2020 2020 2020  ip.             
-00000db0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000dc0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00000dd0: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
-00000de0: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-00000df0: 2020 2020 2020 203c 2f75 6c3e 0a20 2020         </ul>.   
-00000e00: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000e10: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000e20: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-00000e30: 2020 2020 3c2f 7462 6f64 793e 0a20 2020      </tbody>.   
-00000e40: 203c 2f74 6162 6c65 3e0a 0a0a 0a20 2020   </table>....   
-00000e50: 203c 2f6d 6574 616c 3a62 6c6f 636b 3e0a   </metal:block>.
-00000e60: 3c2f 6d65 7461 6c3a 626c 6f63 6b3e 0a0a  </metal:block>..
-00000e70: 3c2f 6d65 7461 6c3a 626c 6f63 6b3e 0a    </metal:block>.
+000002f0: 6279 5f69 6428 6769 6429 3b0a 6772 6f75  by_id(gid);.grou
+00000300: 705f 6c61 6265 6c20 7079 7468 6f6e 3a67  p_label python:g
+00000310: 726f 7570 5f69 6e66 6f2e 6765 7428 2767  roup_info.get('g
+00000320: 726f 7570 5f74 6974 6c65 2729 3b0a 2020  roup_title');.  
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 2020 2020 2020 2061 6273 7572             absur
+00000350: 6c20 7079 7468 6f6e 3a63 6f6e 7465 7874  l python:context
+00000360: 2e61 6273 6f6c 7574 655f 7572 6c28 293b  .absolute_url();
+00000370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000380: 2020 2020 2020 2020 2020 2020 2020 223e                ">
+00000390: 0a0a 2020 2020 3c68 3120 636c 6173 733d  ..    <h1 class=
+000003a0: 2264 6f63 756d 656e 7446 6972 7374 4865  "documentFirstHe
+000003b0: 6164 696e 6722 0a20 2020 2020 2020 2074  ading".        t
+000003c0: 616c 3a63 6f6e 6469 7469 6f6e 3d22 6772  al:condition="gr
+000003d0: 6f75 705f 6c61 6265 6c22 0a20 2020 2020  oup_label".     
+000003e0: 2020 2069 3138 6e3a 7472 616e 736c 6174     i18n:translat
+000003f0: 653d 2222 3e0a 2020 2020 2020 2020 4772  e="">.        Gr
+00000400: 6f75 7020 6164 6d69 6e69 7374 7261 7469  oup administrati
+00000410: 6f6e 2066 6f72 0a20 2020 2020 2020 203c  on for.        <
+00000420: 7461 6c3a 626c 6f63 6b20 7461 6c3a 636f  tal:block tal:co
+00000430: 6e74 656e 743d 2267 726f 7570 5f6c 6162  ntent="group_lab
+00000440: 656c 220a 2020 2020 2020 2020 2020 2020  el".            
+00000450: 2020 2020 2020 2069 3138 6e3a 6e61 6d65         i18n:name
+00000460: 3d22 7661 6c75 6522 2f3e 0a20 2020 203c  ="value"/>.    <
+00000470: 2f68 313e 0a3c 7461 6c3a 6e6f 6c61 6265  /h1>.<tal:nolabe
+00000480: 6c0a 2020 2020 2020 2020 7461 6c3a 636f  l.        tal:co
+00000490: 6e64 6974 696f 6e3d 226e 6f74 3a67 726f  ndition="not:gro
+000004a0: 7570 5f6c 6162 656c 223e 0a20 2020 203c  up_label">.    <
+000004b0: 6831 2063 6c61 7373 3d22 646f 6375 6d65  h1 class="docume
+000004c0: 6e74 4669 7273 7448 6561 6469 6e67 220a  ntFirstHeading".
+000004d0: 2020 2020 2020 2020 6931 386e 3a74 7261          i18n:tra
+000004e0: 6e73 6c61 7465 3d22 223e 0a20 2020 2020  nslate="">.     
+000004f0: 2020 2047 726f 7570 2061 646d 696e 6973     Group adminis
+00000500: 7472 6174 696f 6e20 666f 720a 2020 2020  tration for.    
+00000510: 2020 2020 3c74 7420 7461 6c3a 636f 6e74      <tt tal:cont
+00000520: 656e 743d 2267 6964 220a 2020 2020 2020  ent="gid".      
+00000530: 2020 2020 2020 6931 386e 3a6e 616d 653d        i18n:name=
+00000540: 2276 616c 7565 223e 0a20 2020 2020 2020  "value">.       
+00000550: 2067 726f 7570 5f69 640a 2020 2020 2020   group_id.      
+00000560: 2020 3c2f 7474 3e0a 2020 2020 3c2f 6831    </tt>.    </h1
+00000570: 3e0a 3c70 2069 3138 6e3a 7472 616e 736c  >.<p i18n:transl
+00000580: 6174 653d 2222 3e3c 7374 726f 6e67 3e4e  ate=""><strong>N
+00000590: 6f74 653a 3c2f 7374 726f 6e67 3e0a 5765  ote:</strong>.We
+000005a0: 2063 6f75 6c64 6e27 7420 6765 7420 6120   couldn't get a 
+000005b0: 7469 746c 6520 666f 7220 7468 6973 2067  title for this g
+000005c0: 726f 7570 3b20 7065 7268 6170 7320 6974  roup; perhaps it
+000005d0: 2064 6f65 736e 2774 2065 7869 7374 2079   doesn't exist y
+000005e0: 6574 3f0a 3c65 6d3e 2850 726f 6365 6564  et?.<em>(Proceed
+000005f0: 206f 6e20 796f 7572 206f 776e 2072 6973   on your own ris
+00000600: 6b20 2668 656c 6c69 703b 293c 2f65 6d3e  k &hellip;)</em>
+00000610: 0a3c 2f70 3e0a 3c2f 7461 6c3a 6e6f 6c61  .</p>.</tal:nola
+00000620: 6265 6c3e 0a20 2020 203c 6469 7620 636c  bel>.    <div cl
+00000630: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00000640: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00000650: 6f6c 2d6d 642d 3622 3e0a 2020 2020 2020  ol-md-6">.      
+00000660: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000670: 3d22 6c69 7374 696e 672d 6974 656d 223e  ="listing-item">
+00000680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000690: 203c 6469 7620 636c 6173 733d 2262 6f78   <div class="box
+000006a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000006b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000006c0: 733d 2274 6974 6c65 223e 0a20 2020 2020  s="title">.     
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 203c 6833 2069 3138 6e3a 7472 616e     <h3 i18n:tran
+000006f0: 736c 6174 653d 2222 3e54 414e 204d 616e  slate="">TAN Man
+00000700: 6167 6572 3c2f 6833 3e0a 2020 2020 2020  ager</h3>.      
+00000710: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000720: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000730: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000740: 2020 2020 2020 2020 2020 2020 3c75 6c3e              <ul>
+00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000760: 2020 2020 203c 6c69 3e0a 2020 2020 2020       <li>.      
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 3c61 2074 616c 3a61 7474 7269 6275    <a tal:attribu
+00000790: 7465 733d 2268 7265 6620 7374 7269 6e67  tes="href string
+000007a0: 3a24 7b61 6273 7572 6c7d 2f63 7265 6174  :${absurl}/creat
+000007b0: 655f 7461 6e3f 6769 643d 247b 6769 647d  e_tan?gid=${gid}
+000007c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000007d0: 2020 2020 2020 2020 2020 2020 2069 3138               i18
+000007e0: 6e3a 7472 616e 736c 6174 653d 2222 3e0a  n:translate="">.
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 2020 2043 7265 6174             Creat
+00000810: 6520 5441 4e0a 2020 2020 2020 2020 2020  e TAN.          
+00000820: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000830: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
+00000840: 2020 2020 2020 203c 2f6c 693e 0a20 2020         </li>.   
+00000850: 2020 2020 2020 2020 2020 2020 203c 2f75               </u
+00000860: 6c3e 0a20 2020 2020 2020 2020 2020 203c  l>.            <
+00000870: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
+00000880: 6469 763e 0a20 2020 2020 2020 203c 6469  div>.        <di
+00000890: 7620 636c 6173 733d 2263 6f6c 2d6d 642d  v class="col-md-
+000008a0: 3622 3e0a 2020 2020 2020 2020 2020 2020  6">.            
+000008b0: 3c64 6976 2063 6c61 7373 3d22 6c69 7374  <div class="list
+000008c0: 696e 672d 6974 656d 223e 0a20 2020 2020  ing-item">.     
+000008d0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000008e0: 636c 6173 733d 2262 6f78 223e 0a20 2020  class="box">.   
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 203c 6469 7620 636c 6173 733d 2274 6974   <div class="tit
+00000910: 6c65 223e 0a20 2020 2020 2020 2020 2020  le">.           
+00000920: 2020 2020 2020 2020 2020 2020 203c 6833               <h3
+00000930: 2069 3138 6e3a 7472 616e 736c 6174 653d   i18n:translate=
+00000940: 2222 3e47 726f 7570 204d 616e 6167 656d  "">Group Managem
+00000950: 656e 743c 2f68 333e 0a20 2020 2020 2020  ent</h3>.       
+00000960: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00000970: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000980: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000990: 2020 2020 2020 2020 2020 203c 756c 3e0a             <ul>.
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2020 2020 3c6c 693e 0a20 2020 2020 2020      <li>.       
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 203c 6120 7461 6c3a 6174 7472 6962 7574   <a tal:attribut
+000009e0: 6573 3d22 6872 6566 2073 7472 696e 673a  es="href string:
+000009f0: 247b 6162 7375 726c 7d2f 6772 6f75 705f  ${absurl}/group_
+00000a00: 6164 6d69 6e69 7374 7261 7469 6f6e 5f75  administration_u
+00000a10: 7365 725f 7669 6577 3f67 6964 3d24 7b67  ser_view?gid=${g
+00000a20: 6964 7d22 0a20 2020 2020 2020 2020 2020  id}".           
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 6931 386e 3a74 7261 6e73 6c61 7465 3d22  i18n:translate="
+00000a50: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000a60: 2020 2020 2020 2020 2020 2020 2020 4d61                Ma
+00000a70: 6e61 6765 2067 726f 7570 206d 656d 6265  nage group membe
+00000a80: 7273 6869 7073 0a20 2020 2020 2020 2020  rships.         
+00000a90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000aa0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
+00000ab0: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 2020 3c6c 693e 0a20 2020 2020 2020 2020    <li>.         
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000af0: 6120 7461 6c3a 6174 7472 6962 7574 6573  a tal:attributes
+00000b00: 3d22 6872 6566 2073 7472 696e 673a 247b  ="href string:${
+00000b10: 6162 7375 726c 7d2f 6772 6f75 705f 6164  absurl}/group_ad
+00000b20: 6d69 6e69 7374 7261 7469 6f6e 5f6c 6561  ministration_lea
+00000b30: 726e 696e 675f 7072 6f67 7265 7373 5f76  rning_progress_v
+00000b40: 6965 773f 6769 643d 247b 6769 647d 220a  iew?gid=${gid}".
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 2020 2020 2020 2020 2069 3138 6e3a             i18n:
+00000b70: 7472 616e 736c 6174 653d 226c 6561 726e  translate="learn
+00000b80: 696e 6770 726f 6772 6573 7322 3e0a 2020  ingprogress">.  
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 2020 2020 204c 6561 726e 696e           Learnin
+00000bb0: 6720 7072 6f67 7265 7373 0a20 2020 2020  g progress.     
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 203c 2f61 3e0a 2020 2020 2020 2020     </a>.        
+00000be0: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
+00000bf0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000c00: 2020 3c2f 756c 3e0a 2020 2020 2020 2020    </ul>.        
+00000c10: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000c20: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
+00000c30: 6469 763e 0a20 2020 203c 2f6d 6574 616c  div>.    </metal
+00000c40: 3a62 6c6f 636b 3e0a 3c2f 6d65 7461 6c3a  :block>.</metal:
+00000c50: 626c 6f63 6b3e 0a0a 3c2f 6d65 7461 6c3a  block>..</metal:
+00000c60: 626c 6f63 6b3e 0a                        block>.
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/oldcrumbs.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/oldcrumbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 # visaplan:
 from visaplan.plone.base.typestr import plu2import_label, plu2tup, view2plu
 from visaplan.plone.breadcrumbs.base import (
     BaseCrumb,
     DesktopBrowserCrumb,
     RootedCrumb,
+    SkipCrumbException,
     ViewCrumb,
     register,
     tellabout_call,
     )
 from visaplan.plone.breadcrumbs.utils import (
     crumbdict,
     delete_last_nonfolderish_basecrumb,
     )
 from visaplan.tools.minifuncs import translate_dummy as _
 
 # Logging / Debugging:
+from pdb import set_trace
 from visaplan.plone.tools.log import getLogSupport
+from visaplan.tools.debug import pp
 
 logger, debug_active, DEBUG = getLogSupport(defaultFromDevMode=False)
 
 
 # ---------------------------------------------- [ Crumb-Klassen ... [
 class DesktopCrumbs(BaseCrumb):
     """
@@ -38,30 +41,38 @@
     def tweak(self, crumbs, hub, info, override):
         # override: Schreibtischerkennung übersteuern
         if crumbs[1:] and not override:
             if info['skip_desktop_crumbs']:
                 return
             info['skip_desktop_crumbs'] = True
             # return
+        if not info['user_id']:
+            return
         if not info['personal_desktop_done']:
             delete_last_nonfolderish_basecrumb(info, crumbs)
             # Schreibtisch nur einmal erzeugen:
             crumbs.append(
                     crumbdict(hub['translate']('myUNITRACC'),
                               info['desktop_url']))
             # die die Gruppenangabe auswerten und ggf. in die Sitzungsdaten
             # schreiben:
             info['personal_desktop_done'] = True
         if not info['group_desktop_done']:
             # Gruppenschreibtisch:
             if info['gid'] is not None:
-                crumbs.append(
-                    crumbdict(info['group_title'],
-                              '%(desktop_url)s?gid=%(gid)s'
-                              % info))
+                group_title = info.get('group_title', None)
+                if group_title:
+                    crumbs.append(
+                        crumbdict(group_title,
+                                  '%(desktop_url)s?gid=%(gid)s'
+                                  % info))
+                else:
+                    msg = 'DesktopCrumbs: No title for group %(uid)r!' % info
+                    logger.error(msg)
+                    raise SkipCrumbException()
             info['group_desktop_done'] = True
 
     def __call__(self, crumbs, hub, info, override=None):
         for parent in self.parents:
             parent(crumbs, hub, info)
         self.tweak(crumbs, hub, info, override)
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-articles.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-articles.pt`

 * *Files 8% similar despite different names*

```diff
@@ -32,20 +32,14 @@
                  tal:define="dummy python:request.set('disable_border', 1)" />
     <metal:no-ads fill-slot="column_one_slot"/>
     <metal:no-ads fill-slot="column_two_slot"/>
 
 <body>
 
 
-<metal:cr_outer fill-slot="breadcrumb">
-<!-- [ our-articles.pt: fülle Slot breadcrumb ... [ -->
-    <metal:macro use-macro="here/crumbs/macros/main"/>
-<!-- ] ... our-articles.pt: fülle Slot breadcrumb ] -->
-</metal:cr_outer>
-
 <metal:main fill-slot="main"
             tal:define="
 hai hai | context/hubandinfo/get;
 hub python:hai['hub'];
 info python:hai['info'];
 groupdesktop python:hub['groupdesktop'];
 grpinfo python:groupdesktop.getInfo(topic, hub=hub, info=info);
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
 
-
 ****** Unsere Artikel ******
 
 Please note that your articles have to be submitted so that they can be
 reviewed by the editorial staff of UNITRACC and be considered for the
 publication plan. When an article has been accepted by UNITRACC, you will no
 longer be able to edit the respective content.
 Ein speziell angepaÃter Hinweistext, sofern ein solcher fÃ¼r die Message-ID
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/our-images.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/our-images.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupdesktop/utils.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupdesktop/utils.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/update-0001.sql` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/update-0001.sql`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/sql/update-0003.sql` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/sql/update-0003.sql`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/browser.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,38 @@
 # Python compatibility:
 from __future__ import absolute_import, print_function
 
 from six import string_types as six_string_types
 from six import text_type as six_text_type
 from six.moves import map
 
+# Standard library:
+from collections import defaultdict
+from datetime import date, datetime, timedelta
+from time import localtime, time
+
 # Zope:
+import transaction
 from AccessControl import Unauthorized
+from Products.CMFCore.utils import getToolByName
 from Products.PluggableAuthService.interfaces.plugins import (
     IGroupEnumerationPlugin,
     )
+from zope.component import getMultiAdapter
+from zope.site.hooks import getSite
 
 # visaplan:
-from visaplan.plone.base import BrowserView, Interface, implements
+from visaplan.plone.base import BrowserView, implements
 
 try:
     # Zope:
     from Globals import DevelopmentMode
 except ImportError:
     # Hotfix for Zope 4; how to properly replace this?
     DevelopmentMode = False
-# Standard library:
-from collections import defaultdict
-from datetime import date, datetime, timedelta
-from time import localtime, time
-
-# Zope:
-import transaction
-from Products.CMFCore.utils import getToolByName
-from zope.component import getMultiAdapter
-from zope.site.hooks import getSite
 
 # 3rd party:
 from psycopg2._psycopg import IntegrityError, InterfaceError, InternalError
 
 # visaplan:
 from visaplan.plone.base.permissions import (
     ManageCourses,
@@ -51,34 +50,46 @@
     )
 from visaplan.plone.tools.context import getbrain, message
 from visaplan.plone.tools.forms import (
     back_to_referer,
     detect_duplicates,
     tryagain_url,
     )
+from visaplan.plone.tools.groups import (
+    build_groups_set,
+    get_all_members,
+    groupinfo_factory,
+    is_direct_member__factory,
+    is_member_of__factory,
+    is_member_of_any,
+    userinfo_factory,
+    )
 from visaplan.tools.classes import Proxy
 from visaplan.tools.coding import safe_decode
 from visaplan.tools.dates import make_date_formatter
 from visaplan.tools.lands0 import list_of_strings
 from visaplan.tools.minifuncs import makeBool
 from visaplan.tools.profile import StopWatch
 
 # Local imports:
+from .interface import IGroupSharing
 from .utils import (
-    build_groups_set,
     datefromform,
     default_dates_dict,
     getcoursetitle,
     getgrouptitle,
     gettitle,
     journal_text,
     make_break_at_row,
     make_keyfunction,
     makedate,
-    recursive_members,
+    )
+from visaplan.plone.groups.infofact import (
+    get_group_mapping_course__factory,
+    memberinfo_factory,
     )
 from visaplan.plone.groups.unitraccgroups.utils import (
     ALL_GROUP_SUFFIXES,
     ALUMNI_SUFFIX,
     LEARNER_SUFFIX,
     pretty_group_title,
     split_group_id,
@@ -118,181 +129,18 @@
     from Products.zkb.config import MORE_BORING_GROUPS
     BORING_GROUPS.update(MORE_BORING_GROUPS)
 except:
     pass
 # siehe auch @@groupdesktop.STATIC_GROUPS_BLACKLIST, ...ANONYMOUS_GROUPS
 
 ANCIENT_PAST = makedate('31.12.1999')
-USE_ZOPE_METHODS = 0
+USE_ZOPE_METHODS = 1
 SECS_PER_DAY = 24 * 3600
 ALUMNI_CUT = - (len(ALUMNI_SUFFIX) + 1)  # zum Abschneiden
 
-
-class IGroupSharing(Interface):
-
-    def canManage(self):
-        """
-        Darf der angemeldete Benutzer diese Gruppe bzw., wenn keine angegeben:
-        alle Gruppen bearbeiten?
-        """
-
-    def authManage(self):
-        """
-        Wirft ggf. Unauthorized
-        """
-
-    def get_group_info_by_id(self, group_id, pretty=0, getObject=0):
-        """
-        Gib ein Dict. zurück;
-        - immer vorhandene Schlüssel: id, group_title, group_description
-        - nur bei automatisch erzeugten Gruppen: role, role_translation, brain
-        """
-
-    def get_groups_by_user_id(self, user_id, explicit=True, askdb=None):
-        """
-        Gib eine sortierte Liste von Gruppen-Info-Dictionarys zurück.
-        """
-
-    def get_user_and_all_groups(self, uogid):
-        """
-        Ermittle die IDs aller Gruppen, denen der übergebene User (oder die
-        Gruppe -- uogid) angehört - abzgl. der üblichen Ausnahme
-        'AuthenticatedUsers'.
-        Gib ein 2-Tupel zurück:
-
-        (user_id, set(group_ids))
-
-        Wenn die übergebene ID <uogid> zu einem User gehört, wird sie aus dem
-        Set der Gruppen-IDs entfernt und im ersten Teil des Tupels
-        zurückgegeben; ansonsten ist dieser erste Teil None.
-        """
-
-    def delete_group_membership_by_group_id(self):
-        """
-        Aufgerufen aus manage_group_view;
-        die Gruppenzuordnungen sollen hier *tatsächlich*
-        spurlos beseitigt werden! (Aufräumfunktion)
-
-        Formularfelder:
-        ids -- eine Liste von Member-IDs
-        group_id -- die aufzuräumende Gruppe
-        """
-
-    def add_group_membership(self):
-        """
-        Füge *einen* Benutzer (oder eine Gruppe)
-        einer oder mehreren Gruppen hinzu
-
-        Startdatum ist heute;
-        ein Endedatum wird nicht gesetzt.
-
-        Siehe auch --> add_to_group (mehrere Benutzer, eine Gruppe,
-        variable Datumswerte)
-        """
-
-    def end_group_memberships(self):
-        """
-        *Beende* Gruppenmitgliedschaften (ohne sie spurlos zu entfernen)
-        """
-
-    def delete_group_memberships(self):
-        """
-        Zum Aufruf aus Formularen: *Entferne* Gruppenmitgliedschaften
-        (und lösche sie aus der relationalen Datenbank)
-        """
-
-    def search_groups(self, string_='', sort_=True):
-        """ """
-
-    def get_explicit_group_memberships(self, group_id):
-        """
-        gib die Benutzer und Gruppen zurück, die direkte Mitglieder
-        der übergebenen Gruppe sind
-        """
-
-    def search_groups_and_users(self, string_=''):
-        """ """
-
-    def add_to_group(self):
-        """
-        Füge Benutzer und/oder Gruppen einer Gruppe hinzu.
-        Formulardaten:
-
-        Formular   | Feldname   | Erklärung
-        -----------+------------+----------------------------------------
-        group_id   | group_id_  | ursprünglich ging es nur um Kursgruppen
-        ids:list   | member_id_ | ursprünglich "(Schul-) Klassen", jetzt
-                   |            | allgemein Benutzer- oder Gruppen-IDs
-        start_<id> | start      | Startdatum, d.m.yyyy, default: heute
-        end_<id>   | ends       | Ablaufdatum, d.m.yyyy, default: leer
-        """
-
-    def delete_groups(self):
-        """ """
-
-    def update_group(self):
-        """ """
-
-    def can_view_unitracc_groups(self):
-        """
-        für Schema: regelt den Zugriff auf das Gruppenfreigabe-Widget
-        """
-
-    def get_permission_authors(self):
-        """ """
-
-    def get_custom_search_authors(self):
-        """ """
-
-    def get_group_memberships(self, group_id, explicit=True):
-        """
-        Gib alle Gruppen zurück, deren direktes Mitglied die
-        übergebene Gruppe ist
-        (ACHTUNG, Argument 'explicit' wird bisher nicht berücksichtigt!)
-        """
-
-    def connect_groups(self):
-        """ Verbindet manuell erstellte Gruppen mit automatisch erstellten Kursgruppen. """
-
-    def disconnect_groups(self):
-        """
-        Trennt manuell erstellte Gruppen von automatisch erstellten Kursgruppen.
-        """
-
-    def scheduled_group_memberships(self):
-        """
-        Arbeite die Gruppenzuordnungen ab gemäß der Tabelle
-        unitracc_groupmemberships (neuer cron-Job).
-        """
-
-    def update_view_duration(self):
-        """ Aktualisiert die eingetragenen Daten für die Gruppenzugehörigkeitsdauer """
-
-    def replay_groups(self):
-        """
-        Gruppenzuordnungen "nachholen".  Da die Formulardaten Datumswerte
-        enthalten können, darf das nur von einem Admin gemacht werden.
-        """
-
-    def get_course_info_for_group_ids(self, group_ids):
-        """ """
-
-    def get_group_manager_for_group_id(self, group_id):
-        """ """
-
-    def is_member_of_any(self, group_ids, user_id=None, default=False):
-        """
-        Ist der übergebene Benutzer Mitglied einer der übergebenen Gruppen?
-
-        - wenn user_id nicht übergeben wird, wird der angemeldete Benutzer
-          verwendet
-        - wenn die Liste der Gruppen-IDs leer ist, wird der Vorgabewert
-          verwendet (default)
-        """
-
 PRETTY_MASK = {}
 for role in ALL_GROUP_SUFFIXES:
     PRETTY_MASK[role] = u'%s group "{group}"' % role
 if 0 and 'nur fuer den Parser':
     _('Author group "{group}"')
     _('Reader group "{group}"')
     _('learner group "{group}"')
@@ -447,15 +295,15 @@
         """
 
         context = self.context
 
         #Remove dummy group
         group_ids = self._get_filtered_groups(user_id)
         list_ = []
-        ggibi = groupinfo_factory(self.context, pretty=pretty)
+        ggibi = groupinfo_factory(context, pretty=pretty)
         if explicit:
             is_direct_member_of = is_direct_member__factory(context, user_id)
             for group_id in group_ids:
                 if is_direct_member_of(group_id):
                     list_.append(ggibi(group_id))
             if askdb:
                 # Gruppen-IDs lt. Zope sind definitiv:
@@ -596,15 +444,15 @@
         return group_ids
 
     def get_all_groups(self, pretty=False):
         """
         Gib Gruppeninformationen von allen Gruppen zurück,
         bis auf die langweiligen.
         """
-        ggibi = groupinfo_factory(self.context, pretty)
+        ggibi = groupinfo_factory(self.context, pretty=pretty)
         return sorted([ggibi(gid)
                        for gid in self.get_all_group_ids()
                        ],
                       key=getgrouptitle)
 
     def _get_filtered_groups(self, id):
         """
@@ -626,39 +474,54 @@
             if group:
                 group_ids = set(group.getGroups())
 
         rslt = sorted(group_ids.difference(BORING_GROUPS))
         DBG_P('_get_filtered_groups(%r) --> %s', id, rslt)    # DEBUG
         return rslt
 
-    def get_user_and_all_groups(self, uogid):
+    def get_user_and_all_groups(self, uogid, **kwargs):
         """
         Ermittle die IDs aller Gruppen, denen der übergebene User (oder die
         Gruppe -- uogid) angehört - abzgl. der üblichen Ausnahme
         'AuthenticatedUsers'.
         Gib ein 2-Tupel zurück:
 
         (user_id, set(group_ids))
 
         Wenn die übergebene ID <uogid> zu einem User gehört, wird sie aus dem
         Set der Gruppen-IDs entfernt und im ersten Teil des Tupels
         zurückgegeben; ansonsten ist dieser erste Teil None.
         """
         global USE_ZOPE_METHODS
+        pop = kwargs.pop
+        assert_user = pop('useronly', 0)
+        if kwargs:
+            raise TypeError('Unsupported keyword argument(s)! '
+                            '%s' % (tuple(sorted(set(kwargs))),
+                                    ))
         with StopWatch('@@gs.guaag(%r): USE_ZOPE_METHODS=%r'
                        % (uogid, USE_ZOPE_METHODS),
                        **sw_kwargs) as stopwatch:
             context = self.context
             acl = getToolByName(context, 'acl_users')
-            if USE_ZOPE_METHODS:
+            if USE_ZOPE_METHODS or 1:
                 uogo = acl.getUser(uogid)  # "user or group object"
-                if uogo is None:
+                is_user = uogo is not None
+                if not is_user:
+                    if assert_user:
+                        raise ValueError('User %(uogid)r not found; '
+                                         "I'm not interested in groups!"
+                                         % locals())
                     uogo = acl.getGroup(uogid)
-                group_ids = acl.source_groups.getGroupsForPrincipal(uogo)
-                is_user = uogid not in acl.source_groups._group_principal_map
+                if not uogo:
+                    logger.error('User or group %(uogid)r not found!', locals())
+                    return (None, [])
+
+                group_ids = set(uogo.getGroups())  # WORKS for users
+                group_ids.difference_update(BORING_GROUPS)
                 gcount = len(group_ids)
                 if is_user:
                     return (uogid, group_ids)
                 else:
                     return (None, group_ids)
             else:
                 gpm = acl.source_groups._group_principal_map
@@ -866,14 +729,17 @@
 
     def get_courses_and_desktop_groups(self, user_id, gid=None):
         """
         Gib zwei Listen zurück (courses, desktops1):
         - die Kurse mit den schreibtischrelevanten Gruppen
         - die Gruppen, für die Schreibtische existieren
         """  # ----------------------------------------- [ gcadg ... [
+        # on the way obsoleting this method ... see:
+        # ../groupdesktop/browser.py (_get_courses_and_desktop_groups)
+        # ../base.py                 (my_groups)
         context = self.context
         getAdapter = context.getAdapter
         with StopWatch('@@gs.gcadg', **sw_kwargs) as stopwatch:
             is_direct_member_of = is_direct_member__factory(context, user_id)
             # Verwendung der Gruppeninfo sowohl für Kurse als auch für
             # Schreibtische; teure Berechnung puffern:
             group_info = Proxy(groupinfo_factory(context,
@@ -904,15 +770,15 @@
                     # dic wird auch für ungefilterte Kurse verwendet:
                     dic = group_info[group_id]
                     if is_direct_member_of(group_id):
                         if dic['group_desktop']:
                             desktops1.append(dic)
                         elif dic['group_manager'] == user_id:
                             desktops2.append(dic)
-                        elif id == gid:
+                        elif group_id == gid:
                             desktops2.append(dic)
                     role = dic.get('role')
                     if role == LEARNER_SUFFIX:
                         courses.append(get_mapping_group(group_id))
                     elif role == ALUMNI_SUFFIX:
                         alumni_gids.append(group_id)
                 stopwatch.lap('Alle Kurse des Users')
@@ -950,15 +816,15 @@
                         continue
                     if is_direct_member_of(group_id):
                         dic = group_info[group_id]
                         if dic['group_desktop']:
                             desktops1.append(dic)
                         elif dic['group_manager'] == user_id:
                             desktops2.append(dic)
-                        elif id == gid:
+                        elif group_id == gid:
                             desktops2.append(dic)
 
                 pg = getToolByName(context, 'portal_groups')
                 group = pg.getGroupById(gid)
                 if group:
                     all_groups_of_group = set(group.getGroups())
                 else:
@@ -1039,15 +905,15 @@
         - die der angegebene Benutzer administriert, oder
         - die aktuell ausgewählt ist (nach den echten Schreibtischgruppen)
 
         """
         context = self.context
         # context.getBrowser('authorized').managePortal()
         is_direct_member_of = is_direct_member__factory(context, user_id)
-        ggibi = groupinfo_factory(context, 1, 0)
+        ggibi = groupinfo_factory(context, pretty=1, forlist=0)
 
         list1 = []
         list2 = []
         for id in self._get_all_group_ids():
             if is_direct_member_of(id):
                 dic = ggibi(id)
                 if 0 and not list1:
@@ -1442,15 +1308,23 @@
         Aus edit_group_membership, "Aus ausgewählten Gruppen entfernen":
         löscht die Zuordnungen derzeit spurlos.
         """
         context = self.context
         groups = context.getBrowser('groups')
 
         group = groups.getById(group_id)
-        group.removeMember(user_id)
+        if group is not None:
+            group.removeMember(user_id)
+        else:
+            member_id = user_id
+            message(context,
+                    'Couldn\'t remove user "${member_id}" from non-existing '
+                    'group "${group_id}".',
+                    'error',
+                    locals())
         where = "WHERE member_id_=%(user_id)s AND group_id_=%(group_id)s"
         sql.delete("unitracc_groupmemberships",
                    where,
                    query_data={'user_id': user_id,
                                'group_id': group_id,
                                })
     # ----------------------------- ] ... Mitgliedschaften entfernen ]
@@ -1573,15 +1447,15 @@
                    |            | allgemein Benutzer- oder Gruppen-IDs
         start_<id> | start      | Startdatum, d.m.yyyy, default: heute
         end_<id>   | ends       | Ablaufdatum, d.m.yyyy, default: leer
         """
         context = self.context
         getAdapter = context.getAdapter
 
-        checkperm = getToolByName(self.context, 'portal_membership').checkPermission
+        checkperm = getToolByName(context, 'portal_membership').checkPermission
         if checkperm(ManageGroups, context):
             cg_only = False
         elif checkperm(ManageCourses, context):
             # hat noch keine Wirkung:
             cg_only = True  # "course groups only"
         else:
             raise Unauthorized
@@ -1632,15 +1506,14 @@
     def delete_groups(self):
         """ """
         # TODO: Vorab prüfen, ob die Gruppe(n) Mitglieder hat/haben;
         #       Information über Anzahl direkter und indirekter Mitglieder,
         #       und Löschen nur unter best. Bedingungen?
         context = self.context
 
-        getAdapter = context.getAdapter
         checkperm = getToolByName(context, 'portal_membership').checkPermission
         if not checkperm(ManageGroups, context):
             raise Unauthorized
 
         request = context.REQUEST
         form = request.form
         logger.debug('delete_groups: form=\n%s', pformat(form))
@@ -2210,16 +2083,24 @@
             return self._update_view_duration(group_id, member_id, sql,
                                               start, ends)
 
     @log_or_trace(debug_active, logger=logger)
     def _update_view_duration(self,  # -------------- [ _u.v.d() ... [
                               group_id, member_id,
                               sql,
-                              start, ends, TODAY=None):
+                              start=None, ends=None, TODAY=None):
         """
+        - Füge der Gruppe <group_id> das Mitglied <member_id> hinzu
+          (wenn die weiteren übergebenen Datumswerte None sind)
+          oder entferne es,
+        - pflege die entsprechenden Werte in die Tabelle
+          unitracc_groupmemberships ein,
+          und
+        - schreibe einen entsprechenden Absatz nach var/log/groups.txt
+
         1. Ermittle, ob der heutige Tag im Zeitraum der Zugehörigkeit liegt
         2. Trage neue Werte für Start und Ende für Benutzer und Gruppe in die
         Datenbank ein bzw. aktualisiere einen etwa schon vorhandenen Datensatz
         3. Setze oder entferne entsprechend die Zope-Gruppenzugehörigkeit
         4. Gib einen logischen Wert zurück, der informiert, ob die
         Gruppenmitgliedschaft nach Ausführung besteht (True) oder nicht (False).
 
@@ -2237,14 +2118,16 @@
                 now_active = True
             else:
                 now_active = TODAY < ends
         elif ends is None:
             now_active = start <= TODAY
         else:
             now_active = start <= TODAY < ends
+        if start is None and not nostart:
+            start = TODAY
         # ------------------------------ ... _update_view_duration ...
 
         # 2. Eintragung in Datenbank
         NEWDATA = {'start':  start,
                    'ends':   ends,
                    'active': now_active,
                    }
@@ -2293,27 +2176,37 @@
             sql.insert(table, NEWDATA)
 
         # 3. Zope-Gruppenzugehörigkeit
         context = self.context
         acl = getToolByName(context, 'acl_users')
         groups = context.getBrowser('groups')
         group_o = groups.getById(group_id)
-        members = acl.source_groups._group_principal_map[group_id]
-        if now_active:
-            if member_id not in members:
-                group_o.addMember(member_id)
-            else:
-                NEWDATA['active_before'] = True
-        else:
-            if member_id in members:
-                group_o.removeMember(member_id)
+        try:
+            members = acl.source_groups._group_principal_map[group_id]
+        except KeyError as e:
+            logger.error('Group %(group_id)r not found (anymore)', locals())
+            message(context,
+                    'Couldn\'t remove user "${member_id}" from non-existing '
+                    'group "${group_id}".',
+                    'error',
+                    locals())
+            group_title = None
+        else:
+            if now_active:
+                if member_id not in members:
+                    group_o.addMember(member_id)
+                else:
+                    NEWDATA['active_before'] = True
             else:
-                NEWDATA['active_before'] = False
-        ggibi = groupinfo_factory(context, forlist=1)
-        group_title = ggibi(group_id)['group_title']
+                if member_id in members:
+                    group_o.removeMember(member_id)
+                else:
+                    NEWDATA['active_before'] = False
+            ggibi = groupinfo_factory(context, forlist=1)
+            group_title = ggibi(group_id)['group_title']
         context.getAdapter('grouplog').row_updated(group_id=group_id,
                                                    group_title=group_title,
                                                    member_id=member_id,
                                                    **NEWDATA)
         return now_active  # --------- ] ... _update_view_duration() ]
 
     def get_group_manager_for_group_id(self, group_id):
@@ -2346,25 +2239,24 @@
 
         group_id -- wenn übergeben, wird nur genau diese eine verwendet
         pretty -- siehe groupinfo_factory
         forlist -- wenn von Manager aufgerufen,
                    kann die "kleine Info" besorgt werden (siehe den Code)
         """
         context = self.context
-        getAdapter = context.getAdapter
         checkperm = getToolByName(context, 'portal_membership').checkPermission
         is_group_manager = checkperm(ManageGroups, context)
         if is_group_manager:
             if forlist is None:
                 forlist = True
         else:
             forlist = False  # group_manager-Information wird benötigt
             user = getToolByName(context, 'portal_membership').getAuthenticatedMember()
             user_id = str(user)
-        ggibi = groupinfo_factory(self.context, pretty, forlist)
+        ggibi = groupinfo_factory(context, pretty=pretty, forlist=forlist)
         if group_id:
             group_ids = [group_id]
         elif is_group_manager:
             # alle interessanten:
             group_ids = self.get_all_group_ids()
         else:
             group_ids = set(user.getGroups()).difference(BORING_GROUPS)
@@ -2379,540 +2271,39 @@
         res.sort(key=getgrouptitle)
         return res
 
     def get_all_members(self, group_ids, **kwargs):
         """
         Liefere alle Mitglieder der übergebenen Gruppe(n).
 
-        Schlüsselwortargumente für .utils.recursive_members und
-        groupinfo_factory dürfen angegeben werden;
+        Schlüsselwortargumente für recursive_members und groupinfo_factory
+        (visaplan.plone.tools.groups) dürfen angegeben werden;
         letztere werden aber ignoriert, wenn die vorgabegemäße Filterung
         groups_only=True übersteuert wird. In diesem Fall (potentiell sowohl
         Benutzer als auch Gruppen, oder nur Benutzer) werden nur IDs
         zurückgegeben.
 
         Rückgabe:
         - Sequenz von Gruppeninformationen, mit groups_only=True (Vorgabe);
         - ansonsten nur eine Sequenz der IDs (je nach Aufrufargumenten nur
           Benutzer-IDs, oder gemischt)
         """
-        context = self.context
-        acl = getToolByName(context, 'acl_users')
-        gpm = acl.source_groups._group_principal_map
-        filter_args = {}
-        for key in ('groups_only', 'users_only',
-                    'containers',
-                    'default_to_all'):
-            try:
-                filter_args[key] = kwargs.pop(key)
-            except KeyError:
-                pass
-        members = recursive_members(list_of_strings(group_ids),
-                                    gpm, **filter_args)
-        groups_only = filter_args.get('groups_only', False)
-        if groups_only:
-            format_args = {'pretty': False,
-                           'forlist': True,
-                           }
-            format_args.update(kwargs)
-            ggibi = groupinfo_factory(context, **format_args)
-            res = []
-            for gid in members:
-                res.append(ggibi(gid))
-            return res
-        elif kwargs and debug_active:
-            pp('ignoriere:', kwargs)
-
-        return members
+        return get_all_members(self.context, group_ids, **kwargs)
 
     def is_member_of_any(self, group_ids, user_id=None, default=False):
         """
         Ist der übergebene Benutzer Mitglied einer der übergebenen Gruppen?
 
         - wenn user_id nicht übergeben wird, wird der angemeldete Benutzer
           verwendet
         - wenn die Liste der Gruppen-IDs leer ist, wird der Vorgabewert
           verwendet (default)
         """
-        context = self.context
-        getBrowser = context.getBrowser
-        getBrowser('authorized').raiseAnon()
-        if user_id is not None:
-            # wer darf sowas fragen? Manager, Gruppenmanager, ...?
-            # TODO: Hier entsprechende Überprüfung!
-            pass
-
-        if not group_ids:
-            return default
-        if user_id is None:
-            member = getToolByName(context, 'portal_membership').getAuthenticatedMember()
-            user_id = member.getId()
-
-        return user_id in self.get_all_members(group_ids)
+        return is_member_of_any(self.context, group_ids, user_id, default)
 
 
 # ----------------------------------------- [ Factory-Funktionen ... [
-def is_direct_member__factory(context, userid):
-    """
-    Erzeuge eine Funktion, die prüft, ob der *beim Erzeugen angegebene* Nutzer
-    in der bei jedem Aufruf anzugebenden Gruppe direkt enthalten ist.
-    """
-    acl = getToolByName(context, 'acl_users')
-    gpm = acl.source_groups._group_principal_map
-    # <BTrees.OOBTree.OOBTree object at ...>
-    # print 'gpm: %(gpm)r' % locals()
-
-    def is_direct_member_of(group_id):
-        return userid in gpm[group_id]
-
-    return is_direct_member_of
-
-
-def is_member_of__factory(context, userid):
-    """
-    Erzeuge eine Funktion, die die *direkte oder indirekte* Mitgliedschaft
-    des übergebenen Users in der jeweils zu übergebenden Gruppe überprüft.
-    """
-    acl = getToolByName(context, 'acl_users')
-    gpm = acl.source_groups._group_principal_map
-    # <BTrees.OOBTree.OOBTree object at ...>
-    # print 'gpm: %(gpm)r' % locals()
-
-    groups = build_groups_set(gpm, userid)
-
-    def is_member_of(groupid):
-        return groupid in groups
-
-    return is_member_of
-
-
-def get_group_mapping_course__factory(context, group_ids, group_info):
-    """
-    "get (the) group mapping (the) course"
-
-    Erzeuge eine Funktion, die die Gruppe zurückgibt, die
-    - die übergebene Kursgruppe vermittelt, und
-    - einen Schreibtisch erzeugt
-
-    Argumente:
-    group_ids - vorab ermittelte Menge aller interessierenden Gruppen
-                (in denen der Benutzer direkt oder indirekt Mitglied ist)
-    group_info - ein dict-Objekt zur Pufferung aller angeforderten
-                 Gruppen-Infos (siehe visaplan.tools.classes.Proxy)
-    """
-    getAdapter = context.getAdapter
-    acl = getToolByName(context, 'acl_users')
-    gpm = acl.source_groups._group_principal_map
-
-    def get_group_mapping_course(coursegroup_id):
-        """
-        Gib die erste Gruppe zurück, die die übergebene Kursgruppe vermittelt
-
-        coursegroup_id - die ID einer primären Kursgruppe, die evtl. einen
-                         Schreibtisch erzeugt, wahrscheinlich aber nicht
-
-        Das Ergebnis enthält:
-        - garantiert den Schlüssel 'coursegroup_id'
-        - einen Schlüssel 'stats' für die (hier nicht gefüllte!) Statistik
-        - UID, Title und Brain des Kurses
-        - im Erfolgsfall die Gruppeninfo der nächsten vermittelnden Gruppe
-          (bei user_id -> group_a -> group_b -> group_abc123_learner wäre das
-          die der Gruppe group_a)
-        """
-        course_uid, pseudorole = coursegroup_id.split('_')[1:]
-        course_brain = getbrain(context, course_uid)
-        dic2 = {'coursegroup_id': coursegroup_id,
-                'course_uid': course_uid,
-                'course_brain': course_brain,
-                'course_title': course_brain and course_brain.Title,
-                'stats': None,
-                }
-        done = set()
-
-        def inner(group_id):
-            if group_id in done:
-                return
-            done.add(group_id)
-            if group_id not in group_ids:
-                return
-            # zuerst die Rekursion:
-            for child_id in gpm[group_id]:
-                res = inner(child_id)
-                if res is not None:
-                    return res
-            try:
-                dic = group_info[group_id]
-                if dic['group_desktop']:
-                    return dic
-            except KeyError:
-                pass
-
-        dic = inner(coursegroup_id)
-        if dic is not None:
-            dic2.update(dic)
-        return dic2
-
-    return get_group_mapping_course
-
-
-# -------------------------------- [ groupinfo_factory ... [
-def groupinfo_factory(context, pretty=0, forlist=0, searchtext=0):
-    """
-    Factory-Funktion; als Ersatz für get_group_info_by_id, insbesondere für
-    wiederholte Aufrufe.  Indirektionen etc. werden einmalig beim Erstellen der
-    Funktion aufgelöst und anschließend in einer Closure vorgehalten.
-
-    pretty -- Gruppennamen auflösen, wenn Suffix an ID und Titel
-    forlist -- Minimale Rückgabe (nur ID und Titel),
-               aber mit pretty kombinierbar
-    """
-    getAdapter = context.getAdapter
-    pg = getToolByName(context, 'portal_groups')
-    get_group = pg.getGroupById
-    acl = getToolByName(context, 'acl_users')
-    translate = getAdapter('translate')
-    GROUPS = acl.source_groups._groups
-
-    def minimal_group_info(group_id):
-        """
-        Nur ID und Titel
-        """
-        group = get_group(group_id)
-
-        dict_ = {'id': group_id}
-        try:
-            thegroup = GROUPS[group_id]
-            dict_['group_title'] = safe_decode(thegroup['title'])
-            return dict_
-        except KeyError:
-            return {}
-
-    def basic_group_info(group_id):
-        """
-        Gib ein Dict. zurück;
-        - immer vorhandene Schlüssel:
-          id, group_title, group_description, group_manager, group_desktop
-        - nur bei automatisch erzeugten Gruppen: role, role_translation, brain
-
-        Argumente:
-        group_id -- ein String, normalerweise mit 'group_' beginnend
-        """
-
-        group = get_group(group_id)
-
-        dict_ = {'id': group_id}
-        try:
-            thegroup = GROUPS[group_id]
-            dict_['group_title'] = safe_decode(thegroup['title'])
-        except KeyError:
-            return {}
-        dict_['group_description'] = safe_decode(thegroup['description'])
-        dict_['group_manager'] = thegroup.get('group_manager')
-        dict_['group_desktop'] = thegroup.get('group_desktop')
-
-        dic = split_group_id(group_id)
-        if dic['role'] is not None:
-            dict_.update(dic)
-
-        dict_['role_translation'] = translate(dic['role'])
-        dict_['brain'] = getbrain(context, dic['uid'])
-        return dict_
-
-    def pretty_group_info(group_id):
-        """
-        Ruft basic_group_info auf und fügt einen Schlüssel 'pretty_title'
-        hinzu, der den Gruppentitel ohne das Rollensuffix enthält.
-        """
-        dic = basic_group_info(group_id)
-        try:
-            if 'role' not in dic:
-                dic['pretty_title'] = translate(dic['group_title'])
-                return dic
-            liz = dic['group_title'].split()
-            if liz and liz[-1] == dic['role']:
-                stem = u' '.join(liz[:-1])
-                mask = PRETTY_MASK[dic['role']]
-                dic['pretty_title'] = translate(mask).format(group=stem)
-            else:
-                dic['pretty_title'] = translate(dic['group_title'])
-        except KeyError as e:
-            # evtl. keine Gruppe! (Aufruf durch get_mapping_group)
-            print(e)
-            pass
-        return dic
-
-    @log_or_trace(debug_active, logger=logger)
-    def minimal2_group_info(group_id):
-        """
-        Ruft minimal_group_info auf und modifiziert ggf. den Schlüssel
-        'group_title' (entsprechend dem von pretty_group_info zurückgegebenen
-        Schlüssel 'pretty_title')
-        """
-        dic = minimal_group_info(group_id)
-        if not dic:     # Gruppe nicht (mehr) gefunden;
-            return dic  # {} zurückgeben
-        dic2 = split_group_id(group_id)
-        if dic2['role'] is not None:
-            dic.update(dic2)
-        if 'role' not in dic:
-            dic['group_title'] = translate(dic['group_title'])
-            return dic
-        liz = dic['group_title'].split()
-        if liz and liz[-1] == six_text_type(dic['role']):
-            stem = u' '.join(liz[:-1])
-            mask = PRETTY_MASK[dic['role']]
-            dic['group_title'] = translate(mask).format(group=stem)
-        else:
-            dic['group_title'] = translate(dic['group_title'])
-        return dic
-
-    def make_searchstring(group_info):
-        """
-        Arbeite direkt auf einem group_info-Dict;
-        Gib kein Dict zurück, sondern einen String für Suchzwecke
-        """
-        try:
-            group_id = group_info['id']
-        except KeyError:
-            raise
-        try:
-            res = [safe_decode(group_info['title']),
-                   safe_decode(group_id)]
-        except KeyError:
-            print(list(group_info.items()))
-            raise
-            return u''
-        dic2 = split_group_id(group_id)
-        prettify = True
-        for val in dic2.values():
-            if val is None:
-                prettify = False
-                break  # es sind immer alle None, oder alle nicht None
-            else:
-                res.append(safe_decode(val))
-        if prettify:
-            pretty = pretty_group_title(group_id, res[0], translate)
-            if pretty is not None:
-                res.append(safe_decode(pretty))
-        descr = group_info['description']
-        if descr:
-            res.append(safe_decode(descr))
-        # print res
-        return u' '.join(res)  # .encode('utf-8')
-
-
-    if searchtext:
-        return make_searchstring
-    if forlist:
-        if pretty:
-            return minimal2_group_info
-        else:
-            return minimal_group_info
-    if pretty:
-        return pretty_group_info
-    else:
-        return basic_group_info
-# -------------------------------- ] ... groupinfo_factory ]
-
-# --------------------------------- [ userinfo_factory ... [
-def userinfo_factory(context, pretty=0, forlist=0,
-                     title_or_id=0):
-    """
-    Wie groupinfo_factory, aber für Benutzerobjekte.
-
-    pretty -- für Benutzer: title als formatierter Name
-              (author.get_formatted_name), wenn möglich
-    forlist -- Minimale Rückgabe (nur ID und Titel),
-               aber mit pretty kombinierbar
-    title_or_id -- für Verwendung mit visaplan.tools.classes.Proxy:
-               gib nur den Title oder ersatzweise die ID zurück
-               (mit pretty kombinierbar)
-    """
-    getAdapter = context.getAdapter
-    acl = getToolByName(context, 'acl_users')
-    acl_gu = acl.getUser
-    if pretty or not forlist:
-        getBrowser = context.getBrowser
-        author = getBrowser('author')
-        gbbuid = author.getBrainByUserId
-        gfn = author.get_formatted_name
-
-    # ---------------------------- [ forlist ... [
-    def basic_user_info(member_id):
-        """
-        Basisinformationen über einen Benutzer:
-        id, title
-
-        forlist, not: pretty
-        """
-        member = acl_gu(member_id)
-        if member:
-            return {'id': member_id,
-                    'title': member.getProperty('fullname'),
-                    }
-
-    def pretty_user_info(member_id):
-        """
-        Basisinformationen über einen Benutzer:
-        id, title
-
-        forlist, pretty
-        """
-        member = acl_gu(member_id)
-        if member:
-            brain = gbbuid(member_id)
-            return {'id': member_id,
-                    'title': (brain and gfn(brain))
-                             or member.getProperty('fullname'),
-                    }
-    # ---------------------------- ] ... forlist ]
-
-    # ------------------------ [ title_or_id ... [
-    def pretty_title_or_id(member_id):
-        try:
-            return pretty_user_info(member_id)['title'] \
-                   or member_id
-        except:
-            return None
-
-    def basic_title_or_id(member_id):
-        try:
-            return basic_user_info(member_id)['title'] \
-                   or member_id
-        except:
-            return None
-    # ------------------------ ] ... title_or_id ]
-
-    def full_user_info(member_id):
-        """
-        not: forlist, not: pretty
-        """
-        member = acl_gu(member_id)
-        if member:
-            brain = gbbuid(member_id)
-            return {'id': member_id,
-                    'title': member.getProperty('fullname'),
-                    'brain': brain,
-                    'email': member.getProperty('email'),
-                    }
-
-    def full_pretty_user_info(member_id):
-        """
-        not: forlist, pretty
-        """
-        member = acl_gu(member_id)
-        if member:
-            brain = gbbuid(member_id)
-            return {'id': member_id,
-                    'title': (brain and gfn(brain))
-                             or member.getProperty('fullname'),
-                    'brain': brain,
-                    'email': member.getProperty('email'),
-                    }
-
-    if title_or_id:
-        if pretty:
-            return pretty_title_or_id
-        else:
-            return basic_title_or_id
-    if forlist:
-        if pretty:
-            return pretty_user_info
-        else:
-            return basic_user_info
-    if pretty:
-        return full_pretty_user_info
-    else:
-        return full_user_info
-# --------------------------------- ] ... userinfo_factory ]
-
-# ------------------------------- [ memberinfo_factory ... [
-def memberinfo_factory(context, pretty=0, forlist=0, bloated=0):
-    """
-    Wie groupinfo_factory, aber für Gruppen- und Benutzerobjekte.
-    Es wird zusätzlich ein Feld 'type' gefüllt, das die Werte
-    'user', 'group' oder (mit bloated >= 2) None annehmen kann.
-
-    Die folgenden beiden werden einfach an groupinfo_factory bzw.
-    userinfo_factory weitergereicht:
-
-    pretty -- Gruppennamen auflösen, wenn Suffix an ID und Titel;
-              für benutzer: title als formatierter Name (author
-    forlist -- Minimale Rückgabe (nur ID und Titel),
-               aber mit pretty kombinierbar
-
-    Zusätzliches Argument:
-
-    bloated -- Schlüssel hinzufügen für Mitgliederliste wie in Tabelle
-               unitracc_groupmemberships.
-               Wenn >= 2, werden auch für nicht gefundene Mitglieder Einträge
-               zurückgegeben (noch nicht getestet)
-
-               ACHTUNG: Der Schlüssel 'ismember_zope' wird immer mit True
-                        gefüllt (auch für nicht existierende); das stimmt, wenn
-               die IDs aus einer Zope-Mitgliederliste der interessierenden
-               Gruppe stammen. Wenn die IDs auch aus einer anderen Quelle
-               kommen (z. B. einer Datenbankabfrage), muß dieser Wert
-               anschließend noch manuell korrigiert werden!
-    """
-    ggibi = groupinfo_factory(context, pretty, forlist)
-    guibi = userinfo_factory(context, pretty, forlist)
-
-    # ggibi gibt (für Gruppen) keinen title-Schlüssel zurück:
-    g_title_key = (pretty and 'pretty_title'
-                           or 'group_title')
-
-    def basic_member_info(member_id):
-        """
-        Basisinformationen über ein "Member" (Benutzer oder Gruppe):
-        id, title, type
-
-        Suche zuerst einen Benutzer, dann als Rückfalloption eine Gruppe
-        """
-        member = guibi(member_id)
-        if member is not None:
-            member['type'] = 'user'
-            return member
-        member = ggibi(member_id)
-        if member:
-            member['type'] = 'group'
-            member['title'] = member[g_title_key]
-            return member
-        else:
-            return None  # PEP 20.2
-
-    def bloated_member_info(member_id):
-        """
-        Gib dict-Objekt zurück wie nach dem Einfügen in
-        die Tabelle unitracc_groupmemberships erzeugt
-        """
-        member = basic_member_info(member_id)
-        if member is not None:
-            member.update({'member_id_': member_id,
-                           'start': None,
-                           'ends': None,
-                           'active': True,
-                           'ismember_zope': True,
-                           })
-            return member
-        elif bloated >= 2:
-            return {'id': member_id,
-                    'member_id_': member_id,
-                    'title': 'not found: %(member_id)s'
-                             % locals(),
-                    g_title_key: None,
-                    'type': None,
-                    'ismember_zope': True,
-                    'active': None,
-                    'start': None,
-                    'ends': None,
-                    }
-
-    if bloated:
-        return bloated_member_info
-    else:
-        return basic_member_info
-# ------------------------------- ] ... memberinfo_factory ]
+# (moved to ..infofact package)
 # ----------------------------------------- ] ... Factory-Funktionen ]
 
 if 0 and 'i18n honeypot':
     _('no group')   # -> voc_get_explicit_group_memberships_for_auth
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/cache.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/cache.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/configure.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/configure.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
            xmlns:zcml="http://namespaces.zope.org/zcml">
 
     <browser:page
         for="*"
         name="groupsharing"
         class=".browser.Browser"
         permission="zope2.View"
-        allowed_interface=".browser.IGroupSharing"
+        allowed_interface=".interface.IGroupSharing"
         />
 
 
     <include file="fullpage.zcml" />
     <include file="ajax.zcml"
              zcml:condition="installed visaplan.plone.ajaxnavigation"
              />
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/groupsharing/configure_groupsharing.pt` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/groupsharing/configure_groupsharing.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/resource/group-desktop.js` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/resource/group-desktop.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/browser.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/browser.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/unitraccgroups/utils.py` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/unitraccgroups/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,17 +287,24 @@
     """
     for suff in COURSE_GROUP_SUFFIXES:
         yield generic_group_id(uid, suff)
 
 
 def pretty_group_title(id, title, translate=None):
     """
+    For group ids which contain a "role suffix", return a "pretty" variant
+    of the title:
     >>> pretty_group_title('group_f6350ab731c3601e925eac482206bda5_Author',
     ...                    'SuP-Fachbuch Author')
     u'Author group "SuP-Fachbuch"'
+
+    If the id doesn't contain such a role hint, None is returned:
+    >>> pretty_group_title('group_f6350ab731c3601e925eac482206bda5',
+    ...                    'SuP-Fachbuch Author')
+
     """
     dic = split_group_id(id, resolve_role=False)
     if dic['role'] is None:  # das *Suffix*
         return None
     liz = safe_decode(title).split()
     role = liz.pop()
     if role != safe_decode(dic['role']):
```

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan/plone/groups/views/ajax.zcml` & `visaplan.plone.groups-1.3.3.1/src/visaplan/plone/groups/views/ajax.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/src/visaplan.plone.groups.egg-info/SOURCES.txt` & `visaplan.plone.groups-1.3.3.1/src/visaplan.plone.groups.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,29 @@
 src/visaplan.plone.groups.egg-info/entry_points.txt
 src/visaplan.plone.groups.egg-info/namespace_packages.txt
 src/visaplan.plone.groups.egg-info/not-zip-safe
 src/visaplan.plone.groups.egg-info/requires.txt
 src/visaplan.plone.groups.egg-info/top_level.txt
 src/visaplan/plone/__init__.py
 src/visaplan/plone/groups/__init__.py
+src/visaplan/plone/groups/_base_pio.py
+src/visaplan/plone/groups/_base_tools.py
+src/visaplan/plone/groups/_idxnames.py
+src/visaplan/plone/groups/base.py
 src/visaplan/plone/groups/configure.zcml
+src/visaplan/plone/groups/interfaces.py
 src/visaplan/plone/groups/groupboard/__init__.py
 src/visaplan/plone/groups/groupboard/ajax.zcml
 src/visaplan/plone/groups/groupboard/board.pt
 src/visaplan/plone/groups/groupboard/browser.py
 src/visaplan/plone/groups/groupboard/configure.zcml
 src/visaplan/plone/groups/groupboard/crumbs.py
 src/visaplan/plone/groups/groupboard/fullpage.zcml
+src/visaplan/plone/groups/groupboard/groupboard.pt
+src/visaplan/plone/groups/groupboard/interface.py
 src/visaplan/plone/groups/groupboard/new-thread.pt
 src/visaplan/plone/groups/groupboard/oldcrumbs.py
 src/visaplan/plone/groups/groupboard/thread-reply.pt
 src/visaplan/plone/groups/groupboard/utils.py
 src/visaplan/plone/groups/groupboard/sql/update-0001.sql
 src/visaplan/plone/groups/groupdesktop/__init__.py
 src/visaplan/plone/groups/groupdesktop/ajax.zcml
@@ -38,14 +45,15 @@
 src/visaplan/plone/groups/groupdesktop/configure.zcml
 src/visaplan/plone/groups/groupdesktop/crumbs.py
 src/visaplan/plone/groups/groupdesktop/fullpage.zcml
 src/visaplan/plone/groups/groupdesktop/gdmacros.pt
 src/visaplan/plone/groups/groupdesktop/group_administration_learning_progress_view.pt
 src/visaplan/plone/groups/groupdesktop/group_administration_user_view.pt
 src/visaplan/plone/groups/groupdesktop/group_administration_view.pt
+src/visaplan/plone/groups/groupdesktop/interface.py
 src/visaplan/plone/groups/groupdesktop/oldcrumbs.py
 src/visaplan/plone/groups/groupdesktop/our-animations.pt
 src/visaplan/plone/groups/groupdesktop/our-articles.pt
 src/visaplan/plone/groups/groupdesktop/our-audios.pt
 src/visaplan/plone/groups/groupdesktop/our-binaries.pt
 src/visaplan/plone/groups/groupdesktop/our-courses.pt
 src/visaplan/plone/groups/groupdesktop/our-events.pt
@@ -61,21 +69,30 @@
 src/visaplan/plone/groups/groupsharing/__init__.py
 src/visaplan/plone/groups/groupsharing/ajax.zcml
 src/visaplan/plone/groups/groupsharing/browser.py
 src/visaplan/plone/groups/groupsharing/cache.py
 src/visaplan/plone/groups/groupsharing/configure.zcml
 src/visaplan/plone/groups/groupsharing/configure_groupsharing.pt
 src/visaplan/plone/groups/groupsharing/fullpage.zcml
+src/visaplan/plone/groups/groupsharing/interface.py
 src/visaplan/plone/groups/groupsharing/utils.py
 src/visaplan/plone/groups/groupsharing/sql/update-0001.sql
 src/visaplan/plone/groups/groupsharing/sql/update-0002.sql
 src/visaplan/plone/groups/groupsharing/sql/update-0003.sql
+src/visaplan/plone/groups/infofact/__init__.py
+src/visaplan/plone/groups/infofact/_coursemap.py
+src/visaplan/plone/groups/infofact/_member.py
 src/visaplan/plone/groups/resource/group-desktop.js
 src/visaplan/plone/groups/unitraccgroups/__init__.py
 src/visaplan/plone/groups/unitraccgroups/browser.py
 src/visaplan/plone/groups/unitraccgroups/configure.zcml
 src/visaplan/plone/groups/unitraccgroups/utils.py
 src/visaplan/plone/groups/views/__init__.py
 src/visaplan/plone/groups/views/ajax.zcml
 src/visaplan/plone/groups/views/configure.zcml
 src/visaplan/plone/groups/views/fullpage.zcml
-src/visaplan/plone/groups/views/group-desktop.pt
+src/visaplan/plone/groups/views/group-desktop.pt
+src/visaplan/plone/groups/views/group-macros.pt
+src/visaplan/plone/groups/views/mycalendar.pt
+src/visaplan/plone/groups/views/mycalendar.py
+src/visaplan/plone/groups/views/myfellows.pt
+src/visaplan/plone/groups/views/myfellows.py
```

### Comparing `visaplan.plone.groups-1.2.1/README.rst` & `visaplan.plone.groups-1.3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.groups-1.2.1/setup.py` & `visaplan.plone.groups-1.3.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 def valid_suffix(suffix):
     """
     Enforce our suffix convention
     """
     suffix = suffix.strip()
     if not suffix:
         return suffix
-    allowed = set('.dev0123456789rc')
+    allowed = set('edv.0123456789rcpost')
     disallowed = set(suffix).difference(allowed)
     if disallowed:
         disallowed = ''.join(sorted(disallowed))
         raise ValueError('Version suffix contains disallowed characters'
                          ' (%(disallowed)s)'
                          % locals())
     chunks = suffix.split('.')
     chunk = chunks.pop(0)
-    if chunk:
+    if chunk and not chunk.startswith('rc') and not chunk.startswith('post'):
         raise ValueError('Version suffix must start with "."'
                          ' (%(suffix)r)'
                          % locals())
     if not chunks:
         raise ValueError('Version suffix is too short'
                          ' (%(suffix)r)'
                          % locals())
@@ -54,14 +54,15 @@
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' starts with a digit'
                              % locals())
         char = chunk[-1]
         if char not in '0123456789':
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' doesn\'t end with a digit'
+                             ' (normalization would append a "0")'
                              % locals())
     return suffix  # ... valid_suffix
     # ... get the version ...
     # ... get the version ...
 VERSION = read_version('VERSION',
                        'VERSION_SUFFIX')
 # -------------------------------------------- ] ... get the version ]
@@ -111,18 +112,25 @@
     if pop_user:
         assert 'pick_user' not in kwargs
         assert 'user' not in kwargs
         user = pkg_list.pop(0)
         package = '.'.join(pkg_list)
     else:
         pick_user = pop('pick_user', 'user' not in kwargs)
+        given_user = pop('user', None)
         if pick_user:
             user = pkg_list[0]
-            if 'user' in kwargs:
-                assert pop('user') == user
+            if given_user is not None and given_user != user:
+                raise ValueError('given user %(given_user)r mismatches '
+                                 'user picked from package %(user)r!'
+                                 % locals())
+        elif given_user is not None:
+            user = given_user
+        else:
+            raise ValueError('no user given nor picked!')
     if pop('travis', False):  # reqires github to be trueish
         res.update({  # CHECKME: is there a de-facto standard key for this?
             'Tests': 'https://travis-ci.org/%(user)s/%(package)s' % locals()
             })
     base = 'https://github.com/%(user)s/%(package)s' % locals()
     res.update({
         'Source': base,
@@ -168,22 +176,29 @@
         'visaplan.plone',
         ],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
+        'importlib_metadata',
+        'packaging',
         'six',
         # -*- Extra requirements: -*-
         'visaplan.tools >= 1.2.4',  # connected_dicts
-        'visaplan.plone.tools >=1.1.4',  # message-Funktion
+        'visaplan.plone.tools >=1.1.14',  # bugfix!
         'visaplan.plone.adapters',  # grouplog adapter
         'visaplan.plone.infohubs',
-        'visaplan.plone.base',  # browser base class, permissions
+        'visaplan.plone.base >=1.2.2',  # browser base class, permissions
         # ... further requirements removed
     ],
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
+if 0:
+    from pprint import pprint
+    del setup_kwargs['long_description']
+    pprint(setup_kwargs)
+    raise SystemExit(1)
 setup(**setup_kwargs)
```

