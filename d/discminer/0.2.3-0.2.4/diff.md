# Comparing `tmp/discminer-0.2.3.tar.gz` & `tmp/discminer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.3.tar", last modified: Wed Apr 26 17:35:30 2023, max compression
+gzip compressed data, was "discminer-0.2.4.tar", last modified: Wed May  3 16:14:58 2023, max compression
```

## Comparing `discminer-0.2.3.tar` & `discminer-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.927434 discminer-0.2.3/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.3/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-26 17:35:30.927602 discminer-0.2.3/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.3/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.907942 discminer-0.2.3/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.3/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.3/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.3/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.3/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.3/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.3/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.3/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.3/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.3/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.3/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.3/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.3/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.918342 discminer-0.2.3/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.3/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-26 17:33:09.000000 discminer-0.2.3/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.3/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.3/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.3/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.3/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.3/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.3/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.922450 discminer-0.2.3/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.3/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.3/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.3/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    29646 2023-04-21 14:29:28.000000 discminer-0.2.3/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.3/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.3/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.923889 discminer-0.2.3/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.3/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.3/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.3/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.3/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.920134 discminer-0.2.3/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.3/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-26 17:35:30.928005 discminer-0.2.3/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.3/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.926759 discminer-0.2.3/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.3/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.3/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.3/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.3/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.946268 discminer-0.2.4/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.4/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-03 16:14:58.946473 discminer-0.2.4/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.4/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.920117 discminer-0.2.4/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.4/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.4/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.4/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.4/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.4/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.4/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.4/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.4/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.4/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.4/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.4/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.4/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.932706 discminer-0.2.4/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.4/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-03 16:11:57.000000 discminer-0.2.4/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.4/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.4/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.4/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.4/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.4/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.4/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.939831 discminer-0.2.4/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.4/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.4/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.4/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    29828 2023-05-03 15:29:17.000000 discminer-0.2.4/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.4/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.4/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.942021 discminer-0.2.4/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.4/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.4/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.4/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.4/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.934418 discminer-0.2.4/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.4/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-03 16:14:58.946931 discminer-0.2.4/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.4/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.945362 discminer-0.2.4/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.4/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.4/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.4/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.4/template/prepare_data.py
```

### Comparing `discminer-0.2.3/LICENSE` & `discminer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/PKG-INFO` & `discminer-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.3 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.4 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.3/README.md` & `discminer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/make_channels.py` & `discminer-0.2.4/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/make_parfile.py` & `discminer-0.2.4/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/make_single_moments.py` & `discminer-0.2.4/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_attributes_model.py` & `discminer-0.2.4/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.4/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_moment+offset.py` & `discminer-0.2.4/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_moment+residuals.py` & `discminer-0.2.4/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_peak_residuals.py` & `discminer-0.2.4/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_radial_profiles.py` & `discminer-0.2.4/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_residuals+all.py` & `discminer-0.2.4/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/plot_residuals+deproj.py` & `discminer-0.2.4/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/_mining/utils.py` & `discminer-0.2.4/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/cart.py` & `discminer-0.2.4/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/core.py` & `discminer-0.2.4/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/cube.py` & `discminer-0.2.4/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/disc2d.py` & `discminer-0.2.4/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/grid.py` & `discminer-0.2.4/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_box.png` & `discminer-0.2.4/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_cursor.jpeg` & `discminer-0.2.4/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_path.png` & `discminer-0.2.4/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_return.png` & `discminer-0.2.4/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_surface.png` & `discminer-0.2.4/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/icons/button_trash.jpg` & `discminer-0.2.4/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/pick.py` & `discminer-0.2.4/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/plottools.py` & `discminer-0.2.4/discminer/plottools.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
             dy = 2
         elif sposy>0:
             _va = 'bottom'
             dy = -1
         else:
             return 0
 
-    kwargs = dict(fontsize=SMALL_SIZE+3, ha='center', va=_va, weight='bold', rotation=0)
+    kwargs = dict(fontsize=SMALL_SIZE+3, ha='center', va=_va, weight='bold', zorder=20, rotation=0)
     kwargs.update(kwargs_text)
     for Ri in Rlist:
         ax.text(posx, sposy*(Ri+dy), fmt%Ri, **kwargs)
         
 def _make_text_1D_substructures(ax, gaps=[], rings=[], kinks=[],
                                 label_gaps=False, label_rings=False, label_kinks=False):
     kwargs_text = dict(fontsize=SMALL_SIZE+2, ha='center', va='bottom', transform=ax.transAxes, weight='bold', rotation=90)    
@@ -378,33 +378,36 @@
     kwargs_g.update(kwargs_gaps)
     kwargs_r.update(kwargs_rings)
     kwargs_k.update(kwargs_kinks)        
     if twodim:
         nphi = 100
         phi = np.linspace(0, 2*np.pi, nphi)
         phi_deg = np.degrees(phi-np.pi)
-        subst_fmt = zip([gaps, rings, kinks], ['D%d', 'B%d', 'K%d'], [label_gaps, label_rings, label_kinks])
+        subst_fmt = zip([gaps, rings, kinks],
+                        ['D%d', 'B%d', 'K%d'],
+                        [label_gaps, label_rings, label_kinks],
+                        [kwargs_g['color'], kwargs_r['color'], kwargs_k['color']])
         if polar:
             for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
             for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
             for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
 
-            for subst, fmt, label in subst_fmt:
+            for subst, fmt, label, color in subst_fmt:
                 if label:
-                    _make_text_2D(ax, subst, posx=-45, fmt=fmt)                
+                    _make_text_2D(ax, subst, posx=-45, fmt=fmt, color=color)                
         else:
             cos_phi = np.cos(phi)
             sin_phi = np.sin(phi)
             for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
             for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
             for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
 
-            for subst, fmt, label in subst_fmt:
+            for subst, fmt, label, color in subst_fmt:
                 if label:
-                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt)
+                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt, color=color)
             
     else:
         if func1d=='axvline': func1d=ax.axvline
         elif func1d=='axhline': func1d=ax.axhline            
         for R in gaps: func1d(R, **kwargs_g)
         for R in rings: func1d(R, **kwargs_r)
         for R in kinks: func1d(R, **kwargs_k)
```

### Comparing `discminer-0.2.3/discminer/rail.py` & `discminer-0.2.4/discminer/rail.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,119 +8,153 @@
 from .plottools import make_substructures as make_substruct
 from .tools.utils import hypot_func
 from . import constants as sfc
 from . import units as sfu
 import matplotlib.pyplot as plt
 import matplotlib
 import numpy as np
+from astropy import units as u
 from scipy.interpolate import griddata
 from skimage import measure
 import numbers
 
 get_sky_from_disc_coords = GridTools.get_sky_from_disc_coords
 
 class Rail(object):
-    def __init__(self, model, prop, coord_levels):
+    def __init__(self, model, prop, coord_levels=None):
         """
         Initialise Rail class. This class provides useful methods to compute azimuthal/radial contours and/or azimuthal averages from an input ``prop`` map projected on the sky.
         The methods in this class use the model disc vertical structure to convert sky to disc coordinates, and therefore all quantities returned are referred to the disc reference frame.
 
         Parameters
         ----------
         model : `.disc2d.General2d` instance
            Model to get the disc vertical structure from.
 
         prop : array_like, shape (nx, ny)
            Observable to be analysed, as projected on the sky.
         
-        coord_levels : array_like, shape (nlevels,)
-           Radial or azimuthal levels where *prop* will be mapped.           
+        coord_levels : array_like, shape (nlevels,), optional
+           Radial or azimuthal levels where *prop* will be mapped.
+
+              - If None, coord_levels are assumed to vary linearly and radially as np.arange(model.Rmin, model.Rmax, beam/4)
+              - Does not have any effect on the `Rail.make_filaments` method
         """
         
         _rail_coords = model.projected_coords
         X, Y = model.skygrid['meshgrid']        
         self.X = X/sfu.au
         self.Y = Y/sfu.au
 
         self.R = _rail_coords['R']
         self.phi = _rail_coords['phi']
         self.R_nonan = _rail_coords['R_nonan']                
         self.extent = model.skygrid['extent']
-        self.beam_size = model.beam_size.to('au').value
-        self.prop = prop
-        self.coord_levels = coord_levels
+        self.dpc = model.dpc
+        self.Rmin = model.Rmin
+        self.Rmax = model.Rmax        
+
+        self.beam_size = model.beam_size
+        self.header = model.header
+
+        self.prop = prop        
+        if coord_levels is None:
+            self.coord_levels = np.arange(
+                model.Rmin.to('au').value,
+                model.Rmax.to('au').value,
+                model.beam_size.to('au').value/4
+            )
+        else:
+            self.coord_levels = coord_levels
 
         self._lev_list = None
         self._coord_list = None
         self._resid_list = None
         self._color_list = None
+
+    def make_filaments(self, surface='upper', **kwargs):
+        #FIND FILAMENTS
+        #adapt_thresh is the width of the element used for the adaptive thresholding mask.
+        # This is primarily the step that picks out the filamentary structure. The element size should be similar to the width of the expected filamentary structure
+
+        from fil_finder import FilFinder2D
+
+        kw_fil_mask = dict(
+            verbose=False,
+            border_masking=False,
+            adapt_thresh=self.beam_size,
+            smooth_size=0.2*self.beam_size,
+            size_thresh=500*u.pix**2,
+            fill_hole_size=0.01*u.arcsec**2
+        )
+        kw_fil_mask.update(kwargs)
+        
+        Rgrid = self.R_nonan[surface]        
+        R_min_m=self.Rmin.to('m').value
+        ang_scale = np.abs(self.header['CDELT1'])*u.Unit(self.header['CUNIT1']) #pix size
+                       
+        Rind = (Rgrid>R_min_m) #& (Rgrid<R_max)
+        fil_pos = FilFinder2D(np.where(Rind & (self.prop>0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
+        fil_pos.preprocess_image(skip_flatten=True) 
+        fil_pos.create_mask(**kw_fil_mask)
+        fil_pos.medskel(verbose=False)
+        
+        fil_neg = FilFinder2D(np.where(Rind & (self.prop<0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
+        fil_neg.preprocess_image(skip_flatten=True) 
+        fil_neg.create_mask(**kw_fil_mask)
+        fil_neg.medskel(verbose=False)
+        
+        fil_pos.analyze_skeletons(prune_criteria='length')
+        fil_neg.analyze_skeletons(prune_criteria='length')
+        return fil_pos, fil_neg
         
     def prop_along_coords(self,
                           coord_ref=None,
                           surface='upper',
                           ax=None,
                           ax2=None,
                           acc_threshold=10, #0.05
                           max_prop_threshold=np.inf,
                           color_bounds=[200, 400],
                           colors=['red', 'dodgerblue', '#FFB000'],
                           lws=[0.3, 0.3, 0.3], lw_ax2_factor=1,
                           fold=False,
                           fold_func=np.subtract):
         """
-        Compute radial/azimuthal contours according to the model disc geometry 
-        to get and plot information from the input 2D property ``prop``.    
+        Compute azimuthal contours according to the model disc geometry 
+        to retrieve and plot information from the input two-dimensional map ``prop``.    
 
         Parameters
         ----------
         coord_ref : scalar, optional
-           Reference coordinate (referred to ``coords[0]``). The contour at this coordinate will be highlighted in bold black.
+           The contour at this coordinate will be highlighted in bold black.
 
         ax : `matplotlib.axes` instance, optional
            ax instance where computed contours are to be shown
-
-        prop : array_like, shape (nx, ny)
-           Input 2D field to extract information along contours.
-        
-        coords : list, shape (2,)
-           coords[0] [array_like, shape (nx, ny)], is the coordinate 2D map onto which contours will be computed using the input ``coord_levels``;
-           coords[1] [array_like, shape (nx, ny)], is the coordinate 2D map against which the ``prop`` values are plotted. The output plot is prop vs coords[1]       
-
-        coord_levels : array_like, shape (nlevels,)
-           Contour levels to be extracted from ``coords[0]``.
-           
-        coord_ref : scalar
-           Reference coordinate (referred to ``coords[0]``) to highlight among the other contours.
                    
         ax2 : `matplotlib.axes` instance (or list of instances), optional
            Additional ax(s) instance(s) to plot the location of contours in the disc. 
-           If provided, ``X`` and ``Y`` must also be passed.
            
-        X : array_like, shape (nx, ny), optional
-           Meshgrid of the model x coordinate (see `numpy.meshgrid`). Required if ax2 instance(s) is provided.
-
-        Y : array_like, shape (nx, ny), optional
-           Meshgrid of the model y coordinate (see `numpy.meshgrid`). Required if ax2 instance(s) is provided.
-                   
         acc_threshold : float, optional 
-           Threshold to accept points on contours at a given coords[0] level. If coord level obtained for a pixel is such that np.abs(level_pixel-level_reference)<acc_threshold the pixel value is accepted
+           Threshold to accept points on contours at a given coord_level. If coord_level obtained for a pixel is such that np.abs(level_pixel-level_reference)<acc_threshold the pixel value is accepted
 
         max_prop_threshold : float, optional 
            Threshold to accept points of contours. Rejects residuals of the contour if they are < max_prop_threshold. Useful to reject hot pixels.
 
         color_bounds : array_like, shape (nbounds,), optional
-           Colour bounds with respect to the reference contour coord_ref.
+           Color bounds for contour colors.
            
-        colors : array_like, shape (nbounds+2,), optional
-           Contour colors. (i=0) is reserved for the reference contour coord_ref, 
-           (i>0) for contour colors according to the bounds in color_bounds. 
-           
-        lws : array_like, shape (nbounds+2), optional
-           Contour linewidths. Similarly, (i=0) is reserved for coord_ref and 
-           (i>0) for subsequent bounds.
+        colors : array_like, shape (nbounds+1,), optional
+           Contour colors within bounds. 
+
+        lws : array_like, shape (nbounds+1), optional
+           Contour linewidths within bounds.
+
+        lw_ax2_factor : float, optional
+           Fraction of lws for linewidth value of contours in ax2.
 
         fold : bool, optional
            If True, subtract residuals by folding along the projected minor axis of the disc. Currently working for azimuthal contours only.
            
         fold_func : function, optional
            If fold, this function is used to operate between folded quadrants. Defaults to np.subtract.
         """
@@ -292,15 +326,15 @@
             kwargs_along_coords.update({'surface': surface})
             self.prop_along_coords(**kwargs_along_coords)
 
         lev_list, coord_list, resid_list = self._lev_list, self._coord_list, self._resid_list
         Rgrid = self.R_nonan[surface]/sfu.au
         X = self.X
         Y = self.Y
-        beam_size = self.beam_size
+        beam_size = self.beam_size.to('au').value
         
         frac_annulus = 1.0 #if halves, 0.5; if quadrants, 0.25
         nconts = len(lev_list)
         if resid_thres is None: resid_thres = [np.inf]*nconts #consider all values for the average
         elif resid_thres == '3sigma': resid_thres = [3*np.nanstd(resid_list[i]) for i in range(nconts)] #anything higher than 3sigma is rejected from annulus
         # -np.pi<coord_list<np.pi        
         ind_accep = [(((coord_list[i]<90-mask_ang) & (coord_list[i]>-90+mask_ang)) |
@@ -419,15 +453,15 @@
         
         for phi_dax in [phi_daxes_0, phi_daxes_90, phi_daxes_180, phi_daxes_270]:            
             x_cont, y_cont,_ = GridTools.get_sky_from_disc_coords(R_list[isort], phi_dax, z_list[isort], incl, PA, xc, yc)
             make_ax(x_cont, y_cont)
 
     @staticmethod
     def make_substructures(*args, **kwargs): #Backcompat
-        '''Overlay ring-like (if twodim) or vertical lines (if not twodim) to illustrate the radial location of substructures in the disc'''
+        __doc__ = make_substruct.__doc__
         return make_substruct(*args, **kwargs)
         
     @staticmethod
     def make_contour_lev(prop, lev, X, Y, acc_threshold=20): 
         contour = measure.find_contours(prop, lev)
         inds_cont = np.round(contour[-1]).astype(int)
         inds_cont = [tuple(f) for f in inds_cont]
```

### Comparing `discminer-0.2.3/discminer/testyapf.py` & `discminer-0.2.4/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/tools/discminer.mplstyle` & `discminer-0.2.4/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/tools/fit_kernel.py` & `discminer-0.2.4/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer/tools/utils.py` & `discminer-0.2.4/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/discminer.egg-info/PKG-INFO` & `discminer-0.2.4/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.3 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.4 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.3/discminer.egg-info/SOURCES.txt` & `discminer-0.2.4/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/setup.py` & `discminer-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/template/README.rst` & `discminer-0.2.4/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/template/download_MAPS.sh` & `discminer-0.2.4/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.4/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.3/template/prepare_data.py` & `discminer-0.2.4/template/prepare_data.py`

 * *Files identical despite different names*

