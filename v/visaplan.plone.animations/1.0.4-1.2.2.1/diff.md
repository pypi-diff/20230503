# Comparing `tmp/visaplan.plone.animations-1.0.4.tar.gz` & `tmp/visaplan.plone.animations-1.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.plone.animations-1.0.4.tar", last modified: Wed Dec 16 17:01:52 2020, max compression
+gzip compressed data, was "dist/visaplan.plone.animations-1.2.2.1.tar", last modified: Wed May  3 14:51:04 2023, max compression
```

## Comparing `visaplan.plone.animations-1.0.4.tar` & `visaplan.plone.animations-1.2.2.1.tar`

### file list

```diff
@@ -1,92 +1,97 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-10-01 09:33:39.000000 visaplan.plone.animations-1.0.4/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      678 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       98 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/docs/index.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/browser/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/browser/static/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/browser/static/.gitkeep
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/browser/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      460 2019-11-29 15:17:10.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/browser/configure.zcml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12288 2019-06-27 07:51:30.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/_.swp
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-01 09:58:19.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10056 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/folderish_animation.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9289 2020-10-26 18:07:07.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/folderish_animation.py.old
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      325 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/folderish_animation.xml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/LC_MESSAGES/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1221 2019-11-29 15:17:10.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.mo
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2140 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.po
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1782 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/visaplan.plone.animations.pot
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      286 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/Folder.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      786 2018-10-16 10:11:02.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation--export.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4712 2020-10-29 09:31:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      200 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/browserlayer.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      105 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/catalog.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4661 2018-10-05 16:47:50.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/dexterity_export-20181005164752.zip
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      491 2020-10-26 17:40:31.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/metadata.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       85 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/registry.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      355 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/rolemap.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      171 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types.xml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/uninstall/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      135 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/uninstall/browserlayer.xml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)  1057008 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.0.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   242057 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.0.min.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)  1057330 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.1.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   911189 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-2015.11.26.combined.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   190631 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-2015.11.26.min.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   273199 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-1.10.2.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)   266057 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-1.8.3.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    85582 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-2.2.4.min.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      860 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/type-1.css
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      705 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/type-2.css
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/templates/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3614 2020-10-26 17:40:32.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/templates/animation_onlyme.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1230 2020-10-26 17:40:32.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/templates/animation_view.pt
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/robot/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2916 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/robot/test_ct_folderish_animation.robot
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2031 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/robot/test_example.robot
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3336 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_ct_folderish_animation.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      905 2019-11-29 15:17:10.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_robot.py.disabled
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2451 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      213 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1843 2020-10-26 17:40:31.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      996 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/interfaces.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      411 2019-11-06 10:33:18.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/permissions.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      936 2020-10-26 17:40:32.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      708 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1828 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/testing.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      290 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/upgrades.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      386 2020-10-26 17:40:32.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/upgrades.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.0.4/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4870 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3489 2020-12-16 17:01:51.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-10-02 16:52:56.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      446 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2020-12-16 17:01:50.000000 visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1242 2020-12-16 17:01:14.000000 visaplan.plone.animations-1.0.4/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-10-01 09:33:39.000000 visaplan.plone.animations-1.0.4/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      297 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.0.4/DEVELOP.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-02-20 17:03:44.000000 visaplan.plone.animations-1.0.4/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1449 2019-11-06 10:33:19.000000 visaplan.plone.animations-1.0.4/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1254 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10395 2020-12-09 16:48:51.000000 visaplan.plone.animations-1.0.4/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4870 2020-12-16 17:01:52.000000 visaplan.plone.animations-1.0.4/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-10-01 09:33:39.000000 visaplan.plone.animations-1.2.2.1/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      678 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       98 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/docs/index.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12288 2019-06-27 07:51:30.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/_.swp
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-01 09:58:19.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11406 2023-05-03 10:54:39.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/folderish_animation.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      325 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/folderish_animation.xml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/LC_MESSAGES/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1265 2023-05-03 14:50:58.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.mo
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2140 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.po
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1782 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/visaplan.plone.animations.pot
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      311 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/Folder.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      786 2018-10-16 10:11:02.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation--export.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4798 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      200 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/browserlayer.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      105 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/catalog.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4661 2018-10-05 16:47:50.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/dexterity_export-20181005164752.zip
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      491 2023-04-15 22:23:02.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/metadata.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       85 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/registry.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      355 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/rolemap.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      171 2021-07-30 10:26:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types.xml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/uninstall/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      135 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/uninstall/browserlayer.xml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)  1057008 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.0.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)   242057 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.0.min.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)  1057330 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.1.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)   911189 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-2015.11.26.combined.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)   190631 2019-11-06 10:33:17.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-2015.11.26.min.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)   273199 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-1.10.2.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)   266057 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-1.8.3.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    85582 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-2.2.4.min.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      860 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/type-1.css
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      705 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/type-2.css
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/templates/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3614 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/templates/animation_onlyme.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1230 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/templates/animation_view.pt
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/robot/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2916 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/robot/test_ct_folderish_animation.robot
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2031 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/robot/test_example.robot
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3336 2023-05-03 10:54:39.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_ct_folderish_animation.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      905 2019-11-29 15:17:10.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_robot.py.disabled
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2451 2021-07-30 10:26:45.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_setup.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/thumbnails/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      625 2023-04-20 16:47:59.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/thumbnails/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      966 2023-04-15 23:04:30.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/thumbnails/configure.zcml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/utils/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      114 2023-04-20 16:47:59.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/utils/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3033 2023-04-20 18:02:57.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/utils/_lapa.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      213 2021-07-30 10:26:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2974 2023-04-15 23:04:30.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      996 2021-07-30 10:26:45.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/interfaces.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1245 2022-08-25 13:56:08.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/lapa.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1013 2023-04-20 16:47:58.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/lapainfo.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1148 2023-04-20 16:47:58.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/lapamenu.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      399 2023-04-20 16:47:58.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/metadata.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      245 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/permissions.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1003 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3640 2023-05-03 11:07:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1828 2023-05-03 10:55:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/testing.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      290 2021-07-30 10:26:44.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/upgrades.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1716 2023-04-20 14:29:01.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/upgrades.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10925 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3642 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-10-02 16:52:56.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      434 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4489 2023-05-03 14:50:42.000000 visaplan.plone.animations-1.2.2.1/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-10-01 09:33:39.000000 visaplan.plone.animations-1.2.2.1/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      297 2018-10-02 15:39:44.000000 visaplan.plone.animations-1.2.2.1/DEVELOP.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2021-04-21 09:37:09.000000 visaplan.plone.animations-1.2.2.1/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2223 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      502 2021-07-30 10:34:13.000000 visaplan.plone.animations-1.2.2.1/TODO.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        8 2023-05-03 11:46:41.000000 visaplan.plone.animations-1.2.2.1/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1588 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7729 2023-05-03 11:07:04.000000 visaplan.plone.animations-1.2.2.1/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10925 2023-05-03 14:51:04.000000 visaplan.plone.animations-1.2.2.1/PKG-INFO
```

### Comparing `visaplan.plone.animations-1.0.4/docs/LICENSE.GPL` & `visaplan.plone.animations-1.2.2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/docs/LICENSE.rst` & `visaplan.plone.animations-1.2.2.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/_.swp` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/_.swp`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/content/folderish_animation.py` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/content/folderish_animation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 # Python compatibility:
-from __future__ import absolute_import
+from __future__ import absolute_import, print_function
 
+from importlib_metadata import PackageNotFoundError
+from importlib_metadata import version as pkg_version
 from six.moves import range
 
 # Standard library:
-from time import time
 from cgi import escape as cgi_escape
+from time import time
 
 # Zope:
 from Acquisition import aq_inner
 from Products.Five import BrowserView
 from zope import schema
 from zope.component import getMultiAdapter, getUtility
 from zope.interface import implementer
@@ -28,23 +30,29 @@
 from visaplan.plone.behaviors.interfaces import (
     ICaptionAndLegend,
     IExcludeFromSearch,
     IHeightAndWidth,
     IHierarchicalBuzzword,
     IPreviewImage,
     )
-from visaplan.plone.staticthumbnails.mixin import DedicatedThumbnailMixin
 
 # Local imports:
-from ..interfaces import IFolderishAnimation
+from visaplan.plone.animations.interfaces import IFolderishAnimation
+
+try:
+    pkg_version('visaplan.plone.staticthumbnails')
+except PackageNotFoundError:
+    HAVE_STATICTHUMBNAILS = 0
+else:
+    HAVE_STATICTHUMBNAILS = 1
+    print('We have visaplan.plone.staticthumbnails')
 
 # Logging / Debugging:
 from logging import getLogger
 from pdb import set_trace
-from visaplan.tools.debug import pp
 
 logger = getLogger('visaplan.plone.animations:FolderishAnimation')
 
 # Local imports:
 from .. import _
 
 __all__ = [  # public interface:
@@ -71,26 +79,55 @@
 USE_TIMESTAMPS = True
 
 
 # Is there a better way?
 @implementer(IFolderishAnimation, IHeightAndWidth, ICaptionAndLegend,
              IExcludeFromSearch, IHierarchicalBuzzword,
              IPreviewImage)
-class FolderishAnimation(Container, DedicatedThumbnailMixin):
+class FolderishAnimation(Container):
     """
     Folderish animation type
     """
 
-    def _getDefaultThumbnailPath(self):
-        """
-        Rückgabewert für getThumbnailPath, wenn kein spezielles
-        Vorschaubild für die konkrete Animation konfiguriert
-        """
-        return self._buildStaticImagePath('picto_media_animation_m.png')
+    # (copied from Products.unitracc.content.base)
+    # quick solution, for now; we might use an indexer some day:
+    def getCustomSearch(self, media=0):
+        """
+        Basisversion für alle von UnitraccBase abgeleiteten Typen;
+        jeder Listeneintrag ist ein mögliches Suchkriterium.
+
+        Achtung: Kommaseparierte Werte innerhalb *eines* Listenelements
+                 funktionieren *nicht*!
+        """
+        liz = ['portal_type=' + self.portal_type]
+        if media:
+            mediaType, mediaFormat = self.getContentType().split('/')
+            liz.append('mediaType=' + mediaType)
+            liz.append('mediaFormat=' + mediaFormat)
+        groupsharing = self.restrictedTraverse('@@groupsharing')
+        liz.extend(groupsharing.get_custom_search_authors())
+        try:
+            for group_id in self.getUnitraccGroups():
+                liz.append("groups=" + group_id)
+        except AttributeError as e:
+            logger.error('FolderishAnimation.getCustomSearch: %(e)r',
+                         locals())
+        return liz
+
+
+if HAVE_STATICTHUMBNAILS:
+    # from zope.interface import classImplements
+    # Zope:
+    from zope.interface import alsoProvides
+
+    # visaplan:
+    from visaplan.plone.staticthumbnails.interfaces import IFromImageAttribute
 
+    # classImplements(FolderishAnimation, IFromImageAttribute)
+    alsoProvides(FolderishAnimation, IFromImageAttribute)
 
 def get_js_values(name, o, mtype):
     """
     Values for javascript files
     """
     inline = name.startswith('inline')
     if inline:
@@ -247,15 +284,14 @@
         if 'height' in res and 'width' in res:
             res['_calculated'] = {
                 'style': ';'.join(['%s:%spx' % (k, res[k])
                                    for k in ('height', 'width')
                                    ]),
                 }
             logger.info('style=%(style)s', res['_calculated'])
-        pp(res)
         res['file_elements'] = self._file_elements()
         res['preload_img'] = self._preload_img
 
         scales = getMultiAdapter((context, context.REQUEST), name='images')
         scale = scales.scale('image', scale='preview')
         if scale:
             res['preview_image_tag'] = scale.tag(title=None,
```

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.mo` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 7 messages, Project-Id-Version: visaplan.plone.animations 'Ein ordnerartiger Objekttyp f\303\274r Animationen, die ihre Hilfsdateien enthalten'*

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 00000000: de12 0495 0000 0000 0700 0000 1c00 0000  ................
-00000010: 5400 0000 0000 0000 8c00 0000 0000 0000  T...............
-00000020: 8c00 0000 3b00 0000 8d00 0000 0500 0000  ....;...........
-00000030: c900 0000 1200 0000 cf00 0000 2800 0000  ............(...
-00000040: e200 0000 8500 0000 0b01 0000 0b00 0000  ................
-00000050: 9101 0000 c401 0000 9d01 0000 4d00 0000  ............M...
-00000060: 6203 0000 0b00 0000 b003 0000 1700 0000  b...............
-00000070: bc03 0000 3800 0000 d403 0000 ad00 0000  ....8...........
-00000080: 0d04 0000 0900 0000 bb04 0000 0041 2066  .............A f
-00000090: 6f6c 6465 7269 7368 2061 6e69 6d61 7469  olderish animati
-000000a0: 6f6e 2074 7970 6520 7768 6963 6820 2a63  on type which *c
-000000b0: 6f6e 7461 696e 732a 2061 7578 696c 6961  ontains* auxilia
-000000c0: 7279 2066 696c 6573 0042 6173 6963 0046  ry files.Basic.F
-000000d0: 6f6c 6465 7269 7368 416e 696d 6174 696f  olderishAnimatio
-000000e0: 6e00 4f70 656e 2061 206e 6577 2077 696e  n.Open a new win
-000000f0: 646f 7720 746f 2073 7461 7274 2074 6865  dow to start the
-00000100: 2061 6e69 6d61 7469 6f6e 0054 6865 2069   animation.The i
-00000110: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00000120: 2066 6f6c 6465 7269 7368 2061 6e69 6d61   folderish anima
-00000130: 7469 6f6e 7320 6d69 6768 7420 6576 6f6c  tions might evol
-00000140: 7665 2c20 616e 6420 736f 6d65 206f 6620  ve, and some of 
-00000150: 7468 6520 696d 7072 6f76 656e 7473 206d  the improvents m
-00000160: 6967 6874 2062 6520 696e 636f 6d70 6174  ight be incompat
-00000170: 6962 6c65 2074 6f20 6f6c 6465 7220 616e  ible to older an
-00000180: 696d 6174 696f 6e20 6f62 6a65 6374 732e  imation objects.
-00000190: 0054 7970 6520 6e75 6d62 6572 0050 726f  .Type number.Pro
-000001a0: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
-000001b0: 2076 6973 6170 6c61 6e2e 706c 6f6e 652e   visaplan.plone.
-000001c0: 616e 696d 6174 696f 6e73 0a50 4f54 2d43  animations.POT-C
-000001d0: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
-000001e0: 3139 2d30 352d 3136 2030 393a 3031 2b30  19-05-16 09:01+0
-000001f0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
-00000200: 4461 7465 3a20 3230 3139 2d30 352d 3136  Date: 2019-05-16
-00000210: 2030 393a 3136 2b30 3030 300a 4c61 7374   09:16+0000.Last
-00000220: 2d54 7261 6e73 6c61 746f 723a 2054 6f62  -Translator: Tob
-00000230: 6961 7320 4865 7270 203c 746f 6269 6173  ias Herp <tobias
-00000240: 2e68 6572 7040 7669 7361 706c 616e 2e63  .herp@visaplan.c
-00000250: 6f6d 3e6e 4c61 6e67 7561 6765 2d54 6561  om>nLanguage-Tea
-00000260: 6d3a 204c 414e 4755 4147 4520 3c4c 4c40  m: LANGUAGE <LL@
-00000270: 6c69 2e6f 7267 3e0a 4d49 4d45 2d56 6572  li.org>.MIME-Ver
-00000280: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-00000290: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-000002a0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
-000002b0: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-000002c0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-000002d0: 740a 506c 7572 616c 2d46 6f72 6d73 3a20  t.Plural-Forms: 
-000002e0: 6e70 6c75 7261 6c73 3d31 3b20 706c 7572  nplurals=1; plur
-000002f0: 616c 3d30 0a4c 616e 6775 6167 652d 436f  al=0.Language-Co
-00000300: 6465 3a20 6465 0a4c 616e 6775 6167 652d  de: de.Language-
-00000310: 4e61 6d65 3a20 4765 726d 616e 0a50 7265  Name: German.Pre
-00000320: 6665 7272 6564 2d45 6e63 6f64 696e 6773  ferred-Encodings
-00000330: 3a20 7574 662d 3820 6c61 7469 6e31 0a44  : utf-8 latin1.D
-00000340: 6f6d 6169 6e3a 2076 6973 6170 6c61 6e2e  omain: visaplan.
-00000350: 706c 6f6e 652e 616e 696d 6174 696f 6e73  plone.animations
-00000360: 0a00 4569 6e20 6f72 646e 6572 6172 7469  ..Ein ordnerarti
-00000370: 6765 7220 4f62 6a65 6b74 7479 7020 66c3  ger Objekttyp f.
-00000380: bc72 2041 6e69 6d61 7469 6f6e 656e 2c20  .r Animationen, 
-00000390: 6469 6520 6968 7265 2048 696c 6673 6461  die ihre Hilfsda
-000003a0: 7465 6965 6e20 656e 7468 616c 7465 6e00  teien enthalten.
-000003b0: 4772 756e 646c 6567 656e 6400 416e 696d  Grundlegend.Anim
-000003c0: 6174 696f 6e20 286f 7264 6e65 7261 7274  ation (ordnerart
-000003d0: 6967 2900 4569 6e20 6e65 7565 7320 4665  ig).Ein neues Fe
-000003e0: 6e73 7465 7220 c3b6 6666 6e65 6e2c 2075  nster ..ffnen, u
-000003f0: 6d20 6469 6520 416e 696d 6174 696f 6e20  m die Animation 
-00000400: 6175 737a 7566 c3bc 6872 656e 0044 6965  auszuf..hren.Die
-00000410: 2049 6d70 6c65 6d65 6e74 6965 7275 6e67   Implementierung
-00000420: 2064 6572 206f 7264 6e65 7261 7274 6967   der ordnerartig
-00000430: 656e 2041 6e69 6d61 7469 6f6e 656e 206b  en Animationen k
-00000440: c3b6 6e6e 7465 2073 6963 6820 7765 6974  ..nnte sich weit
-00000450: 6572 656e 7477 6963 6b65 6c6e 2c20 756e  erentwickeln, un
-00000460: 6420 6d61 6e63 6865 2064 6572 2056 6572  d manche der Ver
-00000470: 6265 7373 6572 756e 6765 6e20 6bc3 b66e  besserungen k..n
-00000480: 6e74 656e 206d 6974 2076 6f72 6861 6e64  nten mit vorhand
-00000490: 656e 656e 2041 6e69 6d61 7469 6f6e 736f  enen Animationso
-000004a0: 626a 656b 7465 6e20 696e 6b6f 6d70 6174  bjekten inkompat
-000004b0: 6962 656c 2073 6569 6e2e 0054 7970 6e75  ibel sein..Typnu
-000004c0: 6d6d 6572 00                             mmer.
+00000010: 5400 0000 0b00 0000 8c00 0000 0000 0000  T...............
+00000020: b800 0000 3b00 0000 b900 0000 0500 0000  ....;...........
+00000030: f500 0000 1200 0000 fb00 0000 2800 0000  ............(...
+00000040: 0e01 0000 8500 0000 3701 0000 0b00 0000  ........7.......
+00000050: bd01 0000 c401 0000 c901 0000 4d00 0000  ............M...
+00000060: 8e03 0000 0b00 0000 dc03 0000 1700 0000  ................
+00000070: e803 0000 3800 0000 0004 0000 ad00 0000  ....8...........
+00000080: 3904 0000 0900 0000 e704 0000 0100 0000  9...............
+00000090: 0000 0000 0500 0000 0000 0000 0300 0000  ................
+000000a0: 0000 0000 0200 0000 0400 0000 0000 0000  ................
+000000b0: 0600 0000 0700 0000 0041 2066 6f6c 6465  .........A folde
+000000c0: 7269 7368 2061 6e69 6d61 7469 6f6e 2074  rish animation t
+000000d0: 7970 6520 7768 6963 6820 2a63 6f6e 7461  ype which *conta
+000000e0: 696e 732a 2061 7578 696c 6961 7279 2066  ins* auxiliary f
+000000f0: 696c 6573 0042 6173 6963 0046 6f6c 6465  iles.Basic.Folde
+00000100: 7269 7368 416e 696d 6174 696f 6e00 4f70  rishAnimation.Op
+00000110: 656e 2061 206e 6577 2077 696e 646f 7720  en a new window 
+00000120: 746f 2073 7461 7274 2074 6865 2061 6e69  to start the ani
+00000130: 6d61 7469 6f6e 0054 6865 2069 6d70 6c65  mation.The imple
+00000140: 6d65 6e74 6174 696f 6e20 6f66 2066 6f6c  mentation of fol
+00000150: 6465 7269 7368 2061 6e69 6d61 7469 6f6e  derish animation
+00000160: 7320 6d69 6768 7420 6576 6f6c 7665 2c20  s might evolve, 
+00000170: 616e 6420 736f 6d65 206f 6620 7468 6520  and some of the 
+00000180: 696d 7072 6f76 656e 7473 206d 6967 6874  improvents might
+00000190: 2062 6520 696e 636f 6d70 6174 6962 6c65   be incompatible
+000001a0: 2074 6f20 6f6c 6465 7220 616e 696d 6174   to older animat
+000001b0: 696f 6e20 6f62 6a65 6374 732e 0054 7970  ion objects..Typ
+000001c0: 6520 6e75 6d62 6572 0050 726f 6a65 6374  e number.Project
+000001d0: 2d49 642d 5665 7273 696f 6e3a 2076 6973  -Id-Version: vis
+000001e0: 6170 6c61 6e2e 706c 6f6e 652e 616e 696d  aplan.plone.anim
+000001f0: 6174 696f 6e73 0a50 4f54 2d43 7265 6174  ations.POT-Creat
+00000200: 696f 6e2d 4461 7465 3a20 3230 3139 2d30  ion-Date: 2019-0
+00000210: 352d 3136 2030 393a 3031 2b30 3030 300a  5-16 09:01+0000.
+00000220: 504f 2d52 6576 6973 696f 6e2d 4461 7465  PO-Revision-Date
+00000230: 3a20 3230 3139 2d30 352d 3136 2030 393a  : 2019-05-16 09:
+00000240: 3136 2b30 3030 300a 4c61 7374 2d54 7261  16+0000.Last-Tra
+00000250: 6e73 6c61 746f 723a 2054 6f62 6961 7320  nslator: Tobias 
+00000260: 4865 7270 203c 746f 6269 6173 2e68 6572  Herp <tobias.her
+00000270: 7040 7669 7361 706c 616e 2e63 6f6d 3e6e  p@visaplan.com>n
+00000280: 4c61 6e67 7561 6765 2d54 6561 6d3a 204c  Language-Team: L
+00000290: 414e 4755 4147 4520 3c4c 4c40 6c69 2e6f  ANGUAGE <LL@li.o
+000002a0: 7267 3e0a 4d49 4d45 2d56 6572 7369 6f6e  rg>.MIME-Version
+000002b0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
+000002c0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+000002d0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
+000002e0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
+000002f0: 6e63 6f64 696e 673a 2038 6269 740a 506c  ncoding: 8bit.Pl
+00000300: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
+00000310: 7261 6c73 3d31 3b20 706c 7572 616c 3d30  rals=1; plural=0
+00000320: 0a4c 616e 6775 6167 652d 436f 6465 3a20  .Language-Code: 
+00000330: 6465 0a4c 616e 6775 6167 652d 4e61 6d65  de.Language-Name
+00000340: 3a20 4765 726d 616e 0a50 7265 6665 7272  : German.Preferr
+00000350: 6564 2d45 6e63 6f64 696e 6773 3a20 7574  ed-Encodings: ut
+00000360: 662d 3820 6c61 7469 6e31 0a44 6f6d 6169  f-8 latin1.Domai
+00000370: 6e3a 2076 6973 6170 6c61 6e2e 706c 6f6e  n: visaplan.plon
+00000380: 652e 616e 696d 6174 696f 6e73 0a00 4569  e.animations..Ei
+00000390: 6e20 6f72 646e 6572 6172 7469 6765 7220  n ordnerartiger 
+000003a0: 4f62 6a65 6b74 7479 7020 66c3 bc72 2041  Objekttyp f..r A
+000003b0: 6e69 6d61 7469 6f6e 656e 2c20 6469 6520  nimationen, die 
+000003c0: 6968 7265 2048 696c 6673 6461 7465 6965  ihre Hilfsdateie
+000003d0: 6e20 656e 7468 616c 7465 6e00 4772 756e  n enthalten.Grun
+000003e0: 646c 6567 656e 6400 416e 696d 6174 696f  dlegend.Animatio
+000003f0: 6e20 286f 7264 6e65 7261 7274 6967 2900  n (ordnerartig).
+00000400: 4569 6e20 6e65 7565 7320 4665 6e73 7465  Ein neues Fenste
+00000410: 7220 c3b6 6666 6e65 6e2c 2075 6d20 6469  r ..ffnen, um di
+00000420: 6520 416e 696d 6174 696f 6e20 6175 737a  e Animation ausz
+00000430: 7566 c3bc 6872 656e 0044 6965 2049 6d70  uf..hren.Die Imp
+00000440: 6c65 6d65 6e74 6965 7275 6e67 2064 6572  lementierung der
+00000450: 206f 7264 6e65 7261 7274 6967 656e 2041   ordnerartigen A
+00000460: 6e69 6d61 7469 6f6e 656e 206b c3b6 6e6e  nimationen k..nn
+00000470: 7465 2073 6963 6820 7765 6974 6572 656e  te sich weiteren
+00000480: 7477 6963 6b65 6c6e 2c20 756e 6420 6d61  twickeln, und ma
+00000490: 6e63 6865 2064 6572 2056 6572 6265 7373  nche der Verbess
+000004a0: 6572 756e 6765 6e20 6bc3 b66e 6e74 656e  erungen k..nnten
+000004b0: 206d 6974 2076 6f72 6861 6e64 656e 656e   mit vorhandenen
+000004c0: 2041 6e69 6d61 7469 6f6e 736f 626a 656b   Animationsobjek
+000004d0: 7465 6e20 696e 6b6f 6d70 6174 6962 656c  ten inkompatibel
+000004e0: 2073 6569 6e2e 0054 7970 6e75 6d6d 6572   sein..Typnummer
+000004f0: 00                                       .
```

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.po` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.po`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/locales/visaplan.plone.animations.pot` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/locales/visaplan.plone.animations.pot`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation--export.xml` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation--export.xml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml`

 * *Files 2% similar despite different names*

#### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/types/FolderishAnimation.xml`

```diff
@@ -50,14 +50,15 @@
     <!-- image: -->
     <element value="visaplan.plone.behaviors.interfaces.IPreviewImage"/>
     <element value="plone.namedfile.interfaces.IImageScaleTraversable"/>
     <!--<element value="plone.app.relationfield.behavior.IRelatedItems"/>-->
     <!--<element value="plone.app.versioningbehavior.behaviors.IVersionable" />-->
     <!--<element value="plone.app.contenttypes.behaviors.tableofcontents.ITableOfContents"/>-->
     <!--<element value="plone.app.contenttypes.behaviors.richtext.IRichText"/>-->
+    <element value="visaplan.plone.staticthumbnails.interfaces.IDedicatedThumbnail"/>
   </property>
   <!-- View information -->
   <property name="add_view_expr">string:${folder_url}/++add++FolderishAnimation</property>
   <property name="default_view">view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
```

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles/default/dexterity_export-20181005164752.zip` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles/default/dexterity_export-20181005164752.zip`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.0.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.0.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.0.min.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.0.min.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-1.0.1.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-1.0.1.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-2015.11.26.combined.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-2015.11.26.combined.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/createjs-2015.11.26.min.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/createjs-2015.11.26.min.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-1.10.2.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-1.10.2.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-1.8.3.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-1.8.3.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/jquery-2.2.4.min.js` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/jquery-2.2.4.min.js`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/type-1.css` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/type-1.css`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/resource/type-2.css` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/resource/type-2.css`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/templates/animation_onlyme.pt` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/templates/animation_onlyme.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/templates/animation_view.pt` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/templates/animation_view.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/robot/test_ct_folderish_animation.robot` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/robot/test_ct_folderish_animation.robot`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/robot/test_example.robot` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_ct_folderish_animation.py` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_ct_folderish_animation.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_robot.py.disabled` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_robot.py.disabled`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/tests/test_setup.py` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/configure.zcml` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/configure.zcml`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,91 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
-    xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="visaplan.plone.animations">
 
-  <i18n:registerTranslations directory="locales" />
+    <i18n:registerTranslations directory="locales" />
 
-  <!--
-    Be careful if you use general includeDependencies, it can have sideffects!
-    Better import explicite packages or configurations ;)
-  -->
-  <!--<includeDependencies package="." />-->
-
-  <include package=".browser" />
-  <include package="visaplan.plone.ajaxnavigation" />
-
-  <include file="permissions.zcml" />
-
-  <include file="profiles.zcml" />
-  <include file="upgrades.zcml" />
+    <!--
+      Be careful if you use general includeDependencies, it can have sideffects!
+      Better import explicite packages or configurations ;)
+    -->
+    <!--<includeDependencies package="." />-->
+
+    <include
+	file="permissions.zcml"
+	zcml:condition="installed AccessControl.security"
+	/>
+
+    <include file="profiles.zcml" />
+    <include file="upgrades.zcml" />
+    <include package=".metadata"
+	zcml:condition="installed visaplan.plone.industrialsector"
+        />
 
-  <!-- -*- extra stuff goes here -*- -->
+    <!-- -*- extra stuff goes here -*- -->
     <browser:resourceDirectory
-             name="visaplan.plone.animations"
-             directory="resource" />
+	name="visaplan.plone.animations"
+	directory="resource"
+	/>
 
     <browser:page
         name="view"
         for="visaplan.plone.animations.interfaces.IFolderishAnimation"
         class="visaplan.plone.animations.content.folderish_animation.FolderishAnimationView"
         template="templates/animation_view.pt"
         permission="zope2.View"
         />
 
     <browser:page
-        name="ajax-nav"
-        for="visaplan.plone.animations.interfaces.IFolderishAnimation"
-        class="visaplan.plone.ajaxnavigation.views.NoAjaxBrowserView"
-        layer="visaplan.plone.animations.interfaces.IVisaplanPloneAnimationsLayer"
-        permission="zope.Public"
-        />
-
-    <browser:page
         name="onlyme"
         for="visaplan.plone.animations.interfaces.IFolderishAnimation"
         class="visaplan.plone.animations.content.folderish_animation.FolderishAnimationAjaxView"
         template="templates/animation_onlyme.pt"
         permission="zope2.View"
         />
 
+    <configure
+        zcml:condition="installed visaplan.plone.search">
+
+        <browser:page
+            name="landing_path"
+            for="visaplan.plone.animations.interfaces.IFolderishAnimation"
+            zcml:condition="not-installed visaplan.plone.structures"
+            class=".lapa.LandingPath"
+            permission="zope.Public"
+            /><!-- gf: lapa.py
+                -->
+
+        <configure
+            zcml:condition="installed visaplan.plone.structures">
+
+            <browser:page
+                name="landing_path"
+                for="visaplan.plone.animations.interfaces.IFolderishAnimation"
+                zcml:condition="installed visaplan.plone.menu"
+                class=".lapamenu.LandingPath"
+                permission="zope.Public"
+                /><!-- gf: lapamenu.py
+                    -->
+
+            <browser:page
+                name="landing_path"
+                for="visaplan.plone.animations.interfaces.IFolderishAnimation"
+                zcml:condition="not-installed visaplan.plone.menu"
+                class=".lapainfo.LandingPath"
+                permission="zope.Public"
+                /><!-- gf: lapainfo.py
+                    -->
+
+        </configure>
+    </configure>
+
+    <include package=".thumbnails"
+        zcml:condition="installed visaplan.plone.staticthumbnails"
+        /><!-- gf: thumbnails/configure.zcml
+                   thumbnails/__init__.py
+            -->
+
 </configure>
```

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/interfaces.py` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/interfaces.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/profiles.zcml` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/profiles.zcml`

 * *Files 17% similar despite different names*

```diff
@@ -22,8 +22,12 @@
       />
 
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="visaplan.plone.animations-hiddenprofiles"
       />
 
+  <!-- (for upgrade steps, see (gf):
+       upgrades.zcml
+    -->
+
 </configure>
```

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan/plone/animations/testing.py` & `visaplan.plone.animations-1.2.2.1/src/visaplan/plone/animations/testing.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.animations-1.0.4/src/visaplan.plone.animations.egg-info/SOURCES.txt` & `visaplan.plone.animations-1.2.2.1/src/visaplan.plone.animations.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
 MANIFEST.in
 README.rst
+TODO.rst
 VERSION
 setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/index.rst
 src/visaplan/__init__.py
@@ -18,27 +19,27 @@
 src/visaplan.plone.animations.egg-info/not-zip-safe
 src/visaplan.plone.animations.egg-info/requires.txt
 src/visaplan.plone.animations.egg-info/top_level.txt
 src/visaplan/plone/__init__.py
 src/visaplan/plone/animations/__init__.py
 src/visaplan/plone/animations/configure.zcml
 src/visaplan/plone/animations/interfaces.py
+src/visaplan/plone/animations/lapa.py
+src/visaplan/plone/animations/lapainfo.py
+src/visaplan/plone/animations/lapamenu.py
+src/visaplan/plone/animations/metadata.py
 src/visaplan/plone/animations/permissions.zcml
 src/visaplan/plone/animations/profiles.zcml
 src/visaplan/plone/animations/setuphandlers.py
 src/visaplan/plone/animations/testing.py
 src/visaplan/plone/animations/upgrades.py
 src/visaplan/plone/animations/upgrades.zcml
-src/visaplan/plone/animations/browser/__init__.py
-src/visaplan/plone/animations/browser/configure.zcml
-src/visaplan/plone/animations/browser/static/.gitkeep
 src/visaplan/plone/animations/content/_.swp
 src/visaplan/plone/animations/content/__init__.py
 src/visaplan/plone/animations/content/folderish_animation.py
-src/visaplan/plone/animations/content/folderish_animation.py.old
 src/visaplan/plone/animations/content/folderish_animation.xml
 src/visaplan/plone/animations/locales/visaplan.plone.animations.pot
 src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.mo
 src/visaplan/plone/animations/locales/de/LC_MESSAGES/visaplan.plone.animations.po
 src/visaplan/plone/animations/profiles/default/browserlayer.xml
 src/visaplan/plone/animations/profiles/default/catalog.xml
 src/visaplan/plone/animations/profiles/default/dexterity_export-20181005164752.zip
@@ -63,8 +64,12 @@
 src/visaplan/plone/animations/templates/animation_onlyme.pt
 src/visaplan/plone/animations/templates/animation_view.pt
 src/visaplan/plone/animations/tests/__init__.py
 src/visaplan/plone/animations/tests/test_ct_folderish_animation.py
 src/visaplan/plone/animations/tests/test_robot.py.disabled
 src/visaplan/plone/animations/tests/test_setup.py
 src/visaplan/plone/animations/tests/robot/test_ct_folderish_animation.robot
-src/visaplan/plone/animations/tests/robot/test_example.robot
+src/visaplan/plone/animations/tests/robot/test_example.robot
+src/visaplan/plone/animations/thumbnails/__init__.py
+src/visaplan/plone/animations/thumbnails/configure.zcml
+src/visaplan/plone/animations/utils/__init__.py
+src/visaplan/plone/animations/utils/_lapa.py
```

### Comparing `visaplan.plone.animations-1.0.4/README.rst` & `visaplan.plone.animations-1.2.2.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 =========================
 visaplan.plone.animations
 =========================
+.. image::
+   https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+       :target: https://pycqa.github.io/isort/
 
 A dexterity-based content type for animations.
 
 
 Features
 --------
 
-- Can be bullet points
+- Provides a `FolderishAnimation` content type which ...
+- *contains* it's specific (Javascript, most likely) resources, while
+- using more generic (library) resources, common for all animations of a common
+  type, from a "global" resource path
+- Currently we have exactly *one* type, tailored to our CreateJS_-based
+  animations.
 
 
 Examples
 --------
 
 This add-on can be seen in action at the following sites:
 
-- Is there a page on the internet where everybody can see the features?
 - https://www.unitracc.de
 - https://www.unitracc.com
 
 
 Documentation
 -------------
 
 Sorry, we don't have real user documentation yet.
 
 
 Installation
 ------------
 
-Install visaplan.plone.animations by adding it to your buildout::
+Add visaplan.plone.animations_ to your buildout_::
 
     [buildout]
-
     ...
 
     eggs =
+        ...
         visaplan.plone.animations
 
 
-and then running ``bin/buildout``
+and then running ``bin/buildout``; or add it to the requirements of your own
+extension or policy package.
+
+After (re-) starting your Zope instance, you'll need to "install" the
+extension, using the extensions installation form or the Zope quick-installer.
 
 
 Contribute
 ----------
 
 - Issue Tracker: https://github.com/visaplan/visaplan.plone.animations/issues
 - Source Code: https://github.com/visaplan/visaplan.plone.animations
@@ -62,10 +73,13 @@
 
 
 License
 -------
 
 The project is licensed under the GPLv2.
 
+.. _`CreateJS`: https://www.createjs.com
 .. _`issue tracker`: https://github.com/visaplan/visaplan.plone.animations/issues
+.. _visaplan.plone.animations: https://pypi.org/project/visaplan.plone.animations
+.. _buildout: https://pypi.org/project/zc.buildout
 
 .. vim: tw=79 cc=+1 sw=4 sts=4 si et
```

### Comparing `visaplan.plone.animations-1.0.4/setup.py` & `visaplan.plone.animations-1.2.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,16 @@
 """Installer for the visaplan.plone.animations package."""
 # Python compatibility:
 from __future__ import absolute_import, print_function
 
 # Setup tools:
 from setuptools import find_packages, setup
 
-# Standard library:
-import os
-# ---------------------------------------- [ destination locking ... [
-import sys
 from os.path import isfile
 
-try:  # Python 3:
-    # Standard library:
-    from configparser import ConfigParser
-except ImportError:
-    # Standard library (Python 2):
-    from ConfigParser import ConfigParser
-# ---------------------------------------- ] ... destination locking ]
-
 package_name = 'visaplan.plone.animations'
 
 # -------------------------------------------- [ get the version ... [
 def read_version(fn, sfn):
     main = open(fn).read().strip()
     if sfn is not None and isfile(sfn):
         suffix = valid_suffix(open(sfn).read().strip())
@@ -34,24 +22,24 @@
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
@@ -65,112 +53,29 @@
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
 
 
-# ---------------------------------------- [ destination locking ... [
-COMMANDS_WATCHED = ('register', 'upload')
-def inject_repository_url(server):
-    changed = False
-
-    for command in COMMANDS_WATCHED:
-        if command in sys.argv:
-            #found one command, check for -r or --repository
-            commandpos = sys.argv.index(command)
-            i = commandpos+1
-            repo = None
-            while i<len(sys.argv) and sys.argv[i].startswith('-'):
-                #check all following options (not commands)
-                if (sys.argv[i] == '-r') or (sys.argv[i] == '--repository'):
-                    #next one is the repository itself
-                    try:
-                        repo = sys.argv[i+1]
-                        if repo.lower() != server.lower():
-                            print("You tried to %s to %s, while this package "
-                                  "is locked to %s" % (command, repo, server))
-                            sys.exit(1)
-                        else:
-                            #repo OK
-                            pass
-                    except IndexError:
-                        #end of args
-                        pass
-                i=i+1
-
-            if repo is None:
-                #no repo found for the command
-                print("Adding repository %s to the command %s" % (
-                    server, command ))
-                sys.argv[commandpos+1:commandpos+1] = ['-r', server]
-                changed = True
-
-    if changed:
-        print("Final command: %s" % (' '.join(sys.argv)))
-
-
-def check_repository(name):
-    server = None
-    # find repository in .pypirc file
-    rc = os.path.join(os.path.expanduser('~'), '.pypirc')
-    if os.path.exists(rc):
-        config = ConfigParser()
-        config.read(rc)
-        if 'distutils' in config.sections():
-            # let's get the list of servers
-            index_servers = config.get('distutils', 'index-servers')
-            _servers = [s.strip() for s in index_servers.split('\n')
-                        if s.strip() != '']
-            for srv in _servers:
-                if srv == name:
-                    repos = config.get(srv, 'repository')
-                    print("Found repository %s for %s in '%s'" % (
-                        repos, name, rc))
-                    server = repos
-                    break
-
-    if not server:
-        print("No repository for %s found in '%s'" % (name, rc))
-        sys.exit(1)
-
-    inject_repository_url(server)
-
-
-def check_server(server):
-    if not server:
-        return
-    inject_repository_url(server)
-
-
-# use one of these to check the correct destination:
-PYPI_KEY = 'visaplan'
-PYPI_URL = 'https://pypi.visaplan.com'
-
-for command in COMMANDS_WATCHED:
-    if command in sys.argv:
-        check_repository(PYPI_KEY)
-        # check_server(PYPI_URL)
-        break
-# ---------------------------------------- ] ... destination locking ]
-
-
 # ------------------------------------------- [ for setup_kwargs ... [
 long_description = '\n\n'.join([
     open('README.rst').read(),
     open('CONTRIBUTORS.rst').read(),
+    open('TODO.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 # see as well --> src/visaplan/plone/animations/configure.zcml:
 exclude_subpackages = (
         )
 exclude_packages = []
@@ -207,18 +112,25 @@
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
@@ -259,30 +171,30 @@
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
         'plone.dexterity',
         # -*- Extra requirements: -*-
-        'visaplan.plone.ajaxnavigation',
-        'visaplan.plone.behaviors',
-        'visaplan.plone.staticthumbnails >=1.0.dev3',
+        'visaplan.plone.behaviors >=1.1.0',
+        'visaplan.plone.staticthumbnails >=1.2.0',
         'plone.api',
         'Products.GenericSetup>=1.8.2',
         'z3c.jbot',
         # checked requirements (from imports):
         "plone.app.upgrade",
         "plone.autoform",
         "plone.behavior",
         "plone.supermodel",
         "Products.CMFPlone",
-        "visaplan.tools",
         "zope.component",
         "zope.i18nmessageid",
         "zope.interface",
         "zope.publisher",
         "zope.schema",
         # imported by test code:
         "plone.browserlayer",
@@ -302,8 +214,13 @@
         ],
     },
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

