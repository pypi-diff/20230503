# Comparing `tmp/inkstone-0.2.8.tar.gz` & `tmp/inkstone-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkstone-0.2.8.tar", last modified: Mon Dec  6 01:49:53 2021, max compression
+gzip compressed data, was "inkstone-0.2.9.tar", last modified: Thu Dec 30 02:01:41 2021, max compression
```

## Comparing `inkstone-0.2.8.tar` & `inkstone-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2021-12-06 01:49:53.594061 inkstone-0.2.8/
--rw-rw-rw-   0        0        0    34523 2021-08-20 00:35:47.000000 inkstone-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     3982 2021-12-06 01:49:53.585063 inkstone-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3417 2021-11-09 10:34:53.000000 inkstone-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2021-12-06 01:49:53.526063 inkstone-0.2.8/inkstone/
--rw-rw-rw-   0        0        0       68 2021-11-04 05:58:42.000000 inkstone-0.2.8/inkstone/__init__.py
--rw-rw-rw-   0        0        0     7322 2021-11-10 02:42:48.000000 inkstone-0.2.8/inkstone/bx.py
--rw-rw-rw-   0        0        0      586 2021-11-02 14:20:39.000000 inkstone-0.2.8/inkstone/conv_mtx_idx.py
-drwxrwxrwx   0        0        0        0 2021-12-06 01:49:53.580063 inkstone-0.2.8/inkstone/ft/
--rw-rw-rw-   0        0        0        0 2021-08-30 14:05:39.000000 inkstone-0.2.8/inkstone/ft/__init__.py
--rw-rw-rw-   0        0        0      851 2021-11-03 09:48:00.000000 inkstone-0.2.8/inkstone/ft/ft_1d_sq.py
--rw-rw-rw-   0        0        0      680 2021-11-03 09:48:00.000000 inkstone-0.2.8/inkstone/ft/ft_2d_cnst.py
--rw-rw-rw-   0        0        0     1295 2021-11-03 09:48:00.000000 inkstone-0.2.8/inkstone/ft/ft_2d_disk.py
--rw-rw-rw-   0        0        0     1813 2021-11-03 09:48:01.000000 inkstone-0.2.8/inkstone/ft/ft_2d_ellip.py
--rw-rw-rw-   0        0        0     1569 2021-11-04 05:56:06.000000 inkstone-0.2.8/inkstone/ft/ft_2d_para.py
--rw-rw-rw-   0        0        0     3102 2021-11-04 05:56:07.000000 inkstone-0.2.8/inkstone/ft/ft_2d_poly.py
--rw-rw-rw-   0        0        0      992 2021-11-04 05:56:07.000000 inkstone-0.2.8/inkstone/ft/ft_2d_rct.py
--rw-rw-rw-   0        0        0     2166 2021-11-06 15:08:05.000000 inkstone-0.2.8/inkstone/ft/gibbs.py
--rw-rw-rw-   0        0        0      510 2021-11-03 09:35:39.000000 inkstone-0.2.8/inkstone/ft/poly_area.py
--rw-rw-rw-   0        0        0     4559 2021-11-02 14:20:39.000000 inkstone-0.2.8/inkstone/g_pts.py
--rw-rw-rw-   0        0        0      920 2021-11-02 14:20:39.000000 inkstone-0.2.8/inkstone/g_pts_1d.py
-drwxrwxrwx   0        0        0        0 2021-12-06 01:49:53.584064 inkstone-0.2.8/inkstone/helpers/
--rw-rw-rw-   0        0        0       27 2021-10-31 11:59:20.000000 inkstone-0.2.8/inkstone/helpers/__init__.py
--rw-rw-rw-   0        0        0      791 2021-11-03 09:23:02.000000 inkstone-0.2.8/inkstone/helpers/pt_in_poly.py
--rw-rw-rw-   0        0        0      886 2021-10-31 11:59:20.000000 inkstone-0.2.8/inkstone/im.py
--rw-rw-rw-   0        0        0    31033 2021-12-06 01:09:35.000000 inkstone-0.2.8/inkstone/layer.py
--rw-rw-rw-   0        0        0     3677 2021-11-10 02:42:48.000000 inkstone-0.2.8/inkstone/layer_copy.py
--rw-rw-rw-   0        0        0      552 2021-10-31 11:59:20.000000 inkstone-0.2.8/inkstone/max_idx_diff.py
--rw-rw-rw-   0        0        0     3001 2021-11-04 15:06:40.000000 inkstone-0.2.8/inkstone/mtr.py
--rw-rw-rw-   0        0        0    27285 2021-12-01 11:15:47.000000 inkstone-0.2.8/inkstone/params.py
--rw-rw-rw-   0        0        0     1202 2021-11-02 14:20:39.000000 inkstone-0.2.8/inkstone/recipro.py
--rw-rw-rw-   0        0        0     4150 2021-12-06 01:45:06.000000 inkstone-0.2.8/inkstone/rsp.py
--rw-rw-rw-   0        0        0    14168 2021-11-04 10:05:36.000000 inkstone-0.2.8/inkstone/shps.py
--rw-rw-rw-   0        0        0    59051 2021-12-05 09:05:38.000000 inkstone-0.2.8/inkstone/simulator.py
--rw-rw-rw-   0        0        0     2712 2021-11-05 08:43:38.000000 inkstone-0.2.8/inkstone/sm.py
-drwxrwxrwx   0        0        0        0 2021-12-06 01:49:53.556066 inkstone-0.2.8/inkstone.egg-info/
--rw-rw-rw-   0        0        0     3982 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-12-06 01:49:53.000000 inkstone-0.2.8/inkstone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-06 01:49:53.595062 inkstone-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      986 2021-12-06 01:49:15.000000 inkstone-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-30 02:01:41.325246 inkstone-0.2.9/
+-rw-rw-rw-   0        0        0    34523 2021-08-20 00:35:47.000000 inkstone-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     3982 2021-12-30 02:01:41.324249 inkstone-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3417 2021-11-09 10:34:53.000000 inkstone-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2021-12-30 02:01:41.292245 inkstone-0.2.9/inkstone/
+-rw-rw-rw-   0        0        0       68 2021-11-04 05:58:42.000000 inkstone-0.2.9/inkstone/__init__.py
+-rw-rw-rw-   0        0        0     7322 2021-11-10 02:42:48.000000 inkstone-0.2.9/inkstone/bx.py
+-rw-rw-rw-   0        0        0      586 2021-11-02 14:20:39.000000 inkstone-0.2.9/inkstone/conv_mtx_idx.py
+drwxrwxrwx   0        0        0        0 2021-12-30 02:01:41.319246 inkstone-0.2.9/inkstone/ft/
+-rw-rw-rw-   0        0        0        0 2021-08-30 14:05:39.000000 inkstone-0.2.9/inkstone/ft/__init__.py
+-rw-rw-rw-   0        0        0      851 2021-11-03 09:48:00.000000 inkstone-0.2.9/inkstone/ft/ft_1d_sq.py
+-rw-rw-rw-   0        0        0      680 2021-11-03 09:48:00.000000 inkstone-0.2.9/inkstone/ft/ft_2d_cnst.py
+-rw-rw-rw-   0        0        0     1295 2021-11-03 09:48:00.000000 inkstone-0.2.9/inkstone/ft/ft_2d_disk.py
+-rw-rw-rw-   0        0        0     1813 2021-11-03 09:48:01.000000 inkstone-0.2.9/inkstone/ft/ft_2d_ellip.py
+-rw-rw-rw-   0        0        0     1569 2021-11-04 05:56:06.000000 inkstone-0.2.9/inkstone/ft/ft_2d_para.py
+-rw-rw-rw-   0        0        0     3102 2021-11-04 05:56:07.000000 inkstone-0.2.9/inkstone/ft/ft_2d_poly.py
+-rw-rw-rw-   0        0        0      992 2021-11-04 05:56:07.000000 inkstone-0.2.9/inkstone/ft/ft_2d_rct.py
+-rw-rw-rw-   0        0        0     2166 2021-11-06 15:08:05.000000 inkstone-0.2.9/inkstone/ft/gibbs.py
+-rw-rw-rw-   0        0        0      510 2021-11-03 09:35:39.000000 inkstone-0.2.9/inkstone/ft/poly_area.py
+-rw-rw-rw-   0        0        0     4559 2021-11-02 14:20:39.000000 inkstone-0.2.9/inkstone/g_pts.py
+-rw-rw-rw-   0        0        0      920 2021-11-02 14:20:39.000000 inkstone-0.2.9/inkstone/g_pts_1d.py
+drwxrwxrwx   0        0        0        0 2021-12-30 02:01:41.323245 inkstone-0.2.9/inkstone/helpers/
+-rw-rw-rw-   0        0        0       27 2021-10-31 11:59:20.000000 inkstone-0.2.9/inkstone/helpers/__init__.py
+-rw-rw-rw-   0        0        0      791 2021-11-03 09:23:02.000000 inkstone-0.2.9/inkstone/helpers/pt_in_poly.py
+-rw-rw-rw-   0        0        0      886 2021-10-31 11:59:20.000000 inkstone-0.2.9/inkstone/im.py
+-rw-rw-rw-   0        0        0    31036 2021-12-07 00:40:37.000000 inkstone-0.2.9/inkstone/layer.py
+-rw-rw-rw-   0        0        0     3677 2021-11-10 02:42:48.000000 inkstone-0.2.9/inkstone/layer_copy.py
+-rw-rw-rw-   0        0        0      552 2021-10-31 11:59:20.000000 inkstone-0.2.9/inkstone/max_idx_diff.py
+-rw-rw-rw-   0        0        0     3001 2021-11-04 15:06:40.000000 inkstone-0.2.9/inkstone/mtr.py
+-rw-rw-rw-   0        0        0    27285 2021-12-01 11:15:47.000000 inkstone-0.2.9/inkstone/params.py
+-rw-rw-rw-   0        0        0     1202 2021-11-02 14:20:39.000000 inkstone-0.2.9/inkstone/recipro.py
+-rw-rw-rw-   0        0        0     4150 2021-12-06 01:45:06.000000 inkstone-0.2.9/inkstone/rsp.py
+-rw-rw-rw-   0        0        0    14168 2021-11-04 10:05:36.000000 inkstone-0.2.9/inkstone/shps.py
+-rw-rw-rw-   0        0        0    59918 2021-12-30 01:38:54.000000 inkstone-0.2.9/inkstone/simulator.py
+-rw-rw-rw-   0        0        0     2712 2021-11-05 08:43:38.000000 inkstone-0.2.9/inkstone/sm.py
+drwxrwxrwx   0        0        0        0 2021-12-30 02:01:41.301270 inkstone-0.2.9/inkstone.egg-info/
+-rw-rw-rw-   0        0        0     3982 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2021-12-30 02:01:41.000000 inkstone-0.2.9/inkstone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-30 02:01:41.325246 inkstone-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      986 2021-12-30 01:57:18.000000 inkstone-0.2.9/setup.py
```

### Comparing `inkstone-0.2.8/LICENSE` & `inkstone-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/PKG-INFO` & `inkstone-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkstone
-Version: 0.2.8
+Version: 0.2.9
 Summary: 3D efficient solver for multi-stacked in-plane periodic structures using rcwa.
 Home-page: https://github.com/alexysong/inkstone
 Author: Alex Y. Song
 Author-email: song.alexy@gmail.com
 License: UNKNOWN
 Keywords: rcwa
 Platform: UNKNOWN
```

### Comparing `inkstone-0.2.8/README.md` & `inkstone-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/bx.py` & `inkstone-0.2.9/inkstone/bx.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/conv_mtx_idx.py` & `inkstone-0.2.9/inkstone/conv_mtx_idx.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_1d_sq.py` & `inkstone-0.2.9/inkstone/ft/ft_1d_sq.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_cnst.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_cnst.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_disk.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_disk.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_ellip.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_ellip.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_para.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_para.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_poly.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_poly.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/ft_2d_rct.py` & `inkstone-0.2.9/inkstone/ft/ft_2d_rct.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/ft/gibbs.py` & `inkstone-0.2.9/inkstone/ft/gibbs.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/g_pts.py` & `inkstone-0.2.9/inkstone/g_pts.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/g_pts_1d.py` & `inkstone-0.2.9/inkstone/g_pts_1d.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/helpers/pt_in_poly.py` & `inkstone-0.2.9/inkstone/helpers/pt_in_poly.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/im.py` & `inkstone-0.2.9/inkstone/im.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/layer.py` & `inkstone-0.2.9/inkstone/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
                         w[(w2.real < 0) * (w.imag > 0)] *= -1
                     else:
                         warn("ccpif not recognized. Default to 'ac'.")
                         w[(w2.real < 0) * (w.imag < 0)] *= -1
                 else:
                     w[w.imag < 0] *= -1
             ql = w.T.ravel()  # 1d array length 2num_g
-            vh = -1j * p @ v / w[:, None]
+            vh = -1j * p @ v / w[:, None, :]
 
             psil11, psil12, psil21, psil22 = [np.diag(vh[:, i, j]) for i, j in [(0, 0), (0, 1), (1, 0), (1, 1)]]
             psil = np.block([[psil11, psil12],
                              [psil21, psil22]])
 
             self.ql = ql
             self.phil = phil
```

### Comparing `inkstone-0.2.8/inkstone/layer_copy.py` & `inkstone-0.2.9/inkstone/layer_copy.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/max_idx_diff.py` & `inkstone-0.2.9/inkstone/max_idx_diff.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/mtr.py` & `inkstone-0.2.9/inkstone/mtr.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/params.py` & `inkstone-0.2.9/inkstone/params.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/recipro.py` & `inkstone-0.2.9/inkstone/recipro.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/rsp.py` & `inkstone-0.2.9/inkstone/rsp.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/shps.py` & `inkstone-0.2.9/inkstone/shps.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone/simulator.py` & `inkstone-0.2.9/inkstone/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -583,18 +583,35 @@
                 # csm of previous layer
                 scp11, scp12, scp21, scp22 = csmp
                 # csmr
                 sci11, sci12, sci21, sci22 = csmr
                 # csmr of next layer
                 scin11, scin12, scin21, scin22 = csmrn
 
-                al = 1. / 2. * (bl0 @ sla.solve((I - sci11 @ scp22), (sci11 @ scp21 @ ai_v + sci12 @ bo_v))
-                                + al0 @ sla.solve((I - scp22 @ sci11), (scp21 @ ai_v + scp22 @ sci12 @ bo_v)))
-                bl = 1. / 2. * (bl0 @ sla.solve((I - sc22 @ scin11), (sc21 @ ai_v + sc22 @ scin12 @ bo_v))
-                                + al0 @ sla.solve((I - scin11 @ sc22), (scin11 @ sc21 @ ai_v + scin12 @ bo_v)))
+                if (layersl[i-1].in_mid_out == "in") and not layersl[i-1].is_vac:
+                    sa = sla.lu_solve(scp21, ai_v)
+                    sb = sci12 @ bo_v
+                    al = 1. / 2. * (bl0 @ sla.solve((I - sci11 @ scp22), (sci11 @ sa + sb))
+                                    + al0 @ sla.solve((I - scp22 @ sci11), (sa + scp22 @ sb)))
+                else:
+                    sa = scp21 @ ai_v
+                    sb = sci12 @ bo_v
+                    al = 1. / 2. * (bl0 @ sla.solve((I - sci11 @ scp22), (sci11 @ sa + sb))
+                                    + al0 @ sla.solve((I - scp22 @ sci11), (sa + scp22 @ sb)))
+
+                if (layersl[i+1].in_mid_out == "out") and not layersl[i+1].is_vac:
+                    sa = sc21 @ ai_v
+                    sb = sla.lu_solve(scin12, bo_v)
+                    bl = 1. / 2. * (bl0 @ sla.solve((I - sc22 @ scin11), (sa + sc22 @ sb))
+                                    + al0 @ sla.solve((I - scin11 @ sc22), (scin11 @ sa + sb)))
+                else:
+                    sa = sc21 @ ai_v
+                    sb = scin12 @ bo_v
+                    bl = 1. / 2. * (bl0 @ sla.solve((I - sc22 @ scin11), (sa + sc22 @ sb))
+                                    + al0 @ sla.solve((I - scin11 @ sc22), (scin11 @ sa + sb)))
 
                 # ravel 2d array (just one column) to 1d array
                 al = al.ravel()
                 bl = bl.ravel()
                 layer.al_bl = (al, bl)
 
             layer.need_recalc_al_bl = False
```

### Comparing `inkstone-0.2.8/inkstone/sm.py` & `inkstone-0.2.9/inkstone/sm.py`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/inkstone.egg-info/PKG-INFO` & `inkstone-0.2.9/inkstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkstone
-Version: 0.2.8
+Version: 0.2.9
 Summary: 3D efficient solver for multi-stacked in-plane periodic structures using rcwa.
 Home-page: https://github.com/alexysong/inkstone
 Author: Alex Y. Song
 Author-email: song.alexy@gmail.com
 License: UNKNOWN
 Keywords: rcwa
 Platform: UNKNOWN
```

### Comparing `inkstone-0.2.8/inkstone.egg-info/SOURCES.txt` & `inkstone-0.2.9/inkstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inkstone-0.2.8/setup.py` & `inkstone-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def readme():
     with io.open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 setup(name='inkstone',
-      version='0.2.8',
+      version='0.2.9',
       description='3D efficient solver for multi-stacked in-plane periodic structures using rcwa.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://github.com/alexysong/inkstone',
       # check https://pypi.org/pypi?%3Aaction=list_classifiers for classifiers
       classifiers=[
         'Programming Language :: Python :: 3',
```

