# Comparing `tmp/qt-custom-0.2.8.tar.gz` & `tmp/qt-custom-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\pip_package\qt-custom\dist\.tmp-8egofrgh\qt-custom-0.2.8.tar", last modified: Mon May  1 00:32:47 2023, max compression
+gzip compressed data, was "C:\pip_package\qt-custom\dist\.tmp-uubrnti7\qt-custom-0.2.9.tar", last modified: Mon May  1 02:49:30 2023, max compression
```

## Comparing `qt-custom-0.2.8.tar` & `qt-custom-0.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/
--rw-rw-rw-   0        0        0     1091 2021-12-14 06:26:44.000000 qt-custom-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2022-02-04 21:52:02.000000 qt-custom-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      485 2023-05-01 00:32:47.000000 qt-custom-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       17 2022-02-04 22:03:27.000000 qt-custom-0.2.8/README.md
--rw-rw-rw-   0        0        0      102 2021-12-14 05:48:57.000000 qt-custom-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0      630 2023-05-01 00:32:47.000000 qt-custom-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom/
--rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.8/source/qt_custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom/chart/
--rw-rw-rw-   0        0        0   693248 2023-05-01 00:27:09.000000 qt-custom-0.2.8/source/qt_custom/chart/custom_chart.pyd
--rw-rw-rw-   0        0        0   118784 2023-05-01 00:27:11.000000 qt-custom-0.2.8/source/qt_custom/chart/custom_color.pyd
--rw-rw-rw-   0        0        0   248832 2023-05-01 00:27:13.000000 qt-custom-0.2.8/source/qt_custom/chart/custom_lineseries.pyd
--rw-rw-rw-   0        0        0   427520 2023-05-01 00:27:15.000000 qt-custom-0.2.8/source/qt_custom/chart/custom_markers.pyd
--rw-rw-rw-   0        0        0   207872 2023-05-01 00:08:25.000000 qt-custom-0.2.8/source/qt_custom/custom_listview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    81408 2023-05-01 00:08:28.000000 qt-custom-0.2.8/source/qt_custom/custom_menubar.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   116736 2023-05-01 00:08:26.000000 qt-custom-0.2.8/source/qt_custom/custom_tab.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   123904 2023-05-01 00:08:27.000000 qt-custom-0.2.8/source/qt_custom/custom_tableview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   109568 2023-05-01 00:08:28.000000 qt-custom-0.2.8/source/qt_custom/custom_treeview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    45056 2023-05-01 00:08:29.000000 qt-custom-0.2.8/source/qt_custom/logger_qt_custom.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom/qt5/
--rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.8/source/qt_custom/qt5/__init__.py
--rw-rw-rw-   0        0        0   639488 2022-11-08 03:37:38.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_chart.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   136704 2022-11-08 03:37:40.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_color.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   123904 2022-11-08 03:37:40.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_lineseries.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   194048 2022-10-05 04:03:27.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_listview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   347136 2022-11-08 03:37:43.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_markers.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    90112 2022-10-05 04:03:29.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_menubar.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   131584 2022-10-05 04:03:27.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_tab.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   138240 2022-10-05 04:03:28.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_tableview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   130048 2022-10-05 04:03:29.000000 qt-custom-0.2.8/source/qt_custom/qt5/custom_treeview.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom.egg-info/
--rw-rw-rw-   0        0        0      485 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 00:32:47.000000 qt-custom-0.2.8/source/qt_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/
+-rw-rw-rw-   0        0        0     1091 2021-12-14 06:26:44.000000 qt-custom-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2022-02-04 21:52:02.000000 qt-custom-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      485 2023-05-01 02:49:30.000000 qt-custom-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2022-02-04 22:03:27.000000 qt-custom-0.2.9/README.md
+-rw-rw-rw-   0        0        0      102 2021-12-14 05:48:57.000000 qt-custom-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0      630 2023-05-01 02:49:30.000000 qt-custom-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom/
+-rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.9/source/qt_custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom/chart/
+-rw-rw-rw-   0        0        0   693248 2023-05-01 02:47:57.000000 qt-custom-0.2.9/source/qt_custom/chart/custom_chart.pyd
+-rw-rw-rw-   0        0        0   118272 2023-05-01 02:47:58.000000 qt-custom-0.2.9/source/qt_custom/chart/custom_color.pyd
+-rw-rw-rw-   0        0        0   251392 2023-05-01 02:48:00.000000 qt-custom-0.2.9/source/qt_custom/chart/custom_lineseries.pyd
+-rw-rw-rw-   0        0        0   443392 2023-05-01 02:48:03.000000 qt-custom-0.2.9/source/qt_custom/chart/custom_markers.pyd
+-rw-rw-rw-   0        0        0   207872 2023-05-01 00:08:25.000000 qt-custom-0.2.9/source/qt_custom/custom_listview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    81408 2023-05-01 00:08:28.000000 qt-custom-0.2.9/source/qt_custom/custom_menubar.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   116736 2023-05-01 00:08:26.000000 qt-custom-0.2.9/source/qt_custom/custom_tab.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   123904 2023-05-01 00:08:27.000000 qt-custom-0.2.9/source/qt_custom/custom_tableview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   109568 2023-05-01 00:08:28.000000 qt-custom-0.2.9/source/qt_custom/custom_treeview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    45056 2023-05-01 00:08:29.000000 qt-custom-0.2.9/source/qt_custom/logger_qt_custom.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom/qt5/
+-rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.9/source/qt_custom/qt5/__init__.py
+-rw-rw-rw-   0        0        0   639488 2022-11-08 03:37:38.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_chart.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   136704 2022-11-08 03:37:40.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_color.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   123904 2022-11-08 03:37:40.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_lineseries.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   194048 2022-10-05 04:03:27.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_listview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   347136 2022-11-08 03:37:43.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_markers.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    90112 2022-10-05 04:03:29.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_menubar.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   131584 2022-10-05 04:03:27.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_tab.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   138240 2022-10-05 04:03:28.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_tableview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   130048 2022-10-05 04:03:29.000000 qt-custom-0.2.9/source/qt_custom/qt5/custom_treeview.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 02:49:30.000000 qt-custom-0.2.9/source/qt_custom.egg-info/top_level.txt
```

### Comparing `qt-custom-0.2.8/LICENSE.txt` & `qt-custom-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt-custom-0.2.8/setup.cfg` & `qt-custom-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 742d 6375 7374 6f6d 0d0a 7665   = qt-custom..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 380d 0a61  rsion = 0.2.8..a
+00000020: 7273 696f 6e20 3d20 302e 322e 390d 0a61  rsion = 0.2.9..a
 00000030: 7574 686f 7220 3d20 616e 6f6e 796d 6f75  uthor = anonymou
 00000040: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
 00000050: 3d20 616e 6f6e 796d 6f75 7340 676d 6169  = anonymous@gmai
 00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000070: 6f6e 203d 2043 7573 746f 6d69 7a65 6420  on = Customized 
 00000080: 5174 2043 6c61 7373 6573 0d0a 6c6f 6e67  Qt Classes..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `qt-custom-0.2.8/source/qt_custom.egg-info/SOURCES.txt` & `qt-custom-0.2.9/source/qt_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

