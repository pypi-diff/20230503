# Comparing `tmp/LinkChecker_GUI-10.0.0a3.tar.gz` & `tmp/LinkChecker_GUI-10.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr 21 18:37:43 2023, max compression
+gzip compressed data, last modified: Wed May  3 18:31:49 2023, max compression
```

## Comparing `LinkChecker_GUI-10.0.0a3.tar` & `LinkChecker_GUI-10.0.0a4.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0      752 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.flake8
--rw-r--r--   0        0        0      125 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.git_archival.txt
--rw-r--r--   0        0        0       31 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.gitattributes
--rw-r--r--   0        0        0      104 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.yamllint
--rw-r--r--   0        0        0      115 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/changelog.txt
--rw-r--r--   0        0        0      689 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/pyoxidizer.bzl
--rw-r--r--   0        0        0      456 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tox.ini
--rw-r--r--   0        0        0     3330 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/de.po
--rw-r--r--   0        0        0      214 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/linkchecker-gui.desktop
--rw-r--r--   0        0        0      127 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/po4a.conf
--rw-r--r--   0        0        0     1003 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/de/linkchecker-gui.1
--rw-r--r--   0        0        0      686 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/en/linkchecker-gui.1
--rw-r--r--   0        0        0    67271 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/favicon.icns
--rw-r--r--   0        0        0     3638 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/favicon.ico
--rw-r--r--   0        0        0      144 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/html.footer
--rw-r--r--   0        0        0      764 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/html.header
--rw-r--r--   0        0        0     6893 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/index.txt
--rw-r--r--   0        0        0      746 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/lccollection.qhcp
--rw-r--r--   0        0        0      476 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/lcdoc.qhp
--rw-r--r--   0        0        0     3224 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/pygments.css
--rw-r--r--   0        0        0     5382 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/sphinxdoc.css
--rw-r--r--   0        0        0    26618 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/128x128/linkchecker-gui.png
--rw-r--r--   0        0        0     1085 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/16x16/linkchecker-gui.png
--rw-r--r--   0        0        0     3254 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/32x32/linkchecker-gui.png
--rw-r--r--   0        0        0     6232 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/48x48/linkchecker-gui.png
--rw-r--r--   0        0        0     9761 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/64x64/linkchecker-gui.png
--rw-r--r--   0        0        0    24421 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/__init__.py
--rw-r--r--   0        0        0     2508 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/__main__.py
--rw-r--r--   0        0        0      212 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/_release.py
--rw-r--r--   0        0        0     1573 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/checker.py
--rw-r--r--   0        0        0     2545 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/configuration.py
--rw-r--r--   0        0        0     2580 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/contextmenu.py
--rw-r--r--   0        0        0     1541 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/debug.py
--rw-r--r--   0        0        0     6677 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor.py
--rw-r--r--   0        0        0     4004 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qsci.py
--rw-r--r--   0        0        0     6194 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qt.py
--rw-r--r--   0        0        0     2905 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/help.py
--rw-r--r--   0        0        0     9685 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/lineedit.py
--rw-r--r--   0        0        0    52172 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_rc.py
--rw-r--r--   0        0        0     1666 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_debug.py
--rw-r--r--   0        0        0     2717 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_editor.py
--rw-r--r--   0        0        0    56784 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_main.py
--rw-r--r--   0        0        0     8958 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_options.py
--rw-r--r--   0        0        0     2442 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/logger.py
--rw-r--r--   0        0        0     4135 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/options.py
--rw-r--r--   0        0        0     7561 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/projects.py
--rw-r--r--   0        0        0     2896 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/properties.py
--rw-r--r--   0        0        0     3333 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/recentdocs.py
--rw-r--r--   0        0        0     5746 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/settings.py
--rw-r--r--   0        0        0     2060 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/statistics.py
--rw-r--r--   0        0        0     3480 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/syntax.py
--rw-r--r--   0        0        0     3561 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/updater.py
--rw-r--r--   0        0        0     6925 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/urlmodel.py
--rw-r--r--   0        0        0     2720 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/urlsave.py
--rw-r--r--   0        0        0     1419 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/validator.py
--rw-r--r--   0        0        0    94208 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lccollection.qhc
--rw-r--r--   0        0        0    77824 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lcdoc.qch
--rw-r--r--   0        0        0        0 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/__init__.py
--rw-r--r--   0        0        0     1171 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/containers.py
--rw-r--r--   0        0        0     1259 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/fileutil.py
--rw-r--r--   0        0        0        0 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/__init__.py
--rw-r--r--   0        0        0     2347 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chrome.py
--rw-r--r--   0        0        0     2550 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chromium.py
--rw-r--r--   0        0        0     1733 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/firefox.py
--rw-r--r--   0        0        0     1700 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/opera.py
--rw-r--r--   0        0        0     1428 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/safari.py
--rw-r--r--   0        0        0     1302 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/winutil.py
--rw-r--r--   0        0        0     1668 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/test_containers.py
--rw-r--r--   0        0        0     1287 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/test_gui.py
--rw-r--r--   0        0        0     4084 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tools/hatch_build.py
--rw-r--r--   0        0        0      897 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.gitignore
--rw-r--r--   0        0        0    35141 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/LICENSE
--rw-r--r--   0        0        0      761 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/README.md
--rw-r--r--   0        0        0     2286 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0      752 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.flake8
+-rw-r--r--   0        0        0      125 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.git_archival.txt
+-rw-r--r--   0        0        0       31 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.gitattributes
+-rw-r--r--   0        0        0       38 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.pylintrc
+-rw-r--r--   0        0        0      104 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.yamllint
+-rw-r--r--   0        0        0      115 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/changelog.txt
+-rw-r--r--   0        0        0      689 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/pyoxidizer.bzl
+-rw-r--r--   0        0        0      700 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tox.ini
+-rw-r--r--   0        0        0     3330 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/de.po
+-rw-r--r--   0        0        0      214 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/linkchecker-gui.desktop
+-rw-r--r--   0        0        0      127 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/po4a.conf
+-rw-r--r--   0        0        0     1003 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/de/linkchecker-gui.1
+-rw-r--r--   0        0        0      686 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/en/linkchecker-gui.1
+-rw-r--r--   0        0        0    67271 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/favicon.icns
+-rw-r--r--   0        0        0     3638 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/favicon.ico
+-rw-r--r--   0        0        0      144 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/html.footer
+-rw-r--r--   0        0        0      764 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/html.header
+-rw-r--r--   0        0        0     6893 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/index.txt
+-rw-r--r--   0        0        0      746 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/lccollection.qhcp
+-rw-r--r--   0        0        0      476 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/lcdoc.qhp
+-rw-r--r--   0        0        0     3224 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/pygments.css
+-rw-r--r--   0        0        0     5382 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/sphinxdoc.css
+-rw-r--r--   0        0        0    26618 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/128x128/linkchecker-gui.png
+-rw-r--r--   0        0        0     1085 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/16x16/linkchecker-gui.png
+-rw-r--r--   0        0        0     3254 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/32x32/linkchecker-gui.png
+-rw-r--r--   0        0        0     6232 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/48x48/linkchecker-gui.png
+-rw-r--r--   0        0        0     9761 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/64x64/linkchecker-gui.png
+-rw-r--r--   0        0        0    24415 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/__init__.py
+-rw-r--r--   0        0        0     2545 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/__main__.py
+-rw-r--r--   0        0        0      212 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/_release.py
+-rw-r--r--   0        0        0     1573 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/checker.py
+-rw-r--r--   0        0        0     2545 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/configuration.py
+-rw-r--r--   0        0        0     2580 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/contextmenu.py
+-rw-r--r--   0        0        0     1541 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/debug.py
+-rw-r--r--   0        0        0     6687 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor.py
+-rw-r--r--   0        0        0     4004 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qsci.py
+-rw-r--r--   0        0        0     6194 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qt.py
+-rw-r--r--   0        0        0     2905 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/help.py
+-rw-r--r--   0        0        0     9685 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/lineedit.py
+-rw-r--r--   0        0        0    52172 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_rc.py
+-rw-r--r--   0        0        0     1666 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_debug.py
+-rw-r--r--   0        0        0     2717 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_editor.py
+-rw-r--r--   0        0        0    56784 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_main.py
+-rw-r--r--   0        0        0     8958 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_options.py
+-rw-r--r--   0        0        0     2442 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/logger.py
+-rw-r--r--   0        0        0     4135 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/options.py
+-rw-r--r--   0        0        0     7561 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/projects.py
+-rw-r--r--   0        0        0     2896 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/properties.py
+-rw-r--r--   0        0        0     3333 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/recentdocs.py
+-rw-r--r--   0        0        0     5746 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/settings.py
+-rw-r--r--   0        0        0     2060 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/statistics.py
+-rw-r--r--   0        0        0     3480 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/syntax.py
+-rw-r--r--   0        0        0     3598 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/updater.py
+-rw-r--r--   0        0        0     6926 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlmodel.py
+-rw-r--r--   0        0        0     2754 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlsave.py
+-rw-r--r--   0        0        0     1419 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/validator.py
+-rw-r--r--   0        0        0    94208 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lccollection.qhc
+-rw-r--r--   0        0        0    77824 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lcdoc.qch
+-rw-r--r--   0        0        0        0 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/fileutil.py
+-rw-r--r--   0        0        0     2179 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/url.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/__init__.py
+-rw-r--r--   0        0        0     2347 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chrome.py
+-rw-r--r--   0        0        0     2550 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chromium.py
+-rw-r--r--   0        0        0     1733 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/firefox.py
+-rw-r--r--   0        0        0     1700 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/opera.py
+-rw-r--r--   0        0        0     1428 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/safari.py
+-rw-r--r--   0        0        0     1302 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/winutil.py
+-rw-r--r--   0        0        0     1668 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/__init__.py
+-rw-r--r--   0        0        0     1437 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/test_gui.py
+-rw-r--r--   0        0        0     1079 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/library/test_fileutil.py
+-rw-r--r--   0        0        0     4245 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tools/hatch_build.py
+-rw-r--r--   0        0        0      897 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.gitignore
+-rw-r--r--   0        0        0    35141 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/LICENSE
+-rw-r--r--   0        0        0     1451 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/README.md
+-rw-r--r--   0        0        0     2286 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2248 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/PKG-INFO
```

### Comparing `linkchecker_gui-10.0.0a3/.flake8` & `LinkChecker_GUI-10.0.0a4/.flake8`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/pyoxidizer.bzl` & `LinkChecker_GUI-10.0.0a4/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/de.po` & `LinkChecker_GUI-10.0.0a4/doc/de.po`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/de/linkchecker-gui.1` & `LinkChecker_GUI-10.0.0a4/doc/de/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/en/linkchecker-gui.1` & `LinkChecker_GUI-10.0.0a4/doc/en/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/favicon.icns` & `LinkChecker_GUI-10.0.0a4/doc/html/favicon.icns`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/favicon.ico` & `LinkChecker_GUI-10.0.0a4/doc/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/html.header` & `LinkChecker_GUI-10.0.0a4/doc/html/html.header`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/index.txt` & `LinkChecker_GUI-10.0.0a4/doc/html/index.txt`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/lccollection.qhcp` & `LinkChecker_GUI-10.0.0a4/doc/html/lccollection.qhcp`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/pygments.css` & `LinkChecker_GUI-10.0.0a4/doc/html/pygments.css`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/sphinxdoc.css` & `LinkChecker_GUI-10.0.0a4/doc/html/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/logo/128x128/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0a4/doc/html/logo/128x128/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/logo/16x16/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0a4/doc/html/logo/16x16/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/logo/32x32/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0a4/doc/html/logo/32x32/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/logo/48x48/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0a4/doc/html/logo/48x48/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/doc/html/logo/64x64/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0a4/doc/html/logo/64x64/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/__init__.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,50 +10,50 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
+from enum import Enum
 import os
 import re
 import sys
 import webbrowser
 
 from linkcheck import LinkCheckerError
 from linkcheck import checker as linkchecker_checker
 from linkcheck import configuration as linkchecker_configuration
-from linkcheck import (director, get_link_pat, httputil, i18n, logconf,
+from linkcheck import (director, get_link_pat, httputil, logconf,
                        mimeutil, strformat)
-from linkcheck import url as urlutil
 from linkcheck.parser import parse_text
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 from . import configuration
 from .checker import CheckerThread
 from .contextmenu import ContextMenu
 from .debug import LinkCheckerDebug
 from .editor import EditorWindow
 from .help import HelpWindow
-from .library.containers import enum
+from .library import url as urlutil
 from .linkchecker_ui_main import Ui_MainWindow
 from .logger import GuiLogHandler, SignalLogger, StatusLogger
 from .options import LinkCheckerOptions
 from .projects import ProjectExt, loadproject, openproject, saveproject
 from .properties import clear_properties, set_properties
 from .recentdocs import RecentDocumentModel
 from .settings import Settings
 from .statistics import clear_statistics, set_statistics
 # XXX from .updater import UpdateDialog
 from .urlmodel import UrlItemModel
 from .urlsave import urlsave
 
 DocBaseUrl = "qthelp://linkchecker.app.linkchecker-gui/doc/"
 RegistryBase = "LinkChecker-GUI"
-Status = enum('idle', 'checking')
+Status = Enum("Status", ["idle", "checking"])
 
 MaxMessageLength = 60
 
 
 def get_icon(name):
     """Return QIcon with given pixmap resource name."""
     icon = QtGui.QIcon()
@@ -126,27 +126,28 @@
             self.urlinput.setText(url)
         elif documents:
             self.urlinput.setText(documents[0])
 
     def init_menu(self):
         """Add menu entries for bookmark file checking."""
         self.urlinput.addMenuEntries(self.menuEdit)
-        return  # XXX
+        """  # XXX
         self.menuLang = self.menuEdit.addMenu(_('Languages'))
         self.menuLang.setTitle(_("&Language"))
         # ensure only one action is checked
         langActionGroup = QtGui.QActionGroup(self)
         langActionGroup.triggered.connect(self.switch_language)
         for i, lang in enumerate(sorted(i18n.supported_languages)):
             action = self.menuLang.addAction("&%d %s" % (i, lang))
             action.setCheckable(True)
             action.setData(lang)
             if lang == i18n.default_language:
                 action.setChecked(True)
             langActionGroup.addAction(action)
+        """
 
     def init_drop(self):
         """Set and activate drag-and-drop functions."""
         self.__class__.dragEnterEvent = self.handleDragEvent
         self.__class__.dragMoveEvent = self.handleDragEvent
         self.__class__.dropEvent = self.handleDropEvent
         self.setAcceptDrops(True)
@@ -540,15 +541,15 @@
                 urlitem.url_data.column,
             )
 
     def view_source(self, url, line, col):
         """View URL source in editor window."""
         self.editor.setWindowTitle("View %s" % url)
         self.editor.setUrl(url)
-        data, info = urlutil.get_content(url, proxy=self.config["proxy"])
+        data, info = urlutil.get_content(url)
         if data is None:
             msg = _("An error occurred retreiving URL `%s': %s.") % (url, info)
             self.editor.setText(msg)
         else:
             content_type = httputil.get_content_type(info)
             if not content_type:
                 # read function for content type guessing
@@ -626,15 +627,17 @@
         """Translate menu titles."""
         super().retranslateUi(Window)
         # self.menu_lang is created after calling retranslateUi
         # the first time, so check for its excistance
         if hasattr(self, "menu_lang"):
             self.menuLang.setTitle(_("&Language"))
 
+    '''  # XXX
     def switch_language(self, action):
         """Change UI language."""
         lang = str(action.data().toString())
         i18n.install_language(lang)
         self.retranslateUi(self)
         self.options.retranslateUi(self.options)
         self.debug.retranslateUi(self.debug)
         self.editor.retranslateUi(self.editor)
+    '''
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/__main__.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 import signal
 import sys
 
 from linkcheck import configuration
 from linkcheck.command.linkchecker import drop_privileges
 from linkcheck.fileutil import is_readable
-from PyQt6.QtWidgets import QApplication
+from PyQt6.QtWidgets import QApplication  # pylint: disable=no-name-in-module
 
 from . import LinkCheckerMain
 from .projects import ProjectExt
 
 
 def excepthook(window, etype, evalue, tb):
     """Catch unhandled exceptions."""
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/checker.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/checker.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/configuration.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/configuration.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/contextmenu.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/contextmenu.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/debug.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/debug.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/editor.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         saved = False
         try:
             try:
                 fh = QtCore.QFile(self.filename)
                 if not fh.open(QtCore.QIODevice.OpenModeFlag.WriteOnly):
                     raise OSError(fh.errorString())
                 stream = QtCore.QTextStream(fh)
-                stream.setCodec("UTF-8")
+                stream.setAutoDetectUnicode(False)
                 stream << self.editor.text()
                 self.editor.setModified(False)
                 saved = True
             except OSError as e:
                 err = QtWidgets.QMessageBox(self)
                 err.setText(str(e))
                 err.exec()
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qsci.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qsci.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qt.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qt.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/help.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/help.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/lineedit.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/lineedit.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_rc.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_rc.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_debug.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_debug.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_editor.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_editor.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_main.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_main.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_options.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_options.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/logger.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/logger.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/options.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/options.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/projects.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/projects.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/properties.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/properties.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/recentdocs.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/recentdocs.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/settings.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/settings.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/statistics.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/statistics.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/syntax.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/syntax.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/updater.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
+# pylint: disable=no-name-in-module
+
 from PyQt6 import QtCore, QtWidgets
 from linkcheck import updater, configuration
 
 
 class UpdateThread(QtCore.QThread):
     """Thread to check for updated versions."""
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/urlmodel.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             return EmptyQVariant
         urlitem = self.urls[index.row()]
         column = index.column()
         if role == QtCore.Qt.ItemDataRole.DisplayRole:
             return V(urlitem.display[column])
         elif role == QtCore.Qt.ItemDataRole.ToolTipRole:
             return V(urlitem.tooltips[column])
-        elif role == QtCore.Qt.ItemDataRole.TextColorRole and column == 3:
+        elif role == QtCore.Qt.ItemDataRole.ForegroundRole and column == 3:
             return QtGui.QColor(urlitem.result_color)
         else:
             return EmptyQVariant
 
     def headerData(self, section, orientation, role):
         """Return header column data for given parameters."""
         if (orientation == QtCore.Qt.Orientation.Horizontal
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/urlsave.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlsave.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     Return dialog result."""
     title = _("Save check results")
     func = QtWidgets.QFileDialog.getSaveFileName
     logtype = parent.saveresultas if parent.saveresultas else 'html'
     filters = ";;".join(sortwithfirst(LoggerFilters, Logtype2Filter[logtype]))
     filename = "linkchecker-out" + Logtype2FileExt[logtype]
     filename, selectedFilter = func(parent, title, filename, filters)
-    logtype = Filter2Logtype.get(selectedFilter)
+    logtype = Filter2Logtype.get(selectedFilter if selectedFilter else FilterHtml)
     return filename, logtype
 
 
 def sortwithfirst(sequence, firstelement):
     """Move firstelement in a sequence to the first position."""
     res = []
     for elem in sequence:
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/validator.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/validator.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lccollection.qhc` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lccollection.qhc`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4,25 +4,25 @@
 INSERT INTO NamespaceTable VALUES(1,'linkchecker.app.linkchecker-gui','lcdoc.qch');
 CREATE TABLE FolderTable (Id INTEGER PRIMARY KEY, NamespaceId INTEGER, Name TEXT );
 INSERT INTO FolderTable VALUES(1,1,'doc');
 CREATE TABLE FilterAttributeTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterNameTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterTable (NameId INTEGER, FilterAttributeId INTEGER );
 CREATE TABLE SettingsTable (Key TEXT PRIMARY KEY, Value BLOB );
-INSERT INTO SettingsTable VALUES('LastRegisterTime','2023-04-21T18:37:43.000');
+INSERT INTO SettingsTable VALUES('LastRegisterTime','2023-05-03T18:31:49.000');
 INSERT INTO SettingsTable VALUES('WindowTitle','LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('LastShownPages','qthelp://linkchecker.app.linkchecker-gui/doc/index.html');
 INSERT INTO SettingsTable VALUES('CacheDirectory','linkchecker/LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('CacheDirRelativeToCollection',0);
 INSERT INTO SettingsTable VALUES('EnableFilterFunctionality',0);
 INSERT INTO SettingsTable VALUES('HideFilterFunctionality',1);
 INSERT INTO SettingsTable VALUES('EnableDocumentationManager',0);
 INSERT INTO SettingsTable VALUES('EnableAddressBar',0);
 INSERT INTO SettingsTable VALUES('HideAddressBar',1);
-INSERT INTO SettingsTable VALUES('CreationTime',1682102263);
+INSERT INTO SettingsTable VALUES('CreationTime',1683138709);
 INSERT INTO SettingsTable VALUES('FullTextSearchFallback',0);
 INSERT INTO SettingsTable VALUES('ApplicationIcon',X'89504e470d0a1a0a0000000d49484452000000100000001008060000001ff3ff6100000006624b474400ff00ff00ffa0bda79300000009704859730000375c0000375c01cbc7a4b9000003af4944415438cb05c15b681c550006e0ff9c33979dd95b92cd65d324dd6ed2b4696252a4d634a285168b979712a1166c51fba214aa0f8a102df8526b0b62147c284aa95044a9a4e08bb7b41830921242adb59590d0682fc9ee26d9cbccecccececccec397e1f99fc6206aa2aa152ae92030787c8537bb7f2b3677ede5628d7f6d782c68e5cdec2ed3bb9e5c0adff162aea6aac4923a11f824a544000d2d2721194803c582c886ac5ef9899593e1b694b1ccd6c69893edab0452eef40ed6c26ccad5b81eb5fae6e981f1a6bc54aefe3bd448d4882ed1a3c4cec9223ea10bd03bb7ba6b5eed421afbd455a63b2c88754747626851c8b408b451489d151cae86116517f322a6e85324a089005b0553bfdd107b3ed035d7bc25434686a92250846fe7e688ab575078a1790dc83a2084c37ac976cd9339c9b3a0f9f093c5e6327dfb9846ddb87decd0cf5bc6ac309e6af7c2eafcdfd8a1e6e92375f1c251d1a274b7913d53a8161d598ef8741e885dd1cb00d2ffc835e987c497605394e34051b2e6785643f6e4507c8955bf7a14a0cfbba2278b6b584ed6995c4123a882cb1788b8e7447e2f58dbca9b378e7e921b92936c1a3aa54957544fb4648ac6f042f8f0d81afdfc3f1b72670fbcf058c3f9186132a585aade3e9914ee2397eb262793fb0fee1f111aa2b272c50114f28786408f264ab8ce75265bc71ee22ea7d8750d7bab070ed2a0c9780c632304a16ca25872574794a8a4615cff242d09a07d751301abd86533bbbf1f1e5ff80fee7b1b5f731d44c0b1b0d1d7a2285a46028e6eb500114cbae47635a6485f0b058b508d1cc799cdb7b01851b27706335444b5b2faa850202db81de9c056551e83290d415e238fea6697a2bf4e6663ccfa8f2bbe217f1de9e2fb9d4d8c467d37de0b111f8a601df09601b35488127ba9a15908668944a36bc7a38abb5c6f3d4bcd384bbff463f39357615633b73e49b69ce57c4313469ba08ac1ae44603d9942632299d1472267fb85a2101879064f6a92e5348f7bf7e01f9a2e81bded58ebfeedaf86afe2051fb86797794139b521151181cd3c1e2aad988e82ab8aa301af0f7a5a43e8706a774bdc407b3d98e49b7e6e1e28fca9a9f7ea51c4d3753574f20d9dd4e0ca6923c224864b730b525e1534adfceee1f3aaf690ac9f4a739dbb73b7eb4bd991c9959a8d8672e85af8535e93bdb323265bbde52a8380ae7752e372cd3df5c99b5efcd9d54d2fddf57560a3477fd5b6198040448d22307cc09cb01ff651ee7e33a3aec1ad20474871c4975060d3444505c05c422082bb40d8ebb9bff4c8500706c4ae07f702bc1c500e2ed86000000227a545874536f667477617265000078da2b2f2fd7cbcccb2e4e4e2c48d5cb2f4a070036d806581053ca5c0000000049454e44ae426082');
 CREATE TABLE FileNameTable (FolderId INTEGER, Name TEXT, FileId INTEGER PRIMARY KEY, Title TEXT);
 INSERT INTO FileNameTable VALUES(1,'index.html',1,'Check websites for broken links');
 INSERT INTO FileNameTable VALUES(1,'pygments.css',2,'pygments.css');
 INSERT INTO FileNameTable VALUES(1,'sphinxdoc.css',3,'sphinxdoc.css');
 INSERT INTO FileNameTable VALUES(1,'logo/64x64/linkchecker-gui.png',4,'linkchecker-gui.png');
@@ -31,15 +31,15 @@
 INSERT INTO ContentsTable VALUES(1,1,X'00000000000000140069006e006400650078002e00680074006d006c00000032004c0069006e006b0043006800650063006b0065007200200064006f00630075006d0065006e0074006100740069006f006e');
 CREATE TABLE FileFilterTable (FilterAttributeId INTEGER, FileId INTEGER);
 CREATE TABLE IndexFilterTable (FilterAttributeId INTEGER, IndexId INTEGER);
 CREATE TABLE ContentsFilterTable (FilterAttributeId INTEGER, ContentsId INTEGER );
 CREATE TABLE FileAttributeSetTable (NamespaceId INTEGER, FilterAttributeSetId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE OptimizedFilterTable (NamespaceId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE TimeStampTable (NamespaceId INTEGER, FolderId INTEGER, FilePath TEXT, Size INTEGER, TimeStamp TEXT);
-INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2023-04-21T18:37:43');
+INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2023-05-03T18:31:49');
 CREATE TABLE VersionTable (NamespaceId INTEGER, Version TEXT);
 INSERT INTO VersionTable VALUES(1,NULL);
 CREATE TABLE Filter (FilterId INTEGER PRIMARY KEY, Name TEXT);
 CREATE TABLE ComponentTable (ComponentId INTEGER PRIMARY KEY, Name TEXT);
 INSERT INTO ComponentTable VALUES(1,'doc');
 CREATE TABLE ComponentMapping (ComponentId INTEGER, NamespaceId INTEGER);
 INSERT INTO ComponentMapping VALUES(1,1);
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lcdoc.qch` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lcdoc.qch`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/containers.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/opera.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,50 @@
-# Copyright (C) 2004-2014 Bastian Kleineidam
+# Copyright (C) 2011-2014 Bastian Kleineidam
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-"""
-Special container classes.
-"""
-
-from collections import namedtuple
-
-
-def enum(*names):
-    """Return an enum datatype instance from given list of keyword names.
-    The enum values are zero-based integers.
-
-    >>> Status = enum('open', 'pending', 'closed')
-    >>> Status.open
-    0
-    >>> Status.pending
-    1
-    >>> Status.closed
-    2
+
+import os
+
+# List of possible Opera bookmark files.
+OperaBookmarkFiles = (
+    "bookmarks.adr",  # for Opera >= 10.0
+    "opera6.adr",
+)
+
+
+def get_profile_dir():
+    """Return path where all profiles of current user are stored."""
+    if os.name == "nt":
+        basedir = os.environ["APPDATA"]
+        dirpath = os.path.join(basedir, "Opera", "Opera")
+    elif os.name == "posix":
+        dirpath = os.path.join(os.environ["HOME"], ".opera")
+    return dirpath
+
+
+def find_bookmark_file():
+    """Return the bookmark file of the Opera profile.
+    Returns absolute filename if found, or empty string if no bookmark file
+    could be found.
     """
-    return namedtuple('Enum', ' '.join(names))(*range(len(names)))
+    try:
+        dirname = get_profile_dir()
+        if os.path.isdir(dirname):
+            for name in OperaBookmarkFiles:
+                fname = os.path.join(dirname, name)
+                if os.path.isfile(fname):
+                    return fname
+    except Exception:
+        pass
+    return ""
```

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/fileutil.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/fileutil.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chrome.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chrome.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chromium.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chromium.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/firefox.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/firefox.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/safari.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/safari.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/winutil.py` & `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/winutil.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/tests/__init__.py` & `LinkChecker_GUI-10.0.0a4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/tests/test_gui.py` & `LinkChecker_GUI-10.0.0a4/tests/test_gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 import unittest
-import sys
 
 from . import need_pyqt, need_x11
 
 
 class TestGui(unittest.TestCase):
     """Test OMT GUI client."""
 
     @need_pyqt
     @need_x11
     def test_gui(self):
         from PyQt6 import QtCore, QtTest, QtWidgets
         from linkcheck_gui import LinkCheckerMain
 
-        app = QtWidgets.QApplication(sys.argv)
+        app = QtWidgets.QApplication([])
         window = LinkCheckerMain()
+        window.checker.finished.connect(window.close)
+        window.urlinput.setText("http://localhost/linkcheck-gui")
         window.show()
+        QtTest.QTest.qWaitForWindowExposed(window)
         QtTest.QTest.mouseClick(window.controlButton, QtCore.Qt.MouseButton.LeftButton)
-        window.close()
+        app.exec()
         del window
         del app
```

### Comparing `linkchecker_gui-10.0.0a3/tools/hatch_build.py` & `LinkChecker_GUI-10.0.0a4/tools/hatch_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,22 @@
 """)
 
         index_html = (Path(*HELP_SRC_DIR, "html.header").read_text()
                       + markdown2.markdown_path(str(Path(*HELP_SRC_DIR, "index.txt")))
                       + Path(*HELP_SRC_DIR, "html.footer").read_text())
         Path(*HELP_SRC_DIR, "index.html").write_text(index_html)
 
-        cp = subprocess.run(
-            ["pkg-config", "--variable=libexecdir", "Qt6Help"],
-            capture_output=True, text=True)
-        help_exec_dir = cp.stdout.strip()
+        try:
+            cp = subprocess.run(
+                ["pkg-config", "--variable=libexecdir", "Qt6Help"],
+                capture_output=True, text=True)
+            help_exec_dir = cp.stdout.strip()
+        except FileNotFoundError:
+            self.app.display_warning("pkg-config not installed")
+            help_exec_dir = None
         if help_exec_dir:
             help_generator = Path(help_exec_dir, "qhelpgenerator")
         else:
             # Ubuntu 22.04 doesn't provide Qt6Help.pc, 22.10 does but without libexecdir
             # qhelpgenerator found in bin on 22.04, libexec from 22.10
             help_generator = shutil.which(
                 "qhelpgenerator",
```

### Comparing `linkchecker_gui-10.0.0a3/.gitignore` & `LinkChecker_GUI-10.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/LICENSE` & `LinkChecker_GUI-10.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a3/pyproject.toml` & `LinkChecker_GUI-10.0.0a4/pyproject.toml`

 * *Files identical despite different names*

